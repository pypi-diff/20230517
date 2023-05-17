# Comparing `tmp/pull_dash_components-1.0.0.tar.gz` & `tmp/pull_dash_components-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pull_dash_components-1.0.0.tar", last modified: Thu May 11 08:19:17 2023, max compression
+gzip compressed data, was "pull_dash_components-1.0.1.tar", last modified: Wed May 17 12:00:42 2023, max compression
```

## Comparing `pull_dash_components-1.0.0.tar` & `pull_dash_components-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-11 08:19:17.424915 pull_dash_components-1.0.0/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-04-22 03:25:04.000000 pull_dash_components-1.0.0/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)       97 2023-05-11 08:11:48.000000 pull_dash_components-1.0.0/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      271 2023-05-11 08:19:17.424744 pull_dash_components-1.0.0/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1065 2023-04-24 11:55:04.000000 pull_dash_components-1.0.0/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-11 08:19:17.423847 pull_dash_components-1.0.0/pull_dash_components/
--rw-r--r--   0 eric       (501) staff       (20)     1367 2023-04-22 03:57:51.000000 pull_dash_components-1.0.0/pull_dash_components/AppInput.py
--rw-r--r--   0 eric       (501) staff       (20)     1650 2023-05-11 08:19:08.000000 pull_dash_components-1.0.0/pull_dash_components/Input.py
--rw-r--r--   0 eric       (501) staff       (20)      991 2023-05-11 08:19:08.000000 pull_dash_components-1.0.0/pull_dash_components/PullDashComponents.py
--rw-r--r--   0 eric       (501) staff       (20)     1578 2023-04-22 03:25:04.000000 pull_dash_components-1.0.0/pull_dash_components/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      128 2023-05-11 08:19:08.000000 pull_dash_components-1.0.0/pull_dash_components/_imports_.py
--rw-r--r--   0 eric       (501) staff       (20)     1389 2023-04-22 06:16:52.000000 pull_dash_components-1.0.0/pull_dash_components/index.py
--rw-r--r--   0 eric       (501) staff       (20)     2659 2023-05-11 08:19:08.000000 pull_dash_components-1.0.0/pull_dash_components/metadata.json
--rw-r--r--   0 eric       (501) staff       (20)     1463 2023-05-11 08:16:26.000000 pull_dash_components-1.0.0/pull_dash_components/package-info.json
--rw-r--r--   0 eric       (501) staff       (20)     1458 2023-05-11 08:19:07.000000 pull_dash_components-1.0.0/pull_dash_components/package.json
--rw-r--r--   0 eric       (501) staff       (20)    78449 2023-05-11 08:13:13.000000 pull_dash_components-1.0.0/pull_dash_components/pull_dash_components.js
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-11 08:19:17.424487 pull_dash_components-1.0.0/pull_dash_components.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      271 2023-05-11 08:19:17.000000 pull_dash_components-1.0.0/pull_dash_components.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      570 2023-05-11 08:19:17.000000 pull_dash_components-1.0.0/pull_dash_components.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-11 08:19:17.000000 pull_dash_components-1.0.0/pull_dash_components.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       21 2023-05-11 08:19:17.000000 pull_dash_components-1.0.0/pull_dash_components.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-11 08:19:17.424967 pull_dash_components-1.0.0/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      517 2023-05-11 08:09:53.000000 pull_dash_components-1.0.0/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-17 12:00:42.797879 pull_dash_components-1.0.1/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-04-22 03:25:04.000000 pull_dash_components-1.0.1/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)       97 2023-05-11 08:11:48.000000 pull_dash_components-1.0.1/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      271 2023-05-17 12:00:42.797699 pull_dash_components-1.0.1/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1065 2023-04-24 11:55:04.000000 pull_dash_components-1.0.1/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-17 12:00:42.796217 pull_dash_components-1.0.1/pull_dash_components/
+-rw-r--r--   0 eric       (501) staff       (20)     1367 2023-04-22 03:57:51.000000 pull_dash_components-1.0.1/pull_dash_components/AppInput.py
+-rw-r--r--   0 eric       (501) staff       (20)     1158 2023-05-16 16:01:11.000000 pull_dash_components-1.0.1/pull_dash_components/FullscreenPanel.py
+-rw-r--r--   0 eric       (501) staff       (20)     1650 2023-05-17 12:00:29.000000 pull_dash_components-1.0.1/pull_dash_components/Input.py
+-rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-17 12:00:29.000000 pull_dash_components-1.0.1/pull_dash_components/Panel.py
+-rw-r--r--   0 eric       (501) staff       (20)      991 2023-05-17 12:00:29.000000 pull_dash_components-1.0.1/pull_dash_components/PullDashComponents.py
+-rw-r--r--   0 eric       (501) staff       (20)     1578 2023-04-22 03:25:04.000000 pull_dash_components-1.0.1/pull_dash_components/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      166 2023-05-17 12:00:29.000000 pull_dash_components-1.0.1/pull_dash_components/_imports_.py
+-rw-r--r--   0 eric       (501) staff       (20)     1389 2023-04-22 06:16:52.000000 pull_dash_components-1.0.1/pull_dash_components/index.py
+-rw-r--r--   0 eric       (501) staff       (20)     4213 2023-05-17 12:00:29.000000 pull_dash_components-1.0.1/pull_dash_components/metadata.json
+-rw-r--r--   0 eric       (501) staff       (20)     1463 2023-05-11 08:16:26.000000 pull_dash_components-1.0.1/pull_dash_components/package-info.json
+-rw-r--r--   0 eric       (501) staff       (20)     1458 2023-05-17 12:00:28.000000 pull_dash_components-1.0.1/pull_dash_components/package.json
+-rw-r--r--   0 eric       (501) staff       (20)    81350 2023-05-17 11:56:16.000000 pull_dash_components-1.0.1/pull_dash_components/pull_dash_components.js
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-17 12:00:42.797395 pull_dash_components-1.0.1/pull_dash_components.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      271 2023-05-17 12:00:42.000000 pull_dash_components-1.0.1/pull_dash_components.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      640 2023-05-17 12:00:42.000000 pull_dash_components-1.0.1/pull_dash_components.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-17 12:00:42.000000 pull_dash_components-1.0.1/pull_dash_components.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       21 2023-05-17 12:00:42.000000 pull_dash_components-1.0.1/pull_dash_components.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-17 12:00:42.797930 pull_dash_components-1.0.1/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      517 2023-05-11 08:09:53.000000 pull_dash_components-1.0.1/setup.py
```

### Comparing `pull_dash_components-1.0.0/README.md` & `pull_dash_components-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/AppInput.py` & `pull_dash_components-1.0.1/pull_dash_components/AppInput.py`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/Input.py` & `pull_dash_components-1.0.1/pull_dash_components/Input.py`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/PullDashComponents.py` & `pull_dash_components-1.0.1/pull_dash_components/PullDashComponents.py`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/__init__.py` & `pull_dash_components-1.0.1/pull_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/index.py` & `pull_dash_components-1.0.1/pull_dash_components/index.py`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/metadata.json` & `pull_dash_components-1.0.1/pull_dash_components/metadata.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'src/ts/components/Panel.tsx'": "OrderedDict([('displayName', 'Panel'), ('description', ''), "*

 * *                                  "('props', OrderedDict([('id', OrderedDict([('description', "*

 * *                                  "'Unique ID to identify this component in Dash callbacks.'), "*

 * *                                  "('required', False), ('defaultValue', OrderedDict([('value', "*

 * *                                  "'Math.random().toString(36).substring(2, 7)'), ('computed', "*

 * *                            […]*

```diff
@@ -86,14 +86,81 @@
                 "type": {
                     "name": "any",
                     "raw": "any"
                 }
             }
         }
     },
+    "src/ts/components/Panel.tsx": {
+        "description": "",
+        "displayName": "Panel",
+        "isContext": false,
+        "props": {
+            "bg": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'#ffffff'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string",
+                    "raw": "string"
+                }
+            },
+            "children": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "node",
+                    "raw": "ReactNode"
+                }
+            },
+            "color": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'#0092E4'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string",
+                    "raw": "string"
+                }
+            },
+            "customClass": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string",
+                    "raw": "string"
+                }
+            },
+            "id": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "Math.random().toString(36).substring(2, 7)"
+                },
+                "description": "Unique ID to identify this component in Dash callbacks.",
+                "required": false,
+                "type": {
+                    "name": "string",
+                    "raw": "string"
+                }
+            },
+            "setProps": {
+                "description": "Update props to trigger callbacks.",
+                "required": true,
+                "type": {
+                    "name": "func",
+                    "raw": "(props: Record<string, any>) => void"
+                }
+            }
+        }
+    },
     "src/ts/components/PullDashComponents.tsx": {
         "description": "Component description",
         "displayName": "PullDashComponents",
         "isContext": false,
         "props": {
             "id": {
                 "description": "Unique ID to identify this component in Dash callbacks.",
```

### Comparing `pull_dash_components-1.0.0/pull_dash_components/package-info.json` & `pull_dash_components-1.0.1/pull_dash_components/package-info.json`

 * *Files identical despite different names*

### Comparing `pull_dash_components-1.0.0/pull_dash_components/package.json` & `pull_dash_components-1.0.1/pull_dash_components/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -40,9 +40,9 @@
     "scripts": {
         "build": "npm run build:js && npm run build:backends",
         "build:backends": "dash-generate-components ./src/ts/components pull_dash_components -p package.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:js": "webpack",
         "build:js::dev": "webpack --mode development",
         "watch": "npm run build:js::dev -- --watch"
     },
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `pull_dash_components-1.0.0/pull_dash_components/pull_dash_components.js` & `pull_dash_components-1.0.1/pull_dash_components/pull_dash_components.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
                 e.d(r, {
                     Z: () => i
                 });
                 var n = e(8081),
                     o = e.n(n),
                     u = e(3645),
                     s = e.n(u)()(o());
-                s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Figtree:wght@300;400;500;600;700;800;900&display=swap);"]), s.push([t.id, '.pull-input-group{font-family:"Figtree",sans-serif}.pull-input-group label,.pull-input-group .helper-text{font-style:normal;font-weight:400;font-size:15px;line-height:18px;color:#000;padding-bottom:4px}.pull-input-group .pull-input{box-sizing:border-box;display:flex;flex-direction:row;margin:4px 0;width:171px;overflow:hidden;height:42px;background:#fff;color:#222;border:1px solid #dcdcdc;border-radius:8px}.pull-input-group .pull-input:focus-within{border:1px solid #454545}.pull-input-group .pull-input.disabled{background:#f2f2f2;border:1px solid #f2f2f2}.pull-input-group .pull-input input[type=text]{padding:12px 16px;margin:0;outline:none;border:none;background:rgba(0,0,0,0)}', ""]);
+                s.push([t.id, "@import url(https://fonts.googleapis.com/css2?family=Figtree:wght@300;400;500;600;700;800;900&display=swap);"]), s.push([t.id, '.pull-input-group{font-family:"Figtree",sans-serif}.pull-input-group label,.pull-input-group .helper-text{font-style:normal;font-weight:400;font-size:15px;line-height:18px;color:#000;padding-bottom:4px}.pull-input-group .pull-input{box-sizing:border-box;display:flex;flex-direction:row;margin:4px 0;width:171px;overflow:hidden;height:42px;background:#fff;color:#222;border:1px solid #dcdcdc;border-radius:8px}.pull-input-group .pull-input:focus-within{border:1px solid #454545}.pull-input-group .pull-input.disabled{background:#f2f2f2;border:1px solid #f2f2f2}.pull-input-group .pull-input input[type=text]{padding:12px 16px;margin:0;outline:none;border:none;background:rgba(0,0,0,0)}.pull-panel{transition:all ease-in-out .5s;padding:16px}.pull-panel.fullscreen{position:fixed;top:0;left:0;width:100%;height:100vh;z-index:99999999}.pull-panel button{display:block;width:30px;height:30px;outline:none;border:none;background:none;cursor:pointer}', ""]);
                 const i = s
             },
             3645: t => {
                 "use strict";
                 t.exports = function(t) {
                     var r = [];
                     return r.toString = function() {
@@ -30,17 +30,17 @@
                         ]);
                         var s = {};
                         if (n)
                             for (var i = 0; i < this.length; i++) {
                                 var a = this[i][0];
                                 null != a && (s[a] = !0)
                             }
-                        for (var p = 0; p < t.length; p++) {
-                            var c = [].concat(t[p]);
-                            n && s[c[0]] || (void 0 !== u && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = u), e && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = e) : c[2] = e), o && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = o) : c[4] = "".concat(o)), r.push(c))
+                        for (var c = 0; c < t.length; c++) {
+                            var p = [].concat(t[c]);
+                            n && s[p[0]] || (void 0 !== u && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = u), e && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = e) : p[2] = e), o && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = o) : p[4] = "".concat(o)), r.push(p))
                         }
                     }, r
                 }
             },
             8081: t => {
                 "use strict";
                 t.exports = function(t) {
@@ -228,27 +228,27 @@
             8375: (t, r, e) => {
                 var n = e(6224),
                     o = e(219),
                     u = e(5748),
                     s = e(2220),
                     i = e(1186),
                     a = e(4585),
-                    p = e(793),
-                    c = e(368),
+                    c = e(793),
+                    p = e(368),
                     f = e(3411);
 
                 function l(t, r) {
-                    return o(r) ? r.map(t) : c(r).reduce((function(e, n) {
+                    return o(r) ? r.map(t) : p(r).reduce((function(e, n) {
                         return e[n] = t(r[n]), e
                     }), {})
                 }
                 var x = n((function t(r) {
                     return r = l((function(r) {
                         return "function" == typeof r ? r : t(r)
-                    }), r), s(p(i, 0, a("length", f(r))), (function() {
+                    }), r), s(c(i, 0, a("length", f(r))), (function() {
                         var t = arguments;
                         return l((function(r) {
                             return u(r, t)
                         }), r)
                     }))
                 }));
                 t.exports = x
@@ -281,16 +281,16 @@
                     u = e(7e3),
                     s = e(7031),
                     i = e(3657),
                     a = n((function t(r, e, n) {
                         if (0 === r.length) return e;
                         var a = r[0];
                         if (r.length > 1) {
-                            var p = !i(n) && o(a, n) ? n[a] : u(r[1]) ? [] : {};
-                            e = t(Array.prototype.slice.call(r, 1), e, p)
+                            var c = !i(n) && o(a, n) ? n[a] : u(r[1]) ? [] : {};
+                            e = t(Array.prototype.slice.call(r, 1), e, c)
                         }
                         return s(a, e, n)
                     }));
                 t.exports = a
             },
             962: (t, r, e) => {
                 var n = e(6224),
@@ -449,15 +449,15 @@
                 var n = e(9002),
                     o = e(3087),
                     u = e(864),
                     s = n((function(t, r) {
                         if (t > 10) throw new Error("Constructor with greater than ten arguments");
                         return 0 === t ? function() {
                             return new r
-                        } : o(u(t, (function(t, e, n, o, u, s, i, a, p, c) {
+                        } : o(u(t, (function(t, e, n, o, u, s, i, a, c, p) {
                             switch (arguments.length) {
                                 case 1:
                                     return new r(t);
                                 case 2:
                                     return new r(t, e);
                                 case 3:
                                     return new r(t, e, n);
@@ -468,39 +468,39 @@
                                 case 6:
                                     return new r(t, e, n, o, u, s);
                                 case 7:
                                     return new r(t, e, n, o, u, s, i);
                                 case 8:
                                     return new r(t, e, n, o, u, s, i, a);
                                 case 9:
-                                    return new r(t, e, n, o, u, s, i, a, p);
+                                    return new r(t, e, n, o, u, s, i, a, c);
                                 case 10:
-                                    return new r(t, e, n, o, u, s, i, a, p, c)
+                                    return new r(t, e, n, o, u, s, i, a, c, p)
                             }
                         })))
                     }));
                 t.exports = s
             },
             8907: (t, r, e) => {
                 var n = e(9002),
                     o = e(6692),
                     u = e(2220),
                     s = e(1186),
                     i = e(4585),
                     a = e(793),
-                    p = n((function(t, r) {
+                    c = n((function(t, r) {
                         return u(a(s, 0, i("length", r)), (function() {
                             var e = arguments,
                                 n = this;
                             return t.apply(n, o((function(t) {
                                 return t.apply(n, e)
                             }), r))
                         }))
                     }));
-                t.exports = p
+                t.exports = c
             },
             3558: (t, r, e) => {
                 var n = e(9488),
                     o = e(3087)((function(t, r) {
                         return n((function(r, e) {
                             return t(e) ? r + 1 : r
                         }), 0, r)
@@ -681,20 +681,20 @@
             8403: (t, r, e) => {
                 var n = e(6224),
                     o = e(7587),
                     u = e(219),
                     s = e(8291),
                     i = e(190),
                     a = e(2105),
-                    p = n((function(t) {
+                    c = n((function(t) {
                         return null != t && "function" == typeof t["fantasy-land/empty"] ? t["fantasy-land/empty"]() : null != t && null != t.constructor && "function" == typeof t.constructor["fantasy-land/empty"] ? t.constructor["fantasy-land/empty"]() : null != t && "function" == typeof t.empty ? t.empty() : null != t && null != t.constructor && "function" == typeof t.constructor.empty ? t.constructor.empty() : u(t) ? [] : i(t) ? "" : s(t) ? {} : o(t) ? function() {
                             return arguments
                         }() : a(t) ? t.constructor.from("") : void 0
                     }));
-                t.exports = p
+                t.exports = c
             },
             796: (t, r, e) => {
                 var n = e(9002),
                     o = e(1481),
                     u = e(8703),
                     s = n((function(t, r) {
                         return o(u(t.length, r), t)
@@ -740,21 +740,21 @@
             1383: (t, r, e) => {
                 var n = e(9002),
                     o = e(4793),
                     u = e(4877),
                     s = e(8291),
                     i = e(9488),
                     a = e(123),
-                    p = e(368),
-                    c = n(o(["fantasy-land/filter", "filter"], a, (function(t, r) {
+                    c = e(368),
+                    p = n(o(["fantasy-land/filter", "filter"], a, (function(t, r) {
                         return s(r) ? i((function(e, n) {
                             return t(r[n]) && (e[n] = r[n]), e
-                        }), {}, p(r)) : u(t, r)
+                        }), {}, c(r)) : u(t, r)
                     })));
-                t.exports = c
+                t.exports = p
             },
             6376: (t, r, e) => {
                 var n = e(9002)(e(4793)(["find"], e(7855), (function(t, r) {
                     for (var e = 0, n = r.length; e < n;) {
                         if (t(r[e])) return r[e];
                         e += 1
                     }
@@ -1049,19 +1049,19 @@
                                 return r.apply(this, arguments)
                             };
                         case 8:
                             return function(t, e, n, o, u, s, i, a) {
                                 return r.apply(this, arguments)
                             };
                         case 9:
-                            return function(t, e, n, o, u, s, i, a, p) {
+                            return function(t, e, n, o, u, s, i, a, c) {
                                 return r.apply(this, arguments)
                             };
                         case 10:
-                            return function(t, e, n, o, u, s, i, a, p, c) {
+                            return function(t, e, n, o, u, s, i, a, c, p) {
                                 return r.apply(this, arguments)
                             };
                         default:
                             throw new Error("First argument to _arity must be a non-negative integer no greater than ten")
                     }
                 }
             },
@@ -1245,17 +1245,17 @@
                 }
             },
             2738: (t, r, e) => {
                 var n = e(7455),
                     o = e(6464);
                 t.exports = function t(r, e, u) {
                     return function() {
-                        for (var s = [], i = 0, a = r, p = 0; p < e.length || i < arguments.length;) {
-                            var c;
-                            p < e.length && (!o(e[p]) || i >= arguments.length) ? c = e[p] : (c = arguments[i], i += 1), s[p] = c, o(c) || (a -= 1), p += 1
+                        for (var s = [], i = 0, a = r, c = 0; c < e.length || i < arguments.length;) {
+                            var p;
+                            c < e.length && (!o(e[c]) || i >= arguments.length) ? p = e[c] : (p = arguments[i], i += 1), s[c] = p, o(p) || (a -= 1), c += 1
                         }
                         return a <= 0 ? u.apply(this, s) : n(a, t(r, s, u))
                     }
                 }
             },
             4793: (t, r, e) => {
                 var n = e(219),
@@ -1303,32 +1303,32 @@
             4023: (t, r, e) => {
                 var n = e(4118),
                     o = e(2976),
                     u = e(4931),
                     s = e(7684),
                     i = e(1361),
                     a = e(368),
-                    p = e(6433);
+                    c = e(6433);
 
-                function c(t, r, e, u) {
+                function p(t, r, e, u) {
                     var s = n(t),
                         i = n(r);
 
                     function a(t, r) {
                         return f(t, r, e.slice(), u.slice())
                     }
                     return !o((function(t, r) {
                         return !o(a, r, t)
                     }), i, s)
                 }
 
                 function f(t, r, e, n) {
                     if (i(t, r)) return !0;
-                    var o = p(t);
-                    if (o !== p(r)) return !1;
+                    var o = c(t);
+                    if (o !== c(r)) return !1;
                     if ("function" == typeof t["fantasy-land/equals"] || "function" == typeof r["fantasy-land/equals"]) return "function" == typeof t["fantasy-land/equals"] && t["fantasy-land/equals"](r) && "function" == typeof r["fantasy-land/equals"] && r["fantasy-land/equals"](t);
                     if ("function" == typeof t.equals || "function" == typeof r.equals) return "function" == typeof t.equals && t.equals(r) && "function" == typeof r.equals && r.equals(t);
                     switch (o) {
                         case "Arguments":
                         case "Array":
                         case "Object":
                             if ("function" == typeof t.constructor && "Promise" === u(t.constructor)) return t === r;
@@ -1348,17 +1348,17 @@
                     }
                     for (var l = e.length - 1; l >= 0;) {
                         if (e[l] === t) return n[l] === r;
                         l -= 1
                     }
                     switch (o) {
                         case "Map":
-                            return t.size === r.size && c(t.entries(), r.entries(), e.concat([t]), n.concat([r]));
+                            return t.size === r.size && p(t.entries(), r.entries(), e.concat([t]), n.concat([r]));
                         case "Set":
-                            return t.size === r.size && c(t.values(), r.values(), e.concat([t]), n.concat([r]));
+                            return t.size === r.size && p(t.values(), r.values(), e.concat([t]), n.concat([r]));
                         case "Arguments":
                         case "Array":
                         case "Object":
                         case "Boolean":
                         case "Number":
                         case "String":
                         case "Date":
@@ -1574,15 +1574,15 @@
                     return "[object Uint8ClampedArray]" === r || "[object Int8Array]" === r || "[object Uint8Array]" === r || "[object Int16Array]" === r || "[object Uint16Array]" === r || "[object Int32Array]" === r || "[object Uint32Array]" === r || "[object Float32Array]" === r || "[object Float64Array]" === r || "[object BigInt64Array]" === r || "[object BigUint64Array]" === r
                 }
             },
             5161: (t, r, e) => {
                 var n = e(3219);
                 t.exports = function(t) {
                     return function r(e) {
-                        for (var o, u, s, i = [], a = 0, p = e.length; a < p;) {
+                        for (var o, u, s, i = [], a = 0, c = e.length; a < c;) {
                             if (n(e[a]))
                                 for (s = 0, u = (o = t ? r(e[a]) : e[a]).length; s < u;) i[i.length] = o[s], s += 1;
                             else i[i.length] = e[a];
                             a += 1
                         }
                         return i
                     }
@@ -1704,33 +1704,33 @@
                     a = {
                         "@@transducer/init": Array,
                         "@@transducer/step": function(t, r) {
                             return t.push(r), t
                         },
                         "@@transducer/result": o
                     },
-                    p = {
+                    c = {
                         "@@transducer/init": String,
                         "@@transducer/step": function(t, r) {
                             return t + r
                         },
                         "@@transducer/result": o
                     },
-                    c = {
+                    p = {
                         "@@transducer/init": Object,
                         "@@transducer/step": function(t, r) {
                             return n(t, u(r) ? i(r[0], r[1]) : r)
                         },
                         "@@transducer/result": o
                     };
                 t.exports = function(t) {
                     if (s(t)) return t;
                     if (u(t)) return a;
-                    if ("string" == typeof t) return p;
-                    if ("object" == typeof t) return c;
+                    if ("string" == typeof t) return c;
+                    if ("object" == typeof t) return p;
                     throw new Error("Cannot create transformer for " + t)
                 }
             },
             5123: t => {
                 var r = function(t) {
                         return (t < 10 ? "0" : "") + t
                     },
@@ -1745,48 +1745,48 @@
                 var n = e(7243),
                     o = e(6692),
                     u = e(6001),
                     s = e(5123),
                     i = e(368),
                     a = e(3266);
                 t.exports = function t(r, e) {
-                    var p = function(o) {
+                    var c = function(o) {
                             var u = e.concat([r]);
                             return n(o, u) ? "<Circular>" : t(o, u)
                         },
-                        c = function(t, r) {
+                        p = function(t, r) {
                             return o((function(r) {
-                                return u(r) + ": " + p(t[r])
+                                return u(r) + ": " + c(t[r])
                             }), r.slice().sort())
                         };
                     switch (Object.prototype.toString.call(r)) {
                         case "[object Arguments]":
-                            return "(function() { return arguments; }(" + o(p, r).join(", ") + "))";
+                            return "(function() { return arguments; }(" + o(c, r).join(", ") + "))";
                         case "[object Array]":
-                            return "[" + o(p, r).concat(c(r, a((function(t) {
+                            return "[" + o(c, r).concat(p(r, a((function(t) {
                                 return /^\d+$/.test(t)
                             }), i(r)))).join(", ") + "]";
                         case "[object Boolean]":
-                            return "object" == typeof r ? "new Boolean(" + p(r.valueOf()) + ")" : r.toString();
+                            return "object" == typeof r ? "new Boolean(" + c(r.valueOf()) + ")" : r.toString();
                         case "[object Date]":
-                            return "new Date(" + (isNaN(r.valueOf()) ? p(NaN) : u(s(r))) + ")";
+                            return "new Date(" + (isNaN(r.valueOf()) ? c(NaN) : u(s(r))) + ")";
                         case "[object Null]":
                             return "null";
                         case "[object Number]":
-                            return "object" == typeof r ? "new Number(" + p(r.valueOf()) + ")" : 1 / r == -1 / 0 ? "-0" : r.toString(10);
+                            return "object" == typeof r ? "new Number(" + c(r.valueOf()) + ")" : 1 / r == -1 / 0 ? "-0" : r.toString(10);
                         case "[object String]":
-                            return "object" == typeof r ? "new String(" + p(r.valueOf()) + ")" : u(r);
+                            return "object" == typeof r ? "new String(" + c(r.valueOf()) + ")" : u(r);
                         case "[object Undefined]":
                             return "undefined";
                         default:
                             if ("function" == typeof r.toString) {
                                 var f = r.toString();
                                 if ("[object Object]" !== f) return f
                             }
-                            return "{" + c(r, i(r)).join(", ") + "}"
+                            return "{" + p(r, i(r)).join(", ") + "}"
                     }
                 }
             },
             5750: (t, r, e) => {
                 var n = e(9002),
                     o = e(2157),
                     u = e(3714),
@@ -2248,16 +2248,16 @@
                 var n = e(6224),
                     o = e(7684),
                     u = e(368),
                     s = n((function(t) {
                         for (var r = u(t), e = r.length, n = 0, s = {}; n < e;) {
                             var i = r[n],
                                 a = t[i],
-                                p = o(a, s) ? s[a] : s[a] = [];
-                            p[p.length] = i, n += 1
+                                c = o(a, s) ? s[a] : s[a] = [];
+                            c[c.length] = i, n += 1
                         }
                         return s
                     }));
                 t.exports = s
             },
             2380: (t, r, e) => {
                 var n = e(6224),
@@ -2328,33 +2328,33 @@
                         toString: null
                     }.propertyIsEnumerable("toString"),
                     i = ["constructor", "valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
                     a = function() {
                         "use strict";
                         return arguments.propertyIsEnumerable("length")
                     }(),
-                    p = function(t, r) {
+                    c = function(t, r) {
                         for (var e = 0; e < t.length;) {
                             if (t[e] === r) return !0;
                             e += 1
                         }
                         return !1
                     },
-                    c = "function" != typeof Object.keys || a ? n((function(t) {
+                    p = "function" != typeof Object.keys || a ? n((function(t) {
                         if (Object(t) !== t) return [];
                         var r, e, n = [],
-                            c = a && u(t);
-                        for (r in t) !o(r, t) || c && "length" === r || (n[n.length] = r);
+                            p = a && u(t);
+                        for (r in t) !o(r, t) || p && "length" === r || (n[n.length] = r);
                         if (s)
-                            for (e = i.length - 1; e >= 0;) o(r = i[e], t) && !p(n, r) && (n[n.length] = r), e -= 1;
+                            for (e = i.length - 1; e >= 0;) o(r = i[e], t) && !c(n, r) && (n[n.length] = r), e -= 1;
                         return n
                     })) : n((function(t) {
                         return Object(t) !== t ? [] : Object.keys(t)
                     }));
-                t.exports = c
+                t.exports = p
             },
             7716: (t, r, e) => {
                 var n = e(6224)((function(t) {
                     var r, e = [];
                     for (r in t) e[e.length] = r;
                     return e
                 }));
@@ -2469,30 +2469,30 @@
             1894: (t, r, e) => {
                 var n = e(9002),
                     o = e(4793),
                     u = e(6692),
                     s = e(9488),
                     i = e(2894),
                     a = e(2220),
-                    p = e(368),
-                    c = n(o(["fantasy-land/map", "map"], i, (function(t, r) {
+                    c = e(368),
+                    p = n(o(["fantasy-land/map", "map"], i, (function(t, r) {
                         switch (Object.prototype.toString.call(r)) {
                             case "[object Function]":
                                 return a(r.length, (function() {
                                     return t.call(this, r.apply(this, arguments))
                                 }));
                             case "[object Object]":
                                 return s((function(e, n) {
                                     return e[n] = t(r[n]), e
-                                }), {}, p(r));
+                                }), {}, c(r));
                             default:
                                 return u(t, r)
                         }
                     })));
-                t.exports = c
+                t.exports = p
             },
             1282: (t, r, e) => {
                 var n = e(6370)((function(t, r, e) {
                     for (var n = 0, o = e.length, u = [], s = [r]; n < o;) s = t(s[0], e[n]), u[n] = s[1], n += 1;
                     return [s[0], u]
                 }));
                 t.exports = n
@@ -2682,23 +2682,23 @@
             2514: (t, r, e) => {
                 var n = e(6370),
                     o = e(219),
                     u = e(8291),
                     s = e(7684),
                     i = e(7031),
                     a = e(4693),
-                    p = n((function t(r, e, n) {
+                    c = n((function t(r, e, n) {
                         if (!u(n) && !o(n) || 0 === r.length) return n;
-                        var p = r[0];
-                        if (!s(p, n)) return n;
-                        if (1 === r.length) return a(p, e, n);
-                        var c = t(Array.prototype.slice.call(r, 1), e, n[p]);
-                        return c === n[p] ? n : i(p, c, n)
+                        var c = r[0];
+                        if (!s(c, n)) return n;
+                        if (1 === r.length) return a(c, e, n);
+                        var p = t(Array.prototype.slice.call(r, 1), e, n[c]);
+                        return p === n[c] ? n : i(c, p, n)
                     }));
-                t.exports = p
+                t.exports = c
             },
             2395: (t, r, e) => {
                 var n = e(9002)((function(t, r) {
                     return t % r
                 }));
                 t.exports = n
             },
@@ -2755,20 +2755,20 @@
                                 return r.call(this, t, e, n, o, u, s, i)
                             };
                         case 8:
                             return function(t, e, n, o, u, s, i, a) {
                                 return r.call(this, t, e, n, o, u, s, i, a)
                             };
                         case 9:
-                            return function(t, e, n, o, u, s, i, a, p) {
-                                return r.call(this, t, e, n, o, u, s, i, a, p)
+                            return function(t, e, n, o, u, s, i, a, c) {
+                                return r.call(this, t, e, n, o, u, s, i, a, c)
                             };
                         case 10:
-                            return function(t, e, n, o, u, s, i, a, p, c) {
-                                return r.call(this, t, e, n, o, u, s, i, a, p, c)
+                            return function(t, e, n, o, u, s, i, a, c, p) {
+                                return r.call(this, t, e, n, o, u, s, i, a, c, p)
                             };
                         default:
                             throw new Error("First argument to nAry must be a non-negative integer no greater than ten")
                     }
                 }));
                 t.exports = n
             },
@@ -2997,25 +2997,25 @@
             1446: (t, r, e) => {
                 var n = e(7455),
                     o = e(9002),
                     u = e(6408),
                     s = e(9488),
                     i = e(3656),
                     a = e(9105),
-                    p = o((function(t, r) {
+                    c = o((function(t, r) {
                         if (r.length <= 0) return a;
                         var e = u(r),
                             o = i(r);
                         return n(e.length, (function() {
                             return s((function(r, e) {
                                 return t.call(this, e, r)
                             }), e.apply(this, arguments), o)
                         }))
                     }));
-                t.exports = p
+                t.exports = c
             },
             4585: (t, r, e) => {
                 var n = e(9002),
                     o = e(1894),
                     u = e(2478),
                     s = n((function(t, r) {
                         return o(u(t), r)
@@ -3119,22 +3119,22 @@
             4285: (t, r, e) => {
                 var n = e(5114),
                     o = e(2738),
                     u = e(4793),
                     s = e(7684),
                     i = e(9488),
                     a = e(2157),
-                    p = o(4, [], u([], e(7744), (function(t, r, e, o) {
+                    c = o(4, [], u([], e(7744), (function(t, r, e, o) {
                         return i((function(o, u) {
                             var i = e(u),
-                                p = t(s(i, o) ? o[i] : n(r, [], [], !1), u);
-                            return p && p["@@transducer/reduced"] ? a(o) : (o[i] = p, o)
+                                c = t(s(i, o) ? o[i] : n(r, [], [], !1), u);
+                            return c && c["@@transducer/reduced"] ? a(o) : (o[i] = c, o)
                         }), {}, o)
                     })));
-                t.exports = p
+                t.exports = c
             },
             7981: (t, r, e) => {
                 var n = e(6370)((function(t, r, e) {
                     for (var n = e.length - 1; n >= 0;) {
                         if ((r = t(e[n], r)) && r["@@transducer/reduced"]) {
                             r = r["@@transducer/value"];
                             break
@@ -3751,25 +3751,25 @@
                 });
                 var n = e(3379),
                     o = e.n(n),
                     u = e(7795),
                     s = e.n(u),
                     i = e(3565),
                     a = e.n(i),
-                    p = e(9216),
-                    c = e.n(p),
+                    c = e(9216),
+                    p = e.n(c),
                     f = e(4589),
                     l = e.n(f),
                     x = e(6185),
                     h = {};
                 h.styleTagTransform = l(), h.setAttributes = a(), h.insert = function(t) {
                     var r = document.querySelector("head"),
                         e = window._lastElementInsertedByStyleLoader;
                     e ? e.nextSibling ? r.insertBefore(t, e.nextSibling) : r.appendChild(t) : r.insertBefore(t, r.firstChild), window._lastElementInsertedByStyleLoader = t
-                }, h.domAPI = s(), h.insertStyleElement = c(), o()(x.Z, h);
+                }, h.domAPI = s(), h.insertStyleElement = p(), o()(x.Z, h);
                 const v = x.Z && x.Z.locals ? x.Z.locals : void 0
             },
             3379: t => {
                 "use strict";
                 var r = [];
 
                 function e(t) {
@@ -3779,18 +3779,18 @@
                             break
                         } return e
                 }
 
                 function n(t, n) {
                     for (var u = {}, s = [], i = 0; i < t.length; i++) {
                         var a = t[i],
-                            p = n.base ? a[0] + n.base : a[0],
-                            c = u[p] || 0,
-                            f = "".concat(p, " ").concat(c);
-                        u[p] = c + 1;
+                            c = n.base ? a[0] + n.base : a[0],
+                            p = u[c] || 0,
+                            f = "".concat(c, " ").concat(p);
+                        u[c] = p + 1;
                         var l = e(f),
                             x = {
                                 css: a[1],
                                 media: a[2],
                                 sourceMap: a[3],
                                 supports: a[4],
                                 layer: a[5]
@@ -3823,17 +3823,17 @@
                     var u = n(t = t || [], o = o || {});
                     return function(t) {
                         t = t || [];
                         for (var s = 0; s < u.length; s++) {
                             var i = e(u[s]);
                             r[i].references--
                         }
-                        for (var a = n(t, o), p = 0; p < u.length; p++) {
-                            var c = e(u[p]);
-                            0 === r[c].references && (r[c].updater(), r.splice(c, 1))
+                        for (var a = n(t, o), c = 0; c < u.length; c++) {
+                            var p = e(u[c]);
+                            0 === r[p].references && (r[p].updater(), r.splice(p, 1))
                         }
                         u = a
                     }
                 }
             },
             9216: t => {
                 "use strict";
@@ -3934,64 +3934,145 @@
                     },
                     a = this && this.__importDefault || function(t) {
                         return t && t.__esModule ? t : {
                             default: t
                         }
                     };
                 r.__esModule = !0;
-                var p = s(e(5812)),
-                    c = a(e(5924)),
+                var c = s(e(5812)),
+                    p = a(e(5924)),
                     f = e(36);
                 e(3878);
                 var l = function(t) {
-                        return (0, c.default)(t) ? +t : NaN
+                        return (0, p.default)(t) ? +t : NaN
                     },
                     x = function(t) {
                         var r = t.id,
                             e = t.type,
                             o = t.label,
                             u = t.disabled,
                             s = t.helper_text,
                             a = (t.className, t.value),
-                            c = t.setProps,
+                            p = t.setProps,
                             x = i(t, ["id", "type", "label", "disabled", "helper_text", "className", "value", "setProps"]),
-                            h = (0, p.useRef)(null);
-                        return p.default.createElement("div", {
+                            h = (0, c.useRef)(null);
+                        return c.default.createElement("div", {
                             className: "pull-input-group"
-                        }, o && p.default.createElement("label", {
+                        }, o && c.default.createElement("label", {
                             htmlFor: r
-                        }, o), p.default.createElement("div", {
+                        }, o), c.default.createElement("div", {
                             className: "".concat(u ? "disabled" : "", " pull-input")
-                        }, p.default.createElement("input", n({
+                        }, c.default.createElement("input", n({
                             ref: h,
                             type: e,
                             id: r,
                             disabled: u,
                             onChange: function(t) {
                                 ! function(t) {
                                     if (void 0 === t && (t = {}), "number" === e) {
                                         var r = h.current.value,
                                             o = h.current.checkValidity() ? l(r) : NaN;
-                                        (u = l(a)) === (s = o) || isNaN(u) && isNaN(s) ? Object.keys(t).length && c(t) : c(n(n({}, t), {
+                                        (u = l(a)) === (s = o) || isNaN(u) && isNaN(s) ? Object.keys(t).length && p(t) : p(n(n({}, t), {
                                             value: o
                                         }))
-                                    } else t.value = h.current.value, console.log(t), c(t);
+                                    } else t.value = h.current.value, console.log(t), p(t);
                                     var u, s
                                 }()
                             }
-                        }, (0, f.omit)(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], x)))), s && p.default.createElement("span", null, p.default.createElement("small", {
+                        }, (0, f.omit)(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], x)))), s && c.default.createElement("span", null, c.default.createElement("small", {
                             className: "helper-text"
                         }, s)))
                     };
                 x.defaultProps = {
                     type: "text",
                     disabled: !1,
                     id: Math.random().toString(36).substring(2, 7)
                 }, r.default = x
             },
+            9055: function(t, r, e) {
+                "use strict";
+                var n = this && this.__createBinding || (Object.create ? function(t, r, e, n) {
+                        void 0 === n && (n = e);
+                        var o = Object.getOwnPropertyDescriptor(r, e);
+                        o && !("get" in o ? !r.__esModule : o.writable || o.configurable) || (o = {
+                            enumerable: !0,
+                            get: function() {
+                                return r[e]
+                            }
+                        }), Object.defineProperty(t, n, o)
+                    } : function(t, r, e, n) {
+                        void 0 === n && (n = e), t[n] = r[e]
+                    }),
+                    o = this && this.__setModuleDefault || (Object.create ? function(t, r) {
+                        Object.defineProperty(t, "default", {
+                            enumerable: !0,
+                            value: r
+                        })
+                    } : function(t, r) {
+                        t.default = r
+                    }),
+                    u = this && this.__importStar || function(t) {
+                        if (t && t.__esModule) return t;
+                        var r = {};
+                        if (null != t)
+                            for (var e in t) "default" !== e && Object.prototype.hasOwnProperty.call(t, e) && n(r, t, e);
+                        return o(r, t), r
+                    },
+                    s = this && this.__rest || function(t, r) {
+                        var e = {};
+                        for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && r.indexOf(n) < 0 && (e[n] = t[n]);
+                        if (null != t && "function" == typeof Object.getOwnPropertySymbols) {
+                            var o = 0;
+                            for (n = Object.getOwnPropertySymbols(t); o < n.length; o++) r.indexOf(n[o]) < 0 && Object.prototype.propertyIsEnumerable.call(t, n[o]) && (e[n[o]] = t[n[o]])
+                        }
+                        return e
+                    };
+                r.__esModule = !0;
+                var i = u(e(5812));
+                e(3878);
+                var a = function(t) {
+                    t.id, t.setProps;
+                    var r = t.bg,
+                        e = t.customClass,
+                        n = t.color,
+                        o = t.children,
+                        u = (s(t, ["id", "setProps", "bg", "customClass", "color", "children"]), (0, i.useState)(!1)),
+                        a = u[0],
+                        c = u[1];
+                    return i.default.createElement("div", {
+                        style: {
+                            backgroundColor: r
+                        },
+                        className: "pull-panel ".concat(e, " ").concat(a ? "fullscreen" : "normal-view")
+                    }, i.default.createElement("div", null, i.default.createElement("button", {
+                        onClick: function(t) {
+                            t.preventDefault(), c(!a)
+                        }
+                    }, !a && i.default.createElement("svg", {
+                        xmlns: "http://www.w3.org/2000/svg",
+                        viewBox: "0 0 15 15",
+                        id: "maximize-left"
+                    }, i.default.createElement("path", {
+                        fill: n,
+                        d: "M5.41,4H7A1,1,0,0,0,7,2H3a1,1,0,0,0-.38.08,1,1,0,0,0-.54.54A1,1,0,0,0,2,3V7A1,1,0,0,0,4,7V5.41l5.79,5.8a1,1,0,0,0,1.42,0,1,1,0,0,0,0-1.42ZM21,16a1,1,0,0,0-1,1v1.59l-5.79-5.8a1,1,0,0,0-1.42,1.42L18.59,20H17a1,1,0,0,0,0,2h4a1,1,0,0,0,.38-.08,1,1,0,0,0,.54-.54A1,1,0,0,0,22,21V17A1,1,0,0,0,21,16Z"
+                    })), a && i.default.createElement("svg", {
+                        xmlns: "http://www.w3.org/2000/svg",
+                        viewBox: "0 0 15 15",
+                        id: "compress-alt-left"
+                    }, i.default.createElement("path", {
+                        fill: n,
+                        d: "M10.5,5.5a1,1,0,0,0-1,1V8.09L3.71,2.29A1,1,0,0,0,2.29,3.71L8.09,9.5H6.5a1,1,0,0,0,0,2h4a1,1,0,0,0,.38-.08,1,1,0,0,0,.54-.54,1,1,0,0,0,.08-.38v-4A1,1,0,0,0,10.5,5.5ZM21.71,20.29l-5.8-5.79H17.5a1,1,0,0,0,0-2h-4a1,1,0,0,0-.38.08,1,1,0,0,0-.54.54,1,1,0,0,0-.08.38v4a1,1,0,0,0,2,0V15.91l5.79,5.8a1,1,0,0,0,1.42,0A1,1,0,0,0,21.71,20.29Z"
+                    })))), i.default.createElement("div", null, o))
+                };
+                a.defaultProps = {
+                    id: Math.random().toString(36).substring(2, 7),
+                    bg: "#ffffff",
+                    color: "#0092E4"
+                }, r.default = a
+            },
             8841: function(t, r, e) {
                 "use strict";
                 var n = this && this.__importDefault || function(t) {
                     return t && t.__esModule ? t : {
                         default: t
                     }
                 };
@@ -4008,19 +4089,21 @@
             9294: function(t, r, e) {
                 "use strict";
                 var n = this && this.__importDefault || function(t) {
                     return t && t.__esModule ? t : {
                         default: t
                     }
                 };
-                r.__esModule = !0, r.Input = r.PullDashComponents = void 0;
+                r.__esModule = !0, r.Panel = r.Input = r.PullDashComponents = void 0;
                 var o = n(e(8841));
                 r.PullDashComponents = o.default;
                 var u = n(e(5783));
-                r.Input = u.default
+                r.Input = u.default;
+                var s = n(e(9055));
+                r.Panel = s.default
             },
             5812: r => {
                 "use strict";
                 r.exports = t
             }
         },
         e = {};
```

### Comparing `pull_dash_components-1.0.0/pull_dash_components.egg-info/SOURCES.txt` & `pull_dash_components-1.0.1/pull_dash_components.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 pull_dash_components/AppInput.py
+pull_dash_components/FullscreenPanel.py
 pull_dash_components/Input.py
+pull_dash_components/Panel.py
 pull_dash_components/PullDashComponents.py
 pull_dash_components/__init__.py
 pull_dash_components/_imports_.py
 pull_dash_components/index.py
 pull_dash_components/metadata.json
 pull_dash_components/package-info.json
 pull_dash_components/package.json
```

### Comparing `pull_dash_components-1.0.0/setup.py` & `pull_dash_components-1.0.1/setup.py`

 * *Files identical despite different names*

