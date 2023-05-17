# Comparing `tmp/reacton-1.6.1.tar.gz` & `tmp/reacton-1.7.0.tar.gz`

## Comparing `reacton-1.6.1.tar` & `reacton-1.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 reacton-1.6.1/react_ipywidgets/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reacton-1.6.1/react_ipywidgets/core.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/_version.py
--rw-r--r--   0        0        0   128540 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/bqplot.py
--rw-r--r--   0        0        0    96461 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/core.py
--rw-r--r--   0        0        0    90141 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/core_test.py
--rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/find.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/find_test.py
--rw-r--r--   0        0        0    13737 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/generate.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/generate_test.py
--rw-r--r--   0        0        0     9685 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipycanvas.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipyvue.py
--rw-r--r--   0        0        0   211230 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipyvuetify.py
--rw-r--r--   0        0        0   141391 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipywidgets.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/logging.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/patch.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/patch_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/py.typed
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/rx.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/test.vue
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/test_rx.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/utils.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/utils_test.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/work.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 reacton-1.6.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 reacton-1.6.1/LICENSE
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 reacton-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 reacton-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 reacton-1.7.0/react_ipywidgets/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reacton-1.7.0/react_ipywidgets/core.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/_version.py
+-rw-r--r--   0        0        0   128540 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/bqplot.py
+-rw-r--r--   0        0        0    96885 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/core.py
+-rw-r--r--   0        0        0    90141 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/core_test.py
+-rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/find.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/find_test.py
+-rw-r--r--   0        0        0    13737 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/generate.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/generate_test.py
+-rw-r--r--   0        0        0     9685 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/ipycanvas.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/ipyvue.py
+-rw-r--r--   0        0        0   211230 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/ipyvuetify.py
+-rw-r--r--   0        0        0   141391 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/ipywidgets.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/logging.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/patch.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/patch_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/py.typed
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/rx.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/test.vue
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/test_rx.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/utils.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/utils_test.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 reacton-1.7.0/reacton/work.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 reacton-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 reacton-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 reacton-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 reacton-1.7.0/PKG-INFO
```

### Comparing `reacton-1.6.1/reacton/__init__.py` & `reacton-1.7.0/reacton/__init__.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/bqplot.py` & `reacton-1.7.0/reacton/bqplot.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/core.py` & `reacton-1.7.0/reacton/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,17 +354,27 @@
     def _create_widget(self, kwargs):
         # we can't use our own kwarg, since that contains elements, not widgets
         kwargs, listeners = self._split_kwargs(kwargs)
         assert isinstance(self.component, ComponentWidget)
         # Because we look before and after, we need a lock.
         # A different implementation might avoid this.
         with self.create_lock:
+            rc = get_render_context(required=True)
             before = set(widgets.Widget.widgets)
             try:
                 widget = self.component.widget(**kwargs)
+                hold_trait_notifications = widget.hold_trait_notifications
+
+                @contextlib.contextmanager
+                def hold_trait_notifications_extra(*args, **kwargs):
+                    with rc, hold_trait_notifications(*args, **kwargs):
+                        yield
+
+                widget.hold_trait_notifications = hold_trait_notifications_extra
+
                 if self._meta:
                     widget._react_meta = dict(self._meta)
             except Exception as e:
                 raise RuntimeError(f"Could not create widget {self.component.widget} with {kwargs}") from e
             for name, callback in listeners.items():
                 if callback is not None:
                     self._add_widget_event_listener(widget, name, callback)
```

### Comparing `reacton-1.6.1/reacton/core_test.py` & `reacton-1.7.0/reacton/core_test.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/find.py` & `reacton-1.7.0/reacton/find.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/find_test.py` & `reacton-1.7.0/reacton/find_test.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/generate.py` & `reacton-1.7.0/reacton/generate.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/generate_test.py` & `reacton-1.7.0/reacton/generate_test.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/ipycanvas.py` & `reacton-1.7.0/reacton/ipycanvas.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/ipyvue.py` & `reacton-1.7.0/reacton/ipyvue.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/ipyvuetify.py` & `reacton-1.7.0/reacton/ipyvuetify.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/ipywidgets.py` & `reacton-1.7.0/reacton/ipywidgets.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/logging.py` & `reacton-1.7.0/reacton/logging.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/patch.py` & `reacton-1.7.0/reacton/patch.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/patch_display.py` & `reacton-1.7.0/reacton/patch_display.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/test_rx.py` & `reacton-1.7.0/reacton/test_rx.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/utils.py` & `reacton-1.7.0/reacton/utils.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/reacton/utils_test.py` & `reacton-1.7.0/reacton/utils_test.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/.gitignore` & `reacton-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/LICENSE` & `reacton-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/pyproject.toml` & `reacton-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reacton-1.6.1/PKG-INFO` & `reacton-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacton
-Version: 1.6.1
+Version: 1.7.0
 Project-URL: Home, https://www.github.com/widgetti/reacton
 Project-URL: Documentation, https://reacton.solara.dev
 Project-URL: Source code, https://www.github.com/widgetti/reacton
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Maarten A. Breddels
```

