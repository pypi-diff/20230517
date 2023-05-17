# Comparing `tmp/clean_ioc-0.0.6.tar.gz` & `tmp/clean_ioc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.0.6.tar", max compression
+gzip compressed data, was "clean_ioc-0.1.0.tar", max compression
```

## Comparing `clean_ioc-0.0.6.tar` & `clean_ioc-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/LICENSE
--rw-r--r--   0        0        0    14851 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/README.md
--rw-r--r--   0        0        0    26548 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/clean_ioc/__init__.py
--rw-r--r--   0        0        0      674 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0     1811 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6537 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1112 2023-05-15 21:22:31.088536 clean_ioc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    16063 1970-01-01 00:00:00.000000 clean_ioc-0.0.6/setup.py
--rw-r--r--   0        0        0    15478 1970-01-01 00:00:00.000000 clean_ioc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 21:04:51.684575 clean_ioc-0.1.0/LICENSE
+-rw-r--r--   0        0        0    14851 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/README.md
+-rw-r--r--   0        0        0    27728 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0      674 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0     1811 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6537 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1125 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16063 1970-01-01 00:00:00.000000 clean_ioc-0.1.0/setup.py
+-rw-r--r--   0        0        0    15491 1970-01-01 00:00:00.000000 clean_ioc-0.1.0/PKG-INFO
```

### Comparing `clean_ioc-0.0.6/LICENSE` & `clean_ioc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/README.md` & `clean_ioc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/clean_ioc/__init__.py` & `clean_ioc-0.1.0/clean_ioc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,19 @@
         self.decorated = dependency_node.decorated
 
 
 class DependencyGraph:
     def __init__(self, root_node: DependencyNode, resolved_object: Any):
         self.root_node = root_node
         self.resolved_object = resolved_object
+        self.children: list[DependencyGraph] = []
+
+    def add_child(self, child_graph: DependencyGraph):
+        self.children.append(child_graph)
+        self.root_node.add_child(child_graph.root_node)
 
 
 class CannotResolveException(Exception):
     def __init__(self):
         self.stack = deque()
 
     def append(self, d: Dependency):
@@ -211,20 +216,19 @@
             name="__ROOT__",
             parent_implementation=RootDependency.__PARENT_ROOT__,
             service_type=service_type,
             settings=settings,
             default_value=_empty,
         )
 
-    def run_resolve(self, context: ResolvingContext) -> DependencyGraph:
+    def resolve_dependency_graph(self, context: ResolvingContext) -> DependencyGraph:
         root_node = DependencyNode(
             RootDependency, self.parent_implementation, lifespan=Lifespan.transient
         )
         resolved_object = self.resolve(context=context, depedency_node=root_node)
-
         return DependencyGraph(root_node=root_node, resolved_object=resolved_object)
 
 
 class ImplementationCreator:
     def __init__(
         self,
         creator_function: Callable,
@@ -400,28 +404,59 @@
     def get_decorators(self, service_type: type):
         return self._decorators[service_type]
 
     def get_singleton(self, registartion_id):
         return self._singletons.get(registartion_id)
 
     @property
-    def singleton_items(self):
-        return self._singletons.items()
+    def singletons(self):
+        return self._singletons
 
 
-class ResolvingContext:
+class DependencyCache:
     def __init__(self, registry: Registry, scope: Scope):
         self.registry = registry
         self.scope = scope
-        self._cache = {}
-        self._cache = {
-            **{k: v for k, v in registry.singleton_items},
-            **{k: v for k, v in scope.scoped_items},
+        self._current_items = {
+            **{k: v for k, v in registry.singletons.items()},
+            **{k: v for k, v in scope.scoped_instances.items()},
         }
 
+    def get(self, registration_id: str):
+        instance = self._current_items.get(registration_id, _empty)
+        if instance is not _empty:
+            return instance
+
+        instance = self.registry.singletons.get(registration_id, _empty)
+        if instance is not _empty:
+            self._current_items[registration_id] = instance
+
+        instance = self.scope.scoped_instances.get(registration_id, _empty)
+        if instance is not _empty:
+            self._current_items[registration_id] = instance
+            return instance
+
+        return instance
+
+    def put(self, registration_id: str, instance: Any, lifespan: Lifespan):
+        if lifespan == Lifespan.singleton:
+            self.registry.add_singleton_instance(registration_id, instance)
+        elif lifespan == Lifespan.scoped:
+            self.scope.add_scoped_instance(registration_id, instance)
+
+        if lifespan >= Lifespan.once_per_graph:
+            self._current_items[registration_id] = instance
+
+
+class ResolvingContext:
+    def __init__(self, registry: Registry, scope: Scope):
+        self.registry = registry
+        self.scope = scope
+        self._cache = DependencyCache(registry=registry, scope=scope)
+
     def try_generic_fallback(self, service_type: _GenericAlias):
         return self.find_registration(service_type.__origin__, _all_registartions)
 
     def find_registration(
         self, service_type: type, registration_finder: Callable
     ) -> Registration:
         regs = self.find_registrations(service_type, registration_finder)
@@ -454,24 +489,18 @@
         return [
             d
             for d in self.registry.get_decorators(registration.service_type)
             if d.registartion_filter(registration)
         ]
 
     def get_cached(self, reg_id: str):
-        return self._cache.get(reg_id, _empty)
+        return self._cache.get(reg_id)
 
     def new_instance_created(self, reg_id: str, instance: Any, lifespan: Lifespan):
-        if lifespan == Lifespan.singleton:
-            self.registry.add_singleton_instance(reg_id, instance)
-        elif lifespan == Lifespan.scoped:
-            self.scope.add_scoped_instance(reg_id, instance)
-
-        if lifespan >= Lifespan.once_per_graph:
-            self._cache[reg_id] = instance
+        self._cache.put(registration_id=reg_id, instance=instance, lifespan=lifespan)
 
 
 class Resolver(abc.ABC):
     @abc.abstractmethod
     def resolve(
         self,
         cls: type,
@@ -503,16 +532,16 @@
     def register(self, *args):
         pass
 
     def get_registartions(self, service_tyep):
         return self._registrations[service_tyep]
 
     @property
-    def scoped_items(self):
-        return self._scoped_instances.items()
+    def scoped_instances(self):
+        return self._scoped_instances
 
 
 class ContainerScope(Scope):
     def __init__(self, container: Container):
         self._container = container
         self._registrations = defaultdict(deque)
         self._scoped_instances = {}
@@ -796,15 +825,15 @@
         self,
         service_type,
         filter: RegistartionFilter = _all_registartions,
         scope: Scope = EmptyContainerScope(),
     ) -> Any:
         d = RootDependency(service_type, DependencySettings(filter=filter))
         context = ResolvingContext(self.registry, scope)
-        graph = d.run_resolve(context)
+        graph = d.resolve_dependency_graph(context)
         return graph.resolved_object
 
     def new_scope(
         self, ScopeClass: Type[ContainerScope] = ContainerScope, *args, **kwargs
     ) -> Scope:
         return ScopeClass(self, *args, **kwargs)
```

### Comparing `clean_ioc-0.0.6/clean_ioc/factories.py` & `clean_ioc-0.1.0/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/clean_ioc/functional_utils.py` & `clean_ioc-0.1.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/clean_ioc/registration_filters.py` & `clean_ioc-0.1.0/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/clean_ioc/type_filters.py` & `clean_ioc-0.1.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/clean_ioc/typing_utils.py` & `clean_ioc-0.1.0/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.6/pyproject.toml` & `clean_ioc-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.0.6"
+version = "0.1.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
```

### Comparing `clean_ioc-0.0.6/setup.py` & `clean_ioc-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['clean_ioc']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'clean-ioc',
-    'version': '0.0.6',
+    'version': '0.1.0',
     'description': 'An IOC Container for Python 3.10+',
     'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\n\n```\n',
     'author': 'Peter Daly',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/peter-daly/clean_ioc',
```

### Comparing `clean_ioc-0.0.6/PKG-INFO` & `clean_ioc-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.0.6
+Version: 0.1.0
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://github.com/peter-daly/clean_ioc
 Project-URL: Repository, https://github.com/peter-daly/clean_ioc
 Description-Content-Type: text/markdown
```

