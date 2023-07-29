# Comparing `tmp/dash_intersection_observer-1.0.0.tar.gz` & `tmp/dash_intersection_observer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_intersection_observer-1.0.0.tar", last modified: Wed Jul 26 13:49:45 2023, max compression
+gzip compressed data, was "dash_intersection_observer-1.0.1.tar", last modified: Sat Jul 29 09:19:34 2023, max compression
```

## Comparing `dash_intersection_observer-1.0.0.tar` & `dash_intersection_observer-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2023-07-26 13:49:45.806531 dash_intersection_observer-1.0.0/
--rw-r--r--   0 renaud    (1000) renaud    (1000)        0 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.0/LICENSE
--rw-r--r--   0 renaud    (1000) renaud    (1000)       85 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.0/MANIFEST.in
--rw-r--r--   0 renaud    (1000) renaud    (1000)      235 2023-07-26 13:49:45.806531 dash_intersection_observer-1.0.0/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1070 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.0/README.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2023-07-26 13:49:45.806531 dash_intersection_observer-1.0.0/dash_intersection_observer/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     2506 2023-07-26 13:46:08.000000 dash_intersection_observer-1.0.0/dash_intersection_observer/DashIntersectionObserver.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1590 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.0/dash_intersection_observer/__init__.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)      108 2023-07-26 13:46:08.000000 dash_intersection_observer-1.0.0/dash_intersection_observer/_imports_.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     5825 2023-07-26 13:46:04.000000 dash_intersection_observer-1.0.0/dash_intersection_observer/dash_intersection_observer.js
--rw-r--r--   0 renaud    (1000) renaud    (1000)     2531 2023-07-26 13:46:08.000000 dash_intersection_observer-1.0.0/dash_intersection_observer/metadata.json
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1387 2023-07-26 13:46:05.000000 dash_intersection_observer-1.0.0/dash_intersection_observer/package-info.json
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2023-07-26 13:49:45.806531 dash_intersection_observer-1.0.0/dash_intersection_observer.egg-info/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      235 2023-07-26 13:49:45.000000 dash_intersection_observer-1.0.0/dash_intersection_observer.egg-info/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)      515 2023-07-26 13:49:45.000000 dash_intersection_observer-1.0.0/dash_intersection_observer.egg-info/SOURCES.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2023-07-26 13:49:45.000000 dash_intersection_observer-1.0.0/dash_intersection_observer.egg-info/dependency_links.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)       27 2023-07-26 13:49:45.000000 dash_intersection_observer-1.0.0/dash_intersection_observer.egg-info/top_level.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2023-07-26 13:49:45.806531 dash_intersection_observer-1.0.0/setup.cfg
--rw-r--r--   0 renaud    (1000) renaud    (1000)      494 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.0/setup.py
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2023-07-29 09:19:34.072419 dash_intersection_observer-1.0.1/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)        0 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.1/LICENSE
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       85 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.1/MANIFEST.in
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      235 2023-07-29 09:19:34.072419 dash_intersection_observer-1.0.1/PKG-INFO
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1070 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.1/README.md
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2023-07-29 09:19:34.072419 dash_intersection_observer-1.0.1/dash_intersection_observer/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     2541 2023-07-29 09:17:34.000000 dash_intersection_observer-1.0.1/dash_intersection_observer/DashIntersectionObserver.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1590 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.1/dash_intersection_observer/__init__.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      108 2023-07-29 09:17:34.000000 dash_intersection_observer-1.0.1/dash_intersection_observer/_imports_.py
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     6072 2023-07-29 09:12:48.000000 dash_intersection_observer-1.0.1/dash_intersection_observer/dash_intersection_observer.js
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     2755 2023-07-29 09:17:34.000000 dash_intersection_observer-1.0.1/dash_intersection_observer/metadata.json
+-rw-r--r--   0 renaud    (1000) renaud    (1000)     1387 2023-07-29 09:17:32.000000 dash_intersection_observer-1.0.1/dash_intersection_observer/package-info.json
+drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2023-07-29 09:19:34.072419 dash_intersection_observer-1.0.1/dash_intersection_observer.egg-info/
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      235 2023-07-29 09:19:33.000000 dash_intersection_observer-1.0.1/dash_intersection_observer.egg-info/PKG-INFO
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      515 2023-07-29 09:19:34.000000 dash_intersection_observer-1.0.1/dash_intersection_observer.egg-info/SOURCES.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2023-07-29 09:19:33.000000 dash_intersection_observer-1.0.1/dash_intersection_observer.egg-info/dependency_links.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       27 2023-07-29 09:19:33.000000 dash_intersection_observer-1.0.1/dash_intersection_observer.egg-info/top_level.txt
+-rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2023-07-29 09:19:34.072419 dash_intersection_observer-1.0.1/setup.cfg
+-rw-r--r--   0 renaud    (1000) renaud    (1000)      494 2023-07-26 07:15:48.000000 dash_intersection_observer-1.0.1/setup.py
```

### Comparing `dash_intersection_observer-1.0.0/README.md` & `dash_intersection_observer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dash_intersection_observer-1.0.0/dash_intersection_observer/DashIntersectionObserver.py` & `dash_intersection_observer-1.0.1/dash_intersection_observer/DashIntersectionObserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 
 class DashIntersectionObserver(Component):
     """A DashIntersectionObserver component.
 Component description
 
 Keyword arguments:
 
-- children (a list of or a singular dash component, string or number; required)
+- children (a list of or a singular dash component, string or number; optional)
 
 - id (string; optional):
     Unique ID to identify this component in Dash callbacks.
 
 - className (string; optional):
     CSS class of the wrapping div.
 
 - delay (number; optional):
     Minimum delay between notifications, in milliseconds.
 
 - inView (boolean; optional):
     Whether the component is in the viewport (READONLY).
 
+- inViewCount (number; optional):
+    Number of times the component has been in the viewport.
+
 - initialInView (boolean; optional):
     Set the initial value of the inView boolean.
 
 - rootMargin (string; optional):
     Margin around the root. Can have values similar to the CSS margin
     property.
 
@@ -40,21 +43,18 @@
 - triggerOnce (boolean; optional):
     Only trigger the inView callback once if True."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_intersection_observer'
     _type = 'DashIntersectionObserver'
     @_explicitize_args
-    def __init__(self, children=None, threshold=Component.UNDEFINED, delay=Component.UNDEFINED, rootMargin=Component.UNDEFINED, triggerOnce=Component.UNDEFINED, initialInView=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, inView=Component.UNDEFINED, id=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'className', 'delay', 'inView', 'initialInView', 'rootMargin', 'style', 'threshold', 'triggerOnce']
+    def __init__(self, children=None, threshold=Component.UNDEFINED, delay=Component.UNDEFINED, rootMargin=Component.UNDEFINED, triggerOnce=Component.UNDEFINED, initialInView=Component.UNDEFINED, style=Component.UNDEFINED, className=Component.UNDEFINED, inView=Component.UNDEFINED, inViewCount=Component.UNDEFINED, id=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'className', 'delay', 'inView', 'inViewCount', 'initialInView', 'rootMargin', 'style', 'threshold', 'triggerOnce']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'className', 'delay', 'inView', 'initialInView', 'rootMargin', 'style', 'threshold', 'triggerOnce']
+        self.available_properties = ['children', 'id', 'className', 'delay', 'inView', 'inViewCount', 'initialInView', 'rootMargin', 'style', 'threshold', 'triggerOnce']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
-        if 'children' not in _explicit_args:
-            raise TypeError('Required argument children was not specified.')
-
         super(DashIntersectionObserver, self).__init__(children=children, **args)
```

### Comparing `dash_intersection_observer-1.0.0/dash_intersection_observer/__init__.py` & `dash_intersection_observer-1.0.1/dash_intersection_observer/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_intersection_observer-1.0.0/dash_intersection_observer/dash_intersection_observer.js` & `dash_intersection_observer-1.0.1/dash_intersection_observer/dash_intersection_observer.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -3,26 +3,26 @@
 }(self, (e => (() => {
     "use strict";
     var t = {
             500: (e, t, r) => {
                 var i, n = Object.create,
                     o = Object.defineProperty,
                     s = Object.getOwnPropertyDescriptor,
-                    l = Object.getOwnPropertyNames,
-                    a = Object.getPrototypeOf,
+                    a = Object.getOwnPropertyNames,
+                    l = Object.getPrototypeOf,
                     c = Object.prototype.hasOwnProperty,
                     u = (e, t, r, i) => {
                         if (t && "object" == typeof t || "function" == typeof t)
-                            for (let n of l(t)) c.call(e, n) || n === r || o(e, n, {
+                            for (let n of a(t)) c.call(e, n) || n === r || o(e, n, {
                                 get: () => t[n],
                                 enumerable: !(i = s(t, n)) || i.enumerable
                             });
                         return e
                     },
-                    h = (e, t, r) => (r = null != e ? n(a(e)) : {}, u(!t && e && e.__esModule ? r : o(r, "default", {
+                    h = (e, t, r) => (r = null != e ? n(l(e)) : {}, u(!t && e && e.__esModule ? r : o(r, "default", {
                         value: e,
                         enumerable: !0
                     }), e)),
                     d = (e, t, r) => (((e, t, r) => {
                         t in e ? o(e, t, {
                             enumerable: !0,
                             configurable: !0,
@@ -33,15 +33,15 @@
                     p = {};
                 ((e, t) => {
                     for (var r in t) o(e, r, {
                         get: t[r],
                         enumerable: !0
                     })
                 })(p, {
-                    InView: () => m,
+                    InView: () => O,
                     defaultFallbackInView: () => w,
                     observe: () => V,
                     useInView: () => _
                 }), e.exports = (i = p, u(o({}, "__esModule", {
                     value: !0
                 }), i));
                 var f = h(r(812)),
@@ -95,21 +95,21 @@
                                 id: t,
                                 observer: o,
                                 elements: i
                             }, b.set(t, r)
                         }
                         return r
                     }(r);
-                    let l = s.get(e) || [];
-                    return s.has(e) || s.set(e, l), l.push(t), o.observe(e),
+                    let a = s.get(e) || [];
+                    return s.has(e) || s.set(e, a), a.push(t), o.observe(e),
                         function() {
-                            l.splice(l.indexOf(t), 1), 0 === l.length && (s.delete(e), o.unobserve(e)), 0 === s.size && (o.disconnect(), b.delete(n))
+                            a.splice(a.indexOf(t), 1), 0 === a.length && (s.delete(e), o.unobserve(e)), 0 === s.size && (o.disconnect(), b.delete(n))
                         }
                 }
-                var m = class extends f.Component {
+                var O = class extends f.Component {
                         constructor(e) {
                             super(e), d(this, "node", null), d(this, "_unobserveCb", null), d(this, "handleNode", (e => {
                                 this.node && (this.unobserve(), e || this.props.triggerOnce || this.props.skip || this.setState({
                                     inView: !!this.props.initialInView,
                                     entry: void 0
                                 })), this.node = e || null, this.observeNode()
                             })), d(this, "handleChange", ((e, t) => {
@@ -170,68 +170,68 @@
                             const {
                                 as: t,
                                 triggerOnce: r,
                                 threshold: i,
                                 root: n,
                                 rootMargin: o,
                                 onChange: s,
-                                skip: l,
-                                trackVisibility: a,
+                                skip: a,
+                                trackVisibility: l,
                                 delay: c,
                                 initialInView: u,
                                 fallbackInView: h,
                                 ...d
                             } = this.props;
                             return f.createElement(t || "div", {
                                 ref: this.handleNode,
                                 ...d
                             }, e)
                         }
                     },
-                    O = h(r(812));
+                    m = h(r(812));
 
                 function _({
                     threshold: e,
                     delay: t,
                     trackVisibility: r,
                     rootMargin: i,
                     root: n,
                     triggerOnce: o,
                     skip: s,
-                    initialInView: l,
-                    fallbackInView: a,
+                    initialInView: a,
+                    fallbackInView: l,
                     onChange: c
                 } = {}) {
                     var u;
-                    const [h, d] = O.useState(null), p = O.useRef(), [f, b] = O.useState({
-                        inView: !!l,
+                    const [h, d] = m.useState(null), p = m.useRef(), [f, b] = m.useState({
+                        inView: !!a,
                         entry: void 0
                     });
-                    p.current = c, O.useEffect((() => {
+                    p.current = c, m.useEffect((() => {
                         if (s || !h) return;
-                        let l;
-                        return l = V(h, ((e, t) => {
+                        let a;
+                        return a = V(h, ((e, t) => {
                             b({
                                 inView: e,
                                 entry: t
-                            }), p.current && p.current(e, t), t.isIntersecting && o && l && (l(), l = void 0)
+                            }), p.current && p.current(e, t), t.isIntersecting && o && a && (a(), a = void 0)
                         }), {
                             root: n,
                             rootMargin: i,
                             threshold: e,
                             trackVisibility: r,
                             delay: t
-                        }, a), () => {
-                            l && l()
+                        }, l), () => {
+                            a && a()
                         }
-                    }), [Array.isArray(e) ? e.toString() : e, h, n, i, o, s, r, a, t]);
+                    }), [Array.isArray(e) ? e.toString() : e, h, n, i, o, s, r, l, t]);
                     const v = null == (u = f.entry) ? void 0 : u.target,
-                        y = O.useRef();
+                        y = m.useRef();
                     h || !v || o || s || y.current === v || (y.current = v, b({
-                        inView: !!l,
+                        inView: !!a,
                         entry: void 0
                     }));
                     const g = [d, f.inView, f.entry];
                     return g.ref = g[0], g.inView = g[1], g.entry = g[2], g
                 }
             },
             702: function(e, t, r) {
@@ -248,36 +248,39 @@
                         return e && e.__esModule ? e : {
                             default: e
                         }
                     };
                 t.__esModule = !0;
                 var o = n(r(812)),
                     s = r(500),
-                    l = function(e) {
+                    a = function(e) {
                         var t = e.children,
                             r = e.style,
                             n = e.className,
-                            l = e.id,
-                            a = e.setProps,
-                            c = i(e, ["children", "style", "className", "id", "setProps"]),
-                            u = (0, s.useInView)(c),
-                            h = u.ref,
-                            d = u.inView;
+                            a = e.id,
+                            l = e.setProps,
+                            c = e.triggerOnce,
+                            u = e.inViewCount,
+                            h = i(e, ["children", "style", "className", "id", "setProps", "triggerOnce", "inViewCount"]),
+                            d = o.default.useRef(0),
+                            p = u || 0,
+                            f = (0, s.useInView)(h),
+                            b = f.ref,
+                            v = f.inView;
                         return o.default.useEffect((function() {
-                            a({
-                                inView: d
-                            })
-                        }), [d]), o.default.createElement("div", {
-                            id: l,
-                            ref: h,
+                            var e = {};
+                            c && p < 1 && (v ? (e.inViewCount = p + 1, d.current === p ? e.inView = !0 : e.inView = String(Math.random()), d.current = p + 1) : e.inView = !1), c || (e.inView = v), Object.keys(e).length > 0 && l(e)
+                        }), [v, u]), o.default.createElement("div", {
+                            id: a,
+                            ref: b,
                             style: r,
                             className: n
                         }, t)
                     };
-                l.defaultProps = {}, t.default = l
+                a.defaultProps = {}, t.default = a
             },
             294: function(e, t, r) {
                 var i = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
```

### Comparing `dash_intersection_observer-1.0.0/dash_intersection_observer/metadata.json` & `dash_intersection_observer-1.0.1/dash_intersection_observer/metadata.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9943576388888888%*

 * *Differences: {"'src/ts/components/DashIntersectionObserver.tsx'": "{'props': {'children': {'required': False}, "*

 * *                                                     "'inViewCount': OrderedDict([('description', "*

 * *                                                     "'Number of times the component has been in "*

 * *                                                     "the viewport.'), ('required', False), "*

 * *                                                     "('type', OrderedDict([('name', 'number'), "*

 * *                      […]*

```diff
@@ -2,15 +2,15 @@
     "src/ts/components/DashIntersectionObserver.tsx": {
         "description": "Component description",
         "displayName": "DashIntersectionObserver",
         "isContext": false,
         "props": {
             "children": {
                 "description": "",
-                "required": true,
+                "required": false,
                 "type": {
                     "name": "node",
                     "raw": "ReactNode"
                 }
             },
             "className": {
                 "description": "CSS class of the wrapping div.",
@@ -40,14 +40,22 @@
                 "description": "Whether the component is in the viewport (READONLY).",
                 "required": false,
                 "type": {
                     "name": "bool",
                     "raw": "boolean"
                 }
             },
+            "inViewCount": {
+                "description": "Number of times the component has been in the viewport.",
+                "required": false,
+                "type": {
+                    "name": "number",
+                    "raw": "number"
+                }
+            },
             "initialInView": {
                 "description": "Set the initial value of the inView boolean.",
                 "required": false,
                 "type": {
                     "name": "bool",
                     "raw": "boolean"
                 }
```

### Comparing `dash_intersection_observer-1.0.0/dash_intersection_observer/package-info.json` & `dash_intersection_observer-1.0.1/dash_intersection_observer/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -36,9 +36,9 @@
     "scripts": {
         "build": "npm run build:js && npm run build:backends",
         "build:backends": "dash-generate-components ./src/ts/components dash_intersection_observer -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:js": "webpack",
         "build:js::dev": "webpack --mode development",
         "watch": "npm run build:js::dev -- --watch"
     },
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `dash_intersection_observer-1.0.0/dash_intersection_observer.egg-info/SOURCES.txt` & `dash_intersection_observer-1.0.1/dash_intersection_observer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

