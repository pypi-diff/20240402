# Comparing `tmp/deqarclient-0.5.1.tar.gz` & `tmp/deqarclient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deqarclient-0.5.1.tar", last modified: Sat Jun 18 19:52:54 2022, max compression
+gzip compressed data, was "deqarclient-1.0.0.tar", last modified: Tue Apr  2 16:36:54 2024, max compression
```

## Comparing `deqarclient-0.5.1.tar` & `deqarclient-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 colin      (503) staff       (20)        0 2022-06-18 19:52:54.851610 deqarclient-0.5.1/
--rw-r--r--   0 colin      (503) staff       (20)      910 2022-06-18 19:52:54.851455 deqarclient-0.5.1/PKG-INFO
--rw-r--r--   0 colin      (503) staff       (20)      574 2019-11-10 10:49:59.000000 deqarclient-0.5.1/README.md
-drwxr-xr-x   0 colin      (503) staff       (20)        0 2022-06-18 19:52:54.850619 deqarclient-0.5.1/deqarclient/
--rw-r--r--   0 colin      (503) staff       (20)      190 2022-04-22 17:47:03.000000 deqarclient-0.5.1/deqarclient/__init__.py
--rw-r--r--   0 colin      (503) staff       (20)     1927 2022-04-22 17:47:03.000000 deqarclient-0.5.1/deqarclient/agency.py
--rw-r--r--   0 colin      (503) staff       (20)     9428 2022-06-18 19:48:33.000000 deqarclient-0.5.1/deqarclient/api.py
--rw-r--r--   0 colin      (503) staff       (20)     2592 2022-04-22 17:47:03.000000 deqarclient-0.5.1/deqarclient/auth.py
--rw-r--r--   0 colin      (503) staff       (20)      304 2022-04-22 17:47:03.000000 deqarclient-0.5.1/deqarclient/errors.py
--rw-r--r--   0 colin      (503) staff       (20)    13199 2022-04-22 17:47:03.000000 deqarclient-0.5.1/deqarclient/institution.py
-drwxr-xr-x   0 colin      (503) staff       (20)        0 2022-06-18 19:52:54.851260 deqarclient-0.5.1/deqarclient.egg-info/
--rw-r--r--   0 colin      (503) staff       (20)      910 2022-06-18 19:52:54.000000 deqarclient-0.5.1/deqarclient.egg-info/PKG-INFO
--rw-r--r--   0 colin      (503) staff       (20)      348 2022-06-18 19:52:54.000000 deqarclient-0.5.1/deqarclient.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (503) staff       (20)        1 2022-06-18 19:52:54.000000 deqarclient-0.5.1/deqarclient.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (503) staff       (20)       46 2022-06-18 19:52:54.000000 deqarclient-0.5.1/deqarclient.egg-info/requires.txt
--rw-r--r--   0 colin      (503) staff       (20)       12 2022-06-18 19:52:54.000000 deqarclient-0.5.1/deqarclient.egg-info/top_level.txt
--rwxr-xr-x   0 colin      (503) staff       (20)     3115 2022-04-22 17:47:03.000000 deqarclient-0.5.1/importInstitutions.py
--rw-r--r--   0 colin      (503) staff       (20)       38 2022-06-18 19:52:54.851657 deqarclient-0.5.1/setup.cfg
--rw-r--r--   0 colin      (503) staff       (20)      778 2022-06-18 19:51:17.000000 deqarclient-0.5.1/setup.py
+drwxr-xr-x   0 colin      (503) staff       (20)        0 2024-04-02 16:36:54.935603 deqarclient-1.0.0/
+-rw-r--r--   0 colin      (503) staff       (20)     1007 2024-04-02 16:36:54.935386 deqarclient-1.0.0/PKG-INFO
+-rw-r--r--   0 colin      (503) staff       (20)      574 2019-11-10 10:49:59.000000 deqarclient-1.0.0/README.md
+drwxr-xr-x   0 colin      (503) staff       (20)        0 2024-04-02 16:36:54.933972 deqarclient-1.0.0/deqarclient/
+-rw-r--r--   0 colin      (503) staff       (20)      190 2022-04-22 17:47:03.000000 deqarclient-1.0.0/deqarclient/__init__.py
+-rw-r--r--   0 colin      (503) staff       (20)     1927 2022-04-22 17:47:03.000000 deqarclient-1.0.0/deqarclient/agency.py
+-rw-r--r--   0 colin      (503) staff       (20)    10191 2024-03-05 15:14:46.000000 deqarclient-1.0.0/deqarclient/api.py
+-rw-r--r--   0 colin      (503) staff       (20)     2592 2022-04-22 17:47:03.000000 deqarclient-1.0.0/deqarclient/auth.py
+-rw-r--r--   0 colin      (503) staff       (20)     3482 2023-09-06 20:27:04.000000 deqarclient-1.0.0/deqarclient/csv.py
+-rw-r--r--   0 colin      (503) staff       (20)      304 2022-04-22 17:47:03.000000 deqarclient-1.0.0/deqarclient/errors.py
+-rw-r--r--   0 colin      (503) staff       (20)    15352 2024-03-06 08:04:49.000000 deqarclient-1.0.0/deqarclient/institution.py
+drwxr-xr-x   0 colin      (503) staff       (20)        0 2024-04-02 16:36:54.935136 deqarclient-1.0.0/deqarclient.egg-info/
+-rw-r--r--   0 colin      (503) staff       (20)     1007 2024-04-02 16:36:54.000000 deqarclient-1.0.0/deqarclient.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (503) staff       (20)      367 2024-04-02 16:36:54.000000 deqarclient-1.0.0/deqarclient.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (503) staff       (20)        1 2024-04-02 16:36:54.000000 deqarclient-1.0.0/deqarclient.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (503) staff       (20)       46 2024-04-02 16:36:54.000000 deqarclient-1.0.0/deqarclient.egg-info/requires.txt
+-rw-r--r--   0 colin      (503) staff       (20)       12 2024-04-02 16:36:54.000000 deqarclient-1.0.0/deqarclient.egg-info/top_level.txt
+-rwxr-xr-x   0 colin      (503) staff       (20)     3360 2024-02-22 11:05:17.000000 deqarclient-1.0.0/importInstitutions.py
+-rw-r--r--   0 colin      (503) staff       (20)       38 2024-04-02 16:36:54.935651 deqarclient-1.0.0/setup.cfg
+-rw-r--r--   0 colin      (503) staff       (20)      789 2024-03-29 11:40:32.000000 deqarclient-1.0.0/setup.py
```

### Comparing `deqarclient-0.5.1/PKG-INFO` & `deqarclient-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: deqarclient
-Version: 0.5.1
+Version: 1.0.0
 Summary: Python classes to work with DEQAR APIs
 Home-page: https://github.com/EQAR/deqar-tools/
-Download-URL: https://pypi.org/project//
+Download-URL: https://pypi.org/project/deqarclient/
 Author: Colin Tück
 Author-email: colin.tueck@eqar.eu
 License: GPL
 Keywords: DEQAR
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: coloredlogs
+Requires-Dist: requests
+Requires-Dist: tldextract
+Requires-Dist: transliterate
 
 # deqar-tools
 Collections of additional scripts to manage DEQAR data
 
 ## deqar.py
 Module to work with DEQAR APIs
 
@@ -24,9 +27,7 @@
 Simple shell script wrappers to make requests to DEQAR APIs using [curl](https://curl.haxx.se/)
 
 ## deqar-cli.py
 Simple CLI to search and browse institutions with reports - incomplete, just written for testing the module
 
 ## test-pw.pl
 Perl script to test whether users still have a default password set
-
-
```

### Comparing `deqarclient-0.5.1/README.md` & `deqarclient-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `deqarclient-0.5.1/deqarclient/agency.py` & `deqarclient-1.0.0/deqarclient/agency.py`

 * *Files identical despite different names*

### Comparing `deqarclient-0.5.1/deqarclient/api.py` & `deqarclient-1.0.0/deqarclient/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     _version = '0.3.1'
 
     _Countries = None           # these properties will be instantiated
     _QfEheaLevels = None        # as objects when first accessed
     _HierarchicalTypes = None
     _DomainChecker = None
+    _OrganizationTypes = None
 
     def __init__(self, base, authclass=EqarApiEnvAuth, request_timeout=10, **kwargs):
         """ Constructor prepares for request. Token is taken from parameter, environment or user is prompted to log in. """
         self.session            = requests.Session()
         self.base               = base.rstrip('/')
         self.webapi             = '/webapi/v2'
         self.request_timeout    = request_timeout
@@ -47,15 +48,15 @@
         self.logger.debug("[{} {} started]".format(method, self.base + path))
 
         r = self.session.request(method, self.base + path, timeout=self.request_timeout, **kwargs)
 
         try:
             r.raise_for_status()
         except requests.exceptions.HTTPError:
-            self.logger.error("[HTTP error {}: {}]".format(r.status_code, r.reason))
+            self.logger.error("[HTTP error {}: {}]\nRequest: {}\nResponse: {}".format(r.status_code, r.reason, json.dumps(kwargs.get('json', {}), indent=4, sort_keys=True), json.dumps(r.json(), indent=4, sort_keys=True)))
             raise HttpError("{} {}".format(r.status_code, r.reason))
         else:
             self.logger.debug("[HTTP {} {}]".format(r.status_code, r.reason))
             return(r.json())
 
     def get(self, path, **kwargs):
         """ make a GET request to [path] with parameters from [kwargs] """
@@ -76,43 +77,41 @@
     def get_institution(self, id):
         """ get single institution record [id] """
         return(self.get(self.webapi + "/browse/institutions/{:d}".format(id)))
 
     def create_qf_ehea_level_set(self, *args, **kwargs):
 
         class QfEheaLevelSet (list):
-            """ Actual set of QfEheaLevels - constructed from input string, mainly for HEI data import """
+            """ Actual set of QfEheaLevels - constructed from input list, mainly for HEI data import """
 
             LevelKeywords   = dict(
                                 short=0,
                                 first=1,
                                 second=2,
                                 secound=2,
                                 third=3
                             )
 
-            def __init__(self, api, string, strict=False):
+            def __init__(self, api, source_list, strict=False):
                 """ parses a string for a set of levels, specified by digits or key words, eliminating duplicates and ignoring unknowns """
 
                 recognised = set()
 
-                for l in re.split(r'\s*[^A-Za-z0-9]\s*', string.strip(" ,.\n\r\t\v\f")):
-                    match = re.match('([01235678]|cycle|{})'.format("|".join(self.LevelKeywords.keys())), l);
-                    if match and match.group(1) != 'cycle':
+                for l in source_list:
+                    match = re.search('([01235678]|{})'.format("|".join(self.LevelKeywords.keys())), l, re.IGNORECASE);
+                    if match:
                         m = match.group(1)
                         if m.isdigit():
                             if int(m) > 4:
                                 m = int(m) - 5
                         else:
-                            m = self.LevelKeywords[m]
+                            m = self.LevelKeywords[m.lower()]
                         level = api.QfEheaLevels.get(m)
                         recognised.add(level['code'])
                         api.logger.debug('  [{}] => {}/{}'.format(l, level['id'], level['level']))
-                    elif match and match.group(1) == 'cycle':
-                        pass
                     elif strict:
                         raise(DataError('  [{}] : QF-EHEA level not recognised, ignored.'.format(l)))
                     else:
                         api.logger.debug('  [{}] : QF-EHEA level not recognised, ignored.'.format(l))
 
                 for i in recognised:
                     self.append(api.QfEheaLevels.get(i))
@@ -175,14 +174,31 @@
                             return l
                     return None
             self._HierarchicalTypes = HierarchicalTypes(self)
 
         return(self._HierarchicalTypes)
 
     @property
+    def OrganizationTypes(self):
+        if not self._OrganizationTypes:
+            class OrganizationTypes:
+                """ Class to look up organization types (for AP) """
+                def __init__(self, api):
+                    self.types = api.get("/adminapi/v1/select/institutions/organization_type/")
+                def get(self, which):
+                    if type(which) == str and which.isdigit():
+                        which = int(which)
+                    for l in self.types:
+                        if which in [ l['id'], l['type'] ]:
+                            return l
+                    return None
+            self._OrganizationTypes = OrganizationTypes(self)
+        return(self._OrganizationTypes)
+
+    @property
     def DomainChecker(self):
 
         if not self._DomainChecker:
 
             class DomainChecker:
 
                 """ Fetches website addresses of all known institutions and allows to check against it """
```

### Comparing `deqarclient-0.5.1/deqarclient/auth.py` & `deqarclient-1.0.0/deqarclient/auth.py`

 * *Files identical despite different names*

### Comparing `deqarclient-0.5.1/deqarclient/institution.py` & `deqarclient-1.0.0/deqarclient/institution.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class NewInstitution:
 
     """
     creates a new institution record from CSV input
     """
 
-    def __init__(self, api, data):
+    def __init__(self, api, data, other_provider=False):
 
         def csv_coalesce(*args):
             for column in args:
                 if column in data and data[column]:
                     if isinstance(data[column], str):
                         return(data[column].strip())
                     else:
@@ -44,15 +44,16 @@
         if csv_coalesce('name_english'):
             self.api.logger.debug('  - English name given, used as primary')
         else:
             self.api.logger.debug('  - No English name, used official name as primary')
         self.api.logger.debug('  - webiste={}'.format(csv_coalesce('website_link')))
 
         # normalise website
-        website = self._url_normalise(csv_coalesce('website_link'))
+        #website = self._url_normalise(csv_coalesce('website_link'))
+        website = csv_coalesce('website_link')
         data['website_link'] = website
 
         # check for duplicate by internet domain
         self.api.DomainChecker.query(csv_coalesce('website_link'))
         if self.api.DomainChecker.core_domain(website) != self.api.DomainChecker.core_domain(csv_coalesce('website_link')):
             self.api.DomainChecker.query(website)
 
@@ -64,18 +65,19 @@
                 raise DataError("Unknown country [{}]".format(which))
             self.api.logger.debug('  - country [{}] resolved to {} (ID {})'.format(which,country['name_english'],country['id']))
         else:
             raise DataError("Country needs to be specified")
 
         # basic record
         self.institution = dict(
+            is_other_provider=other_provider,
             name_primary=name_primary,
             website_link=website,
             names=[ { 'name_official': csv_coalesce('name_official') }],
-            countries=[ { 'country': country['id'] } ],
+            countries=[ { 'country': country['id'], 'country_verified': True } ],
             flags=[ ]
         )
 
         # sanity check names
         if 'name_english' in data and data['name_english'] == data['name_official']:
             warn(DataWarning("  - !!! DUPLICATE NAME: English name [{}] identical to official name.".format(data['name_english'])))
             del data['name_english']
@@ -106,14 +108,35 @@
         if csv_coalesce('name_version'):
             self._query_name(csv_coalesce('name_version'))
             self.institution['names'][0]['alternative_names'] = [ { 'name': csv_coalesce('name_version') } ]
         if csv_coalesce('acronym'):
             self.institution['names'][0]['acronym'] = csv_coalesce('acronym')
         if csv_coalesce('city'):
             self.institution['countries'][0]['city'] = csv_coalesce('city')
+        if csv_coalesce('latitude'):
+            self.institution['countries'][0]['lat'] = csv_coalesce('latitude')
+        if csv_coalesce('longitude'):
+            self.institution['countries'][0]['long'] = csv_coalesce('longitude')
+        if csv_coalesce('other_location'):
+            for location in csv_coalesce('other_location'):
+                if 'country' in location:
+                    country = self.api.Countries.get(location['country'])
+                    if not country:
+                        raise DataError("Unknown country [{}]".format(location['country']))
+                    self.api.logger.debug('  - country [{}] resolved to {} (ID {})'.format(location['country'],country['name_english'],country['id']))
+                else:
+                    raise DataError("Country needs to be specified for each location")
+                add_location = { 'country': country['id'], 'country_verified': False }
+                if 'city' in location:
+                    add_location['city'] = location['city']
+                if 'latitude' in location:
+                    add_location['lat'] = location['latitude']
+                if 'longitude' in location:
+                    add_location['long'] = location['longitude']
+                self.institution['countries'].append(add_location)
         if csv_coalesce('founding_date'):
             match = re.match(r'^\s*([0-9]{4})(-(?:1[012]|0?[0-9])-(?:31|30|[012]?[0-9]))?\s*$', data['founding_date'])
             if match:
                 if match[2] is None:
                     self.institution['founding_date'] = match[1] + '-01-01'
                 else:
                     self.institution['founding_date'] = match[1] + match[2]
@@ -124,31 +147,38 @@
             if match:
                 if match[2] is None:
                     self.institution['closing_date'] = match[1] + '-12-31'
                 else:
                     self.institution['closing_date'] = match[1] + match[2]
             else:
                 raise DataError("Malformed closing_date: [{}]".format(data['closing_date']))
+        if csv_coalesce('type_provider'):
+            organization_type = self.api.OrganizationTypes.get(csv_coalesce('type_provider'))
+            if organization_type:
+                self.institution['organization_type'] = organization_type['id']
+                self.api.logger.debug('  - organization type: {} (ID {})'.format(organization_type['type'], organization_type['id']))
+            else:
+                raise DataError("Unknown type of provider [{}]".format(data['type_provider']))
+        if csv_coalesce('source_information'):
+            self.institution['source_of_information'] = csv_coalesce('source_information')
 
         # process identifier
         if csv_coalesce('identifier'):
             self.institution['identifiers'] = [ { 'identifier': csv_coalesce('identifier') } ]
             if 'identifier_resource' not in data and 'agency_id' not in data:
                 raise(DataError("Identifier needs to have an agency ID or a resource."))
-            if 'identifier_resource' in data and 'agency_id' in data:
-                warn(DataWarning("  - identifier [{}] should not have both agency_id AND a resource".format(csv_coalesce('identifier'))))
             if 'identifier_resource' in data:
                 self.institution['identifiers'][0]['resource'] = csv_coalesce('identifier_resource')
                 self.api.logger.info('  - identifier [{}] with resource [{}]'.format(csv_coalesce('identifier'), csv_coalesce('identifier_resource')))
             else:
                 self.institution['identifiers'][0]['resource'] = 'local identifier'
-                self.api.logger.info('  - identifier [{}] as local identifier'.format(csv_coalesce('identifier')))
-            if 'agency_id' in data:
                 self.institution['identifiers'][0]['agency'] = csv_coalesce('agency_id')
-                self.api.logger.info('  linked to agency ID [{}]'.format(csv_coalesce('agency_id')))
+                self.api.logger.info('  - identifier [{}] as local identifier of agency ID [{}]'.format(csv_coalesce('identifier'), csv_coalesce('agency_id')))
+            if 'identifier_source' in data:
+                self.institution['identifiers'][0]['source'] = csv_coalesce('identifier_source')
 
         # process parent institution
         if csv_coalesce('parent_id', 'parent_deqar_id'):
             match = re.match('\s*(DEQARINST)?([0-9]+)\s*', str(csv_coalesce('parent_id', 'parent_deqar_id')).upper())
             if match:
                 self.institution['hierarchical_parent'] = [ { 'institution': int(match.group(2)) } ]
                 if csv_coalesce('parent_type'):
@@ -158,30 +188,32 @@
                         raise DataError('Unknown parent_type: [{}]'.format(csv_coalesce('parent_type')))
                 self.api.logger.info('  - hierarchical parent ID [{}] (source: [{}])'.format(int(match.group(2)), csv_coalesce('parent_id', 'parent_deqar_id')))
             else:
                 raise DataError('Malformed parent_id: [{}]'.format(csv_coalesce('parent_id', 'parent_deqar_id')))
 
         # process QF levels
         if csv_coalesce('qf_ehea_levels'):
-            self.institution['qf_ehea_levels'] = self.api.create_qf_ehea_level_set(data['qf_ehea_levels'])
+            self.institution['qf_ehea_levels'] = self.api.create_qf_ehea_level_set(re.split(r'\s*[^A-Za-z0-9]\s*', csv_coalesce('qf_ehea_levels')))
+        elif csv_coalesce('qf_ehea_level'):
+            self.institution['qf_ehea_levels'] = self.api.create_qf_ehea_level_set(data['qf_ehea_level'])
         else:
             self.institution['qf_ehea_levels'] = list()
 
     def _url_normalise(self, website):
         """
         normalises the URL, add http protocol if none specified, resolves redirects
         """
         match = re.match(r'^\s*([a-z0-9]+://)?([^/]+)(/.*)?$', website, flags=re.IGNORECASE)
         if match:
             protocol = (match[1] or 'http://').lower()
             domain = match[2].lower()
             path = match[3] or '/'
             url = protocol + domain + path
             try:
-                r = requests.head(url, allow_redirects=True)
+                r = requests.head(url, allow_redirects=True, timeout=self.api.request_timeout)
             except requests.exceptions.ConnectionError:
                 self.api.logger.warning("  - could not connect to URL [{}]".format(url))
                 return url
             else:
                 if r.status_code in [ requests.codes.ok, requests.codes.created ]:
                     if r.url != url:
                         self.api.logger.warning("  - URL [{}] was redirected to [{}]".format(url, r.url))
```

### Comparing `deqarclient-0.5.1/deqarclient.egg-info/PKG-INFO` & `deqarclient-1.0.0/deqarclient.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: deqarclient
-Version: 0.5.1
+Version: 1.0.0
 Summary: Python classes to work with DEQAR APIs
 Home-page: https://github.com/EQAR/deqar-tools/
-Download-URL: https://pypi.org/project//
+Download-URL: https://pypi.org/project/deqarclient/
 Author: Colin Tück
 Author-email: colin.tueck@eqar.eu
 License: GPL
 Keywords: DEQAR
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: coloredlogs
+Requires-Dist: requests
+Requires-Dist: tldextract
+Requires-Dist: transliterate
 
 # deqar-tools
 Collections of additional scripts to manage DEQAR data
 
 ## deqar.py
 Module to work with DEQAR APIs
 
@@ -24,9 +27,7 @@
 Simple shell script wrappers to make requests to DEQAR APIs using [curl](https://curl.haxx.se/)
 
 ## deqar-cli.py
 Simple CLI to search and browse institutions with reports - incomplete, just written for testing the module
 
 ## test-pw.pl
 Perl script to test whether users still have a default password set
-
-
```

### Comparing `deqarclient-0.5.1/importInstitutions.py` & `deqarclient-1.0.0/importInstitutions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from deqarclient.api import EqarApi
 from deqarclient.errors import DataError
 from deqarclient.auth import EqarApiInteractiveAuth
+from deqarclient.csv import flat_to_nested
 
 import os
 import argparse
 import csv
 import logging
 import coloredlogs
 
 parser = argparse.ArgumentParser()
 parser.add_argument("FILE", help="CSV file to import")
+parser.add_argument("-a", "--ap", help="load organisations as other providers (default: higher education institutions)",
+                    action="store_true")
 parser.add_argument("-b", "--base", help="Base URL to the DEQAR admin API (can also be set as DEQAR_BASE environment variable)")
 parser.add_argument("--direct", help="post institution records directly (otherwise, whole file is read first)",
                     action="store_true")
 parser.add_argument("-o", "--output", help="create CSV file with DEQARINST IDs of newly added institutions")
 parser.add_argument("-i", "--ignore", help="ignore data errors: skip input line instead of raising an exception",
                     action="store_true")
 parser.add_argument("-v", "--verbose", help="increase output verbosity",
@@ -52,15 +55,15 @@
         outwriter = csv.DictWriter(outfile, fieldnames=outfields)
         outwriter.writeheader()
 
     for data in inreader:
 
         try:
 
-            institution = api.create_institution(data)
+            institution = api.create_institution(flat_to_nested(data), other_provider=args.ap)
 
             if args.direct:
                 # in direct-post mode, we upload immediately
                 data['deqar_id'] = institution.post()
                 if args.output:
                     outwriter.writerow(data)
             else:
```

### Comparing `deqarclient-0.5.1/setup.py` & `deqarclient-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='deqarclient',
-    version='0.5.1',
+    version='1.0.0',
     description='Python classes to work with DEQAR APIs',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPL',
     packages=find_packages(),
     scripts=['importInstitutions.py'],
     author='Colin Tück',
     author_email='colin.tueck@eqar.eu',
     keywords=['DEQAR'],
     url='https://github.com/EQAR/deqar-tools/',
-    download_url='https://pypi.org/project//'
+    download_url='https://pypi.org/project/deqarclient/'
 )
 
 install_requires = [
     'coloredlogs',
     'requests',
     'tldextract',
     'transliterate'
```

