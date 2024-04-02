# Comparing `tmp/clean_ioc-0.8.0.tar.gz` & `tmp/clean_ioc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.8.0.tar", max compression
+gzip compressed data, was "clean_ioc-0.9.0.tar", max compression
```

## Comparing `clean_ioc-0.8.0.tar` & `clean_ioc-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     2051 2023-08-31 08:36:53.269066 clean_ioc-0.8.0/CHANGES.rst
--rw-r--r--   0        0        0     1067 2023-01-24 06:53:30.309697 clean_ioc-0.8.0/LICENSE
--rw-r--r--   0        0        0    20308 2024-01-24 14:07:23.249191 clean_ioc-0.8.0/README.md
--rw-r--r--   0        0        0    43351 2024-01-25 18:25:19.680086 clean_ioc-0.8.0/clean_ioc/__init__.py
--rw-r--r--   0        0        0     1790 2024-01-23 15:03:27.389899 clean_ioc-0.8.0/clean_ioc/bundles.py
--rw-r--r--   0        0        0     1261 2024-01-18 16:05:33.367371 clean_ioc-0.8.0/clean_ioc/ext/fastapi/__init__.py
--rw-r--r--   0        0        0      680 2024-01-24 13:17:58.247187 clean_ioc-0.8.0/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-03-01 21:27:40.225942 clean_ioc-0.8.0/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0      558 2023-07-26 15:24:12.965511 clean_ioc-0.8.0/clean_ioc/list_reduction_filters.py
--rw-r--r--   0        0        0     1251 2024-01-17 20:22:28.452934 clean_ioc-0.8.0/clean_ioc/modules.py
--rw-r--r--   0        0        0      405 2023-07-26 19:42:13.609646 clean_ioc-0.8.0/clean_ioc/parent_context_filters.py
--rw-r--r--   0        0        0     2228 2023-07-05 20:43:32.736456 clean_ioc-0.8.0/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-01-24 16:24:19.736817 clean_ioc-0.8.0/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6555 2023-07-26 09:59:03.030145 clean_ioc-0.8.0/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1399 2024-01-17 20:22:28.453624 clean_ioc-0.8.0/clean_ioc/utils.py
--rw-r--r--   0        0        0      601 2024-01-24 14:05:46.041128 clean_ioc-0.8.0/clean_ioc/value_factories.py
--rw-r--r--   0        0        0     1415 2024-01-24 14:00:53.928345 clean_ioc-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    21037 1970-01-01 00:00:00.000000 clean_ioc-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2051 2023-08-31 08:36:53.269066 clean_ioc-0.9.0/CHANGES.rst
+-rw-r--r--   0        0        0     1067 2023-01-24 06:53:30.309697 clean_ioc-0.9.0/LICENSE
+-rw-r--r--   0        0        0    20308 2024-01-24 14:07:23.249191 clean_ioc-0.9.0/README.md
+-rw-r--r--   0        0        0    45213 2024-01-29 21:28:48.975881 clean_ioc-0.9.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0     1790 2024-01-23 15:03:27.389899 clean_ioc-0.9.0/clean_ioc/bundles.py
+-rw-r--r--   0        0        0       34 2024-01-29 21:28:48.960772 clean_ioc-0.9.0/clean_ioc/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     1261 2024-01-29 21:28:48.961191 clean_ioc-0.9.0/clean_ioc/ext/fastapi/core.py
+-rw-r--r--   0        0        0      680 2024-01-24 13:17:58.247187 clean_ioc-0.9.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-03-01 21:27:40.225942 clean_ioc-0.9.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0      558 2023-07-26 15:24:12.965511 clean_ioc-0.9.0/clean_ioc/list_reduction_filters.py
+-rw-r--r--   0        0        0     1251 2024-01-25 23:41:53.115843 clean_ioc-0.9.0/clean_ioc/modules.py
+-rw-r--r--   0        0        0      405 2023-07-26 19:42:13.609646 clean_ioc-0.9.0/clean_ioc/parent_context_filters.py
+-rw-r--r--   0        0        0     2228 2023-07-05 20:43:32.736456 clean_ioc-0.9.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-01-24 16:24:19.736817 clean_ioc-0.9.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6555 2023-07-26 09:59:03.030145 clean_ioc-0.9.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1399 2024-01-17 20:22:28.453624 clean_ioc-0.9.0/clean_ioc/utils.py
+-rw-r--r--   0        0        0      603 2024-01-29 21:28:48.962161 clean_ioc-0.9.0/clean_ioc/value_factories.py
+-rw-r--r--   0        0        0     1415 2024-01-29 21:28:48.976503 clean_ioc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    21037 1970-01-01 00:00:00.000000 clean_ioc-0.9.0/PKG-INFO
```

### Comparing `clean_ioc-0.8.0/CHANGES.rst` & `clean_ioc-0.9.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/LICENSE` & `clean_ioc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/README.md` & `clean_ioc-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/__init__.py` & `clean_ioc-0.9.0/clean_ioc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,44 @@
 )
 import inspect
 
 
 TService = TypeVar("TService")
 
 
-class _empty:
+class SingletonMeta(type):
+    __INSTANCE__ = None
+
+    def __call__(cls, *args, **kwargs):
+        if cls.__INSTANCE__ is None:
+            cls.__INSTANCE__ = super().__call__(*args, **kwargs)
+
+        return cls.__INSTANCE__
+
+
+class _empty(metaclass=SingletonMeta):
+    def __bool__(self):
+        return False
+
+
+class _unknown(metaclass=SingletonMeta):
     def __bool__(self):
         return False
 
 
+EMPTY = _empty()
+UNKNOWN = _unknown()
+
+
 class ArgInfo:
     def __init__(self, name: str, arg_type: type, default_value: Any):
         self.name = name
         self.arg_type = arg_type
         self.default_value = (
-            _empty if default_value == inspect._empty else default_value
+            _empty() if default_value == inspect._empty else default_value
         )
 
 
 def get_arg_info(
     subject: Callable, local_ns: dict = {}, global_ns: dict | None = None
 ) -> dict[str, ArgInfo]:
     arg_spec_fn = subject if inspect.isfunction(subject) else subject.__init__
@@ -88,45 +107,83 @@
     parent: __Node__
     children: list[__Node__]
     decorator: __Node__
     decorated: __Node__
     pre_configured_by: __Node__
     pre_configures: __Node__
     registration_name: str | None = None
+    instance: Any = UNKNOWN
+    lifespan: Lifespan
+
+    @property
+    def implementation_type(self):
+        return (
+            self.implementation
+            if isinstance(self.implementation, type)
+            else type(self.implementation)
+        )
+
+    @property
+    def instance_type(self):
+        return type(self.instance)
 
     @property
     def generic_mapping(self):
         return get_typevar_to_type_mapping(self.service_type)
 
     @property
-    def bottom_decorated(self):
-        bottom = self.implementation
-        decorated = self.decorated
-        while decorated:
-            bottom = decorated.implementation
-            decorated = decorated.decorated
-        return bottom
+    def bottom_decorated_node(self):
+        if not self.decorated:
+            return self
+        return self.decorated.bottom_decorated_node
+
+    @property
+    def top_decorated_node(self):
+        if not self.decorator:
+            return self
+        return self.decorator.top_decorated_node
 
     def has_dependant_service_type(self, service_type: type) -> bool:
         for child in self.children:
             if child.service_type == service_type:
                 return True
             if child.has_dependant_service_type(service_type):
                 return True
         return False
 
+    def has_dependant_implementation_type(self, implementation_type: type) -> bool:
+        for child in self.children:
+            if child.implementation_type == implementation_type:
+                return True
+            if child.has_dependant_implementation_type(implementation_type):
+                return True
+        return False
+
+    def has_dependant_instance_type(self, instance_type: type) -> bool:
+        for child in self.children:
+            if child.instance_type == instance_type:
+                return True
+            if child.has_dependant_instance_type(instance_type):
+                return True
+        return False
+
+    def __repr__(self) -> str:
+        return f"{self.service_type}--{self.implementation}"
+
 
 class EmptyNode(__Node__):
     def __init__(self):
         self.service_type = _empty
         self.implementation = _empty
         self.parent = self
         self.decorated = self
         self.pre_configured_by = self
         self.registration_name = None
+        self.instance = EMPTY
+        self.lifespan = Lifespan.singleton
 
     def __bool__(self):
         return False
 
     @property
     def children(self):
         return ()
@@ -146,29 +203,53 @@
         self.registration_name: str | None = registration_name
         self.parent = EmptyNode()
         self.children = []
         self.decorated = EmptyNode()
         self.decorator = EmptyNode()
         self.pre_configured_by = EmptyNode()
         self.pre_configures = EmptyNode()
+        self.instance = UNKNOWN
+
+    def set_instance(self, instance: Any):
+        if self.instance is UNKNOWN:
+            self.instance = instance
+        else:
+            raise Exception("Cannot set instance on a node that already has one")
 
     def add_child(self, child_node: DependencyNode):
         self.children.append(child_node)
         child_node.parent = self
 
     def add_decorator(self, decorator_node: DependencyNode):
         self.decorator = decorator_node
         decorator_node.decorated = self
         decorator_node.parent = self.parent
+        self.parent.children.append(decorator_node)
+        self.parent.children.remove(self)
 
     def add_pre_configuration(self, pre_configuration_node: DependencyNode):
         self.pre_configured_by = pre_configuration_node
         pre_configuration_node.pre_configures = self
 
 
+class RootNode(DependencyNode):
+    def __init__(self, root_dependency: RootDependency):
+        self.root_dependency = root_dependency
+        super().__init__(
+            service_type=root_dependency.service_type,
+            implementation=root_dependency.parent_implementation,
+            lifespan=Lifespan.once_per_graph,
+        )
+
+    def resolve(self, context: ResolvingContext):
+        self.root_dependency.resolve(context, self)
+        self.set_instance(self.children[0].instance)
+        return self
+
+
 class DependencyContext:
     def __init__(self, name: str, dependency_node: DependencyNode):
         self.name = name
         self.service_type = dependency_node.service_type
         self.implementation = dependency_node.implementation
         self.parent = dependency_node.parent
         self.decorated = dependency_node.decorated
@@ -181,26 +262,14 @@
 
 
 class DecoratorContext:
     def __init__(self, decorated: DependencyNode):
         self.decorated = decorated
 
 
-class DependencyGraph:
-    def __init__(self, root_node: DependencyNode, resolved_object: Any):
-        self.root_node = root_node
-        self.resolved_instance = resolved_object
-        self.children: list[DependencyGraph] = []
-
-    def has_dependant_service_type(self, service_type: type) -> bool:
-        if self.root_node.service_type == service_type:
-            return True
-        return self.root_node.has_dependant_service_type(service_type)
-
-
 class CannotResolveException(Exception):
     def __init__(self):
         self.stack = deque()
 
     def append(self, d: Dependency):
         self.stack.appendleft(d)
 
@@ -263,29 +332,40 @@
     def resolve(self, context: ResolvingContext, dependency_node: DependencyNode):
         parent_context = ParentContext(paramater_name=self.name, parent=dependency_node)
         dependency_context = DependencyContext(
             name=self.name, dependency_node=dependency_node
         )
         value = self.settings.value_factory(self.default_value, dependency_context)
 
-        if not value == _empty:
+        if value is not EMPTY:
             return value
 
         if self.is_dependency_context:
             return DependencyContext(name=self.name, dependency_node=dependency_node)
 
         if self.generic_collection_type:
             regs = context.find_registrations(
                 service_type=self.service_type.__args__[0],  # type: ignore
                 registration_filter=self.settings.filter,
                 registration_list_reducing_filter=self.settings.list_reducing_filter,
                 parent_context=parent_context,
             )
-            generator = (r.build(context, dependency_node) for r in regs)
-            return self.generic_collection_type(generator)
+            sequence_node = DependencyNode(
+                service_type=self.service_type,
+                implementation=self.generic_collection_type,
+                lifespan=Lifespan.transient,
+            )
+
+            dependency_node.add_child(sequence_node)
+
+            generator = (r.build(context, sequence_node) for r in regs)
+            collection = self.generic_collection_type(generator)
+            sequence_node.set_instance(collection)
+
+            return collection
         try:
             reg = context.find_registration(
                 service_type=self.service_type,
                 registration_filter=self.settings.filter,
                 parent_context=parent_context,
             )
             return reg.build(context, dependency_node)
@@ -301,27 +381,24 @@
 
     def __init__(self, service_type: type, settings: DependencySettings):
         super().__init__(
             name="__ROOT__",
             parent_implementation=RootDependency.__PARENT_ROOT__,
             service_type=service_type,
             settings=settings,
-            default_value=_empty,
+            default_value=_empty(),
         )
 
     def resolve_instance(self, context: ResolvingContext) -> Any:
-        graph = self.resolve_dependency_graph(context)
-        return graph.resolved_instance
+        root_node = self.resolve_dependency_graph(context)
+        return root_node.instance
 
-    def resolve_dependency_graph(self, context: ResolvingContext) -> DependencyGraph:
-        root_node = DependencyNode(
-            RootDependency, self.parent_implementation, lifespan=Lifespan.once_per_graph
-        )
-        resolved_object = self.resolve(context=context, dependency_node=root_node)
-        return DependencyGraph(root_node=root_node, resolved_object=resolved_object)
+    def resolve_dependency_graph(self, context: ResolvingContext) -> RootNode:
+        root_node = RootNode(self)
+        return root_node.resolve(context)
 
 
 class ImplementationCreator:
     def __init__(
         self,
         creator_function: Callable,
         dependency_config: dict[str, DependencySettings] = {},
@@ -330,16 +407,16 @@
         self.creator_function = creator_function
         self.dependencies: dict[str, Dependency] = self._get_dependencies(
             self.creator_function, self.dependency_config
         )
 
     @classmethod
     def _get_default_value(cls, paramater: inspect.Parameter):
-        default_value = _empty
-        if not paramater.default == inspect._empty:
+        default_value = EMPTY
+        if not paramater.default == inspect._empty():
             default_value = paramater.default
         return default_value
 
     @classmethod
     def _get_dependencies(
         cls,
         creator_function: Callable,
@@ -359,15 +436,15 @@
 
         for extra_kwarg in set(dependency_config.keys()) ^ set(dependencies.keys()):
             dependencies[extra_kwarg] = Dependency(
                 name=extra_kwarg,
                 parent_implementation=creator_function,
                 service_type=Any,
                 settings=dependency_config[extra_kwarg],
-                default_value=_empty,
+                default_value=_empty(),
             )
 
         return dependencies
 
     def create(
         self,
         context: ResolvingContext,
@@ -500,78 +577,86 @@
     def has_tag(self, name: str, value: str | None):
         if value is not None:
             return any(t.name == name and t.value == value for t in self.tags)
 
         return any(t.name == name for t in self.tags)
 
     def build(self, context: ResolvingContext, parent_node: DependencyNode):
-        my_node = DependencyNode(
+        cached_node = context.get_cached(self.id)
+        if cached_node:
+            parent_node.add_child(cached_node)
+            return cached_node.instance
+
+        new_instance_node = DependencyNode(
             service_type=self.service_type,
             implementation=self.implementation,
             lifespan=self.lifespan,
             registration_name=self.name,
         )
 
-        parent_node.add_child(my_node)
+        parent_node.add_child(new_instance_node)
 
         pre_configurations = context.find_pre_configurations_that_apply(self)
 
         for pre_configuration in pre_configurations:
             pre_configuration_node = DependencyNode(
                 self.service_type,
                 pre_configuration.configuration_fn,
                 lifespan=Lifespan.singleton,
             )
-            my_node.add_pre_configuration(pre_configuration_node)
+            new_instance_node.add_pre_configuration(pre_configuration_node)
 
             pre_configuration.run(context, pre_configuration_node)
+            pre_configuration_node.set_instance(pre_configuration)
+
+        built_instance = self.creator.create(context, new_instance_node)
+
+        new_instance_node.set_instance(built_instance)
+
+        decorator_context = DecoratorContext(decorated=new_instance_node)
+        top_decorated_node = new_instance_node
 
-        cached_instance = context.get_cached(self.id)
-        if not cached_instance == _empty:
-            return cached_instance
-        built_instance = self.creator.create(context, my_node)
-        decorator_context = DecoratorContext(decorated=my_node)
-        decorated_node = my_node
         for dec in context.find_decorators_that_apply(self, decorator_context):
-            next_dec_node = DependencyNode(
+            next_decorated_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=dec.decorator_type,
                 lifespan=self.lifespan,
             )
-            decorated_node.add_decorator(next_dec_node)
-            built_instance = dec.decorate(built_instance, context, next_dec_node)
-            decorated_node = next_dec_node
+            top_decorated_node.add_decorator(next_decorated_node)
+            built_instance = dec.decorate(built_instance, context, next_decorated_node)
+            next_decorated_node.set_instance(built_instance)
+            top_decorated_node = next_decorated_node
 
-        context.new_instance_created(self, built_instance, decorated_node)
+        context.new_instance_created(self, top_decorated_node)
         return built_instance
 
 
 class Registry:
     def __init__(self):
         self._registrations: dict[type, deque[Registration]] = defaultdict(deque)
         self._decorators: dict[type, deque[Decorator]] = defaultdict(deque)
         self._pre_configurations: dict[type, deque[PreConfiguration]] = defaultdict(
             deque
         )
-        self._singletons: dict[str, Any] = {}
+        self._singletons: dict[str, DependencyNode] = {}
         self._run_preconfigurations: list[str] = []
 
     def add_registration(self, registration: Registration):
         self._registrations[registration.service_type].appendleft(registration)
 
     def add_decorator(self, decorator: Decorator):
         self._decorators[decorator.service_type].appendleft(decorator)
 
     def add_pre_configuration(self, pre_configuration: PreConfiguration):
         self._pre_configurations[pre_configuration.service_type].appendleft(
             pre_configuration
         )
 
-    def add_singleton_instance(self, registration_id: str, instance: Any):
-        self._singletons[registration_id] = instance
+    def add_singleton_instance(self, registration: Registration, node: DependencyNode):
+        self._singletons[registration.id] = node
 
     def mark_pre_configuration_as_run(self, pre_configuration_id):
         self._run_preconfigurations.append(pre_configuration_id)
 
     def get_registrations(self, service_type: type):
         return self._registrations[service_type]
 
@@ -593,53 +678,47 @@
         return self._run_preconfigurations
 
 
 class DependencyCache:
     def __init__(self, registry: Registry, scope: Scope):
         self.registry = registry
         self.scope = scope
-        self._current_items = {
+        self._current_items: dict[str, DependencyNode] = {
             **{k: v for k, v in registry.singletons.items()},
             **{k: v for k, v in scope.scoped_instances.items()},
         }
 
-    def get(self, registration_id: str):
-        instance = self._current_items.get(registration_id, _empty)
-        if instance is not _empty:
-            return instance
-
-        instance = self.scope.scoped_instances.get(registration_id, _empty)
-        if instance is not _empty:
-            self._current_items[registration_id] = instance
-            return instance
-
-        instance = self.registry.singletons.get(registration_id, _empty)
-        if instance is not _empty:
-            self._current_items[registration_id] = instance
+    def get(self, registration_id: str) -> DependencyNode | None:
+        node = self._current_items.get(registration_id)
+        if node:
+            return node
+
+        node = self.scope.scoped_instances.get(registration_id)
+        if node:
+            self._current_items[registration_id] = node
+            return node
+
+        node = self.registry.singletons.get(registration_id)
+        if node:
+            self._current_items[registration_id] = node
+            return node
 
-        return instance
+        return None
 
-    def put(
-        self, registration: Registration, instance: Any, dependency_node: DependencyNode
-    ):
+    def put(self, registration: Registration, dependency_node: DependencyNode):
         if registration.lifespan == Lifespan.singleton:
-            self.registry.add_singleton_instance(
-                registration_id=registration.id,
-                instance=instance,
-            )
+            self.registry.add_singleton_instance(registration, dependency_node)
         elif registration.lifespan == Lifespan.scoped:
             self.scope.add_scoped_instance(
-                registration.id,
-                registration.service_type,
-                instance,
-                registration.scoped_teardown,
+                registration,
+                dependency_node,
             )
 
         if registration.lifespan >= Lifespan.once_per_graph:
-            self._current_items[registration.id] = instance
+            self._current_items[registration.id] = dependency_node
 
 
 class ResolvingContext:
     def __init__(self, registry: Registry, scope: Scope):
         self.registry = registry
         self.scope = scope
         self._cache = DependencyCache(registry=registry, scope=scope)
@@ -719,25 +798,19 @@
         return [
             c
             for c in self.registry.get_pre_configurations(registration.service_type)
             if c.id not in self.registry.run_pre_configurations
             and c.filter(registration)
         ]
 
-    def get_cached(self, reg_id: str) -> Any:
+    def get_cached(self, reg_id: str) -> DependencyNode | None:
         return self._cache.get(reg_id)
 
-    def new_instance_created(
-        self, registration: Registration, instance: Any, dependency_node: DependencyNode
-    ):
-        self._cache.put(
-            registration=registration,
-            instance=instance,
-            dependency_node=dependency_node,
-        )
+    def new_instance_created(self, registration: Registration, node: DependencyNode):
+        self._cache.put(registration=registration, dependency_node=node)
 
     def mark_pre_configuration_as_ran(self, preconfiguration_id: str):
         self.registry.mark_pre_configuration_as_run(preconfiguration_id)
 
 
 class Resolver(abc.ABC):
     @abc.abstractmethod
@@ -752,16 +825,15 @@
 
 
 class Scope(Resolver):
     def __init__(
         self,
     ):
         self._registrations: dict[type, deque[Registration]] = defaultdict(deque)
-        self._scoped_instances: dict[str, Any] = {}
-        self._resolved_instances: dict[type, deque[Any]] = defaultdict(deque)
+        self._scoped_instances: dict[str, DependencyNode] = {}
         self._sync_teardowns: dict[str, Callable] = {}
         self._async_teardowns: dict[str, Callable] = {}
 
     async def __aenter__(self):
         await self.before_start_async()
         return self
 
@@ -788,37 +860,30 @@
         pass
 
     async def after_finish_async(self):
         pass
 
     async def _run_async_teardowns(self):
         for registration_id, teardown_fn in self._async_teardowns.items():
-            instance = self._scoped_instances[registration_id]
-            await teardown_fn(instance)
+            cached_dependency = self._scoped_instances[registration_id]
+            await teardown_fn(cached_dependency.instance)
 
     def _run_sync_teardowns(self):
         for registration_id, teardown_fn in self._sync_teardowns.items():
-            instance = self._scoped_instances[registration_id]
-            teardown_fn(instance)
+            cached_dependency = self._scoped_instances[registration_id]
+            teardown_fn(cached_dependency.instance)
 
-    def add_scoped_instance(
-        self,
-        registration_id: str,
-        service_type: type,
-        instance: Any,
-        teardown: Callable | None,
-    ):
-        self._scoped_instances[registration_id] = instance
-        self._resolved_instances[service_type].appendleft(instance)
-        if teardown:
-            is_async = inspect.iscoroutinefunction(teardown)
+    def add_scoped_instance(self, registration: Registration, node: DependencyNode):
+        self._scoped_instances[registration.id] = node
+        if registration.scoped_teardown:
+            is_async = inspect.iscoroutinefunction(registration.scoped_teardown)
             if is_async:
-                self._async_teardowns[registration_id] = teardown
+                self._async_teardowns[registration.id] = registration.scoped_teardown
             else:
-                self._sync_teardowns[registration_id] = teardown
+                self._sync_teardowns[registration.id] = registration.scoped_teardown
 
     @abc.abstractmethod
     def register(
         self,
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
@@ -832,19 +897,14 @@
     def get_registrations(self, service_tyep):
         return self._registrations[service_tyep]
 
     @property
     def scoped_instances(self):
         return self._scoped_instances
 
-    def get_resolved_instances(
-        self, service_type: type[TService]
-    ) -> Sequence[TService]:
-        return self._resolved_instances[service_type]
-
 
 class ContainerScope(Scope):
     def __init__(self, container: Container):
         super().__init__()
         self._container = container
         self.register(ContainerScope, instance=self)
         self.register(Resolver, instance=self)
@@ -1209,18 +1269,18 @@
     ) -> TService:
         d = RootDependency(service_type, DependencySettings(filter=filter))
         context = ResolvingContext(self.registry, scope)
         return d.resolve_instance(context)
 
     def resolve_dependency_graph(
         self,
-        service_type: type[TService],
+        service_type: type,
         filter: RegistrationFilter = _default_registration_filter,
         scope: Scope = EmptyContainerScope(),
-    ) -> DependencyGraph:
+    ) -> __Node__:
         d = RootDependency(service_type, DependencySettings(filter=filter))
         context = ResolvingContext(self.registry, scope)
         return d.resolve_dependency_graph(context)
 
     def new_scope(
         self, ScopeClass: Type[ContainerScope] = ContainerScope, *args, **kwargs
     ) -> Scope:
```

### Comparing `clean_ioc-0.8.0/clean_ioc/bundles.py` & `clean_ioc-0.9.0/clean_ioc/bundles.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/ext/fastapi/__init__.py` & `clean_ioc-0.9.0/clean_ioc/ext/fastapi/core.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/factories.py` & `clean_ioc-0.9.0/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/functional_utils.py` & `clean_ioc-0.9.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/list_reduction_filters.py` & `clean_ioc-0.9.0/clean_ioc/list_reduction_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/modules.py` & `clean_ioc-0.9.0/clean_ioc/modules.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/registration_filters.py` & `clean_ioc-0.9.0/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/type_filters.py` & `clean_ioc-0.9.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/typing_utils.py` & `clean_ioc-0.9.0/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/utils.py` & `clean_ioc-0.9.0/clean_ioc/utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.8.0/clean_ioc/value_factories.py` & `clean_ioc-0.9.0/clean_ioc/value_factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
     Returns:
         None
     """
     return constant(value)
 
 
-dont_use_default_parameter = constant(_empty)
+dont_use_default_parameter = constant(_empty())
```

### Comparing `clean_ioc-0.8.0/pyproject.toml` & `clean_ioc-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.8.0"
+version = "0.9.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
```

### Comparing `clean_ioc-0.8.0/PKG-INFO` & `clean_ioc-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.8.0
+Version: 0.9.0
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

