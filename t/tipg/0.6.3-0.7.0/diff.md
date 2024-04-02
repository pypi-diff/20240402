# Comparing `tmp/tipg-0.6.3.tar.gz` & `tmp/tipg-0.7.0.tar.gz`

## Comparing `tipg-0.6.3.tar` & `tipg-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/__init__.py
--rw-r--r--   0        0        0    32930 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/collections.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/database.py
--rw-r--r--   0        0        0    15616 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/dependencies.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/errors.py
--rw-r--r--   0        0        0    71197 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/factory.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/logger.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/main.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/middleware.py
--rw-r--r--   0        0        0    27266 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/settings.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/filter/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/filter/evaluate.py
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/filter/filters.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/resources/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/resources/enums.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/resources/response.py
--rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/sql/dbcatalog.sql
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/collection.html
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/collections.html
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/conformance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/debug.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/footer.html
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/header.html
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/item.html
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/items.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/landing.html
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/map.html
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/queryables.html
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/tilematrixset.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/tilematrixsets.html
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/tileset.html
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.6.3/tipg/templates/tilesets.html
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 tipg-0.6.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.6.3/LICENSE
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tipg-0.6.3/README.md
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 tipg-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 tipg-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/__init__.py
+-rw-r--r--   0        0        0    32930 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/collections.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/database.py
+-rw-r--r--   0        0        0    15579 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/dependencies.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/errors.py
+-rw-r--r--   0        0        0    73931 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/factory.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/logger.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/main.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/middleware.py
+-rw-r--r--   0        0        0    27240 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/settings.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/filter/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/filter/evaluate.py
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/filter/filters.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/resources/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/resources/enums.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/resources/response.py
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/sql/dbcatalog.sql
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/collection.html
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/collections.html
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/conformance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/debug.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/footer.html
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/header.html
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/item.html
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/items.html
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/landing.html
+-rw-r--r--   0        0        0    15452 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/map.html
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/queryables.html
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tilematrixset.html
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tilematrixsets.html
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tileset.html
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tilesets.html
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tipg-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tipg-0.7.0/README.md
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 tipg-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 tipg-0.7.0/PKG-INFO
```

### Comparing `tipg-0.6.3/tipg/collections.py` & `tipg-0.7.0/tipg/collections.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/database.py` & `tipg-0.7.0/tipg/database.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/dependencies.py` & `tipg-0.7.0/tipg/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,16 +314,14 @@
     return sortby
 
 
 def TileParams(
     z: Annotated[
         int,
         Path(
-            ge=0,
-            le=30,
             description="Identifier (Z) selecting one of the scales defined in the TileMatrixSet and representing the scaleDenominator the tile.",
         ),
     ],
     x: Annotated[
         int,
         Path(
             description="Column (X) index of the tile on the selected TileMatrix. It cannot exceed the MatrixHeight-1 for the selected TileMatrix.",
```

### Comparing `tipg-0.6.3/tipg/errors.py` & `tipg-0.7.0/tipg/errors.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/factory.py` & `tipg-0.7.0/tipg/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """tipg.factory: router factories."""
 
 import abc
 import csv
-import json
 import re
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, Generator, Iterable, List, Literal, Optional
 from urllib.parse import urlencode
 
 import jinja2
 import orjson
@@ -109,54 +108,61 @@
     # Write all remaining rows
     for row in data:
         yield writer.writerow(row)
 
 
 def create_html_response(
     request: Request,
-    data: str,
+    data: Any,
     templates: Jinja2Templates,
     template_name: str,
+    title: Optional[str] = None,
     router_prefix: Optional[str] = None,
+    **kwargs: Any,
 ) -> _TemplateResponse:
     """Create Template response."""
     urlpath = request.url.path
     if root_path := request.app.root_path:
         urlpath = re.sub(r"^" + root_path, "", urlpath)
 
+    if router_prefix:
+        urlpath = re.sub(r"^" + router_prefix, "", urlpath)
+
     crumbs = []
     baseurl = str(request.base_url).rstrip("/")
 
+    if router_prefix:
+        baseurl += router_prefix
+
     crumbpath = str(baseurl)
+    if urlpath == "/":
+        urlpath = ""
+
     for crumb in urlpath.split("/"):
         crumbpath = crumbpath.rstrip("/")
         part = crumb
         if part is None or part == "":
             part = "Home"
         crumbpath += f"/{crumb}"
         crumbs.append({"url": crumbpath.rstrip("/"), "part": part.capitalize()})
 
-    if router_prefix:
-        baseurl += router_prefix
-
     return templates.TemplateResponse(
         request,
         name=f"{template_name}.html",
         context={
-            "response": orjson.loads(data),
+            "response": data,
             "template": {
                 "api_root": baseurl,
                 "params": request.query_params,
-                "title": "",
+                "title": title or template_name,
             },
             "crumbs": crumbs,
-            "url": str(request.url),
-            "baseurl": baseurl,
-            "urlpath": str(request.url.path),
-            "urlparams": str(request.url.query),
+            "url": baseurl + urlpath,
+            "params": str(request.url.query),
+            **kwargs,
         },
     )
 
 
 # ref: https://github.com/python/mypy/issues/5374
 @dataclass  # type: ignore
 class EndpointsFactory(metaclass=abc.ABCMeta):
@@ -177,18 +183,18 @@
     # Full application with Landing and Conformance
     with_common: bool = True
 
     title: str = "OGC API"
 
     def __post_init__(self):
         """Post Init: register route and configure specific options."""
-        self.register_routes()
         if self.with_common:
-            self._conformance_route()
             self._landing_route()
+            self._conformance_route()
+        self.register_routes()
 
     def url_for(self, request: Request, name: str, **path_params: Any) -> str:
         """Return full url (with prefix) for a specific handler."""
         url_path = self.router.url_path_for(name, **path_params)
 
         base_url = str(request.base_url)
         if self.router_prefix:
@@ -203,23 +209,27 @@
             base_url += prefix
 
         return str(url_path.make_absolute_url(base_url=base_url))
 
     def _create_html_response(
         self,
         request: Request,
-        data: str,
+        data: Any,
         template_name: str,
+        title: Optional[str] = None,
+        **kwargs: Any,
     ) -> _TemplateResponse:
         return create_html_response(
             request,
             data,
             templates=self.templates,
             template_name=template_name,
+            title=title,
             router_prefix=self.router_prefix,
+            **kwargs,
         )
 
     @abc.abstractmethod
     def register_routes(self):
         """Register factory Routes."""
         ...
 
@@ -258,15 +268,15 @@
         ):
             """Get conformance."""
             data = model.Conformance(conformsTo=[*COMMON_CONFORMS, *self.conforms_to])
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="conformance",
                 )
 
             return data
 
     def _landing_route(self):
         """Register Landing (/) and Conformance (/conformance) routes."""
@@ -321,16 +331,17 @@
                     *self.links(request),
                 ],
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="landing",
+                    title=self.title,
                 )
 
             return data
 
 
 @dataclass
 class OGCFeaturesFactory(EndpointsFactory):
@@ -350,49 +361,53 @@
             model.Link(
                 title="List of Collections",
                 href=self.url_for(request, "collections"),
                 type=MediaType.json,
                 rel="data",
             ),
             model.Link(
-                title="Collection metadata",
+                title="Collection metadata (Template URL)",
                 href=self.url_for(
                     request,
                     "collection",
                     collectionId="{collectionId}",
                 ),
                 type=MediaType.json,
                 rel="data",
+                templated=True,
             ),
             model.Link(
-                title="Collection queryables",
+                title="Collection queryables (Template URL)",
                 href=self.url_for(
                     request,
                     "queryables",
                     collectionId="{collectionId}",
                 ),
                 type=MediaType.schemajson,
                 rel="queryables",
+                templated=True,
             ),
             model.Link(
-                title="Collection Features",
+                title="Collection Features (Template URL)",
                 href=self.url_for(request, "items", collectionId="{collectionId}"),
                 type=MediaType.geojson,
                 rel="data",
+                templated=True,
             ),
             model.Link(
-                title="Collection Feature",
+                title="Collection Feature (Template URL)",
                 href=self.url_for(
                     request,
                     "item",
                     collectionId="{collectionId}",
                     itemId="{itemId}",
                 ),
                 type=MediaType.geojson,
                 rel="data",
+                templated=True,
             ),
         ]
 
     def register_routes(self):
         """Register OGC Features endpoints."""
         self._collections_route()
         self._collection_route()
@@ -511,16 +526,17 @@
                     for collection in collection_list["collections"]
                 ],
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="collections",
+                    title="Collections list",
                 )
 
             return data
 
     def _collection_route(self):
         @self.router.get(
             "/collections/{collectionId}",
@@ -598,16 +614,17 @@
                     ],
                 }
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="collection",
+                    title=f"{collection.id} collection",
                 )
 
             return data
 
     def _queryables_route(self):
         @self.router.get(
             "/collections/{collectionId}/queryables",
@@ -643,16 +660,17 @@
                 link=self_url + qs,
                 properties=collection.queryables,
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="queryables",
+                    title=f"{collection.id} queryables",
                 )
 
             return data
 
     def _items_route(self):  # noqa: C901
         @self.router.get(
             "/collections/{collectionId}/items",
@@ -898,15 +916,18 @@
                     for feature in item_list["items"]
                 ],
             }
 
             # HTML Response
             if output_type == MediaType.html:
                 return self._create_html_response(
-                    request, orjsonDumps(data).decode(), template_name="items"
+                    request,
+                    orjson.loads(orjsonDumps(data).decode()),
+                    template_name="items",
+                    title=f"{collection.id} items",
                 )
 
             # GeoJSONSeq Response
             elif output_type == MediaType.geojsonseq:
                 return StreamingResponse(
                     (orjsonDumps(f) + b"\n" for f in data["features"]),  # type: ignore
                     media_type=MediaType.geojsonseq,
@@ -1063,16 +1084,17 @@
                 ],
             }
 
             # HTML Response
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    orjsonDumps(data).decode(),
+                    orjson.loads(orjsonDumps(data).decode()),
                     template_name="item",
+                    title=f"{collection.id}/{itemId} item",
                 )
 
             # Default to GeoJSON Response
             return GeoJSONResponse(data)
 
 
 @dataclass
@@ -1085,70 +1107,95 @@
     @property
     def conforms_to(self) -> List[str]:
         """Factory conformances."""
         return TILES_CONFORMS
 
     def links(self, request: Request) -> List[model.Link]:
         """OGC Tiles API links."""
-        return [
+        links = [
             model.Link(
-                title="Collection Vector Tiles",
+                title="Collection Vector Tiles (Template URL)",
                 href=self.url_for(
                     request,
                     "collection_get_tile",
                     collectionId="{collectionId}",
                     z="{z}",
                     x="{x}",
                     y="{y}",
                 ),
                 type=MediaType.mvt,
                 rel="data",
+                templated=True,
             ),
             model.Link(
-                title="Collection TileSets",
+                title="Collection TileSets (Template URL)",
                 href=self.url_for(
                     request,
                     "collection_tileset_list",
                     collectionId="{collectionId}",
                 ),
                 type=MediaType.json,
                 rel="data",
+                templated=True,
             ),
             model.Link(
-                title="Collection TileSet",
+                title="Collection TileSet (Template URL)",
                 href=self.url_for(
                     request,
                     "collection_tileset",
                     collectionId="{collectionId}",
                     tileMatrixSetId="{tileMatrixSetId}",
                 ),
                 type=MediaType.json,
                 rel="data",
+                templated=True,
             ),
+        ]
+
+        if self.with_viewer:
+            links.append(
+                model.Link(
+                    title="Collection Map viewer (Template URL)",
+                    href=self.url_for(
+                        request,
+                        "viewer_endpoint",
+                        collectionId="{collectionId}",
+                        tileMatrixSetId="{tileMatrixSetId}",
+                    ),
+                    type=MediaType.html,
+                    rel="data",
+                    templated=True,
+                )
+            )
+
+        links += [
             model.Link(
                 title="TileMatrixSets",
                 href=self.url_for(
                     request,
                     "tilematrixsets",
                 ),
                 type=MediaType.json,
                 rel="data",
             ),
             model.Link(
-                title="TileMatrixSet",
+                title="TileMatrixSet (Template URL)",
                 href=self.url_for(
                     request,
                     "tilematrixset",
                     tileMatrixSetId="{tileMatrixSetId}",
                 ),
                 type=MediaType.json,
                 rel="data",
+                templated=True,
             ),
         ]
 
+        return links
+
     def register_routes(self):  # noqa: C901
         """Register OGC Tiles endpoints."""
         self._tilematrixsets_routes()
         self._tilesets_routes()
         self._tile_routes()
         self._tilejson_routes()
         self._stylejson_routes()
@@ -1197,16 +1244,17 @@
                     for tms_id in self.supported_tms.list()
                 ]
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="tilematrixsets",
+                    title="TileMatrixSets list",
                 )
 
             return data
 
         @self.router.get(
             "/tileMatrixSets/{tileMatrixSetId}",
             response_model=TileMatrixSet,
@@ -1230,31 +1278,29 @@
                 Path(description="Identifier for a supported TileMatrixSet."),
             ],
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
         ):
             """
             OGC Specification: http://docs.opengeospatial.org/per/19-069.html#_tilematrixset
             """
-            data = self.supported_tms.get(tileMatrixSetId)
+            tms = self.supported_tms.get(tileMatrixSetId)
 
             if output_type == MediaType.html:
-                # For visualization purpose we add the tms bbox
-                data = {
-                    **data.model_dump(exclude_none=True, mode="json"),
-                    "bbox": data.bbox,
-                }
                 return self._create_html_response(
                     request,
-                    json.dumps(
-                        data,
-                    ),
+                    {
+                        **tms.model_dump(exclude_none=True, mode="json"),
+                        # For visualization purpose we add the tms bbox
+                        "bbox": tms.bbox,
+                    },
                     template_name="tilematrixset",
+                    title=f"{tileMatrixSetId} TileMatrixSet",
                 )
 
-            return data
+            return tms
 
     def _tilesets_routes(self):
         @self.router.get(
             "/collections/{collectionId}/tiles",
             response_model=model.TileSetList,
             response_class=ORJSONResponse,
             response_model_exclude_none=True,
@@ -1334,16 +1380,17 @@
                     ]
                 }
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="tilesets",
+                    title=f"{collection.id} tilesets",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}/tiles/{tileMatrixSetId}",
             response_model=model.TileSet,
@@ -1398,66 +1445,85 @@
                         "maxTileRow": matrix.matrixHeight,
                         "minTileCol": 0,
                         "maxTileCol": matrix.matrixWidth,
                     }
                     for matrix in tms
                 ]
 
+            links = [
+                {
+                    "href": self.url_for(
+                        request,
+                        "collection_tileset",
+                        collectionId=collection.id,
+                        tileMatrixSetId=tileMatrixSetId,
+                    ),
+                    "rel": "self",
+                    "type": "application/json",
+                    "title": f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
+                },
+                {
+                    "href": self.url_for(
+                        request,
+                        "tilematrixset",
+                        tileMatrixSetId=tileMatrixSetId,
+                    ),
+                    "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
+                    "type": "application/json",
+                    "title": f"Definition of '{tileMatrixSetId}' tileMatrixSet",
+                },
+                {
+                    "href": self.url_for(
+                        request,
+                        "collection_get_tile",
+                        tileMatrixSetId=tileMatrixSetId,
+                        collectionId=collection.id,
+                        z="{z}",
+                        x="{x}",
+                        y="{y}",
+                    ),
+                    "rel": "tile",
+                    "type": "application/vnd.mapbox-vector-tile",
+                    "title": "Templated link for retrieving Vector tiles",
+                    "templated": True,
+                },
+            ]
+
+            if self.with_viewer:
+                links.append(
+                    {
+                        "href": self.url_for(
+                            request,
+                            "viewer_endpoint",
+                            tileMatrixSetId=tileMatrixSetId,
+                            collectionId=collection.id,
+                        ),
+                        "type": "text/html",
+                        "rel": "data",
+                        "title": f"Map viewer for '{tileMatrixSetId}' tileMatrixSet",
+                    }
+                )
+
             data = model.TileSet.model_validate(
                 {
                     "title": f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
                     "dataType": "vector",
                     "crs": tms.crs,
                     "boundingBox": collection_bbox,
-                    "links": [
-                        {
-                            "href": self.url_for(
-                                request,
-                                "collection_tileset",
-                                collectionId=collection.id,
-                                tileMatrixSetId=tileMatrixSetId,
-                            ),
-                            "rel": "self",
-                            "type": "application/json",
-                            "title": f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
-                        },
-                        {
-                            "href": self.url_for(
-                                request,
-                                "tilematrixset",
-                                tileMatrixSetId=tileMatrixSetId,
-                            ),
-                            "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
-                            "type": "application/json",
-                            "title": f"Definition of '{tileMatrixSetId}' tileMatrixSet",
-                        },
-                        {
-                            "href": self.url_for(
-                                request,
-                                "collection_get_tile",
-                                tileMatrixSetId=tileMatrixSetId,
-                                collectionId=collection.id,
-                                z="{z}",
-                                x="{x}",
-                                y="{y}",
-                            ),
-                            "rel": "tile",
-                            "type": "application/vnd.mapbox-vector-tile",
-                            "title": "Templated link for retrieving Vector tiles",
-                        },
-                    ],
+                    "links": links,
                     "tileMatrixSetLimits": tilematrix_limit,
                 }
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.model_dump_json(exclude_none=True),
+                    data.model_dump(exclude_none=True, mode="json"),
                     template_name="tileset",
+                    title=f"{collection.id} {tileMatrixSetId} tileset",
                 )
 
             return data
 
     def _tile_routes(self):
         @self.router.get(
             "/collections/{collectionId}/tiles/{tileMatrixSetId}/{z}/{x}/{y}",
@@ -1468,14 +1534,15 @@
         )
         @self.router.get(
             "/collections/{collectionId}/tiles/{z}/{x}/{y}",
             response_class=Response,
             responses={200: {"content": {MediaType.mvt.value: {}}}},
             operation_id=".collection.vector.getTile",
             tags=["OGC Tiles API"],
+            deprecated=True,
         )
         async def collection_get_tile(
             request: Request,
             collection: Annotated[Collection, Depends(self.collection_dependency)],
             tile: Annotated[Tile, Depends(TileParams)],
             tileMatrixSetId: Annotated[
                 Literal[tuple(self.supported_tms.list())],
@@ -1551,14 +1618,15 @@
             "/collections/{collectionId}/tilejson.json",
             response_model=model.TileJSON,
             responses={200: {"description": "Return a tilejson"}},
             response_model_exclude_none=True,
             response_class=ORJSONResponse,
             operation_id=".collection.vector.getTileJSON",
             tags=["OGC Tiles API"],
+            deprecated=True,
         )
         async def collection_tilejson(
             request: Request,
             collection: Annotated[Collection, Depends(self.collection_dependency)],
             tileMatrixSetId: Annotated[
                 Literal[tuple(self.supported_tms.list())],
                 f"Identifier selecting one of the TileMatrixSetId supported (default: '{tms_settings.default_tms}')",
@@ -1652,14 +1720,15 @@
             "/collections/{collectionId}/style.json",
             response_model=model.StyleJSON,
             responses={200: {"description": "Return a StyleJSON"}},
             response_model_exclude_none=True,
             response_class=ORJSONResponse,
             operation_id=".collection.vector.getStyleJSON",
             tags=["OGC Tiles API"],
+            deprecated=True,
         )
         async def collection_stylejson(
             request: Request,
             collection: Annotated[Collection, Depends(self.collection_dependency)],
             tileMatrixSetId: Annotated[
                 Literal[tuple(self.supported_tms.list())],
                 f"Identifier selecting one of the TileMatrixSetId supported (default: '{tms_settings.default_tms}')",
@@ -1709,20 +1778,15 @@
             if tileMatrixSetId == tms_settings.default_tms:
                 minzoom = minzoom or tms_settings.default_minzoom
                 maxzoom = maxzoom or tms_settings.default_maxzoom
 
             minzoom = minzoom if minzoom is not None else tms.minzoom
             maxzoom = maxzoom if maxzoom is not None else tms.maxzoom
 
-            bounds = collection.bounds or [
-                180,
-                -85.05112877980659,
-                180,
-                85.0511287798066,
-            ]
+            bounds = list(collection.bounds) or list(tms.bbox)
 
             style_json = {
                 "name": "TiPg",
                 "sources": {
                     collection.id: {
                         "type": "vector",
                         "scheme": "xyz",
@@ -1783,27 +1847,37 @@
 
         if self.with_viewer:
 
             @self.router.get(
                 "/collections/{collectionId}/{tileMatrixSetId}/viewer",
                 response_class=HTMLResponse,
                 operation_id=".collection.vector.viewerTms",
+                deprecated=True,
+                tags=["Map Viewer"],
             )
             @self.router.get(
                 "/collections/{collectionId}/viewer",
                 response_class=HTMLResponse,
                 operation_id=".collection.vector.viewer",
+                deprecated=True,
+                tags=["Map Viewer"],
+            )
+            @self.router.get(
+                "/collections/{collectionId}/tiles/{tileMatrixSetId}/viewer",
+                response_class=HTMLResponse,
+                operation_id=".collection.vector.map",
+                tags=["Map Viewer"],
             )
             def viewer_endpoint(
                 request: Request,
                 collection: Annotated[Collection, Depends(self.collection_dependency)],
                 tileMatrixSetId: Annotated[
-                    Literal["WebMercatorQuad"],
-                    "Identifier selecting one of the TileMatrixSetId supported (default: 'WebMercatorQuad')",
-                ] = "WebMercatorQuad",
+                    Literal[tuple(self.supported_tms.list())],
+                    f"Identifier selecting one of the TileMatrixSetId supported (default: '{tms_settings.default_tms}')",
+                ] = tms_settings.default_tms,
                 minzoom: Annotated[
                     Optional[int],
                     Query(description="Overwrite default minzoom."),
                 ] = None,
                 maxzoom: Annotated[
                     Optional[int],
                     Query(description="Overwrite default maxzoom."),
@@ -1813,32 +1887,35 @@
                     Query(
                         description="Select geometry column.",
                         alias="geom-column",
                     ),
                 ] = None,
             ):
                 """Return Simple HTML Viewer for a collection."""
-                self.supported_tms.get(tileMatrixSetId)
+                tms = self.supported_tms.get(tileMatrixSetId)
 
                 tilejson_url = self.url_for(
                     request,
                     "collection_tilejson",
                     collectionId=collection.id,
                     tileMatrixSetId=tileMatrixSetId,
                 )
                 if request.query_params._list:
                     tilejson_url += f"?{urlencode(request.query_params._list)}"
 
-                return self.templates.TemplateResponse(
+                return self._create_html_response(
                     request,
-                    name="map.html",
-                    context={
+                    {
+                        "title": collection.id,
                         "tilejson_endpoint": tilejson_url,
+                        "tms": tms,
+                        "resolutions": [matrix.cellSize for matrix in tms],
                     },
-                    media_type="text/html",
+                    template_name="map",
+                    title=f"{collection.id} viewer",
                 )
 
 
 @dataclass
 class Endpoints(EndpointsFactory):
     """OGC Features and Tiles Endpoints Factory."""
```

### Comparing `tipg-0.6.3/tipg/main.py` & `tipg-0.7.0/tipg/main.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/middleware.py` & `tipg-0.7.0/tipg/middleware.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/model.py` & `tipg-0.7.0/tipg/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,16 +303,16 @@
     template: Optional[str] = None
     legend: Optional[str] = None
     scheme: Literal["xyz", "tms"] = "xyz"
     tiles: List[str]
     vector_layers: Optional[List[LayerJSON]] = None
     grids: Optional[List[str]] = None
     data: Optional[List[str]] = None
-    minzoom: int = Field(0, ge=0, le=30)
-    maxzoom: int = Field(30, ge=0, le=30)
+    minzoom: int = Field(0)
+    maxzoom: int = Field(30)
     fillzoom: Optional[int] = None
     bounds: List[float] = [180, -85.05112877980659, 180, 85.0511287798066]
     center: Optional[Tuple[float, float, int]] = None
 
     @model_validator(mode="after")
     def compute_center(self):
         """Compute center if it does not exist."""
```

### Comparing `tipg-0.6.3/tipg/settings.py` & `tipg-0.7.0/tipg/settings.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/filter/evaluate.py` & `tipg-0.7.0/tipg/filter/evaluate.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/filter/filters.py` & `tipg-0.7.0/tipg/filter/filters.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/resources/enums.py` & `tipg-0.7.0/tipg/resources/enums.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/resources/response.py` & `tipg-0.7.0/tipg/resources/response.py`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/sql/dbcatalog.sql` & `tipg-0.7.0/tipg/sql/dbcatalog.sql`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/tipg/templates/collection.html` & `tipg-0.7.0/tipg/templates/collection.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %} {% if not loop.last %}
     <li class="breadcrumb-item">
       <a href="{{ crumb.url }}/">{{ crumb.part }}</a>
     </li>
     {% else %}
     <li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
     {% endif %} {% endfor %}
 
     <li class="ml-auto json-link">
-      <a target="_blank" href="{{ url }}?f=json">JSON</a>
+      <a target="_blank" href="{{ urlq }}f=json">JSON</a>
     </li>
   </ol>
 </nav>
 
 <h1>Collection: {{ response.title or response.id }}</h1>
 
 <div class="row">
```

### Comparing `tipg-0.6.3/tipg/templates/collections.html` & `tipg-0.7.0/tipg/templates/collections.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 {% include "header.html" %}
 
 {% set show_prev_link = false %}
 {% set show_next_link = false %}
-{%  if 'items?' in url %}
-  {% set urlq = url + '&' %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
   {% else %}
   {% set urlq = url + '?' %}
 {% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=json">JSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=json">JSON</a></li>
   </ol>
 </nav>
 
 <h1>Collections</h1>
 
 <p>
   <b>Number of matching collections:</b> {{ response.numberMatched }}<br/>
```

### Comparing `tipg-0.6.3/tipg/templates/conformance.html` & `tipg-0.7.0/tipg/templates/tilematrixsets.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=json">JSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=json">JSON</a></li>
   </ol>
 </nav>
 
-<h1>{{ template.title }}Conformance</h1>
+<h1>{{ template.title }}TileMatrixSets</h1>
 
-<p>This API implements the conformance classes from standards and community specifications that are listed below.</p>
+<p>This API implements <a target="_blank" href="https://www.ogc.org/standard/tms/">TileMatrixSets</a> that are listed below.</p>
 
 <h2>Links</h2>
 <ul>
-{% for url in response.conformsTo %}
-  <li> <a target="_blank" href="{{ url }}">{{ url }}</a></li>
+{% for tms in response.tileMatrixSets %}
+  <li> <a href="{{ tms.links[0].href }}">{{ tms.id }}</a></li>
 {% endfor %}
 </ul>
 
 {% include "footer.html" %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-{% include "header.html" %}
+{% include "header.html" %} {% if params %} {% set urlq = url + '?' + params +
+'&' %} {% else %} {% set urlq = url + '?' %} {% endif %}
    1. {% for crumb in crumbs %} {% if not loop.last %}
    2. _{_{_ _c_r_u_m_b_._p_a_r_t_ _}_}
    3. {% else %}
    4. {{ crumb.part }}
    5. {% endif %} {% endfor %}
    6. _J_S_O_N
-************ {{{{ tteemmppllaattee..ttiittllee }}}}CCoonnffoorrmmaannccee ************
-This API implements the conformance classes from standards and community
-specifications that are listed below.
+************ {{{{ tteemmppllaattee..ttiittllee }}}}TTiilleeMMaattrriixxSSeettss ************
+This API implements _T_i_l_e_M_a_t_r_i_x_S_e_t_s that are listed below.
 ********** LLiinnkkss **********
-    * {% for url in response.conformsTo %}
-    * _{_{_ _u_r_l_ _}_}
+    * {% for tms in response.tileMatrixSets %}
+    * _{_{_ _t_m_s_._i_d_ _}_}
     * {% endfor %}
 {% include "footer.html" %}
```

### Comparing `tipg-0.6.3/tipg/templates/header.html` & `tipg-0.7.0/tipg/templates/header.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <title>{{ template.title }}</title>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.5.3/css/bootstrap.min.css" />
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.7.1/leaflet.css" />
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.css" />
     <style>
       html { position: relative; min-height: 100%; }
       body { padding-top: 5rem; margin-bottom: 40px; }
       #page { padding: 1.5rem 1.5rem; }
       .navbar { border-bottom: 8px solid #3333A4; }
       .navbar-brand { font-size: 2rem; color: #3333A4 !important; text-shadow: 2px 2px 4px #ccc; }
       .json-link { font-weight: normal; }
     </style>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
     <script src="https://files.dnr.state.mn.us/lib/bootstrap4/javascripts/bootstrap.min.js"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.7.1/leaflet.js"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.js"></script>
   </head>
   <body>
     <nav class="navbar navbar-expand-md navbar-light fixed-top bg-light">
       <a href="{{ template.api_root }}/">
         <img style="max-width: 60px;height: auto;" src="data:image/png;base64,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" alt="Development Seed">
       </a>
       <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar" aria-controls="navbar" aria-expanded="false" aria-label="Toggle navigation">
```

### Comparing `tipg-0.6.3/tipg/templates/item.html` & `tipg-0.7.0/tipg/templates/item.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=geojson">GeoJSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=geojson">GeoJSON</a></li>
   </ol>
 </nav>
 
 <h1>Collection Item: {{ response.id }}</h1>
 
 <div class="row">
   <div class="col-sm">
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% include "header.html" %}
+{% include "header.html" %} {% if params %} {% set urlq = url + '?' + params +
+'&' %} {% else %} {% set urlq = url + '?' %} {% endif %}
    1. {% for crumb in crumbs %} {% if not loop.last %}
    2. _{_{_ _c_r_u_m_b_._p_a_r_t_ _}_}
    3. {% else %}
    4. {{ crumb.part }}
    5. {% endif %} {% endfor %}
    6. _G_e_o_J_S_O_N
 ************ CCoolllleeccttiioonn IItteemm:: {{{{ rreessppoonnssee..iidd }}}} ************
```

### Comparing `tipg-0.6.3/tipg/templates/items.html` & `tipg-0.7.0/tipg/templates/items.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% include "header.html" %}
 
 {% set show_prev_link = false %}
 {% set show_next_link = false %}
-{%  if 'items?' in url %}
-  {% set urlq = url + '&' %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
   {% else %}
   {% set urlq = url + '?' %}
 {% endif %}
 
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
```

### Comparing `tipg-0.6.3/tipg/templates/landing.html` & `tipg-0.7.0/tipg/templates/landing.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=json">JSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=json">JSON</a></li>
   </ol>
 </nav>
 
 <h1>{{ response.title }}</h1>
 <p>
   {{ response.description }}
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% include "header.html" %}
+{% include "header.html" %} {% if params %} {% set urlq = url + '?' + params +
+'&' %} {% else %} {% set urlq = url + '?' %} {% endif %}
    1. {% for crumb in crumbs %} {% if not loop.last %}
    2. _{_{_ _c_r_u_m_b_._p_a_r_t_ _}_}
    3. {% else %}
    4. {{ crumb.part }}
    5. {% endif %} {% endfor %}
    6. _J_S_O_N
 ************ {{{{ rreessppoonnssee..ttiittllee }}}} ************
```

### Comparing `tipg-0.6.3/tipg/templates/queryables.html` & `tipg-0.7.0/tipg/templates/tilesets.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=schemajson">JSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=json">JSON</a></li>
   </ol>
 </nav>
 
-<h1>Collection: {{ response.title or response.id }}</h1>
+<h1>{{ template.title }} TileSet list</h1>
+
+<h2>Links</h2>
+<ul>
+{% for tileset in response.tilesets %}
+  <li> <a href="{{ tileset.links[0].href }}">{{ tileset.title }}</a></li>
+{% endfor %}
+</ul>
 
-<div class="row">
-  <div class="col-sm">
-    <h2>Queryables</h2>
-    <ul>
-    {% for k,v in response.properties.items() %}
-      <li>{% if '$ref' in v %}
-          <a href="{{ v['$ref'] }}">{{ k }}</a>
-          {% else %}
-          {{ k }}: {{ v['type'] }}
-          {% endif %}
-    {% endfor %}
-    </ul>
-  </div>
-</div>
 
 {% include "footer.html" %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-{% include "header.html" %}
+{% include "header.html" %} {% if params %} {% set urlq = url + '?' + params +
+'&' %} {% else %} {% set urlq = url + '?' %} {% endif %}
    1. {% for crumb in crumbs %} {% if not loop.last %}
    2. _{_{_ _c_r_u_m_b_._p_a_r_t_ _}_}
    3. {% else %}
    4. {{ crumb.part }}
    5. {% endif %} {% endfor %}
    6. _J_S_O_N
-************ CCoolllleeccttiioonn:: {{{{ rreessppoonnssee..ttiittllee oorr rreessppoonnssee..iidd }}}} ************
-********** QQuueerryyaabblleess **********
-    * {% for k,v in response.properties.items() %}
-    * {% if '$ref' in v %} _{_{_ _k_ _}_} {% else %} {{ k }}: {{ v['type'] }} {% endif
-      %} {% endfor %}
+************ {{{{ tteemmppllaattee..ttiittllee }}}} TTiilleeSSeett lliisstt ************
+********** LLiinnkkss **********
+    * {% for tileset in response.tilesets %}
+    * _{_{_ _t_i_l_e_s_e_t_._t_i_t_l_e_ _}_}
+    * {% endfor %}
 {% include "footer.html" %}
```

### Comparing `tipg-0.6.3/tipg/templates/tilematrixset.html` & `tipg-0.7.0/tipg/templates/tilematrixset.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=json">JSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=json">JSON</a></li>
   </ol>
 </nav>
 
 <h1>{{ response.title or response.id }}</h1>
 
 <div class="row">
   <div class="col-sm">
```

### Comparing `tipg-0.6.3/tipg/templates/tileset.html` & `tipg-0.7.0/tipg/templates/tileset.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 {% include "header.html" %}
+{% if params %}
+  {% set urlq = url + '?' + params + '&' %}
+  {% else %}
+  {% set urlq = url + '?' %}
+{% endif %}
 
 <nav aria-label="breadcrumb">
   <ol class="breadcrumb bg-light">
     {% for crumb in crumbs %}
       {% if not loop.last %}
     <li class="breadcrumb-item"><a href="{{ crumb.url }}/">{{ crumb.part }}</a></li>
       {% else %}<li class="breadcrumb-item active" aria-current="page">{{ crumb.part }}</li>
       {% endif %}
     {% endfor %}
 
-    <li class="ml-auto json-link"><a target="_blank" href="{{ url }}?f=json">JSON</a></li>
+    <li class="ml-auto json-link"><a target="_blank" href="{{ urlq }}f=json">JSON</a></li>
   </ol>
 </nav>
 
 <h1>{{ response.title}}</h1>
 
 <div class="row" style="margin-top: 30px;">
   <div class="col-sm">
```

### Comparing `tipg-0.6.3/.gitignore` & `tipg-0.7.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -108,7 +108,8 @@
 .benchmarks/
 
 .pgdata/
 docs/src/api/*
 
 traefik.toml
 routes.toml
+.tms/
```

### Comparing `tipg-0.6.3/LICENSE` & `tipg-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/README.md` & `tipg-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/pyproject.toml` & `tipg-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tipg-0.6.3/PKG-INFO` & `tipg-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tipg
-Version: 0.6.3
+Version: 0.7.0
 Summary: Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
 Project-URL: Homepage, https://developmentseed.org/tipg
 Project-URL: Source, https://github.com/developmentseed/tipg
 Project-URL: Documentation, https://developmentseed.org/tipg/
 Author-email: Vincent Sarago <vincent@developmentseed.org>, David Bitner <david@developmentseed.org>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tipg Version: 0.6.3 Summary: Simple and Fast
+Metadata-Version: 2.3 Name: tipg Version: 0.7.0 Summary: Simple and Fast
 Geospatial OGC Features and Tiles API for PostGIS. Project-URL: Homepage,
 https://developmentseed.org/tipg Project-URL: Source, https://github.com/
 developmentseed/tipg Project-URL: Documentation, https://developmentseed.org/
 tipg/ Author-email: Vincent Sarago
 developmentseed.org>, David Bitner
 developmentseed.org> License: MIT License Copyright (c) 2022 Development Seed
 Permission is hereby granted, free of charge, to any person obtaining a copy of
```

