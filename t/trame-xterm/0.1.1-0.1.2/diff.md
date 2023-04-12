# Comparing `tmp/trame-xterm-0.1.1.tar.gz` & `tmp/trame-xterm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-xterm-0.1.1.tar", last modified: Thu Apr  6 20:31:30 2023, max compression
+gzip compressed data, was "trame-xterm-0.1.2.tar", last modified: Wed Apr 12 22:08:28 2023, max compression
```

## Comparing `trame-xterm-0.1.1.tar` & `trame-xterm-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.902161 trame-xterm-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-06 20:31:30.902161 trame-xterm-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      570 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      901 2023-04-06 20:31:30.902161 trame-xterm-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.898161 trame-xterm-0.1.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.898161 trame-xterm-0.1.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame/modules/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.898161 trame-xterm-0.1.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame/widgets/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.898161 trame-xterm-0.1.1/trame_xterm/
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame_xterm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.898161 trame-xterm-0.1.1/trame_xterm/module/
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame_xterm/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.902161 trame-xterm-0.1.1/trame_xterm/module/serve/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-04-06 20:31:26.000000 trame-xterm-0.1.1/trame_xterm/module/serve/style.css
--rw-r--r--   0 root         (0) root         (0)   396435 2023-04-06 20:31:26.000000 trame-xterm-0.1.1/trame_xterm/module/serve/trame-xterm.mjs
--rw-r--r--   0 root         (0) root         (0)   278873 2023-04-06 20:31:27.000000 trame-xterm-0.1.1/trame_xterm/module/serve/trame-xterm.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.902161 trame-xterm-0.1.1/trame_xterm/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame_xterm/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14604 2023-04-06 20:31:12.000000 trame-xterm-0.1.1/trame_xterm/widgets/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:31:30.898161 trame-xterm-0.1.1/trame_xterm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-06 20:31:30.000000 trame-xterm-0.1.1/trame_xterm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-06 20:31:30.000000 trame-xterm-0.1.1/trame_xterm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 20:31:30.000000 trame-xterm-0.1.1/trame_xterm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-06 20:31:30.000000 trame-xterm-0.1.1/trame_xterm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-06 20:31:30.000000 trame-xterm-0.1.1/trame_xterm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      570 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      901 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.336667 trame-xterm-0.1.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.336667 trame-xterm-0.1.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/modules/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/widgets/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame_xterm/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame_xterm/module/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/trame_xterm/module/serve/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-04-12 22:08:24.000000 trame-xterm-0.1.2/trame_xterm/module/serve/style.css
+-rw-r--r--   0 root         (0) root         (0)   396472 2023-04-12 22:08:24.000000 trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.mjs
+-rw-r--r--   0 root         (0) root         (0)   278894 2023-04-12 22:08:24.000000 trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/trame_xterm/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14722 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/widgets/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame_xterm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/top_level.txt
```

### Comparing `trame-xterm-0.1.1/LICENSE` & `trame-xterm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.1/PKG-INFO` & `trame-xterm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-xterm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Trame widget to expose xterm.js
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-xterm-0.1.1/README.rst` & `trame-xterm-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.1/setup.cfg` & `trame-xterm-0.1.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-xterm
-version = 0.1.1
+version = 0.1.2
 description = Trame widget to expose xterm.js
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-xterm-0.1.1/trame_xterm/module/serve/style.css` & `trame-xterm-0.1.2/trame_xterm/module/serve/style.css`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.1/trame_xterm/module/serve/trame-xterm.mjs` & `trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
   }
 };
 (function(X, J) {
   (function(Z, G) {
     X.exports = G();
   })(self, function() {
     return (() => {
-      var Z = { 4567: (T, i, o) => {
+      var Z = { 4567: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.AccessibilityManager = void 0;
-        const h = o(9042), u = o(6114), d = o(9924), _ = o(3656), g = o(844), v = o(5596), c = o(9631);
+        const a = h(9042), u = h(6114), d = h(9924), _ = h(3656), g = h(844), v = h(5596), c = h(9631);
         class e extends g.Disposable {
           constructor(n, t) {
             super(), this._terminal = n, this._renderService = t, this._liveRegionLineCount = 0, this._charsToConsume = [], this._charsToAnnounce = "", this._accessibilityTreeRoot = document.createElement("div"), this._accessibilityTreeRoot.classList.add("xterm-accessibility"), this._accessibilityTreeRoot.tabIndex = 0, this._rowContainer = document.createElement("div"), this._rowContainer.setAttribute("role", "list"), this._rowContainer.classList.add("xterm-accessibility-tree"), this._rowElements = [];
             for (let r = 0; r < this._terminal.rows; r++)
               this._rowElements[r] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[r]);
             if (this._topBoundaryFocusListener = (r) => this._handleBoundaryFocus(r, 0), this._bottomBoundaryFocusListener = (r) => this._handleBoundaryFocus(r, 1), this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._refreshRowsDimensions(), this._accessibilityTreeRoot.appendChild(this._rowContainer), this._renderRowsDebouncer = new d.TimeBasedDebouncer(this._renderRows.bind(this)), this._refreshRows(), this._liveRegion = document.createElement("div"), this._liveRegion.classList.add("live-region"), this._liveRegion.setAttribute("aria-live", "assertive"), this._accessibilityTreeRoot.appendChild(this._liveRegion), !this._terminal.element)
               throw new Error("Cannot enable accessibility before Terminal.open");
@@ -29,19 +29,19 @@
           }
           _handleBoundaryFocus(n, t) {
             const r = n.target, l = this._rowElements[t === 0 ? 1 : this._rowElements.length - 2];
             if (r.getAttribute("aria-posinset") === (t === 0 ? "1" : `${this._terminal.buffer.lines.length}`) || n.relatedTarget !== l)
               return;
             let f, m;
             if (t === 0 ? (f = r, m = this._rowElements.pop(), this._rowContainer.removeChild(m)) : (f = this._rowElements.shift(), m = r, this._rowContainer.removeChild(f)), f.removeEventListener("focus", this._topBoundaryFocusListener), m.removeEventListener("focus", this._bottomBoundaryFocusListener), t === 0) {
-              const a = this._createAccessibilityTreeNode();
-              this._rowElements.unshift(a), this._rowContainer.insertAdjacentElement("afterbegin", a);
+              const o = this._createAccessibilityTreeNode();
+              this._rowElements.unshift(o), this._rowContainer.insertAdjacentElement("afterbegin", o);
             } else {
-              const a = this._createAccessibilityTreeNode();
-              this._rowElements.push(a), this._rowContainer.appendChild(a);
+              const o = this._createAccessibilityTreeNode();
+              this._rowElements.push(o), this._rowContainer.appendChild(o);
             }
             this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._terminal.scrollLines(t === 0 ? -1 : 1), this._rowElements[t === 0 ? 1 : this._rowElements.length - 2].focus(), n.preventDefault(), n.stopImmediatePropagation();
           }
           _handleResize(n) {
             this._rowElements[this._rowElements.length - 1].removeEventListener("focus", this._bottomBoundaryFocusListener);
             for (let t = this._rowContainer.children.length; t < this._terminal.rows; t++)
               this._rowElements[t] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[t]);
@@ -55,15 +55,15 @@
           }
           _handleTab(n) {
             for (let t = 0; t < n; t++)
               this._handleChar(" ");
           }
           _handleChar(n) {
             this._liveRegionLineCount < 21 && (this._charsToConsume.length > 0 ? this._charsToConsume.shift() !== n && (this._charsToAnnounce += n) : this._charsToAnnounce += n, n === `
-` && (this._liveRegionLineCount++, this._liveRegionLineCount === 21 && (this._liveRegion.textContent += h.tooMuchOutput)), u.isMac && this._liveRegion.textContent && this._liveRegion.textContent.length > 0 && !this._liveRegion.parentNode && setTimeout(() => {
+` && (this._liveRegionLineCount++, this._liveRegionLineCount === 21 && (this._liveRegion.textContent += a.tooMuchOutput)), u.isMac && this._liveRegion.textContent && this._liveRegion.textContent.length > 0 && !this._liveRegion.parentNode && setTimeout(() => {
               this._accessibilityTreeRoot.appendChild(this._liveRegion);
             }, 0));
           }
           _clearLiveRegion() {
             this._liveRegion.textContent = "", this._liveRegionLineCount = 0, u.isMac && (0, c.removeElementFromParent)(this._liveRegion);
           }
           _handleKey(n) {
@@ -71,16 +71,16 @@
           }
           _refreshRows(n, t) {
             this._renderRowsDebouncer.refresh(n, t, this._terminal.rows);
           }
           _renderRows(n, t) {
             const r = this._terminal.buffer, l = r.lines.length.toString();
             for (let f = n; f <= t; f++) {
-              const m = r.translateBufferLineToString(r.ydisp + f, !0), a = (r.ydisp + f + 1).toString(), p = this._rowElements[f];
-              p && (m.length === 0 ? p.innerText = " " : p.textContent = m, p.setAttribute("aria-posinset", a), p.setAttribute("aria-setsize", l));
+              const m = r.translateBufferLineToString(r.ydisp + f, !0), o = (r.ydisp + f + 1).toString(), p = this._rowElements[f];
+              p && (m.length === 0 ? p.innerText = " " : p.textContent = m, p.setAttribute("aria-posinset", o), p.setAttribute("aria-setsize", l));
             }
             this._announceCharacters();
           }
           _refreshRowsDimensions() {
             if (this._renderService.dimensions.css.cell.height) {
               this._accessibilityTreeRoot.style.width = `${this._renderService.dimensions.css.canvas.width}px`, this._rowElements.length !== this._terminal.rows && this._handleResize(this._terminal.rows);
               for (let n = 0; n < this._terminal.rows; n++)
@@ -92,40 +92,40 @@
           }
           _announceCharacters() {
             this._charsToAnnounce.length !== 0 && (this._liveRegion.textContent += this._charsToAnnounce, this._charsToAnnounce = "");
           }
         }
         i.AccessibilityManager = e;
       }, 3614: (T, i) => {
-        function o(_) {
+        function h(_) {
           return _.replace(/\r?\n/g, "\r");
         }
-        function h(_, g) {
+        function a(_, g) {
           return g ? "\x1B[200~" + _ + "\x1B[201~" : _;
         }
         function u(_, g, v) {
-          _ = h(_ = o(_), v.decPrivateModes.bracketedPasteMode), v.triggerDataEvent(_, !0), g.value = "";
+          _ = a(_ = h(_), v.decPrivateModes.bracketedPasteMode), v.triggerDataEvent(_, !0), g.value = "";
         }
         function d(_, g, v) {
           const c = v.getBoundingClientRect(), e = _.clientX - c.left - 10, s = _.clientY - c.top - 10;
           g.style.width = "20px", g.style.height = "20px", g.style.left = `${e}px`, g.style.top = `${s}px`, g.style.zIndex = "1000", g.focus();
         }
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.rightClickHandler = i.moveTextAreaUnderMouseCursor = i.paste = i.handlePasteEvent = i.copyHandler = i.bracketTextForPaste = i.prepareTextForTerminal = void 0, i.prepareTextForTerminal = o, i.bracketTextForPaste = h, i.copyHandler = function(_, g) {
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.rightClickHandler = i.moveTextAreaUnderMouseCursor = i.paste = i.handlePasteEvent = i.copyHandler = i.bracketTextForPaste = i.prepareTextForTerminal = void 0, i.prepareTextForTerminal = h, i.bracketTextForPaste = a, i.copyHandler = function(_, g) {
           _.clipboardData && _.clipboardData.setData("text/plain", g.selectionText), _.preventDefault();
         }, i.handlePasteEvent = function(_, g, v) {
           _.stopPropagation(), _.clipboardData && u(_.clipboardData.getData("text/plain"), g, v);
         }, i.paste = u, i.moveTextAreaUnderMouseCursor = d, i.rightClickHandler = function(_, g, v, c, e) {
           d(_, g, v), e && c.rightClickSelect(_), g.value = c.selectionText, g.select();
         };
-      }, 7239: (T, i, o) => {
+      }, 7239: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.ColorContrastCache = void 0;
-        const h = o(1505);
+        const a = h(1505);
         i.ColorContrastCache = class {
           constructor() {
-            this._color = new h.TwoKeyMap(), this._css = new h.TwoKeyMap();
+            this._color = new a.TwoKeyMap(), this._css = new a.TwoKeyMap();
           }
           setCss(u, d, _) {
             this._css.set(u, d, _);
           }
           getCss(u, d) {
             return this._css.get(u, d);
           }
@@ -136,43 +136,43 @@
             return this._color.get(u, d);
           }
           clear() {
             this._color.clear(), this._css.clear();
           }
         };
       }, 9631: (T, i) => {
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.removeElementFromParent = void 0, i.removeElementFromParent = function(...o) {
-          var h;
-          for (const u of o)
-            (h = u == null ? void 0 : u.parentElement) === null || h === void 0 || h.removeChild(u);
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.removeElementFromParent = void 0, i.removeElementFromParent = function(...h) {
+          var a;
+          for (const u of h)
+            (a = u == null ? void 0 : u.parentElement) === null || a === void 0 || a.removeChild(u);
         };
       }, 3656: (T, i) => {
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.addDisposableDomListener = void 0, i.addDisposableDomListener = function(o, h, u, d) {
-          o.addEventListener(h, u, d);
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.addDisposableDomListener = void 0, i.addDisposableDomListener = function(h, a, u, d) {
+          h.addEventListener(a, u, d);
           let _ = !1;
           return { dispose: () => {
-            _ || (_ = !0, o.removeEventListener(h, u, d));
+            _ || (_ = !0, h.removeEventListener(a, u, d));
           } };
         };
-      }, 6465: function(T, i, o) {
-        var h = this && this.__decorate || function(e, s, n, t) {
+      }, 6465: function(T, i, h) {
+        var a = this && this.__decorate || function(e, s, n, t) {
           var r, l = arguments.length, f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             f = Reflect.decorate(e, s, n, t);
           else
             for (var m = e.length - 1; m >= 0; m--)
               (r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
           return l > 3 && f && Object.defineProperty(s, n, f), f;
         }, u = this && this.__param || function(e, s) {
           return function(n, t) {
             s(n, t, e);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.Linkifier2 = void 0;
-        const d = o(2585), _ = o(8460), g = o(844), v = o(3656);
+        const d = h(2585), _ = h(8460), g = h(844), v = h(3656);
         let c = class extends g.Disposable {
           constructor(e) {
             super(), this._bufferService = e, this._linkProviders = [], this._linkCacheDisposables = [], this._isMouseOut = !0, this._activeLine = -1, this._onShowLinkUnderline = this.register(new _.EventEmitter()), this.onShowLinkUnderline = this._onShowLinkUnderline.event, this._onHideLinkUnderline = this.register(new _.EventEmitter()), this.onHideLinkUnderline = this._onHideLinkUnderline.event, this.register((0, g.getDisposeArrayDisposable)(this._linkCacheDisposables)), this.register((0, g.toDisposable)(() => {
               this._lastMouseEvent = void 0;
             }));
           }
           get currentLink() {
@@ -217,29 +217,29 @@
               l == null || l.forEach((f) => {
                 f.link.dispose && f.link.dispose();
               });
             }), this._activeProviderReplies = /* @__PURE__ */ new Map(), this._activeLine = e.y);
             let r = !1;
             for (const [l, f] of this._linkProviders.entries())
               s ? !((t = this._activeProviderReplies) === null || t === void 0) && t.get(l) && (r = this._checkLinkProviderResult(l, e, r)) : f.provideLinks(e.y, (m) => {
-                var a, p;
+                var o, p;
                 if (this._isMouseOut)
                   return;
                 const C = m == null ? void 0 : m.map((y) => ({ link: y }));
-                (a = this._activeProviderReplies) === null || a === void 0 || a.set(l, C), r = this._checkLinkProviderResult(l, e, r), ((p = this._activeProviderReplies) === null || p === void 0 ? void 0 : p.size) === this._linkProviders.length && this._removeIntersectingLinks(e.y, this._activeProviderReplies);
+                (o = this._activeProviderReplies) === null || o === void 0 || o.set(l, C), r = this._checkLinkProviderResult(l, e, r), ((p = this._activeProviderReplies) === null || p === void 0 ? void 0 : p.size) === this._linkProviders.length && this._removeIntersectingLinks(e.y, this._activeProviderReplies);
               });
           }
           _removeIntersectingLinks(e, s) {
             const n = /* @__PURE__ */ new Set();
             for (let t = 0; t < s.size; t++) {
               const r = s.get(t);
               if (r)
                 for (let l = 0; l < r.length; l++) {
-                  const f = r[l], m = f.link.range.start.y < e ? 0 : f.link.range.start.x, a = f.link.range.end.y > e ? this._bufferService.cols : f.link.range.end.x;
-                  for (let p = m; p <= a; p++) {
+                  const f = r[l], m = f.link.range.start.y < e ? 0 : f.link.range.start.x, o = f.link.range.end.y > e ? this._bufferService.cols : f.link.range.end.x;
+                  for (let p = m; p <= o; p++) {
                     if (n.has(p)) {
                       r.splice(l--, 1);
                       break;
                     }
                     n.add(p);
                   }
                 }
@@ -255,15 +255,15 @@
               this._activeProviderReplies.has(f) && !this._activeProviderReplies.get(f) || (l = !0);
             if (!l && r) {
               const f = r.find((m) => this._linkAtPosition(m.link, s));
               f && (n = !0, this._handleNewLink(f));
             }
             if (this._activeProviderReplies.size === this._linkProviders.length && !n)
               for (let f = 0; f < this._activeProviderReplies.size; f++) {
-                const m = (t = this._activeProviderReplies.get(f)) === null || t === void 0 ? void 0 : t.find((a) => this._linkAtPosition(a.link, s));
+                const m = (t = this._activeProviderReplies.get(f)) === null || t === void 0 ? void 0 : t.find((o) => this._linkAtPosition(o.link, s));
                 if (m) {
                   n = !0, this._handleNewLink(m);
                   break;
                 }
               }
             return n;
           }
@@ -324,58 +324,58 @@
             if (t)
               return { x: t[0], y: t[1] + this._bufferService.buffer.ydisp };
           }
           _createLinkUnderlineEvent(e, s, n, t, r) {
             return { x1: e, y1: s, x2: n, y2: t, cols: this._bufferService.cols, fg: r };
           }
         };
-        c = h([u(0, d.IBufferService)], c), i.Linkifier2 = c;
+        c = a([u(0, d.IBufferService)], c), i.Linkifier2 = c;
       }, 9042: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.tooMuchOutput = i.promptLabel = void 0, i.promptLabel = "Terminal input", i.tooMuchOutput = "Too much output to announce, navigate to rows manually to read";
-      }, 3730: function(T, i, o) {
-        var h = this && this.__decorate || function(c, e, s, n) {
+      }, 3730: function(T, i, h) {
+        var a = this && this.__decorate || function(c, e, s, n) {
           var t, r = arguments.length, l = r < 3 ? e : n === null ? n = Object.getOwnPropertyDescriptor(e, s) : n;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             l = Reflect.decorate(c, e, s, n);
           else
             for (var f = c.length - 1; f >= 0; f--)
               (t = c[f]) && (l = (r < 3 ? t(l) : r > 3 ? t(e, s, l) : t(e, s)) || l);
           return r > 3 && l && Object.defineProperty(e, s, l), l;
         }, u = this && this.__param || function(c, e) {
           return function(s, n) {
             e(s, n, c);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.OscLinkProvider = void 0;
-        const d = o(511), _ = o(2585);
+        const d = h(511), _ = h(2585);
         let g = class {
           constructor(c, e, s) {
             this._bufferService = c, this._optionsService = e, this._oscLinkService = s;
           }
           provideLinks(c, e) {
             var s;
             const n = this._bufferService.buffer.lines.get(c - 1);
             if (!n)
               return void e(void 0);
             const t = [], r = this._optionsService.rawOptions.linkHandler, l = new d.CellData(), f = n.getTrimmedLength();
-            let m = -1, a = -1, p = !1;
+            let m = -1, o = -1, p = !1;
             for (let C = 0; C < f; C++)
-              if (a !== -1 || n.hasContent(C)) {
+              if (o !== -1 || n.hasContent(C)) {
                 if (n.loadCell(C, l), l.hasExtendedAttrs() && l.extended.urlId) {
-                  if (a === -1) {
-                    a = C, m = l.extended.urlId;
+                  if (o === -1) {
+                    o = C, m = l.extended.urlId;
                     continue;
                   }
                   p = l.extended.urlId !== m;
                 } else
-                  a !== -1 && (p = !0);
-                if (p || a !== -1 && C === f - 1) {
+                  o !== -1 && (p = !0);
+                if (p || o !== -1 && C === f - 1) {
                   const y = (s = this._oscLinkService.getLinkData(m)) === null || s === void 0 ? void 0 : s.uri;
                   if (y) {
-                    const w = { start: { x: a + 1, y: c }, end: { x: C + (p || C !== f - 1 ? 0 : 1), y: c } };
+                    const w = { start: { x: o + 1, y: c }, end: { x: C + (p || C !== f - 1 ? 0 : 1), y: c } };
                     let D = !1;
                     if (!(r != null && r.allowNonHttpProtocols))
                       try {
                         const x = new URL(y);
                         ["http:", "https:"].includes(x.protocol) || (D = !0);
                       } catch {
                         D = !0;
@@ -384,15 +384,15 @@
                       var H;
                       return (H = r == null ? void 0 : r.hover) === null || H === void 0 ? void 0 : H.call(r, x, I, w);
                     }, leave: (x, I) => {
                       var H;
                       return (H = r == null ? void 0 : r.leave) === null || H === void 0 ? void 0 : H.call(r, x, I, w);
                     } });
                   }
-                  p = !1, l.hasExtendedAttrs() && l.extended.urlId ? (a = C, m = l.extended.urlId) : (a = -1, m = -1);
+                  p = !1, l.hasExtendedAttrs() && l.extended.urlId ? (o = C, m = l.extended.urlId) : (o = -1, m = -1);
                 }
               }
             e(t);
           }
         };
         function v(c, e) {
           if (confirm(`Do you want to navigate to ${e}?
@@ -405,47 +405,47 @@
               } catch {
               }
               s.location.href = e;
             } else
               console.warn("Opening link blocked as opener could not be cleared");
           }
         }
-        g = h([u(0, _.IBufferService), u(1, _.IOptionsService), u(2, _.IOscLinkService)], g), i.OscLinkProvider = g;
+        g = a([u(0, _.IBufferService), u(1, _.IOptionsService), u(2, _.IOscLinkService)], g), i.OscLinkProvider = g;
       }, 6193: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.RenderDebouncer = void 0, i.RenderDebouncer = class {
-          constructor(o, h) {
-            this._parentWindow = o, this._renderCallback = h, this._refreshCallbacks = [];
+          constructor(h, a) {
+            this._parentWindow = h, this._renderCallback = a, this._refreshCallbacks = [];
           }
           dispose() {
             this._animationFrame && (this._parentWindow.cancelAnimationFrame(this._animationFrame), this._animationFrame = void 0);
           }
-          addRefreshCallback(o) {
-            return this._refreshCallbacks.push(o), this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh())), this._animationFrame;
+          addRefreshCallback(h) {
+            return this._refreshCallbacks.push(h), this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh())), this._animationFrame;
           }
-          refresh(o, h, u) {
-            this._rowCount = u, o = o !== void 0 ? o : 0, h = h !== void 0 ? h : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, o) : o, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, h) : h, this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh()));
+          refresh(h, a, u) {
+            this._rowCount = u, h = h !== void 0 ? h : 0, a = a !== void 0 ? a : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, h) : h, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, a) : a, this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh()));
           }
           _innerRefresh() {
             if (this._animationFrame = void 0, this._rowStart === void 0 || this._rowEnd === void 0 || this._rowCount === void 0)
               return void this._runRefreshCallbacks();
-            const o = Math.max(this._rowStart, 0), h = Math.min(this._rowEnd, this._rowCount - 1);
-            this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(o, h), this._runRefreshCallbacks();
+            const h = Math.max(this._rowStart, 0), a = Math.min(this._rowEnd, this._rowCount - 1);
+            this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(h, a), this._runRefreshCallbacks();
           }
           _runRefreshCallbacks() {
-            for (const o of this._refreshCallbacks)
-              o(0);
+            for (const h of this._refreshCallbacks)
+              h(0);
             this._refreshCallbacks = [];
           }
         };
-      }, 5596: (T, i, o) => {
+      }, 5596: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.ScreenDprMonitor = void 0;
-        const h = o(844);
-        class u extends h.Disposable {
+        const a = h(844);
+        class u extends a.Disposable {
           constructor(_) {
-            super(), this._parentWindow = _, this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this.register((0, h.toDisposable)(() => {
+            super(), this._parentWindow = _, this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this.register((0, a.toDisposable)(() => {
               this.clearListener();
             }));
           }
           setListener(_) {
             this._listener && this.clearListener(), this._listener = _, this._outerListener = () => {
               this._listener && (this._listener(this._parentWindow.devicePixelRatio, this._currentDevicePixelRatio), this._updateDpr());
             }, this._updateDpr();
@@ -455,17 +455,17 @@
             this._outerListener && ((_ = this._resolutionMediaMatchList) === null || _ === void 0 || _.removeListener(this._outerListener), this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this._resolutionMediaMatchList = this._parentWindow.matchMedia(`screen and (resolution: ${this._parentWindow.devicePixelRatio}dppx)`), this._resolutionMediaMatchList.addListener(this._outerListener));
           }
           clearListener() {
             this._resolutionMediaMatchList && this._listener && this._outerListener && (this._resolutionMediaMatchList.removeListener(this._outerListener), this._resolutionMediaMatchList = void 0, this._listener = void 0, this._outerListener = void 0);
           }
         }
         i.ScreenDprMonitor = u;
-      }, 3236: (T, i, o) => {
+      }, 3236: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.Terminal = void 0;
-        const h = o(2950), u = o(1680), d = o(3614), _ = o(2584), g = o(5435), v = o(9312), c = o(6114), e = o(3656), s = o(9042), n = o(4567), t = o(1296), r = o(7399), l = o(8460), f = o(8437), m = o(3230), a = o(4725), p = o(428), C = o(8934), y = o(6465), w = o(5114), D = o(8969), x = o(8055), I = o(4269), H = o(5941), S = o(3107), b = o(5744), L = o(9074), R = o(2585), M = o(3730), F = o(844), $ = o(6731), O = typeof window < "u" ? window.document : null;
+        const a = h(2950), u = h(1680), d = h(3614), _ = h(2584), g = h(5435), v = h(9312), c = h(6114), e = h(3656), s = h(9042), n = h(4567), t = h(1296), r = h(7399), l = h(8460), f = h(8437), m = h(3230), o = h(4725), p = h(428), C = h(8934), y = h(6465), w = h(5114), D = h(8969), x = h(8055), I = h(4269), H = h(5941), S = h(3107), b = h(5744), L = h(9074), R = h(2585), M = h(3730), F = h(844), $ = h(6731), O = typeof window < "u" ? window.document : null;
         class N extends D.CoreTerminal {
           constructor(E = {}) {
             super(E), this.browser = c, this._keyDownHandled = !1, this._keyDownSeen = !1, this._keyPressHandled = !1, this._unprocessedDeadKey = !1, this._onCursorMove = this.register(new l.EventEmitter()), this.onCursorMove = this._onCursorMove.event, this._onKey = this.register(new l.EventEmitter()), this.onKey = this._onKey.event, this._onRender = this.register(new l.EventEmitter()), this.onRender = this._onRender.event, this._onSelectionChange = this.register(new l.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onTitleChange = this.register(new l.EventEmitter()), this.onTitleChange = this._onTitleChange.event, this._onBell = this.register(new l.EventEmitter()), this.onBell = this._onBell.event, this._onFocus = this.register(new l.EventEmitter()), this._onBlur = this.register(new l.EventEmitter()), this._onA11yCharEmitter = this.register(new l.EventEmitter()), this._onA11yTabEmitter = this.register(new l.EventEmitter()), this._onWillOpen = this.register(new l.EventEmitter()), this._setup(), this.linkifier2 = this.register(this._instantiationService.createInstance(y.Linkifier2)), this.linkifier2.registerLinkProvider(this._instantiationService.createInstance(M.OscLinkProvider)), this._decorationService = this._instantiationService.createInstance(L.DecorationService), this._instantiationService.setService(R.IDecorationService, this._decorationService), this.register(this._inputHandler.onRequestBell(() => this._onBell.fire())), this.register(this._inputHandler.onRequestRefreshRows((A, B) => this.refresh(A, B))), this.register(this._inputHandler.onRequestSendFocus(() => this._reportFocus())), this.register(this._inputHandler.onRequestReset(() => this.reset())), this.register(this._inputHandler.onRequestWindowsOptionsReport((A) => this._reportWindowsOptions(A))), this.register(this._inputHandler.onColor((A) => this._handleColorEvent(A))), this.register((0, l.forwardEvent)(this._inputHandler.onCursorMove, this._onCursorMove)), this.register((0, l.forwardEvent)(this._inputHandler.onTitleChange, this._onTitleChange)), this.register((0, l.forwardEvent)(this._inputHandler.onA11yChar, this._onA11yCharEmitter)), this.register((0, l.forwardEvent)(this._inputHandler.onA11yTab, this._onA11yTabEmitter)), this.register(this._bufferService.onResize((A) => this._afterResize(A.cols, A.rows))), this.register((0, F.toDisposable)(() => {
               var A, B;
               this._customKeyEventHandler = void 0, (B = (A = this.element) === null || A === void 0 ? void 0 : A.parentNode) === null || B === void 0 || B.removeChild(this.element);
             }));
           }
@@ -569,22 +569,22 @@
           }
           open(E) {
             var A;
             if (!E)
               throw new Error("Terminal requires a parent element.");
             E.isConnected || this._logService.debug("Terminal.open was called on an element that was not attached to the DOM"), this._document = E.ownerDocument, this.element = this._document.createElement("div"), this.element.dir = "ltr", this.element.classList.add("terminal"), this.element.classList.add("xterm"), this.element.setAttribute("tabindex", "0"), E.appendChild(this.element);
             const B = O.createDocumentFragment();
-            this._viewportElement = O.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), B.appendChild(this._viewportElement), this._viewportScrollArea = O.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = O.createElement("div"), this.screenElement.classList.add("xterm-screen"), this._helperContainer = O.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), B.appendChild(this.screenElement), this.textarea = O.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", s.promptLabel), c.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this._instantiationService.createInstance(w.CoreBrowserService, this.textarea, (A = this._document.defaultView) !== null && A !== void 0 ? A : window), this._instantiationService.setService(a.ICoreBrowserService, this._coreBrowserService), this.register((0, e.addDisposableDomListener)(this.textarea, "focus", (P) => this._handleTextAreaFocus(P))), this.register((0, e.addDisposableDomListener)(this.textarea, "blur", () => this._handleTextAreaBlur())), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(p.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(a.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance($.ThemeService), this._instantiationService.setService(a.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(I.CharacterJoinerService), this._instantiationService.setService(a.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(m.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(a.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange((P) => this._onRender.fire(P))), this.onResize((P) => this._renderService.resize(P.cols, P.rows)), this._compositionView = O.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(h.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this.element.appendChild(B);
+            this._viewportElement = O.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), B.appendChild(this._viewportElement), this._viewportScrollArea = O.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = O.createElement("div"), this.screenElement.classList.add("xterm-screen"), this._helperContainer = O.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), B.appendChild(this.screenElement), this.textarea = O.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", s.promptLabel), c.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this._instantiationService.createInstance(w.CoreBrowserService, this.textarea, (A = this._document.defaultView) !== null && A !== void 0 ? A : window), this._instantiationService.setService(o.ICoreBrowserService, this._coreBrowserService), this.register((0, e.addDisposableDomListener)(this.textarea, "focus", (P) => this._handleTextAreaFocus(P))), this.register((0, e.addDisposableDomListener)(this.textarea, "blur", () => this._handleTextAreaBlur())), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(p.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(o.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance($.ThemeService), this._instantiationService.setService(o.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(I.CharacterJoinerService), this._instantiationService.setService(o.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(m.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(o.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange((P) => this._onRender.fire(P))), this.onResize((P) => this._renderService.resize(P.cols, P.rows)), this._compositionView = O.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(a.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this.element.appendChild(B);
             try {
               this._onWillOpen.fire(this.element);
             } catch {
             }
-            this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this._mouseService = this._instantiationService.createInstance(C.MouseService), this._instantiationService.setService(a.IMouseService, this._mouseService), this.viewport = this._instantiationService.createInstance(u.Viewport, (P) => this.scrollLines(P, !0, 1), this._viewportElement, this._viewportScrollArea), this.register(this._inputHandler.onRequestSyncScrollBar(() => this.viewport.syncScrollArea())), this.register(this.viewport), this.register(this.onCursorMove(() => {
+            this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this._mouseService = this._instantiationService.createInstance(C.MouseService), this._instantiationService.setService(o.IMouseService, this._mouseService), this.viewport = this._instantiationService.createInstance(u.Viewport, (P) => this.scrollLines(P, !0, 1), this._viewportElement, this._viewportScrollArea), this.register(this._inputHandler.onRequestSyncScrollBar(() => this.viewport.syncScrollArea())), this.register(this.viewport), this.register(this.onCursorMove(() => {
               this._renderService.handleCursorMove(), this._syncTextArea();
-            })), this.register(this.onResize(() => this._renderService.handleResize(this.cols, this.rows))), this.register(this.onBlur(() => this._renderService.handleBlur())), this.register(this.onFocus(() => this._renderService.handleFocus())), this.register(this._renderService.onDimensionsChange(() => this.viewport.syncScrollArea())), this._selectionService = this.register(this._instantiationService.createInstance(v.SelectionService, this.element, this.screenElement, this.linkifier2)), this._instantiationService.setService(a.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines((P) => this.scrollLines(P.amount, P.suppressScrollEvent))), this.register(this._selectionService.onSelectionChange(() => this._onSelectionChange.fire())), this.register(this._selectionService.onRequestRedraw((P) => this._renderService.handleSelectionChanged(P.start, P.end, P.columnSelectMode))), this.register(this._selectionService.onLinuxMouseSelection((P) => {
+            })), this.register(this.onResize(() => this._renderService.handleResize(this.cols, this.rows))), this.register(this.onBlur(() => this._renderService.handleBlur())), this.register(this.onFocus(() => this._renderService.handleFocus())), this.register(this._renderService.onDimensionsChange(() => this.viewport.syncScrollArea())), this._selectionService = this.register(this._instantiationService.createInstance(v.SelectionService, this.element, this.screenElement, this.linkifier2)), this._instantiationService.setService(o.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines((P) => this.scrollLines(P.amount, P.suppressScrollEvent))), this.register(this._selectionService.onSelectionChange(() => this._onSelectionChange.fire())), this.register(this._selectionService.onRequestRedraw((P) => this._renderService.handleSelectionChanged(P.start, P.end, P.columnSelectMode))), this.register(this._selectionService.onLinuxMouseSelection((P) => {
               this.textarea.value = P, this.textarea.focus(), this.textarea.select();
             })), this.register(this._onScroll.event((P) => {
               this.viewport.syncScrollArea(), this._selectionService.refresh();
             })), this.register((0, e.addDisposableDomListener)(this._viewportElement, "scroll", () => this._selectionService.refresh())), this.linkifier2.attachToDom(this.screenElement, this._mouseService, this._renderService), this.register(this._instantiationService.createInstance(S.BufferDecorationRenderer, this.screenElement)), this.register((0, e.addDisposableDomListener)(this.element, "mousedown", (P) => this._selectionService.handleMouseDown(P))), this.coreMouseService.areMouseEventsActive ? (this._selectionService.disable(), this.element.classList.add("enable-mouse-events")) : this._selectionService.enable(), this.options.screenReaderMode && (this._accessibilityManager = new n.AccessibilityManager(this, this._renderService)), this.register(this.optionsService.onSpecificOptionChange("screenReaderMode", (P) => this._handleScreenReaderModeOptionChange(P))), this.options.overviewRulerWidth && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(b.OverviewRulerRenderer, this._viewportElement, this.screenElement))), this.optionsService.onSpecificOptionChange("overviewRulerWidth", (P) => {
               !this._overviewRulerRenderer && P && this._viewportElement && this.screenElement && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(b.OverviewRulerRenderer, this._viewportElement, this.screenElement)));
             }), this._charSizeService.measure(), this.refresh(0, this.rows - 1), this._initGlobal(), this.bindMouse();
           }
@@ -811,58 +811,58 @@
             if (this.options.cancelEvents || A)
               return E.preventDefault(), E.stopPropagation(), !1;
           }
         }
         i.Terminal = N;
       }, 9924: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.TimeBasedDebouncer = void 0, i.TimeBasedDebouncer = class {
-          constructor(o, h = 1e3) {
-            this._renderCallback = o, this._debounceThresholdMS = h, this._lastRefreshMs = 0, this._additionalRefreshRequested = !1;
+          constructor(h, a = 1e3) {
+            this._renderCallback = h, this._debounceThresholdMS = a, this._lastRefreshMs = 0, this._additionalRefreshRequested = !1;
           }
           dispose() {
             this._refreshTimeoutID && clearTimeout(this._refreshTimeoutID);
           }
-          refresh(o, h, u) {
-            this._rowCount = u, o = o !== void 0 ? o : 0, h = h !== void 0 ? h : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, o) : o, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, h) : h;
+          refresh(h, a, u) {
+            this._rowCount = u, h = h !== void 0 ? h : 0, a = a !== void 0 ? a : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, h) : h, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, a) : a;
             const d = Date.now();
             if (d - this._lastRefreshMs >= this._debounceThresholdMS)
               this._lastRefreshMs = d, this._innerRefresh();
             else if (!this._additionalRefreshRequested) {
               const _ = d - this._lastRefreshMs, g = this._debounceThresholdMS - _;
               this._additionalRefreshRequested = !0, this._refreshTimeoutID = window.setTimeout(() => {
                 this._lastRefreshMs = Date.now(), this._innerRefresh(), this._additionalRefreshRequested = !1, this._refreshTimeoutID = void 0;
               }, g);
             }
           }
           _innerRefresh() {
             if (this._rowStart === void 0 || this._rowEnd === void 0 || this._rowCount === void 0)
               return;
-            const o = Math.max(this._rowStart, 0), h = Math.min(this._rowEnd, this._rowCount - 1);
-            this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(o, h);
+            const h = Math.max(this._rowStart, 0), a = Math.min(this._rowEnd, this._rowCount - 1);
+            this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(h, a);
           }
         };
-      }, 1680: function(T, i, o) {
-        var h = this && this.__decorate || function(e, s, n, t) {
+      }, 1680: function(T, i, h) {
+        var a = this && this.__decorate || function(e, s, n, t) {
           var r, l = arguments.length, f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             f = Reflect.decorate(e, s, n, t);
           else
             for (var m = e.length - 1; m >= 0; m--)
               (r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
           return l > 3 && f && Object.defineProperty(s, n, f), f;
         }, u = this && this.__param || function(e, s) {
           return function(n, t) {
             s(n, t, e);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.Viewport = void 0;
-        const d = o(844), _ = o(3656), g = o(4725), v = o(2585);
+        const d = h(844), _ = h(3656), g = h(4725), v = h(2585);
         let c = class extends d.Disposable {
-          constructor(e, s, n, t, r, l, f, m, a) {
-            super(), this._scrollLines = e, this._viewportElement = s, this._scrollArea = n, this._bufferService = t, this._optionsService = r, this._charSizeService = l, this._renderService = f, this._coreBrowserService = m, this.scrollBarWidth = 0, this._currentRowHeight = 0, this._currentDeviceCellHeight = 0, this._lastRecordedBufferLength = 0, this._lastRecordedViewportHeight = 0, this._lastRecordedBufferHeight = 0, this._lastTouchY = 0, this._lastScrollTop = 0, this._wheelPartialScroll = 0, this._refreshAnimationFrame = null, this._ignoreNextScrollEvent = !1, this._smoothScrollState = { startTime: 0, origin: -1, target: -1 }, this.scrollBarWidth = this._viewportElement.offsetWidth - this._scrollArea.offsetWidth || 15, this.register((0, _.addDisposableDomListener)(this._viewportElement, "scroll", this._handleScroll.bind(this))), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate((p) => this._activeBuffer = p.activeBuffer)), this._renderDimensions = this._renderService.dimensions, this.register(this._renderService.onDimensionsChange((p) => this._renderDimensions = p)), this._handleThemeChange(a.colors), this.register(a.onChangeColors((p) => this._handleThemeChange(p))), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.syncScrollArea())), setTimeout(() => this.syncScrollArea(), 0);
+          constructor(e, s, n, t, r, l, f, m, o) {
+            super(), this._scrollLines = e, this._viewportElement = s, this._scrollArea = n, this._bufferService = t, this._optionsService = r, this._charSizeService = l, this._renderService = f, this._coreBrowserService = m, this.scrollBarWidth = 0, this._currentRowHeight = 0, this._currentDeviceCellHeight = 0, this._lastRecordedBufferLength = 0, this._lastRecordedViewportHeight = 0, this._lastRecordedBufferHeight = 0, this._lastTouchY = 0, this._lastScrollTop = 0, this._wheelPartialScroll = 0, this._refreshAnimationFrame = null, this._ignoreNextScrollEvent = !1, this._smoothScrollState = { startTime: 0, origin: -1, target: -1 }, this.scrollBarWidth = this._viewportElement.offsetWidth - this._scrollArea.offsetWidth || 15, this.register((0, _.addDisposableDomListener)(this._viewportElement, "scroll", this._handleScroll.bind(this))), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate((p) => this._activeBuffer = p.activeBuffer)), this._renderDimensions = this._renderService.dimensions, this.register(this._renderService.onDimensionsChange((p) => this._renderDimensions = p)), this._handleThemeChange(o.colors), this.register(o.onChangeColors((p) => this._handleThemeChange(p))), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.syncScrollArea())), setTimeout(() => this.syncScrollArea(), 0);
           }
           _handleThemeChange(e) {
             this._viewportElement.style.backgroundColor = e.background.css;
           }
           _refresh(e) {
             if (e)
               return this._innerRefresh(), void (this._refreshAnimationFrame !== null && this._coreBrowserService.window.cancelAnimationFrame(this._refreshAnimationFrame));
@@ -930,31 +930,31 @@
             this._lastTouchY = e.touches[0].pageY;
           }
           handleTouchMove(e) {
             const s = this._lastTouchY - e.touches[0].pageY;
             return this._lastTouchY = e.touches[0].pageY, s !== 0 && (this._viewportElement.scrollTop += s, this._bubbleScroll(e, s));
           }
         };
-        c = h([u(3, v.IBufferService), u(4, v.IOptionsService), u(5, g.ICharSizeService), u(6, g.IRenderService), u(7, g.ICoreBrowserService), u(8, g.IThemeService)], c), i.Viewport = c;
-      }, 3107: function(T, i, o) {
-        var h = this && this.__decorate || function(e, s, n, t) {
+        c = a([u(3, v.IBufferService), u(4, v.IOptionsService), u(5, g.ICharSizeService), u(6, g.IRenderService), u(7, g.ICoreBrowserService), u(8, g.IThemeService)], c), i.Viewport = c;
+      }, 3107: function(T, i, h) {
+        var a = this && this.__decorate || function(e, s, n, t) {
           var r, l = arguments.length, f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             f = Reflect.decorate(e, s, n, t);
           else
             for (var m = e.length - 1; m >= 0; m--)
               (r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
           return l > 3 && f && Object.defineProperty(s, n, f), f;
         }, u = this && this.__param || function(e, s) {
           return function(n, t) {
             s(n, t, e);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferDecorationRenderer = void 0;
-        const d = o(3656), _ = o(4725), g = o(844), v = o(2585);
+        const d = h(3656), _ = h(4725), g = h(844), v = h(2585);
         let c = class extends g.Disposable {
           constructor(e, s, n, t) {
             super(), this._screenElement = e, this._bufferService = s, this._decorationService = n, this._renderService = t, this._decorationElements = /* @__PURE__ */ new Map(), this._altBufferIsActive = !1, this._dimensionsChanged = !1, this._container = document.createElement("div"), this._container.classList.add("xterm-decoration-container"), this._screenElement.appendChild(this._container), this.register(this._renderService.onRenderedViewportChange(() => this._doRefreshDecorations())), this.register(this._renderService.onDimensionsChange(() => {
               this._dimensionsChanged = !0, this._queueRefresh();
             })), this.register((0, d.addDisposableDomListener)(window, "resize", () => this._queueRefresh())), this.register(this._bufferService.buffers.onBufferActivate(() => {
               this._altBufferIsActive = this._bufferService.buffer === this._bufferService.buffers.alt;
             })), this.register(this._decorationService.onDecorationRegistered(() => this._queueRefresh())), this.register(this._decorationService.onDecorationRemoved((r) => this._removeDecoration(r))), this.register((0, g.toDisposable)(() => {
@@ -998,73 +998,73 @@
             (e.options.anchor || "left") === "right" ? s.style.right = t ? t * this._renderService.dimensions.css.cell.width + "px" : "" : s.style.left = t ? t * this._renderService.dimensions.css.cell.width + "px" : "";
           }
           _removeDecoration(e) {
             var s;
             (s = this._decorationElements.get(e)) === null || s === void 0 || s.remove(), this._decorationElements.delete(e), e.dispose();
           }
         };
-        c = h([u(1, v.IBufferService), u(2, v.IDecorationService), u(3, _.IRenderService)], c), i.BufferDecorationRenderer = c;
+        c = a([u(1, v.IBufferService), u(2, v.IDecorationService), u(3, _.IRenderService)], c), i.BufferDecorationRenderer = c;
       }, 5871: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.ColorZoneStore = void 0, i.ColorZoneStore = class {
           constructor() {
             this._zones = [], this._zonePool = [], this._zonePoolIndex = 0, this._linePadding = { full: 0, left: 0, center: 0, right: 0 };
           }
           get zones() {
             return this._zonePool.length = Math.min(this._zonePool.length, this._zones.length), this._zones;
           }
           clear() {
             this._zones.length = 0, this._zonePoolIndex = 0;
           }
-          addDecoration(o) {
-            if (o.options.overviewRulerOptions) {
-              for (const h of this._zones)
-                if (h.color === o.options.overviewRulerOptions.color && h.position === o.options.overviewRulerOptions.position) {
-                  if (this._lineIntersectsZone(h, o.marker.line))
+          addDecoration(h) {
+            if (h.options.overviewRulerOptions) {
+              for (const a of this._zones)
+                if (a.color === h.options.overviewRulerOptions.color && a.position === h.options.overviewRulerOptions.position) {
+                  if (this._lineIntersectsZone(a, h.marker.line))
                     return;
-                  if (this._lineAdjacentToZone(h, o.marker.line, o.options.overviewRulerOptions.position))
-                    return void this._addLineToZone(h, o.marker.line);
+                  if (this._lineAdjacentToZone(a, h.marker.line, h.options.overviewRulerOptions.position))
+                    return void this._addLineToZone(a, h.marker.line);
                 }
               if (this._zonePoolIndex < this._zonePool.length)
-                return this._zonePool[this._zonePoolIndex].color = o.options.overviewRulerOptions.color, this._zonePool[this._zonePoolIndex].position = o.options.overviewRulerOptions.position, this._zonePool[this._zonePoolIndex].startBufferLine = o.marker.line, this._zonePool[this._zonePoolIndex].endBufferLine = o.marker.line, void this._zones.push(this._zonePool[this._zonePoolIndex++]);
-              this._zones.push({ color: o.options.overviewRulerOptions.color, position: o.options.overviewRulerOptions.position, startBufferLine: o.marker.line, endBufferLine: o.marker.line }), this._zonePool.push(this._zones[this._zones.length - 1]), this._zonePoolIndex++;
+                return this._zonePool[this._zonePoolIndex].color = h.options.overviewRulerOptions.color, this._zonePool[this._zonePoolIndex].position = h.options.overviewRulerOptions.position, this._zonePool[this._zonePoolIndex].startBufferLine = h.marker.line, this._zonePool[this._zonePoolIndex].endBufferLine = h.marker.line, void this._zones.push(this._zonePool[this._zonePoolIndex++]);
+              this._zones.push({ color: h.options.overviewRulerOptions.color, position: h.options.overviewRulerOptions.position, startBufferLine: h.marker.line, endBufferLine: h.marker.line }), this._zonePool.push(this._zones[this._zones.length - 1]), this._zonePoolIndex++;
             }
           }
-          setPadding(o) {
-            this._linePadding = o;
+          setPadding(h) {
+            this._linePadding = h;
           }
-          _lineIntersectsZone(o, h) {
-            return h >= o.startBufferLine && h <= o.endBufferLine;
+          _lineIntersectsZone(h, a) {
+            return a >= h.startBufferLine && a <= h.endBufferLine;
           }
-          _lineAdjacentToZone(o, h, u) {
-            return h >= o.startBufferLine - this._linePadding[u || "full"] && h <= o.endBufferLine + this._linePadding[u || "full"];
+          _lineAdjacentToZone(h, a, u) {
+            return a >= h.startBufferLine - this._linePadding[u || "full"] && a <= h.endBufferLine + this._linePadding[u || "full"];
           }
-          _addLineToZone(o, h) {
-            o.startBufferLine = Math.min(o.startBufferLine, h), o.endBufferLine = Math.max(o.endBufferLine, h);
+          _addLineToZone(h, a) {
+            h.startBufferLine = Math.min(h.startBufferLine, a), h.endBufferLine = Math.max(h.endBufferLine, a);
           }
         };
-      }, 5744: function(T, i, o) {
-        var h = this && this.__decorate || function(r, l, f, m) {
-          var a, p = arguments.length, C = p < 3 ? l : m === null ? m = Object.getOwnPropertyDescriptor(l, f) : m;
+      }, 5744: function(T, i, h) {
+        var a = this && this.__decorate || function(r, l, f, m) {
+          var o, p = arguments.length, C = p < 3 ? l : m === null ? m = Object.getOwnPropertyDescriptor(l, f) : m;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             C = Reflect.decorate(r, l, f, m);
           else
             for (var y = r.length - 1; y >= 0; y--)
-              (a = r[y]) && (C = (p < 3 ? a(C) : p > 3 ? a(l, f, C) : a(l, f)) || C);
+              (o = r[y]) && (C = (p < 3 ? o(C) : p > 3 ? o(l, f, C) : o(l, f)) || C);
           return p > 3 && C && Object.defineProperty(l, f, C), C;
         }, u = this && this.__param || function(r, l) {
           return function(f, m) {
             l(f, m, r);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.OverviewRulerRenderer = void 0;
-        const d = o(5871), _ = o(3656), g = o(4725), v = o(844), c = o(2585), e = { full: 0, left: 0, center: 0, right: 0 }, s = { full: 0, left: 0, center: 0, right: 0 }, n = { full: 0, left: 0, center: 0, right: 0 };
+        const d = h(5871), _ = h(3656), g = h(4725), v = h(844), c = h(2585), e = { full: 0, left: 0, center: 0, right: 0 }, s = { full: 0, left: 0, center: 0, right: 0 }, n = { full: 0, left: 0, center: 0, right: 0 };
         let t = class extends v.Disposable {
-          constructor(r, l, f, m, a, p, C) {
+          constructor(r, l, f, m, o, p, C) {
             var y;
-            super(), this._viewportElement = r, this._screenElement = l, this._bufferService = f, this._decorationService = m, this._renderService = a, this._optionsService = p, this._coreBrowseService = C, this._colorZoneStore = new d.ColorZoneStore(), this._shouldUpdateDimensions = !0, this._shouldUpdateAnchor = !0, this._lastKnownBufferLength = 0, this._canvas = document.createElement("canvas"), this._canvas.classList.add("xterm-decoration-overview-ruler"), this._refreshCanvasDimensions(), (y = this._viewportElement.parentElement) === null || y === void 0 || y.insertBefore(this._canvas, this._viewportElement);
+            super(), this._viewportElement = r, this._screenElement = l, this._bufferService = f, this._decorationService = m, this._renderService = o, this._optionsService = p, this._coreBrowseService = C, this._colorZoneStore = new d.ColorZoneStore(), this._shouldUpdateDimensions = !0, this._shouldUpdateAnchor = !0, this._lastKnownBufferLength = 0, this._canvas = document.createElement("canvas"), this._canvas.classList.add("xterm-decoration-overview-ruler"), this._refreshCanvasDimensions(), (y = this._viewportElement.parentElement) === null || y === void 0 || y.insertBefore(this._canvas, this._viewportElement);
             const w = this._canvas.getContext("2d");
             if (!w)
               throw new Error("Ctx cannot be null");
             this._ctx = w, this._registerDecorationListeners(), this._registerBufferChangeListeners(), this._registerDimensionChangeListeners(), this.register((0, v.toDisposable)(() => {
               var D;
               (D = this._canvas) === null || D === void 0 || D.remove();
             }));
@@ -1119,31 +1119,31 @@
           }
           _queueRefresh(r, l) {
             this._shouldUpdateDimensions = r || this._shouldUpdateDimensions, this._shouldUpdateAnchor = l || this._shouldUpdateAnchor, this._animationFrame === void 0 && (this._animationFrame = this._coreBrowseService.window.requestAnimationFrame(() => {
               this._refreshDecorations(), this._animationFrame = void 0;
             }));
           }
         };
-        t = h([u(2, c.IBufferService), u(3, c.IDecorationService), u(4, g.IRenderService), u(5, c.IOptionsService), u(6, g.ICoreBrowserService)], t), i.OverviewRulerRenderer = t;
-      }, 2950: function(T, i, o) {
-        var h = this && this.__decorate || function(c, e, s, n) {
+        t = a([u(2, c.IBufferService), u(3, c.IDecorationService), u(4, g.IRenderService), u(5, c.IOptionsService), u(6, g.ICoreBrowserService)], t), i.OverviewRulerRenderer = t;
+      }, 2950: function(T, i, h) {
+        var a = this && this.__decorate || function(c, e, s, n) {
           var t, r = arguments.length, l = r < 3 ? e : n === null ? n = Object.getOwnPropertyDescriptor(e, s) : n;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             l = Reflect.decorate(c, e, s, n);
           else
             for (var f = c.length - 1; f >= 0; f--)
               (t = c[f]) && (l = (r < 3 ? t(l) : r > 3 ? t(e, s, l) : t(e, s)) || l);
           return r > 3 && l && Object.defineProperty(e, s, l), l;
         }, u = this && this.__param || function(c, e) {
           return function(s, n) {
             e(s, n, c);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CompositionHelper = void 0;
-        const d = o(4725), _ = o(2585), g = o(2584);
+        const d = h(4725), _ = h(2585), g = h(2584);
         let v = class {
           constructor(c, e, s, n, t, r) {
             this._textarea = c, this._compositionView = e, this._bufferService = s, this._optionsService = n, this._coreService = t, this._renderService = r, this._isComposing = !1, this._isSendingComposition = !1, this._compositionPosition = { start: 0, end: 0 }, this._dataAlreadySent = "";
           }
           get isComposing() {
             return this._isComposing;
           }
@@ -1198,35 +1198,35 @@
                 const r = this._compositionView.getBoundingClientRect();
                 this._textarea.style.left = t + "px", this._textarea.style.top = n + "px", this._textarea.style.width = Math.max(r.width, 1) + "px", this._textarea.style.height = Math.max(r.height, 1) + "px", this._textarea.style.lineHeight = r.height + "px";
               }
               c || setTimeout(() => this.updateCompositionElements(!0), 0);
             }
           }
         };
-        v = h([u(2, _.IBufferService), u(3, _.IOptionsService), u(4, _.ICoreService), u(5, d.IRenderService)], v), i.CompositionHelper = v;
+        v = a([u(2, _.IBufferService), u(3, _.IOptionsService), u(4, _.ICoreService), u(5, d.IRenderService)], v), i.CompositionHelper = v;
       }, 9806: (T, i) => {
-        function o(h, u, d) {
-          const _ = d.getBoundingClientRect(), g = h.getComputedStyle(d), v = parseInt(g.getPropertyValue("padding-left")), c = parseInt(g.getPropertyValue("padding-top"));
+        function h(a, u, d) {
+          const _ = d.getBoundingClientRect(), g = a.getComputedStyle(d), v = parseInt(g.getPropertyValue("padding-left")), c = parseInt(g.getPropertyValue("padding-top"));
           return [u.clientX - _.left - v, u.clientY - _.top - c];
         }
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.getCoords = i.getCoordsRelativeToElement = void 0, i.getCoordsRelativeToElement = o, i.getCoords = function(h, u, d, _, g, v, c, e, s) {
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.getCoords = i.getCoordsRelativeToElement = void 0, i.getCoordsRelativeToElement = h, i.getCoords = function(a, u, d, _, g, v, c, e, s) {
           if (!v)
             return;
-          const n = o(h, u, d);
+          const n = h(a, u, d);
           return n ? (n[0] = Math.ceil((n[0] + (s ? c / 2 : 0)) / c), n[1] = Math.ceil(n[1] / e), n[0] = Math.min(Math.max(n[0], 1), _ + (s ? 1 : 0)), n[1] = Math.min(Math.max(n[1], 1), g), n) : void 0;
         };
-      }, 9504: (T, i, o) => {
+      }, 9504: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.moveToCellSequence = void 0;
-        const h = o(2584);
+        const a = h(2584);
         function u(e, s, n, t) {
-          const r = e - d(e, n), l = s - d(s, n), f = Math.abs(r - l) - function(m, a, p) {
+          const r = e - d(e, n), l = s - d(s, n), f = Math.abs(r - l) - function(m, o, p) {
             let C = 0;
-            const y = m - d(m, p), w = a - d(a, p);
+            const y = m - d(m, p), w = o - d(o, p);
             for (let D = 0; D < Math.abs(y - w); D++) {
-              const x = _(m, a) === "A" ? -1 : 1, I = p.buffer.lines.get(y + x * D);
+              const x = _(m, o) === "A" ? -1 : 1, I = p.buffer.lines.get(y + x * D);
               I != null && I.isWrapped && C++;
             }
             return C;
           }(e, s, n);
           return c(f, v(_(e, s), t));
         }
         function d(e, s) {
@@ -1235,208 +1235,208 @@
             n++, t = s.buffer.lines.get(--e), r = t == null ? void 0 : t.isWrapped;
           return n;
         }
         function _(e, s) {
           return e > s ? "A" : "B";
         }
         function g(e, s, n, t, r, l) {
-          let f = e, m = s, a = "";
+          let f = e, m = s, o = "";
           for (; f !== n || m !== t; )
-            f += r ? 1 : -1, r && f > l.cols - 1 ? (a += l.buffer.translateBufferLineToString(m, !1, e, f), f = 0, e = 0, m++) : !r && f < 0 && (a += l.buffer.translateBufferLineToString(m, !1, 0, e + 1), f = l.cols - 1, e = f, m--);
-          return a + l.buffer.translateBufferLineToString(m, !1, e, f);
+            f += r ? 1 : -1, r && f > l.cols - 1 ? (o += l.buffer.translateBufferLineToString(m, !1, e, f), f = 0, e = 0, m++) : !r && f < 0 && (o += l.buffer.translateBufferLineToString(m, !1, 0, e + 1), f = l.cols - 1, e = f, m--);
+          return o + l.buffer.translateBufferLineToString(m, !1, e, f);
         }
         function v(e, s) {
           const n = s ? "O" : "[";
-          return h.C0.ESC + n + e;
+          return a.C0.ESC + n + e;
         }
         function c(e, s) {
           e = Math.floor(e);
           let n = "";
           for (let t = 0; t < e; t++)
             n += s;
           return n;
         }
         i.moveToCellSequence = function(e, s, n, t) {
           const r = n.buffer.x, l = n.buffer.y;
           if (!n.buffer.hasScrollback)
-            return function(a, p, C, y, w, D) {
-              return u(p, y, w, D).length === 0 ? "" : c(g(a, p, a, p - d(p, w), !1, w).length, v("D", D));
-            }(r, l, 0, s, n, t) + u(l, s, n, t) + function(a, p, C, y, w, D) {
+            return function(o, p, C, y, w, D) {
+              return u(p, y, w, D).length === 0 ? "" : c(g(o, p, o, p - d(p, w), !1, w).length, v("D", D));
+            }(r, l, 0, s, n, t) + u(l, s, n, t) + function(o, p, C, y, w, D) {
               let x;
               x = u(p, y, w, D).length > 0 ? y - d(y, w) : p;
               const I = y, H = function(S, b, L, R, M, F) {
                 let $;
                 return $ = u(L, R, M, F).length > 0 ? R - d(R, M) : b, S < L && $ <= R || S >= L && $ < R ? "C" : "D";
-              }(a, p, C, y, w, D);
-              return c(g(a, x, C, I, H === "C", w).length, v(H, D));
+              }(o, p, C, y, w, D);
+              return c(g(o, x, C, I, H === "C", w).length, v(H, D));
             }(r, l, e, s, n, t);
           let f;
           if (l === s)
             return f = r > e ? "D" : "C", c(Math.abs(r - e), v(f, t));
           f = l > s ? "D" : "C";
           const m = Math.abs(l - s);
-          return c(function(a, p) {
-            return p.cols - a;
+          return c(function(o, p) {
+            return p.cols - o;
           }(l > s ? e : r, n) + (m - 1) * n.cols + 1 + ((l > s ? r : e) - 1), v(f, t));
         };
-      }, 1296: function(T, i, o) {
-        var h = this && this.__decorate || function(a, p, C, y) {
+      }, 1296: function(T, i, h) {
+        var a = this && this.__decorate || function(o, p, C, y) {
           var w, D = arguments.length, x = D < 3 ? p : y === null ? y = Object.getOwnPropertyDescriptor(p, C) : y;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-            x = Reflect.decorate(a, p, C, y);
+            x = Reflect.decorate(o, p, C, y);
           else
-            for (var I = a.length - 1; I >= 0; I--)
-              (w = a[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
+            for (var I = o.length - 1; I >= 0; I--)
+              (w = o[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
           return D > 3 && x && Object.defineProperty(p, C, x), x;
-        }, u = this && this.__param || function(a, p) {
+        }, u = this && this.__param || function(o, p) {
           return function(C, y) {
-            p(C, y, a);
+            p(C, y, o);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.DomRenderer = void 0;
-        const d = o(9631), _ = o(3787), g = o(2223), v = o(6171), c = o(4725), e = o(8055), s = o(8460), n = o(844), t = o(2585), r = "xterm-dom-renderer-owner-", l = "xterm-focus";
+        const d = h(9631), _ = h(3787), g = h(2223), v = h(6171), c = h(4725), e = h(8055), s = h(8460), n = h(844), t = h(2585), r = "xterm-dom-renderer-owner-", l = "xterm-focus";
         let f = 1, m = class extends n.Disposable {
-          constructor(a, p, C, y, w, D, x, I, H, S) {
-            super(), this._element = a, this._screenElement = p, this._viewportElement = C, this._linkifier2 = y, this._charSizeService = D, this._optionsService = x, this._bufferService = I, this._coreBrowserService = H, this._terminalClass = f++, this._rowElements = [], this._cellToRowElements = [], this.onRequestRedraw = this.register(new s.EventEmitter()).event, this._rowContainer = document.createElement("div"), this._rowContainer.classList.add("xterm-rows"), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = document.createElement("div"), this._selectionContainer.classList.add("xterm-selection"), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, v.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange(() => this._handleOptionsChanged())), this.register(S.onChangeColors((b) => this._injectCss(b))), this._injectCss(S.colors), this._rowFactory = w.createInstance(_.DomRendererRowFactory, document), this._element.classList.add(r + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline((b) => this._handleLinkHover(b))), this.register(this._linkifier2.onHideLinkUnderline((b) => this._handleLinkLeave(b))), this.register((0, n.toDisposable)(() => {
+          constructor(o, p, C, y, w, D, x, I, H, S) {
+            super(), this._element = o, this._screenElement = p, this._viewportElement = C, this._linkifier2 = y, this._charSizeService = D, this._optionsService = x, this._bufferService = I, this._coreBrowserService = H, this._terminalClass = f++, this._rowElements = [], this._cellToRowElements = [], this.onRequestRedraw = this.register(new s.EventEmitter()).event, this._rowContainer = document.createElement("div"), this._rowContainer.classList.add("xterm-rows"), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = document.createElement("div"), this._selectionContainer.classList.add("xterm-selection"), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, v.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange(() => this._handleOptionsChanged())), this.register(S.onChangeColors((b) => this._injectCss(b))), this._injectCss(S.colors), this._rowFactory = w.createInstance(_.DomRendererRowFactory, document), this._element.classList.add(r + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline((b) => this._handleLinkHover(b))), this.register(this._linkifier2.onHideLinkUnderline((b) => this._handleLinkLeave(b))), this.register((0, n.toDisposable)(() => {
               this._element.classList.remove(r + this._terminalClass), (0, d.removeElementFromParent)(this._rowContainer, this._selectionContainer, this._themeStyleElement, this._dimensionsStyleElement);
             }));
           }
           _updateDimensions() {
-            const a = this._coreBrowserService.dpr;
-            this.dimensions.device.char.width = this._charSizeService.width * a, this.dimensions.device.char.height = Math.ceil(this._charSizeService.height * a), this.dimensions.device.cell.width = this.dimensions.device.char.width + Math.round(this._optionsService.rawOptions.letterSpacing), this.dimensions.device.cell.height = Math.floor(this.dimensions.device.char.height * this._optionsService.rawOptions.lineHeight), this.dimensions.device.char.left = 0, this.dimensions.device.char.top = 0, this.dimensions.device.canvas.width = this.dimensions.device.cell.width * this._bufferService.cols, this.dimensions.device.canvas.height = this.dimensions.device.cell.height * this._bufferService.rows, this.dimensions.css.canvas.width = Math.round(this.dimensions.device.canvas.width / a), this.dimensions.css.canvas.height = Math.round(this.dimensions.device.canvas.height / a), this.dimensions.css.cell.width = this.dimensions.css.canvas.width / this._bufferService.cols, this.dimensions.css.cell.height = this.dimensions.css.canvas.height / this._bufferService.rows;
+            const o = this._coreBrowserService.dpr;
+            this.dimensions.device.char.width = this._charSizeService.width * o, this.dimensions.device.char.height = Math.ceil(this._charSizeService.height * o), this.dimensions.device.cell.width = this.dimensions.device.char.width + Math.round(this._optionsService.rawOptions.letterSpacing), this.dimensions.device.cell.height = Math.floor(this.dimensions.device.char.height * this._optionsService.rawOptions.lineHeight), this.dimensions.device.char.left = 0, this.dimensions.device.char.top = 0, this.dimensions.device.canvas.width = this.dimensions.device.cell.width * this._bufferService.cols, this.dimensions.device.canvas.height = this.dimensions.device.cell.height * this._bufferService.rows, this.dimensions.css.canvas.width = Math.round(this.dimensions.device.canvas.width / o), this.dimensions.css.canvas.height = Math.round(this.dimensions.device.canvas.height / o), this.dimensions.css.cell.width = this.dimensions.css.canvas.width / this._bufferService.cols, this.dimensions.css.cell.height = this.dimensions.css.canvas.height / this._bufferService.rows;
             for (const C of this._rowElements)
               C.style.width = `${this.dimensions.css.canvas.width}px`, C.style.height = `${this.dimensions.css.cell.height}px`, C.style.lineHeight = `${this.dimensions.css.cell.height}px`, C.style.overflow = "hidden";
             this._dimensionsStyleElement || (this._dimensionsStyleElement = document.createElement("style"), this._screenElement.appendChild(this._dimensionsStyleElement));
             const p = `${this._terminalSelector} .xterm-rows span { display: inline-block; height: 100%; vertical-align: top; width: ${this.dimensions.css.cell.width}px}`;
             this._dimensionsStyleElement.textContent = p, this._selectionContainer.style.height = this._viewportElement.style.height, this._screenElement.style.width = `${this.dimensions.css.canvas.width}px`, this._screenElement.style.height = `${this.dimensions.css.canvas.height}px`;
           }
-          _injectCss(a) {
+          _injectCss(o) {
             this._themeStyleElement || (this._themeStyleElement = document.createElement("style"), this._screenElement.appendChild(this._themeStyleElement));
-            let p = `${this._terminalSelector} .xterm-rows { color: ${a.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px;}`;
-            p += `${this._terminalSelector} span:not(.${_.BOLD_CLASS}) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.${_.BOLD_CLASS} { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.${_.ITALIC_CLASS} { font-style: italic;}`, p += "@keyframes blink_box_shadow_" + this._terminalClass + " { 50% {  box-shadow: none; }}", p += "@keyframes blink_block_" + this._terminalClass + ` { 0% {  background-color: ${a.cursor.css};  color: ${a.cursorAccent.css}; } 50% {  background-color: ${a.cursorAccent.css};  color: ${a.cursor.css}; }}`, p += `${this._terminalSelector} .xterm-rows:not(.xterm-focus) .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { outline: 1px solid ${a.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}:not(.${_.CURSOR_STYLE_BLOCK_CLASS}) { animation: blink_box_shadow_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { animation: blink_block_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { background-color: ${a.cursor.css}; color: ${a.cursorAccent.css};}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BAR_CLASS} { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${a.cursor.css} inset;}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_UNDERLINE_CLASS} { box-shadow: 0 -1px 0 ${a.cursor.css} inset;}`, p += `${this._terminalSelector} .xterm-selection { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .xterm-selection div { position: absolute; background-color: ${a.selectionBackgroundOpaque.css};}${this._terminalSelector} .xterm-selection div { position: absolute; background-color: ${a.selectionInactiveBackgroundOpaque.css};}`;
-            for (const [C, y] of a.ansi.entries())
+            let p = `${this._terminalSelector} .xterm-rows { color: ${o.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px;}`;
+            p += `${this._terminalSelector} span:not(.${_.BOLD_CLASS}) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.${_.BOLD_CLASS} { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.${_.ITALIC_CLASS} { font-style: italic;}`, p += "@keyframes blink_box_shadow_" + this._terminalClass + " { 50% {  box-shadow: none; }}", p += "@keyframes blink_block_" + this._terminalClass + ` { 0% {  background-color: ${o.cursor.css};  color: ${o.cursorAccent.css}; } 50% {  background-color: ${o.cursorAccent.css};  color: ${o.cursor.css}; }}`, p += `${this._terminalSelector} .xterm-rows:not(.xterm-focus) .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { outline: 1px solid ${o.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}:not(.${_.CURSOR_STYLE_BLOCK_CLASS}) { animation: blink_box_shadow_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { animation: blink_block_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { background-color: ${o.cursor.css}; color: ${o.cursorAccent.css};}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BAR_CLASS} { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${o.cursor.css} inset;}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_UNDERLINE_CLASS} { box-shadow: 0 -1px 0 ${o.cursor.css} inset;}`, p += `${this._terminalSelector} .xterm-selection { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .xterm-selection div { position: absolute; background-color: ${o.selectionBackgroundOpaque.css};}${this._terminalSelector} .xterm-selection div { position: absolute; background-color: ${o.selectionInactiveBackgroundOpaque.css};}`;
+            for (const [C, y] of o.ansi.entries())
               p += `${this._terminalSelector} .xterm-fg-${C} { color: ${y.css}; }${this._terminalSelector} .xterm-bg-${C} { background-color: ${y.css}; }`;
-            p += `${this._terminalSelector} .xterm-fg-${g.INVERTED_DEFAULT_COLOR} { color: ${e.color.opaque(a.background).css}; }${this._terminalSelector} .xterm-bg-${g.INVERTED_DEFAULT_COLOR} { background-color: ${a.foreground.css}; }`, this._themeStyleElement.textContent = p;
+            p += `${this._terminalSelector} .xterm-fg-${g.INVERTED_DEFAULT_COLOR} { color: ${e.color.opaque(o.background).css}; }${this._terminalSelector} .xterm-bg-${g.INVERTED_DEFAULT_COLOR} { background-color: ${o.foreground.css}; }`, this._themeStyleElement.textContent = p;
           }
           handleDevicePixelRatioChange() {
             this._updateDimensions();
           }
-          _refreshRowElements(a, p) {
+          _refreshRowElements(o, p) {
             for (let C = this._rowElements.length; C <= p; C++) {
               const y = document.createElement("div");
               this._rowContainer.appendChild(y), this._rowElements.push(y);
             }
             for (; this._rowElements.length > p; )
               this._rowContainer.removeChild(this._rowElements.pop());
           }
-          handleResize(a, p) {
-            this._refreshRowElements(a, p), this._updateDimensions();
+          handleResize(o, p) {
+            this._refreshRowElements(o, p), this._updateDimensions();
           }
           handleCharSizeChanged() {
             this._updateDimensions();
           }
           handleBlur() {
             this._rowContainer.classList.remove(l);
           }
           handleFocus() {
             this._rowContainer.classList.add(l);
           }
-          handleSelectionChanged(a, p, C) {
+          handleSelectionChanged(o, p, C) {
             for (; this._selectionContainer.children.length; )
               this._selectionContainer.removeChild(this._selectionContainer.children[0]);
-            if (this._rowFactory.handleSelectionChanged(a, p, C), this.renderRows(0, this._bufferService.rows - 1), !a || !p)
+            if (this._rowFactory.handleSelectionChanged(o, p, C), this.renderRows(0, this._bufferService.rows - 1), !o || !p)
               return;
-            const y = a[1] - this._bufferService.buffer.ydisp, w = p[1] - this._bufferService.buffer.ydisp, D = Math.max(y, 0), x = Math.min(w, this._bufferService.rows - 1);
+            const y = o[1] - this._bufferService.buffer.ydisp, w = p[1] - this._bufferService.buffer.ydisp, D = Math.max(y, 0), x = Math.min(w, this._bufferService.rows - 1);
             if (D >= this._bufferService.rows || x < 0)
               return;
             const I = document.createDocumentFragment();
             if (C) {
-              const H = a[0] > p[0];
-              I.appendChild(this._createSelectionElement(D, H ? p[0] : a[0], H ? a[0] : p[0], x - D + 1));
+              const H = o[0] > p[0];
+              I.appendChild(this._createSelectionElement(D, H ? p[0] : o[0], H ? o[0] : p[0], x - D + 1));
             } else {
-              const H = y === D ? a[0] : 0, S = D === w ? p[0] : this._bufferService.cols;
+              const H = y === D ? o[0] : 0, S = D === w ? p[0] : this._bufferService.cols;
               I.appendChild(this._createSelectionElement(D, H, S));
               const b = x - D - 1;
               if (I.appendChild(this._createSelectionElement(D + 1, 0, this._bufferService.cols, b)), D !== x) {
                 const L = w === x ? p[0] : this._bufferService.cols;
                 I.appendChild(this._createSelectionElement(x, 0, L));
               }
             }
             this._selectionContainer.appendChild(I);
           }
-          _createSelectionElement(a, p, C, y = 1) {
+          _createSelectionElement(o, p, C, y = 1) {
             const w = document.createElement("div");
-            return w.style.height = y * this.dimensions.css.cell.height + "px", w.style.top = a * this.dimensions.css.cell.height + "px", w.style.left = p * this.dimensions.css.cell.width + "px", w.style.width = this.dimensions.css.cell.width * (C - p) + "px", w;
+            return w.style.height = y * this.dimensions.css.cell.height + "px", w.style.top = o * this.dimensions.css.cell.height + "px", w.style.left = p * this.dimensions.css.cell.width + "px", w.style.width = this.dimensions.css.cell.width * (C - p) + "px", w;
           }
           handleCursorMove() {
           }
           _handleOptionsChanged() {
             this._updateDimensions();
           }
           clear() {
-            for (const a of this._rowElements)
-              a.replaceChildren();
+            for (const o of this._rowElements)
+              o.replaceChildren();
           }
-          renderRows(a, p) {
+          renderRows(o, p) {
             const C = this._bufferService.buffer.ybase + this._bufferService.buffer.y, y = Math.min(this._bufferService.buffer.x, this._bufferService.cols - 1), w = this._optionsService.rawOptions.cursorBlink;
-            for (let D = a; D <= p; D++) {
+            for (let D = o; D <= p; D++) {
               const x = this._rowElements[D], I = D + this._bufferService.buffer.ydisp, H = this._bufferService.buffer.lines.get(I), S = this._optionsService.rawOptions.cursorStyle;
               this._cellToRowElements[D] && this._cellToRowElements[D].length === this._bufferService.cols || (this._cellToRowElements[D] = new Int16Array(this._bufferService.cols)), x.replaceChildren(this._rowFactory.createRow(H, I, I === C, S, y, w, this.dimensions.css.cell.width, this._bufferService.cols, this._cellToRowElements[D]));
             }
           }
           get _terminalSelector() {
             return `.${r}${this._terminalClass}`;
           }
-          _handleLinkHover(a) {
-            this._setCellUnderline(a.x1, a.x2, a.y1, a.y2, a.cols, !0);
+          _handleLinkHover(o) {
+            this._setCellUnderline(o.x1, o.x2, o.y1, o.y2, o.cols, !0);
           }
-          _handleLinkLeave(a) {
-            this._setCellUnderline(a.x1, a.x2, a.y1, a.y2, a.cols, !1);
+          _handleLinkLeave(o) {
+            this._setCellUnderline(o.x1, o.x2, o.y1, o.y2, o.cols, !1);
           }
-          _setCellUnderline(a, p, C, y, w, D) {
-            if (a = this._cellToRowElements[C][a], p = this._cellToRowElements[y][p], a !== -1 && p !== -1)
-              for (; a !== p || C !== y; ) {
+          _setCellUnderline(o, p, C, y, w, D) {
+            if (o = this._cellToRowElements[C][o], p = this._cellToRowElements[y][p], o !== -1 && p !== -1)
+              for (; o !== p || C !== y; ) {
                 const x = this._rowElements[C];
                 if (!x)
                   return;
-                const I = x.children[a];
-                I && (I.style.textDecoration = D ? "underline" : "none"), ++a >= w && (a = 0, C++);
+                const I = x.children[o];
+                I && (I.style.textDecoration = D ? "underline" : "none"), ++o >= w && (o = 0, C++);
               }
           }
         };
-        m = h([u(4, t.IInstantiationService), u(5, c.ICharSizeService), u(6, t.IOptionsService), u(7, t.IBufferService), u(8, c.ICoreBrowserService), u(9, c.IThemeService)], m), i.DomRenderer = m;
-      }, 3787: function(T, i, o) {
-        var h = this && this.__decorate || function(f, m, a, p) {
-          var C, y = arguments.length, w = y < 3 ? m : p === null ? p = Object.getOwnPropertyDescriptor(m, a) : p;
+        m = a([u(4, t.IInstantiationService), u(5, c.ICharSizeService), u(6, t.IOptionsService), u(7, t.IBufferService), u(8, c.ICoreBrowserService), u(9, c.IThemeService)], m), i.DomRenderer = m;
+      }, 3787: function(T, i, h) {
+        var a = this && this.__decorate || function(f, m, o, p) {
+          var C, y = arguments.length, w = y < 3 ? m : p === null ? p = Object.getOwnPropertyDescriptor(m, o) : p;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-            w = Reflect.decorate(f, m, a, p);
+            w = Reflect.decorate(f, m, o, p);
           else
             for (var D = f.length - 1; D >= 0; D--)
-              (C = f[D]) && (w = (y < 3 ? C(w) : y > 3 ? C(m, a, w) : C(m, a)) || w);
-          return y > 3 && w && Object.defineProperty(m, a, w), w;
+              (C = f[D]) && (w = (y < 3 ? C(w) : y > 3 ? C(m, o, w) : C(m, o)) || w);
+          return y > 3 && w && Object.defineProperty(m, o, w), w;
         }, u = this && this.__param || function(f, m) {
-          return function(a, p) {
-            m(a, p, f);
+          return function(o, p) {
+            m(o, p, f);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.DomRendererRowFactory = i.CURSOR_STYLE_UNDERLINE_CLASS = i.CURSOR_STYLE_BAR_CLASS = i.CURSOR_STYLE_BLOCK_CLASS = i.CURSOR_BLINK_CLASS = i.CURSOR_CLASS = i.STRIKETHROUGH_CLASS = i.UNDERLINE_CLASS = i.ITALIC_CLASS = i.DIM_CLASS = i.BOLD_CLASS = void 0;
-        const d = o(2223), _ = o(643), g = o(511), v = o(2585), c = o(8055), e = o(4725), s = o(4269), n = o(6171), t = o(3734);
+        const d = h(2223), _ = h(643), g = h(511), v = h(2585), c = h(8055), e = h(4725), s = h(4269), n = h(6171), t = h(3734);
         i.BOLD_CLASS = "xterm-bold", i.DIM_CLASS = "xterm-dim", i.ITALIC_CLASS = "xterm-italic", i.UNDERLINE_CLASS = "xterm-underline", i.STRIKETHROUGH_CLASS = "xterm-strikethrough", i.CURSOR_CLASS = "xterm-cursor", i.CURSOR_BLINK_CLASS = "xterm-cursor-blink", i.CURSOR_STYLE_BLOCK_CLASS = "xterm-cursor-block", i.CURSOR_STYLE_BAR_CLASS = "xterm-cursor-bar", i.CURSOR_STYLE_UNDERLINE_CLASS = "xterm-cursor-underline";
         let r = class {
-          constructor(f, m, a, p, C, y, w) {
-            this._document = f, this._characterJoinerService = m, this._optionsService = a, this._coreBrowserService = p, this._coreService = C, this._decorationService = y, this._themeService = w, this._workCell = new g.CellData(), this._columnSelectMode = !1;
+          constructor(f, m, o, p, C, y, w) {
+            this._document = f, this._characterJoinerService = m, this._optionsService = o, this._coreBrowserService = p, this._coreService = C, this._decorationService = y, this._themeService = w, this._workCell = new g.CellData(), this._columnSelectMode = !1;
           }
-          handleSelectionChanged(f, m, a) {
-            this._selectionStart = f, this._selectionEnd = m, this._columnSelectMode = a;
+          handleSelectionChanged(f, m, o) {
+            this._selectionStart = f, this._selectionEnd = m, this._columnSelectMode = o;
           }
-          createRow(f, m, a, p, C, y, w, D, x) {
+          createRow(f, m, o, p, C, y, w, D, x) {
             const I = this._document.createDocumentFragment(), H = this._characterJoinerService.getJoinedCharacters(m);
             let S = 0;
             for (let M = Math.min(f.length, D) - 1; M >= 0; M--)
-              if (f.loadCell(M, this._workCell).getCode() !== _.NULL_CELL_CODE || a && M === C) {
+              if (f.loadCell(M, this._workCell).getCode() !== _.NULL_CELL_CODE || o && M === C) {
                 S = M + 1;
                 break;
               }
             const b = this._themeService.colors;
             let L = -1, R = 0;
             for (; R < S; R++) {
               f.loadCell(R, this._workCell);
@@ -1448,15 +1448,15 @@
               let F = !1, $ = R, O = this._workCell;
               if (H.length > 0 && R === H[0][0]) {
                 F = !0;
                 const j = H.shift();
                 O = new s.JoinedCellData(this._workCell, f.translateToString(!0, j[0], j[1]), j[1] - j[0]), $ = j[1] - 1, M = O.getWidth();
               }
               const N = this._document.createElement("span");
-              if (M > 1 && (N.style.width = w * M + "px"), F && (N.style.display = "inline", C >= R && C <= $ && (C = R)), !this._coreService.isCursorHidden && a && R === C)
+              if (M > 1 && (N.style.width = w * M + "px"), F && (N.style.display = "inline", C >= R && C <= $ && (C = R)), !this._coreService.isCursorHidden && o && R === C)
                 switch (N.classList.add(i.CURSOR_CLASS), y && N.classList.add(i.CURSOR_BLINK_CLASS), p) {
                   case "bar":
                     N.classList.add(i.CURSOR_STYLE_BAR_CLASS);
                     break;
                   case "underline":
                     N.classList.add(i.CURSOR_STYLE_UNDERLINE_CLASS);
                     break;
@@ -1508,144 +1508,144 @@
                 default:
                   this._applyMinimumContrast(N, q, b.foreground, O, z, void 0) || P && N.classList.add(`xterm-fg-${d.INVERTED_DEFAULT_COLOR}`);
               }
               I.appendChild(N), x[R] = ++L, R = $;
             }
             return R < D - 1 && x.subarray(R).fill(++L), I;
           }
-          _applyMinimumContrast(f, m, a, p, C, y) {
+          _applyMinimumContrast(f, m, o, p, C, y) {
             if (this._optionsService.rawOptions.minimumContrastRatio === 1 || (0, n.excludeFromContrastRatioDemands)(p.getCode()))
               return !1;
             let w;
-            return C || y || (w = this._themeService.colors.contrastCache.getColor(m.rgba, a.rgba)), w === void 0 && (w = c.color.ensureContrastRatio(C || m, y || a, this._optionsService.rawOptions.minimumContrastRatio), this._themeService.colors.contrastCache.setColor((C || m).rgba, (y || a).rgba, w ?? null)), !!w && (this._addStyle(f, `color:${w.css}`), !0);
+            return C || y || (w = this._themeService.colors.contrastCache.getColor(m.rgba, o.rgba)), w === void 0 && (w = c.color.ensureContrastRatio(C || m, y || o, this._optionsService.rawOptions.minimumContrastRatio), this._themeService.colors.contrastCache.setColor((C || m).rgba, (y || o).rgba, w ?? null)), !!w && (this._addStyle(f, `color:${w.css}`), !0);
           }
           _addStyle(f, m) {
             f.setAttribute("style", `${f.getAttribute("style") || ""}${m};`);
           }
           _isCellInSelection(f, m) {
-            const a = this._selectionStart, p = this._selectionEnd;
-            return !(!a || !p) && (this._columnSelectMode ? a[0] <= p[0] ? f >= a[0] && m >= a[1] && f < p[0] && m <= p[1] : f < a[0] && m >= a[1] && f >= p[0] && m <= p[1] : m > a[1] && m < p[1] || a[1] === p[1] && m === a[1] && f >= a[0] && f < p[0] || a[1] < p[1] && m === p[1] && f < p[0] || a[1] < p[1] && m === a[1] && f >= a[0]);
+            const o = this._selectionStart, p = this._selectionEnd;
+            return !(!o || !p) && (this._columnSelectMode ? o[0] <= p[0] ? f >= o[0] && m >= o[1] && f < p[0] && m <= p[1] : f < o[0] && m >= o[1] && f >= p[0] && m <= p[1] : m > o[1] && m < p[1] || o[1] === p[1] && m === o[1] && f >= o[0] && f < p[0] || o[1] < p[1] && m === p[1] && f < p[0] || o[1] < p[1] && m === o[1] && f >= o[0]);
           }
         };
-        function l(f, m, a) {
-          for (; f.length < a; )
+        function l(f, m, o) {
+          for (; f.length < o; )
             f = m + f;
           return f;
         }
-        r = h([u(1, e.ICharacterJoinerService), u(2, v.IOptionsService), u(3, e.ICoreBrowserService), u(4, v.ICoreService), u(5, v.IDecorationService), u(6, e.IThemeService)], r), i.DomRendererRowFactory = r;
-      }, 2223: (T, i, o) => {
+        r = a([u(1, e.ICharacterJoinerService), u(2, v.IOptionsService), u(3, e.ICoreBrowserService), u(4, v.ICoreService), u(5, v.IDecorationService), u(6, e.IThemeService)], r), i.DomRendererRowFactory = r;
+      }, 2223: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.TEXT_BASELINE = i.DIM_OPACITY = i.INVERTED_DEFAULT_COLOR = void 0;
-        const h = o(6114);
-        i.INVERTED_DEFAULT_COLOR = 257, i.DIM_OPACITY = 0.5, i.TEXT_BASELINE = h.isFirefox || h.isLegacyEdge ? "bottom" : "ideographic";
+        const a = h(6114);
+        i.INVERTED_DEFAULT_COLOR = 257, i.DIM_OPACITY = 0.5, i.TEXT_BASELINE = a.isFirefox || a.isLegacyEdge ? "bottom" : "ideographic";
       }, 6171: (T, i) => {
-        function o(h) {
-          return 57508 <= h && h <= 57558;
+        function h(a) {
+          return 57508 <= a && a <= 57558;
         }
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.createRenderDimensions = i.excludeFromContrastRatioDemands = i.isRestrictedPowerlineGlyph = i.isPowerlineGlyph = i.throwIfFalsy = void 0, i.throwIfFalsy = function(h) {
-          if (!h)
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.createRenderDimensions = i.excludeFromContrastRatioDemands = i.isRestrictedPowerlineGlyph = i.isPowerlineGlyph = i.throwIfFalsy = void 0, i.throwIfFalsy = function(a) {
+          if (!a)
             throw new Error("value must not be falsy");
-          return h;
-        }, i.isPowerlineGlyph = o, i.isRestrictedPowerlineGlyph = function(h) {
-          return 57520 <= h && h <= 57527;
-        }, i.excludeFromContrastRatioDemands = function(h) {
-          return o(h) || function(u) {
+          return a;
+        }, i.isPowerlineGlyph = h, i.isRestrictedPowerlineGlyph = function(a) {
+          return 57520 <= a && a <= 57527;
+        }, i.excludeFromContrastRatioDemands = function(a) {
+          return h(a) || function(u) {
             return 9472 <= u && u <= 9631;
-          }(h);
+          }(a);
         }, i.createRenderDimensions = function() {
           return { css: { canvas: { width: 0, height: 0 }, cell: { width: 0, height: 0 } }, device: { canvas: { width: 0, height: 0 }, cell: { width: 0, height: 0 }, char: { width: 0, height: 0, left: 0, top: 0 } } };
         };
       }, 456: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.SelectionModel = void 0, i.SelectionModel = class {
-          constructor(o) {
-            this._bufferService = o, this.isSelectAllActive = !1, this.selectionStartLength = 0;
+          constructor(h) {
+            this._bufferService = h, this.isSelectAllActive = !1, this.selectionStartLength = 0;
           }
           clearSelection() {
             this.selectionStart = void 0, this.selectionEnd = void 0, this.isSelectAllActive = !1, this.selectionStartLength = 0;
           }
           get finalSelectionStart() {
             return this.isSelectAllActive ? [0, 0] : this.selectionEnd && this.selectionStart && this.areSelectionValuesReversed() ? this.selectionEnd : this.selectionStart;
           }
           get finalSelectionEnd() {
             if (this.isSelectAllActive)
               return [this._bufferService.cols, this._bufferService.buffer.ybase + this._bufferService.rows - 1];
             if (this.selectionStart) {
               if (!this.selectionEnd || this.areSelectionValuesReversed()) {
-                const o = this.selectionStart[0] + this.selectionStartLength;
-                return o > this._bufferService.cols ? o % this._bufferService.cols == 0 ? [this._bufferService.cols, this.selectionStart[1] + Math.floor(o / this._bufferService.cols) - 1] : [o % this._bufferService.cols, this.selectionStart[1] + Math.floor(o / this._bufferService.cols)] : [o, this.selectionStart[1]];
+                const h = this.selectionStart[0] + this.selectionStartLength;
+                return h > this._bufferService.cols ? h % this._bufferService.cols == 0 ? [this._bufferService.cols, this.selectionStart[1] + Math.floor(h / this._bufferService.cols) - 1] : [h % this._bufferService.cols, this.selectionStart[1] + Math.floor(h / this._bufferService.cols)] : [h, this.selectionStart[1]];
               }
               if (this.selectionStartLength && this.selectionEnd[1] === this.selectionStart[1]) {
-                const o = this.selectionStart[0] + this.selectionStartLength;
-                return o > this._bufferService.cols ? [o % this._bufferService.cols, this.selectionStart[1] + Math.floor(o / this._bufferService.cols)] : [Math.max(o, this.selectionEnd[0]), this.selectionEnd[1]];
+                const h = this.selectionStart[0] + this.selectionStartLength;
+                return h > this._bufferService.cols ? [h % this._bufferService.cols, this.selectionStart[1] + Math.floor(h / this._bufferService.cols)] : [Math.max(h, this.selectionEnd[0]), this.selectionEnd[1]];
               }
               return this.selectionEnd;
             }
           }
           areSelectionValuesReversed() {
-            const o = this.selectionStart, h = this.selectionEnd;
-            return !(!o || !h) && (o[1] > h[1] || o[1] === h[1] && o[0] > h[0]);
+            const h = this.selectionStart, a = this.selectionEnd;
+            return !(!h || !a) && (h[1] > a[1] || h[1] === a[1] && h[0] > a[0]);
           }
-          handleTrim(o) {
-            return this.selectionStart && (this.selectionStart[1] -= o), this.selectionEnd && (this.selectionEnd[1] -= o), this.selectionEnd && this.selectionEnd[1] < 0 ? (this.clearSelection(), !0) : (this.selectionStart && this.selectionStart[1] < 0 && (this.selectionStart[1] = 0), !1);
+          handleTrim(h) {
+            return this.selectionStart && (this.selectionStart[1] -= h), this.selectionEnd && (this.selectionEnd[1] -= h), this.selectionEnd && this.selectionEnd[1] < 0 ? (this.clearSelection(), !0) : (this.selectionStart && this.selectionStart[1] < 0 && (this.selectionStart[1] = 0), !1);
           }
         };
-      }, 428: function(T, i, o) {
-        var h = this && this.__decorate || function(e, s, n, t) {
+      }, 428: function(T, i, h) {
+        var a = this && this.__decorate || function(e, s, n, t) {
           var r, l = arguments.length, f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             f = Reflect.decorate(e, s, n, t);
           else
             for (var m = e.length - 1; m >= 0; m--)
               (r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
           return l > 3 && f && Object.defineProperty(s, n, f), f;
         }, u = this && this.__param || function(e, s) {
           return function(n, t) {
             s(n, t, e);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CharSizeService = void 0;
-        const d = o(2585), _ = o(8460), g = o(844);
+        const d = h(2585), _ = h(8460), g = h(844);
         let v = class extends g.Disposable {
           constructor(e, s, n) {
             super(), this._optionsService = n, this.width = 0, this.height = 0, this._onCharSizeChange = this.register(new _.EventEmitter()), this.onCharSizeChange = this._onCharSizeChange.event, this._measureStrategy = new c(e, s, this._optionsService), this.register(this._optionsService.onMultipleOptionChange(["fontFamily", "fontSize"], () => this.measure()));
           }
           get hasValidSize() {
             return this.width > 0 && this.height > 0;
           }
           measure() {
             const e = this._measureStrategy.measure();
             e.width === this.width && e.height === this.height || (this.width = e.width, this.height = e.height, this._onCharSizeChange.fire());
           }
         };
-        v = h([u(2, d.IOptionsService)], v), i.CharSizeService = v;
+        v = a([u(2, d.IOptionsService)], v), i.CharSizeService = v;
         class c {
           constructor(s, n, t) {
             this._document = s, this._parentElement = n, this._optionsService = t, this._result = { width: 0, height: 0 }, this._measureElement = this._document.createElement("span"), this._measureElement.classList.add("xterm-char-measure-element"), this._measureElement.textContent = "W", this._measureElement.setAttribute("aria-hidden", "true"), this._parentElement.appendChild(this._measureElement);
           }
           measure() {
             this._measureElement.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._measureElement.style.fontSize = `${this._optionsService.rawOptions.fontSize}px`;
             const s = this._measureElement.getBoundingClientRect();
             return s.width !== 0 && s.height !== 0 && (this._result.width = s.width, this._result.height = Math.ceil(s.height)), this._result;
           }
         }
-      }, 4269: function(T, i, o) {
-        var h = this && this.__decorate || function(s, n, t, r) {
+      }, 4269: function(T, i, h) {
+        var a = this && this.__decorate || function(s, n, t, r) {
           var l, f = arguments.length, m = f < 3 ? n : r === null ? r = Object.getOwnPropertyDescriptor(n, t) : r;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             m = Reflect.decorate(s, n, t, r);
           else
-            for (var a = s.length - 1; a >= 0; a--)
-              (l = s[a]) && (m = (f < 3 ? l(m) : f > 3 ? l(n, t, m) : l(n, t)) || m);
+            for (var o = s.length - 1; o >= 0; o--)
+              (l = s[o]) && (m = (f < 3 ? l(m) : f > 3 ? l(n, t, m) : l(n, t)) || m);
           return f > 3 && m && Object.defineProperty(n, t, m), m;
         }, u = this && this.__param || function(s, n) {
           return function(t, r) {
             n(t, r, s);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CharacterJoinerService = i.JoinedCellData = void 0;
-        const d = o(3734), _ = o(643), g = o(511), v = o(2585);
+        const d = h(3734), _ = h(643), g = h(511), v = h(2585);
         class c extends d.AttributeData {
           constructor(n, t, r) {
             super(), this.content = 0, this.combinedData = "", this.fg = n.fg, this.bg = n.bg, this.combinedData = t, this._width = r;
           }
           isCombined() {
             return 2097152;
           }
@@ -1683,67 +1683,67 @@
           getJoinedCharacters(n) {
             if (this._characterJoiners.length === 0)
               return [];
             const t = this._bufferService.buffer.lines.get(n);
             if (!t || t.length === 0)
               return [];
             const r = [], l = t.translateToString(!0);
-            let f = 0, m = 0, a = 0, p = t.getFg(0), C = t.getBg(0);
+            let f = 0, m = 0, o = 0, p = t.getFg(0), C = t.getBg(0);
             for (let y = 0; y < t.getTrimmedLength(); y++)
               if (t.loadCell(y, this._workCell), this._workCell.getWidth() !== 0) {
                 if (this._workCell.fg !== p || this._workCell.bg !== C) {
                   if (y - f > 1) {
-                    const w = this._getJoinedRanges(l, a, m, t, f);
+                    const w = this._getJoinedRanges(l, o, m, t, f);
                     for (let D = 0; D < w.length; D++)
                       r.push(w[D]);
                   }
-                  f = y, a = m, p = this._workCell.fg, C = this._workCell.bg;
+                  f = y, o = m, p = this._workCell.fg, C = this._workCell.bg;
                 }
                 m += this._workCell.getChars().length || _.WHITESPACE_CELL_CHAR.length;
               }
             if (this._bufferService.cols - f > 1) {
-              const y = this._getJoinedRanges(l, a, m, t, f);
+              const y = this._getJoinedRanges(l, o, m, t, f);
               for (let w = 0; w < y.length; w++)
                 r.push(y[w]);
             }
             return r;
           }
           _getJoinedRanges(n, t, r, l, f) {
             const m = n.substring(t, r);
-            let a = [];
+            let o = [];
             try {
-              a = this._characterJoiners[0].handler(m);
+              o = this._characterJoiners[0].handler(m);
             } catch (p) {
               console.error(p);
             }
             for (let p = 1; p < this._characterJoiners.length; p++)
               try {
                 const C = this._characterJoiners[p].handler(m);
                 for (let y = 0; y < C.length; y++)
-                  ie._mergeRanges(a, C[y]);
+                  ie._mergeRanges(o, C[y]);
               } catch (C) {
                 console.error(C);
               }
-            return this._stringRangesToCellRanges(a, l, f), a;
+            return this._stringRangesToCellRanges(o, l, f), o;
           }
           _stringRangesToCellRanges(n, t, r) {
-            let l = 0, f = !1, m = 0, a = n[l];
-            if (a) {
+            let l = 0, f = !1, m = 0, o = n[l];
+            if (o) {
               for (let p = r; p < this._bufferService.cols; p++) {
                 const C = t.getWidth(p), y = t.getString(p).length || _.WHITESPACE_CELL_CHAR.length;
                 if (C !== 0) {
-                  if (!f && a[0] <= m && (a[0] = p, f = !0), a[1] <= m) {
-                    if (a[1] = p, a = n[++l], !a)
+                  if (!f && o[0] <= m && (o[0] = p, f = !0), o[1] <= m) {
+                    if (o[1] = p, o = n[++l], !o)
                       break;
-                    a[0] <= m ? (a[0] = p, f = !0) : f = !1;
+                    o[0] <= m ? (o[0] = p, f = !0) : f = !1;
                   }
                   m += y;
                 }
               }
-              a && (a[1] = this._bufferService.cols);
+              o && (o[1] = this._bufferService.cols);
             }
           }
           static _mergeRanges(n, t) {
             let r = !1;
             for (let l = 0; l < n.length; l++) {
               const f = n[l];
               if (r) {
@@ -1759,82 +1759,82 @@
                   return f[0] = Math.min(t[0], f[0]), n;
                 t[0] < f[1] && (f[0] = Math.min(t[0], f[0]), r = !0);
               }
             }
             return r ? n[n.length - 1][1] = t[1] : n.push(t), n;
           }
         };
-        e = h([u(0, v.IBufferService)], e), i.CharacterJoinerService = e;
+        e = a([u(0, v.IBufferService)], e), i.CharacterJoinerService = e;
       }, 5114: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CoreBrowserService = void 0, i.CoreBrowserService = class {
-          constructor(o, h) {
-            this._textarea = o, this.window = h, this._isFocused = !1, this._cachedIsFocused = void 0, this._textarea.addEventListener("focus", () => this._isFocused = !0), this._textarea.addEventListener("blur", () => this._isFocused = !1);
+          constructor(h, a) {
+            this._textarea = h, this.window = a, this._isFocused = !1, this._cachedIsFocused = void 0, this._textarea.addEventListener("focus", () => this._isFocused = !0), this._textarea.addEventListener("blur", () => this._isFocused = !1);
           }
           get dpr() {
             return this.window.devicePixelRatio;
           }
           get isFocused() {
             return this._cachedIsFocused === void 0 && (this._cachedIsFocused = this._isFocused && this._textarea.ownerDocument.hasFocus(), queueMicrotask(() => this._cachedIsFocused = void 0)), this._cachedIsFocused;
           }
         };
-      }, 8934: function(T, i, o) {
-        var h = this && this.__decorate || function(v, c, e, s) {
+      }, 8934: function(T, i, h) {
+        var a = this && this.__decorate || function(v, c, e, s) {
           var n, t = arguments.length, r = t < 3 ? c : s === null ? s = Object.getOwnPropertyDescriptor(c, e) : s;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             r = Reflect.decorate(v, c, e, s);
           else
             for (var l = v.length - 1; l >= 0; l--)
               (n = v[l]) && (r = (t < 3 ? n(r) : t > 3 ? n(c, e, r) : n(c, e)) || r);
           return t > 3 && r && Object.defineProperty(c, e, r), r;
         }, u = this && this.__param || function(v, c) {
           return function(e, s) {
             c(e, s, v);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.MouseService = void 0;
-        const d = o(4725), _ = o(9806);
+        const d = h(4725), _ = h(9806);
         let g = class {
           constructor(v, c) {
             this._renderService = v, this._charSizeService = c;
           }
           getCoords(v, c, e, s, n) {
             return (0, _.getCoords)(window, v, c, e, s, this._charSizeService.hasValidSize, this._renderService.dimensions.css.cell.width, this._renderService.dimensions.css.cell.height, n);
           }
           getMouseReportCoords(v, c) {
             const e = (0, _.getCoordsRelativeToElement)(window, v, c);
             if (!(!this._charSizeService.hasValidSize || e[0] < 0 || e[1] < 0 || e[0] >= this._renderService.dimensions.css.canvas.width || e[1] >= this._renderService.dimensions.css.canvas.height))
               return { col: Math.floor(e[0] / this._renderService.dimensions.css.cell.width), row: Math.floor(e[1] / this._renderService.dimensions.css.cell.height), x: Math.floor(e[0]), y: Math.floor(e[1]) };
           }
         };
-        g = h([u(0, d.IRenderService), u(1, d.ICharSizeService)], g), i.MouseService = g;
-      }, 3230: function(T, i, o) {
-        var h = this && this.__decorate || function(r, l, f, m) {
-          var a, p = arguments.length, C = p < 3 ? l : m === null ? m = Object.getOwnPropertyDescriptor(l, f) : m;
+        g = a([u(0, d.IRenderService), u(1, d.ICharSizeService)], g), i.MouseService = g;
+      }, 3230: function(T, i, h) {
+        var a = this && this.__decorate || function(r, l, f, m) {
+          var o, p = arguments.length, C = p < 3 ? l : m === null ? m = Object.getOwnPropertyDescriptor(l, f) : m;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             C = Reflect.decorate(r, l, f, m);
           else
             for (var y = r.length - 1; y >= 0; y--)
-              (a = r[y]) && (C = (p < 3 ? a(C) : p > 3 ? a(l, f, C) : a(l, f)) || C);
+              (o = r[y]) && (C = (p < 3 ? o(C) : p > 3 ? o(l, f, C) : o(l, f)) || C);
           return p > 3 && C && Object.defineProperty(l, f, C), C;
         }, u = this && this.__param || function(r, l) {
           return function(f, m) {
             l(f, m, r);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.RenderService = void 0;
-        const d = o(6193), _ = o(8460), g = o(844), v = o(5596), c = o(3656), e = o(2585), s = o(4725), n = o(7226);
+        const d = h(6193), _ = h(8460), g = h(844), v = h(5596), c = h(3656), e = h(2585), s = h(4725), n = h(7226);
         let t = class extends g.Disposable {
-          constructor(r, l, f, m, a, p, C, y) {
+          constructor(r, l, f, m, o, p, C, y) {
             if (super(), this._rowCount = r, this._charSizeService = m, this._pausedResizeTask = new n.DebouncedIdleTask(), this._isPaused = !1, this._needsFullRefresh = !1, this._isNextRenderRedrawOnly = !0, this._needsSelectionRefresh = !1, this._canvasWidth = 0, this._canvasHeight = 0, this._selectionState = { start: void 0, end: void 0, columnSelectMode: !1 }, this._onDimensionsChange = this.register(new _.EventEmitter()), this.onDimensionsChange = this._onDimensionsChange.event, this._onRenderedViewportChange = this.register(new _.EventEmitter()), this.onRenderedViewportChange = this._onRenderedViewportChange.event, this._onRender = this.register(new _.EventEmitter()), this.onRender = this._onRender.event, this._onRefreshRequest = this.register(new _.EventEmitter()), this.onRefreshRequest = this._onRefreshRequest.event, this.register({ dispose: () => {
               var w;
               return (w = this._renderer) === null || w === void 0 ? void 0 : w.dispose();
             } }), this._renderDebouncer = new d.RenderDebouncer(C.window, (w, D) => this._renderRows(w, D)), this.register(this._renderDebouncer), this._screenDprMonitor = new v.ScreenDprMonitor(C.window), this._screenDprMonitor.setListener(() => this.handleDevicePixelRatioChange()), this.register(this._screenDprMonitor), this.register(p.onResize(() => this._fullRefresh())), this.register(p.buffers.onBufferActivate(() => {
               var w;
               return (w = this._renderer) === null || w === void 0 ? void 0 : w.clear();
-            })), this.register(f.onOptionChange(() => this._handleOptionsChanged())), this.register(this._charSizeService.onCharSizeChange(() => this.handleCharSizeChanged())), this.register(a.onDecorationRegistered(() => this._fullRefresh())), this.register(a.onDecorationRemoved(() => this._fullRefresh())), this.register(f.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio"], () => {
+            })), this.register(f.onOptionChange(() => this._handleOptionsChanged())), this.register(this._charSizeService.onCharSizeChange(() => this.handleCharSizeChanged())), this.register(o.onDecorationRegistered(() => this._fullRefresh())), this.register(o.onDecorationRemoved(() => this._fullRefresh())), this.register(f.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio"], () => {
               this.clear(), this.handleResize(p.cols, p.rows), this._fullRefresh();
             })), this.register(f.onMultipleOptionChange(["cursorBlink", "cursorStyle"], () => this.refreshRows(p.buffer.y, p.buffer.y, !0))), this.register((0, c.addDisposableDomListener)(C.window, "resize", () => this.handleDevicePixelRatioChange())), this.register(y.onChangeColors(() => this._fullRefresh())), "IntersectionObserver" in C.window) {
               const w = new C.window.IntersectionObserver((D) => this._handleIntersectionChange(D[D.length - 1]), { threshold: 0 });
               w.observe(l), this.register({ dispose: () => w.disconnect() });
             }
           }
           get dimensions() {
@@ -1902,34 +1902,34 @@
             (r = this._renderer) === null || r === void 0 || r.handleCursorMove();
           }
           clear() {
             var r;
             (r = this._renderer) === null || r === void 0 || r.clear();
           }
         };
-        t = h([u(2, e.IOptionsService), u(3, s.ICharSizeService), u(4, e.IDecorationService), u(5, e.IBufferService), u(6, s.ICoreBrowserService), u(7, s.IThemeService)], t), i.RenderService = t;
-      }, 9312: function(T, i, o) {
-        var h = this && this.__decorate || function(a, p, C, y) {
+        t = a([u(2, e.IOptionsService), u(3, s.ICharSizeService), u(4, e.IDecorationService), u(5, e.IBufferService), u(6, s.ICoreBrowserService), u(7, s.IThemeService)], t), i.RenderService = t;
+      }, 9312: function(T, i, h) {
+        var a = this && this.__decorate || function(o, p, C, y) {
           var w, D = arguments.length, x = D < 3 ? p : y === null ? y = Object.getOwnPropertyDescriptor(p, C) : y;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-            x = Reflect.decorate(a, p, C, y);
+            x = Reflect.decorate(o, p, C, y);
           else
-            for (var I = a.length - 1; I >= 0; I--)
-              (w = a[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
+            for (var I = o.length - 1; I >= 0; I--)
+              (w = o[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
           return D > 3 && x && Object.defineProperty(p, C, x), x;
-        }, u = this && this.__param || function(a, p) {
+        }, u = this && this.__param || function(o, p) {
           return function(C, y) {
-            p(C, y, a);
+            p(C, y, o);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.SelectionService = void 0;
-        const d = o(6114), _ = o(456), g = o(511), v = o(8460), c = o(4725), e = o(2585), s = o(9806), n = o(9504), t = o(844), r = o(4841), l = String.fromCharCode(160), f = new RegExp(l, "g");
+        const d = h(6114), _ = h(456), g = h(511), v = h(8460), c = h(4725), e = h(2585), s = h(9806), n = h(9504), t = h(844), r = h(4841), l = String.fromCharCode(160), f = new RegExp(l, "g");
         let m = class extends t.Disposable {
-          constructor(a, p, C, y, w, D, x, I, H) {
-            super(), this._element = a, this._screenElement = p, this._linkifier = C, this._bufferService = y, this._coreService = w, this._mouseService = D, this._optionsService = x, this._renderService = I, this._coreBrowserService = H, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new g.CellData(), this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new v.EventEmitter()), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new v.EventEmitter()), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new v.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new v.EventEmitter()), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = (S) => this._handleMouseMove(S), this._mouseUpListener = (S) => this._handleMouseUp(S), this._coreService.onUserInput(() => {
+          constructor(o, p, C, y, w, D, x, I, H) {
+            super(), this._element = o, this._screenElement = p, this._linkifier = C, this._bufferService = y, this._coreService = w, this._mouseService = D, this._optionsService = x, this._renderService = I, this._coreBrowserService = H, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new g.CellData(), this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new v.EventEmitter()), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new v.EventEmitter()), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new v.EventEmitter()), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new v.EventEmitter()), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = (S) => this._handleMouseMove(S), this._mouseUpListener = (S) => this._handleMouseUp(S), this._coreService.onUserInput(() => {
               this.hasSelection && this.clearSelection();
             }), this._trimListener = this._bufferService.buffer.lines.onTrim((S) => this._handleTrim(S)), this.register(this._bufferService.buffers.onBufferActivate((S) => this._handleBufferActivate(S))), this.enable(), this._model = new _.SelectionModel(this._bufferService), this._activeSelectionMode = 0, this.register((0, t.toDisposable)(() => {
               this._removeMouseDownListeners();
             }));
           }
           reset() {
             this.clearSelection();
@@ -1943,207 +1943,207 @@
           get selectionStart() {
             return this._model.finalSelectionStart;
           }
           get selectionEnd() {
             return this._model.finalSelectionEnd;
           }
           get hasSelection() {
-            const a = this._model.finalSelectionStart, p = this._model.finalSelectionEnd;
-            return !(!a || !p || a[0] === p[0] && a[1] === p[1]);
+            const o = this._model.finalSelectionStart, p = this._model.finalSelectionEnd;
+            return !(!o || !p || o[0] === p[0] && o[1] === p[1]);
           }
           get selectionText() {
-            const a = this._model.finalSelectionStart, p = this._model.finalSelectionEnd;
-            if (!a || !p)
+            const o = this._model.finalSelectionStart, p = this._model.finalSelectionEnd;
+            if (!o || !p)
               return "";
             const C = this._bufferService.buffer, y = [];
             if (this._activeSelectionMode === 3) {
-              if (a[0] === p[0])
+              if (o[0] === p[0])
                 return "";
-              const w = a[0] < p[0] ? a[0] : p[0], D = a[0] < p[0] ? p[0] : a[0];
-              for (let x = a[1]; x <= p[1]; x++) {
+              const w = o[0] < p[0] ? o[0] : p[0], D = o[0] < p[0] ? p[0] : o[0];
+              for (let x = o[1]; x <= p[1]; x++) {
                 const I = C.translateBufferLineToString(x, !0, w, D);
                 y.push(I);
               }
             } else {
-              const w = a[1] === p[1] ? p[0] : void 0;
-              y.push(C.translateBufferLineToString(a[1], !0, a[0], w));
-              for (let D = a[1] + 1; D <= p[1] - 1; D++) {
+              const w = o[1] === p[1] ? p[0] : void 0;
+              y.push(C.translateBufferLineToString(o[1], !0, o[0], w));
+              for (let D = o[1] + 1; D <= p[1] - 1; D++) {
                 const x = C.lines.get(D), I = C.translateBufferLineToString(D, !0);
                 x != null && x.isWrapped ? y[y.length - 1] += I : y.push(I);
               }
-              if (a[1] !== p[1]) {
+              if (o[1] !== p[1]) {
                 const D = C.lines.get(p[1]), x = C.translateBufferLineToString(p[1], !0, 0, p[0]);
                 D && D.isWrapped ? y[y.length - 1] += x : y.push(x);
               }
             }
             return y.map((w) => w.replace(f, " ")).join(d.isWindows ? `\r
 ` : `
 `);
           }
           clearSelection() {
             this._model.clearSelection(), this._removeMouseDownListeners(), this.refresh(), this._onSelectionChange.fire();
           }
-          refresh(a) {
-            this._refreshAnimationFrame || (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame(() => this._refresh())), d.isLinux && a && this.selectionText.length && this._onLinuxMouseSelection.fire(this.selectionText);
+          refresh(o) {
+            this._refreshAnimationFrame || (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame(() => this._refresh())), d.isLinux && o && this.selectionText.length && this._onLinuxMouseSelection.fire(this.selectionText);
           }
           _refresh() {
             this._refreshAnimationFrame = void 0, this._onRedrawRequest.fire({ start: this._model.finalSelectionStart, end: this._model.finalSelectionEnd, columnSelectMode: this._activeSelectionMode === 3 });
           }
-          _isClickInSelection(a) {
-            const p = this._getMouseBufferCoords(a), C = this._model.finalSelectionStart, y = this._model.finalSelectionEnd;
+          _isClickInSelection(o) {
+            const p = this._getMouseBufferCoords(o), C = this._model.finalSelectionStart, y = this._model.finalSelectionEnd;
             return !!(C && y && p) && this._areCoordsInSelection(p, C, y);
           }
-          isCellInSelection(a, p) {
+          isCellInSelection(o, p) {
             const C = this._model.finalSelectionStart, y = this._model.finalSelectionEnd;
-            return !(!C || !y) && this._areCoordsInSelection([a, p], C, y);
+            return !(!C || !y) && this._areCoordsInSelection([o, p], C, y);
           }
-          _areCoordsInSelection(a, p, C) {
-            return a[1] > p[1] && a[1] < C[1] || p[1] === C[1] && a[1] === p[1] && a[0] >= p[0] && a[0] < C[0] || p[1] < C[1] && a[1] === C[1] && a[0] < C[0] || p[1] < C[1] && a[1] === p[1] && a[0] >= p[0];
+          _areCoordsInSelection(o, p, C) {
+            return o[1] > p[1] && o[1] < C[1] || p[1] === C[1] && o[1] === p[1] && o[0] >= p[0] && o[0] < C[0] || p[1] < C[1] && o[1] === C[1] && o[0] < C[0] || p[1] < C[1] && o[1] === p[1] && o[0] >= p[0];
           }
-          _selectWordAtCursor(a, p) {
+          _selectWordAtCursor(o, p) {
             var C, y;
             const w = (y = (C = this._linkifier.currentLink) === null || C === void 0 ? void 0 : C.link) === null || y === void 0 ? void 0 : y.range;
             if (w)
               return this._model.selectionStart = [w.start.x - 1, w.start.y - 1], this._model.selectionStartLength = (0, r.getRangeLength)(w, this._bufferService.cols), this._model.selectionEnd = void 0, !0;
-            const D = this._getMouseBufferCoords(a);
+            const D = this._getMouseBufferCoords(o);
             return !!D && (this._selectWordAt(D, p), this._model.selectionEnd = void 0, !0);
           }
           selectAll() {
             this._model.isSelectAllActive = !0, this.refresh(), this._onSelectionChange.fire();
           }
-          selectLines(a, p) {
-            this._model.clearSelection(), a = Math.max(a, 0), p = Math.min(p, this._bufferService.buffer.lines.length - 1), this._model.selectionStart = [0, a], this._model.selectionEnd = [this._bufferService.cols, p], this.refresh(), this._onSelectionChange.fire();
+          selectLines(o, p) {
+            this._model.clearSelection(), o = Math.max(o, 0), p = Math.min(p, this._bufferService.buffer.lines.length - 1), this._model.selectionStart = [0, o], this._model.selectionEnd = [this._bufferService.cols, p], this.refresh(), this._onSelectionChange.fire();
           }
-          _handleTrim(a) {
-            this._model.handleTrim(a) && this.refresh();
+          _handleTrim(o) {
+            this._model.handleTrim(o) && this.refresh();
           }
-          _getMouseBufferCoords(a) {
-            const p = this._mouseService.getCoords(a, this._screenElement, this._bufferService.cols, this._bufferService.rows, !0);
+          _getMouseBufferCoords(o) {
+            const p = this._mouseService.getCoords(o, this._screenElement, this._bufferService.cols, this._bufferService.rows, !0);
             if (p)
               return p[0]--, p[1]--, p[1] += this._bufferService.buffer.ydisp, p;
           }
-          _getMouseEventScrollAmount(a) {
-            let p = (0, s.getCoordsRelativeToElement)(this._coreBrowserService.window, a, this._screenElement)[1];
+          _getMouseEventScrollAmount(o) {
+            let p = (0, s.getCoordsRelativeToElement)(this._coreBrowserService.window, o, this._screenElement)[1];
             const C = this._renderService.dimensions.css.canvas.height;
             return p >= 0 && p <= C ? 0 : (p > C && (p -= C), p = Math.min(Math.max(p, -50), 50), p /= 50, p / Math.abs(p) + Math.round(14 * p));
           }
-          shouldForceSelection(a) {
-            return d.isMac ? a.altKey && this._optionsService.rawOptions.macOptionClickForcesSelection : a.shiftKey;
+          shouldForceSelection(o) {
+            return d.isMac ? o.altKey && this._optionsService.rawOptions.macOptionClickForcesSelection : o.shiftKey;
           }
-          handleMouseDown(a) {
-            if (this._mouseDownTimeStamp = a.timeStamp, (a.button !== 2 || !this.hasSelection) && a.button === 0) {
+          handleMouseDown(o) {
+            if (this._mouseDownTimeStamp = o.timeStamp, (o.button !== 2 || !this.hasSelection) && o.button === 0) {
               if (!this._enabled) {
-                if (!this.shouldForceSelection(a))
+                if (!this.shouldForceSelection(o))
                   return;
-                a.stopPropagation();
+                o.stopPropagation();
               }
-              a.preventDefault(), this._dragScrollAmount = 0, this._enabled && a.shiftKey ? this._handleIncrementalClick(a) : a.detail === 1 ? this._handleSingleClick(a) : a.detail === 2 ? this._handleDoubleClick(a) : a.detail === 3 && this._handleTripleClick(a), this._addMouseDownListeners(), this.refresh(!0);
+              o.preventDefault(), this._dragScrollAmount = 0, this._enabled && o.shiftKey ? this._handleIncrementalClick(o) : o.detail === 1 ? this._handleSingleClick(o) : o.detail === 2 ? this._handleDoubleClick(o) : o.detail === 3 && this._handleTripleClick(o), this._addMouseDownListeners(), this.refresh(!0);
             }
           }
           _addMouseDownListeners() {
             this._screenElement.ownerDocument && (this._screenElement.ownerDocument.addEventListener("mousemove", this._mouseMoveListener), this._screenElement.ownerDocument.addEventListener("mouseup", this._mouseUpListener)), this._dragScrollIntervalTimer = this._coreBrowserService.window.setInterval(() => this._dragScroll(), 50);
           }
           _removeMouseDownListeners() {
             this._screenElement.ownerDocument && (this._screenElement.ownerDocument.removeEventListener("mousemove", this._mouseMoveListener), this._screenElement.ownerDocument.removeEventListener("mouseup", this._mouseUpListener)), this._coreBrowserService.window.clearInterval(this._dragScrollIntervalTimer), this._dragScrollIntervalTimer = void 0;
           }
-          _handleIncrementalClick(a) {
-            this._model.selectionStart && (this._model.selectionEnd = this._getMouseBufferCoords(a));
+          _handleIncrementalClick(o) {
+            this._model.selectionStart && (this._model.selectionEnd = this._getMouseBufferCoords(o));
           }
-          _handleSingleClick(a) {
-            if (this._model.selectionStartLength = 0, this._model.isSelectAllActive = !1, this._activeSelectionMode = this.shouldColumnSelect(a) ? 3 : 0, this._model.selectionStart = this._getMouseBufferCoords(a), !this._model.selectionStart)
+          _handleSingleClick(o) {
+            if (this._model.selectionStartLength = 0, this._model.isSelectAllActive = !1, this._activeSelectionMode = this.shouldColumnSelect(o) ? 3 : 0, this._model.selectionStart = this._getMouseBufferCoords(o), !this._model.selectionStart)
               return;
             this._model.selectionEnd = void 0;
             const p = this._bufferService.buffer.lines.get(this._model.selectionStart[1]);
             p && p.length !== this._model.selectionStart[0] && p.hasWidth(this._model.selectionStart[0]) === 0 && this._model.selectionStart[0]++;
           }
-          _handleDoubleClick(a) {
-            this._selectWordAtCursor(a, !0) && (this._activeSelectionMode = 1);
+          _handleDoubleClick(o) {
+            this._selectWordAtCursor(o, !0) && (this._activeSelectionMode = 1);
           }
-          _handleTripleClick(a) {
-            const p = this._getMouseBufferCoords(a);
+          _handleTripleClick(o) {
+            const p = this._getMouseBufferCoords(o);
             p && (this._activeSelectionMode = 2, this._selectLineAt(p[1]));
           }
-          shouldColumnSelect(a) {
-            return a.altKey && !(d.isMac && this._optionsService.rawOptions.macOptionClickForcesSelection);
+          shouldColumnSelect(o) {
+            return o.altKey && !(d.isMac && this._optionsService.rawOptions.macOptionClickForcesSelection);
           }
-          _handleMouseMove(a) {
-            if (a.stopImmediatePropagation(), !this._model.selectionStart)
+          _handleMouseMove(o) {
+            if (o.stopImmediatePropagation(), !this._model.selectionStart)
               return;
             const p = this._model.selectionEnd ? [this._model.selectionEnd[0], this._model.selectionEnd[1]] : null;
-            if (this._model.selectionEnd = this._getMouseBufferCoords(a), !this._model.selectionEnd)
+            if (this._model.selectionEnd = this._getMouseBufferCoords(o), !this._model.selectionEnd)
               return void this.refresh(!0);
-            this._activeSelectionMode === 2 ? this._model.selectionEnd[1] < this._model.selectionStart[1] ? this._model.selectionEnd[0] = 0 : this._model.selectionEnd[0] = this._bufferService.cols : this._activeSelectionMode === 1 && this._selectToWordAt(this._model.selectionEnd), this._dragScrollAmount = this._getMouseEventScrollAmount(a), this._activeSelectionMode !== 3 && (this._dragScrollAmount > 0 ? this._model.selectionEnd[0] = this._bufferService.cols : this._dragScrollAmount < 0 && (this._model.selectionEnd[0] = 0));
+            this._activeSelectionMode === 2 ? this._model.selectionEnd[1] < this._model.selectionStart[1] ? this._model.selectionEnd[0] = 0 : this._model.selectionEnd[0] = this._bufferService.cols : this._activeSelectionMode === 1 && this._selectToWordAt(this._model.selectionEnd), this._dragScrollAmount = this._getMouseEventScrollAmount(o), this._activeSelectionMode !== 3 && (this._dragScrollAmount > 0 ? this._model.selectionEnd[0] = this._bufferService.cols : this._dragScrollAmount < 0 && (this._model.selectionEnd[0] = 0));
             const C = this._bufferService.buffer;
             if (this._model.selectionEnd[1] < C.lines.length) {
               const y = C.lines.get(this._model.selectionEnd[1]);
               y && y.hasWidth(this._model.selectionEnd[0]) === 0 && this._model.selectionEnd[0]++;
             }
             p && p[0] === this._model.selectionEnd[0] && p[1] === this._model.selectionEnd[1] || this.refresh(!0);
           }
           _dragScroll() {
             if (this._model.selectionEnd && this._model.selectionStart && this._dragScrollAmount) {
               this._onRequestScrollLines.fire({ amount: this._dragScrollAmount, suppressScrollEvent: !1 });
-              const a = this._bufferService.buffer;
-              this._dragScrollAmount > 0 ? (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = this._bufferService.cols), this._model.selectionEnd[1] = Math.min(a.ydisp + this._bufferService.rows, a.lines.length - 1)) : (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = 0), this._model.selectionEnd[1] = a.ydisp), this.refresh();
+              const o = this._bufferService.buffer;
+              this._dragScrollAmount > 0 ? (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = this._bufferService.cols), this._model.selectionEnd[1] = Math.min(o.ydisp + this._bufferService.rows, o.lines.length - 1)) : (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = 0), this._model.selectionEnd[1] = o.ydisp), this.refresh();
             }
           }
-          _handleMouseUp(a) {
-            const p = a.timeStamp - this._mouseDownTimeStamp;
-            if (this._removeMouseDownListeners(), this.selectionText.length <= 1 && p < 500 && a.altKey && this._optionsService.rawOptions.altClickMovesCursor) {
+          _handleMouseUp(o) {
+            const p = o.timeStamp - this._mouseDownTimeStamp;
+            if (this._removeMouseDownListeners(), this.selectionText.length <= 1 && p < 500 && o.altKey && this._optionsService.rawOptions.altClickMovesCursor) {
               if (this._bufferService.buffer.ybase === this._bufferService.buffer.ydisp) {
-                const C = this._mouseService.getCoords(a, this._element, this._bufferService.cols, this._bufferService.rows, !1);
+                const C = this._mouseService.getCoords(o, this._element, this._bufferService.cols, this._bufferService.rows, !1);
                 if (C && C[0] !== void 0 && C[1] !== void 0) {
                   const y = (0, n.moveToCellSequence)(C[0] - 1, C[1] - 1, this._bufferService, this._coreService.decPrivateModes.applicationCursorKeys);
                   this._coreService.triggerDataEvent(y, !0);
                 }
               }
             } else
               this._fireEventIfSelectionChanged();
           }
           _fireEventIfSelectionChanged() {
-            const a = this._model.finalSelectionStart, p = this._model.finalSelectionEnd, C = !(!a || !p || a[0] === p[0] && a[1] === p[1]);
-            C ? a && p && (this._oldSelectionStart && this._oldSelectionEnd && a[0] === this._oldSelectionStart[0] && a[1] === this._oldSelectionStart[1] && p[0] === this._oldSelectionEnd[0] && p[1] === this._oldSelectionEnd[1] || this._fireOnSelectionChange(a, p, C)) : this._oldHasSelection && this._fireOnSelectionChange(a, p, C);
+            const o = this._model.finalSelectionStart, p = this._model.finalSelectionEnd, C = !(!o || !p || o[0] === p[0] && o[1] === p[1]);
+            C ? o && p && (this._oldSelectionStart && this._oldSelectionEnd && o[0] === this._oldSelectionStart[0] && o[1] === this._oldSelectionStart[1] && p[0] === this._oldSelectionEnd[0] && p[1] === this._oldSelectionEnd[1] || this._fireOnSelectionChange(o, p, C)) : this._oldHasSelection && this._fireOnSelectionChange(o, p, C);
           }
-          _fireOnSelectionChange(a, p, C) {
-            this._oldSelectionStart = a, this._oldSelectionEnd = p, this._oldHasSelection = C, this._onSelectionChange.fire();
+          _fireOnSelectionChange(o, p, C) {
+            this._oldSelectionStart = o, this._oldSelectionEnd = p, this._oldHasSelection = C, this._onSelectionChange.fire();
           }
-          _handleBufferActivate(a) {
-            this.clearSelection(), this._trimListener.dispose(), this._trimListener = a.activeBuffer.lines.onTrim((p) => this._handleTrim(p));
+          _handleBufferActivate(o) {
+            this.clearSelection(), this._trimListener.dispose(), this._trimListener = o.activeBuffer.lines.onTrim((p) => this._handleTrim(p));
           }
-          _convertViewportColToCharacterIndex(a, p) {
+          _convertViewportColToCharacterIndex(o, p) {
             let C = p;
             for (let y = 0; p >= y; y++) {
-              const w = a.loadCell(y, this._workCell).getChars().length;
+              const w = o.loadCell(y, this._workCell).getChars().length;
               this._workCell.getWidth() === 0 ? C-- : w > 1 && p !== y && (C += w - 1);
             }
             return C;
           }
-          setSelection(a, p, C) {
-            this._model.clearSelection(), this._removeMouseDownListeners(), this._model.selectionStart = [a, p], this._model.selectionStartLength = C, this.refresh(), this._fireEventIfSelectionChanged();
+          setSelection(o, p, C) {
+            this._model.clearSelection(), this._removeMouseDownListeners(), this._model.selectionStart = [o, p], this._model.selectionStartLength = C, this.refresh(), this._fireEventIfSelectionChanged();
           }
-          rightClickSelect(a) {
-            this._isClickInSelection(a) || (this._selectWordAtCursor(a, !1) && this.refresh(!0), this._fireEventIfSelectionChanged());
+          rightClickSelect(o) {
+            this._isClickInSelection(o) || (this._selectWordAtCursor(o, !1) && this.refresh(!0), this._fireEventIfSelectionChanged());
           }
-          _getWordAt(a, p, C = !0, y = !0) {
-            if (a[0] >= this._bufferService.cols)
+          _getWordAt(o, p, C = !0, y = !0) {
+            if (o[0] >= this._bufferService.cols)
               return;
-            const w = this._bufferService.buffer, D = w.lines.get(a[1]);
+            const w = this._bufferService.buffer, D = w.lines.get(o[1]);
             if (!D)
               return;
-            const x = w.translateBufferLineToString(a[1], !1);
-            let I = this._convertViewportColToCharacterIndex(D, a[0]), H = I;
-            const S = a[0] - I;
+            const x = w.translateBufferLineToString(o[1], !1);
+            let I = this._convertViewportColToCharacterIndex(D, o[0]), H = I;
+            const S = o[0] - I;
             let b = 0, L = 0, R = 0, M = 0;
             if (x.charAt(I) === " ") {
               for (; I > 0 && x.charAt(I - 1) === " "; )
                 I--;
               for (; H < x.length && x.charAt(H + 1) === " "; )
                 H++;
             } else {
-              let O = a[0], N = a[0];
+              let O = o[0], N = o[0];
               D.getWidth(O) === 0 && (b++, O--), D.getWidth(N) === 2 && (L++, N++);
               const k = D.getString(N).length;
               for (k > 1 && (M += k - 1, H += k - 1); O > 0 && I > 0 && !this._isCharWordSeparator(D.loadCell(O - 1, this._workCell)); ) {
                 D.loadCell(O - 1, this._workCell);
                 const E = this._workCell.getChars().length;
                 this._workCell.getWidth() === 0 ? (b++, O--) : E > 1 && (R += E - 1, I -= E - 1), I--, O--;
               }
@@ -2153,86 +2153,86 @@
                 this._workCell.getWidth() === 2 ? (L++, N++) : E > 1 && (M += E - 1, H += E - 1), H++, N++;
               }
             }
             H++;
             let F = I + S - b + R, $ = Math.min(this._bufferService.cols, H - I + b + L - R - M);
             if (p || x.slice(I, H).trim() !== "") {
               if (C && F === 0 && D.getCodePoint(0) !== 32) {
-                const O = w.lines.get(a[1] - 1);
+                const O = w.lines.get(o[1] - 1);
                 if (O && D.isWrapped && O.getCodePoint(this._bufferService.cols - 1) !== 32) {
-                  const N = this._getWordAt([this._bufferService.cols - 1, a[1] - 1], !1, !0, !1);
+                  const N = this._getWordAt([this._bufferService.cols - 1, o[1] - 1], !1, !0, !1);
                   if (N) {
                     const k = this._bufferService.cols - N.start;
                     F -= k, $ += k;
                   }
                 }
               }
               if (y && F + $ === this._bufferService.cols && D.getCodePoint(this._bufferService.cols - 1) !== 32) {
-                const O = w.lines.get(a[1] + 1);
+                const O = w.lines.get(o[1] + 1);
                 if (O != null && O.isWrapped && O.getCodePoint(0) !== 32) {
-                  const N = this._getWordAt([0, a[1] + 1], !1, !1, !0);
+                  const N = this._getWordAt([0, o[1] + 1], !1, !1, !0);
                   N && ($ += N.length);
                 }
               }
               return { start: F, length: $ };
             }
           }
-          _selectWordAt(a, p) {
-            const C = this._getWordAt(a, p);
+          _selectWordAt(o, p) {
+            const C = this._getWordAt(o, p);
             if (C) {
               for (; C.start < 0; )
-                C.start += this._bufferService.cols, a[1]--;
-              this._model.selectionStart = [C.start, a[1]], this._model.selectionStartLength = C.length;
+                C.start += this._bufferService.cols, o[1]--;
+              this._model.selectionStart = [C.start, o[1]], this._model.selectionStartLength = C.length;
             }
           }
-          _selectToWordAt(a) {
-            const p = this._getWordAt(a, !0);
+          _selectToWordAt(o) {
+            const p = this._getWordAt(o, !0);
             if (p) {
-              let C = a[1];
+              let C = o[1];
               for (; p.start < 0; )
                 p.start += this._bufferService.cols, C--;
               if (!this._model.areSelectionValuesReversed())
                 for (; p.start + p.length > this._bufferService.cols; )
                   p.length -= this._bufferService.cols, C++;
               this._model.selectionEnd = [this._model.areSelectionValuesReversed() ? p.start : p.start + p.length, C];
             }
           }
-          _isCharWordSeparator(a) {
-            return a.getWidth() !== 0 && this._optionsService.rawOptions.wordSeparator.indexOf(a.getChars()) >= 0;
+          _isCharWordSeparator(o) {
+            return o.getWidth() !== 0 && this._optionsService.rawOptions.wordSeparator.indexOf(o.getChars()) >= 0;
           }
-          _selectLineAt(a) {
-            const p = this._bufferService.buffer.getWrappedRangeForLine(a), C = { start: { x: 0, y: p.first }, end: { x: this._bufferService.cols - 1, y: p.last } };
+          _selectLineAt(o) {
+            const p = this._bufferService.buffer.getWrappedRangeForLine(o), C = { start: { x: 0, y: p.first }, end: { x: this._bufferService.cols - 1, y: p.last } };
             this._model.selectionStart = [0, p.first], this._model.selectionEnd = void 0, this._model.selectionStartLength = (0, r.getRangeLength)(C, this._bufferService.cols);
           }
         };
-        m = h([u(3, e.IBufferService), u(4, e.ICoreService), u(5, c.IMouseService), u(6, e.IOptionsService), u(7, c.IRenderService), u(8, c.ICoreBrowserService)], m), i.SelectionService = m;
-      }, 4725: (T, i, o) => {
+        m = a([u(3, e.IBufferService), u(4, e.ICoreService), u(5, c.IMouseService), u(6, e.IOptionsService), u(7, c.IRenderService), u(8, c.ICoreBrowserService)], m), i.SelectionService = m;
+      }, 4725: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.IThemeService = i.ICharacterJoinerService = i.ISelectionService = i.IRenderService = i.IMouseService = i.ICoreBrowserService = i.ICharSizeService = void 0;
-        const h = o(8343);
-        i.ICharSizeService = (0, h.createDecorator)("CharSizeService"), i.ICoreBrowserService = (0, h.createDecorator)("CoreBrowserService"), i.IMouseService = (0, h.createDecorator)("MouseService"), i.IRenderService = (0, h.createDecorator)("RenderService"), i.ISelectionService = (0, h.createDecorator)("SelectionService"), i.ICharacterJoinerService = (0, h.createDecorator)("CharacterJoinerService"), i.IThemeService = (0, h.createDecorator)("ThemeService");
-      }, 6731: function(T, i, o) {
-        var h = this && this.__decorate || function(m, a, p, C) {
-          var y, w = arguments.length, D = w < 3 ? a : C === null ? C = Object.getOwnPropertyDescriptor(a, p) : C;
+        const a = h(8343);
+        i.ICharSizeService = (0, a.createDecorator)("CharSizeService"), i.ICoreBrowserService = (0, a.createDecorator)("CoreBrowserService"), i.IMouseService = (0, a.createDecorator)("MouseService"), i.IRenderService = (0, a.createDecorator)("RenderService"), i.ISelectionService = (0, a.createDecorator)("SelectionService"), i.ICharacterJoinerService = (0, a.createDecorator)("CharacterJoinerService"), i.IThemeService = (0, a.createDecorator)("ThemeService");
+      }, 6731: function(T, i, h) {
+        var a = this && this.__decorate || function(m, o, p, C) {
+          var y, w = arguments.length, D = w < 3 ? o : C === null ? C = Object.getOwnPropertyDescriptor(o, p) : C;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-            D = Reflect.decorate(m, a, p, C);
+            D = Reflect.decorate(m, o, p, C);
           else
             for (var x = m.length - 1; x >= 0; x--)
-              (y = m[x]) && (D = (w < 3 ? y(D) : w > 3 ? y(a, p, D) : y(a, p)) || D);
-          return w > 3 && D && Object.defineProperty(a, p, D), D;
-        }, u = this && this.__param || function(m, a) {
+              (y = m[x]) && (D = (w < 3 ? y(D) : w > 3 ? y(o, p, D) : y(o, p)) || D);
+          return w > 3 && D && Object.defineProperty(o, p, D), D;
+        }, u = this && this.__param || function(m, o) {
           return function(p, C) {
-            a(p, C, m);
+            o(p, C, m);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.ThemeService = i.DEFAULT_ANSI_COLORS = void 0;
-        const d = o(7239), _ = o(8055), g = o(8460), v = o(844), c = o(2585), e = _.css.toColor("#ffffff"), s = _.css.toColor("#000000"), n = _.css.toColor("#ffffff"), t = _.css.toColor("#000000"), r = { css: "rgba(255, 255, 255, 0.3)", rgba: 4294967117 };
+        const d = h(7239), _ = h(8055), g = h(8460), v = h(844), c = h(2585), e = _.css.toColor("#ffffff"), s = _.css.toColor("#000000"), n = _.css.toColor("#ffffff"), t = _.css.toColor("#000000"), r = { css: "rgba(255, 255, 255, 0.3)", rgba: 4294967117 };
         i.DEFAULT_ANSI_COLORS = Object.freeze((() => {
-          const m = [_.css.toColor("#2e3436"), _.css.toColor("#cc0000"), _.css.toColor("#4e9a06"), _.css.toColor("#c4a000"), _.css.toColor("#3465a4"), _.css.toColor("#75507b"), _.css.toColor("#06989a"), _.css.toColor("#d3d7cf"), _.css.toColor("#555753"), _.css.toColor("#ef2929"), _.css.toColor("#8ae234"), _.css.toColor("#fce94f"), _.css.toColor("#729fcf"), _.css.toColor("#ad7fa8"), _.css.toColor("#34e2e2"), _.css.toColor("#eeeeec")], a = [0, 95, 135, 175, 215, 255];
+          const m = [_.css.toColor("#2e3436"), _.css.toColor("#cc0000"), _.css.toColor("#4e9a06"), _.css.toColor("#c4a000"), _.css.toColor("#3465a4"), _.css.toColor("#75507b"), _.css.toColor("#06989a"), _.css.toColor("#d3d7cf"), _.css.toColor("#555753"), _.css.toColor("#ef2929"), _.css.toColor("#8ae234"), _.css.toColor("#fce94f"), _.css.toColor("#729fcf"), _.css.toColor("#ad7fa8"), _.css.toColor("#34e2e2"), _.css.toColor("#eeeeec")], o = [0, 95, 135, 175, 215, 255];
           for (let p = 0; p < 216; p++) {
-            const C = a[p / 36 % 6 | 0], y = a[p / 6 % 6 | 0], w = a[p % 6];
+            const C = o[p / 36 % 6 | 0], y = o[p / 6 % 6 | 0], w = o[p % 6];
             m.push({ css: _.channels.toCss(C, y, w), rgba: _.channels.toRgba(C, y, w) });
           }
           for (let p = 0; p < 24; p++) {
             const C = 8 + 10 * p;
             m.push({ css: _.channels.toCss(C, C, C), rgba: _.channels.toRgba(C, C, C) });
           }
           return m;
@@ -2241,19 +2241,19 @@
           constructor(m) {
             super(), this._optionsService = m, this._onChangeColors = this.register(new g.EventEmitter()), this.onChangeColors = this._onChangeColors.event, this._contrastCache = new d.ColorContrastCache(), this._colors = { foreground: e, background: s, cursor: n, cursorAccent: t, selectionForeground: void 0, selectionBackgroundTransparent: r, selectionBackgroundOpaque: _.color.blend(s, r), selectionInactiveBackgroundTransparent: r, selectionInactiveBackgroundOpaque: _.color.blend(s, r), ansi: i.DEFAULT_ANSI_COLORS.slice(), contrastCache: this._contrastCache }, this._updateRestoreColors(), this._setTheme(this._optionsService.rawOptions.theme), this.register(this._optionsService.onSpecificOptionChange("minimumContrastRatio", () => this._contrastCache.clear())), this.register(this._optionsService.onSpecificOptionChange("theme", () => this._setTheme(this._optionsService.rawOptions.theme)));
           }
           get colors() {
             return this._colors;
           }
           _setTheme(m = {}) {
-            const a = this._colors;
-            if (a.foreground = f(m.foreground, e), a.background = f(m.background, s), a.cursor = f(m.cursor, n), a.cursorAccent = f(m.cursorAccent, t), a.selectionBackgroundTransparent = f(m.selectionBackground, r), a.selectionBackgroundOpaque = _.color.blend(a.background, a.selectionBackgroundTransparent), a.selectionInactiveBackgroundTransparent = f(m.selectionInactiveBackground, a.selectionBackgroundTransparent), a.selectionInactiveBackgroundOpaque = _.color.blend(a.background, a.selectionInactiveBackgroundTransparent), a.selectionForeground = m.selectionForeground ? f(m.selectionForeground, _.NULL_COLOR) : void 0, a.selectionForeground === _.NULL_COLOR && (a.selectionForeground = void 0), _.color.isOpaque(a.selectionBackgroundTransparent) && (a.selectionBackgroundTransparent = _.color.opacity(a.selectionBackgroundTransparent, 0.3)), _.color.isOpaque(a.selectionInactiveBackgroundTransparent) && (a.selectionInactiveBackgroundTransparent = _.color.opacity(a.selectionInactiveBackgroundTransparent, 0.3)), a.ansi = i.DEFAULT_ANSI_COLORS.slice(), a.ansi[0] = f(m.black, i.DEFAULT_ANSI_COLORS[0]), a.ansi[1] = f(m.red, i.DEFAULT_ANSI_COLORS[1]), a.ansi[2] = f(m.green, i.DEFAULT_ANSI_COLORS[2]), a.ansi[3] = f(m.yellow, i.DEFAULT_ANSI_COLORS[3]), a.ansi[4] = f(m.blue, i.DEFAULT_ANSI_COLORS[4]), a.ansi[5] = f(m.magenta, i.DEFAULT_ANSI_COLORS[5]), a.ansi[6] = f(m.cyan, i.DEFAULT_ANSI_COLORS[6]), a.ansi[7] = f(m.white, i.DEFAULT_ANSI_COLORS[7]), a.ansi[8] = f(m.brightBlack, i.DEFAULT_ANSI_COLORS[8]), a.ansi[9] = f(m.brightRed, i.DEFAULT_ANSI_COLORS[9]), a.ansi[10] = f(m.brightGreen, i.DEFAULT_ANSI_COLORS[10]), a.ansi[11] = f(m.brightYellow, i.DEFAULT_ANSI_COLORS[11]), a.ansi[12] = f(m.brightBlue, i.DEFAULT_ANSI_COLORS[12]), a.ansi[13] = f(m.brightMagenta, i.DEFAULT_ANSI_COLORS[13]), a.ansi[14] = f(m.brightCyan, i.DEFAULT_ANSI_COLORS[14]), a.ansi[15] = f(m.brightWhite, i.DEFAULT_ANSI_COLORS[15]), m.extendedAnsi) {
-              const p = Math.min(a.ansi.length - 16, m.extendedAnsi.length);
+            const o = this._colors;
+            if (o.foreground = f(m.foreground, e), o.background = f(m.background, s), o.cursor = f(m.cursor, n), o.cursorAccent = f(m.cursorAccent, t), o.selectionBackgroundTransparent = f(m.selectionBackground, r), o.selectionBackgroundOpaque = _.color.blend(o.background, o.selectionBackgroundTransparent), o.selectionInactiveBackgroundTransparent = f(m.selectionInactiveBackground, o.selectionBackgroundTransparent), o.selectionInactiveBackgroundOpaque = _.color.blend(o.background, o.selectionInactiveBackgroundTransparent), o.selectionForeground = m.selectionForeground ? f(m.selectionForeground, _.NULL_COLOR) : void 0, o.selectionForeground === _.NULL_COLOR && (o.selectionForeground = void 0), _.color.isOpaque(o.selectionBackgroundTransparent) && (o.selectionBackgroundTransparent = _.color.opacity(o.selectionBackgroundTransparent, 0.3)), _.color.isOpaque(o.selectionInactiveBackgroundTransparent) && (o.selectionInactiveBackgroundTransparent = _.color.opacity(o.selectionInactiveBackgroundTransparent, 0.3)), o.ansi = i.DEFAULT_ANSI_COLORS.slice(), o.ansi[0] = f(m.black, i.DEFAULT_ANSI_COLORS[0]), o.ansi[1] = f(m.red, i.DEFAULT_ANSI_COLORS[1]), o.ansi[2] = f(m.green, i.DEFAULT_ANSI_COLORS[2]), o.ansi[3] = f(m.yellow, i.DEFAULT_ANSI_COLORS[3]), o.ansi[4] = f(m.blue, i.DEFAULT_ANSI_COLORS[4]), o.ansi[5] = f(m.magenta, i.DEFAULT_ANSI_COLORS[5]), o.ansi[6] = f(m.cyan, i.DEFAULT_ANSI_COLORS[6]), o.ansi[7] = f(m.white, i.DEFAULT_ANSI_COLORS[7]), o.ansi[8] = f(m.brightBlack, i.DEFAULT_ANSI_COLORS[8]), o.ansi[9] = f(m.brightRed, i.DEFAULT_ANSI_COLORS[9]), o.ansi[10] = f(m.brightGreen, i.DEFAULT_ANSI_COLORS[10]), o.ansi[11] = f(m.brightYellow, i.DEFAULT_ANSI_COLORS[11]), o.ansi[12] = f(m.brightBlue, i.DEFAULT_ANSI_COLORS[12]), o.ansi[13] = f(m.brightMagenta, i.DEFAULT_ANSI_COLORS[13]), o.ansi[14] = f(m.brightCyan, i.DEFAULT_ANSI_COLORS[14]), o.ansi[15] = f(m.brightWhite, i.DEFAULT_ANSI_COLORS[15]), m.extendedAnsi) {
+              const p = Math.min(o.ansi.length - 16, m.extendedAnsi.length);
               for (let C = 0; C < p; C++)
-                a.ansi[C + 16] = f(m.extendedAnsi[C], i.DEFAULT_ANSI_COLORS[C + 16]);
+                o.ansi[C + 16] = f(m.extendedAnsi[C], i.DEFAULT_ANSI_COLORS[C + 16]);
             }
             this._contrastCache.clear(), this._updateRestoreColors(), this._onChangeColors.fire(this.colors);
           }
           restoreColor(m) {
             this._restoreColor(m), this._onChangeColors.fire(this.colors);
           }
           _restoreColor(m) {
@@ -2268,39 +2268,39 @@
                 case 258:
                   this._colors.cursor = this._restoreColors.cursor;
                   break;
                 default:
                   this._colors.ansi[m] = this._restoreColors.ansi[m];
               }
             else
-              for (let a = 0; a < this._restoreColors.ansi.length; ++a)
-                this._colors.ansi[a] = this._restoreColors.ansi[a];
+              for (let o = 0; o < this._restoreColors.ansi.length; ++o)
+                this._colors.ansi[o] = this._restoreColors.ansi[o];
           }
           modifyColors(m) {
             m(this._colors), this._onChangeColors.fire(this.colors);
           }
           _updateRestoreColors() {
             this._restoreColors = { foreground: this._colors.foreground, background: this._colors.background, cursor: this._colors.cursor, ansi: this._colors.ansi.slice() };
           }
         };
-        function f(m, a) {
+        function f(m, o) {
           if (m !== void 0)
             try {
               return _.css.toColor(m);
             } catch {
             }
-          return a;
+          return o;
         }
-        l = h([u(0, c.IOptionsService)], l), i.ThemeService = l;
-      }, 6349: (T, i, o) => {
+        l = a([u(0, c.IOptionsService)], l), i.ThemeService = l;
+      }, 6349: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CircularList = void 0;
-        const h = o(8460), u = o(844);
+        const a = h(8460), u = h(844);
         class d extends u.Disposable {
           constructor(g) {
-            super(), this._maxLength = g, this.onDeleteEmitter = this.register(new h.EventEmitter()), this.onDelete = this.onDeleteEmitter.event, this.onInsertEmitter = this.register(new h.EventEmitter()), this.onInsert = this.onInsertEmitter.event, this.onTrimEmitter = this.register(new h.EventEmitter()), this.onTrim = this.onTrimEmitter.event, this._array = new Array(this._maxLength), this._startIndex = 0, this._length = 0;
+            super(), this._maxLength = g, this.onDeleteEmitter = this.register(new a.EventEmitter()), this.onDelete = this.onDeleteEmitter.event, this.onInsertEmitter = this.register(new a.EventEmitter()), this.onInsert = this.onInsertEmitter.event, this.onTrimEmitter = this.register(new a.EventEmitter()), this.onTrim = this.onTrimEmitter.event, this._array = new Array(this._maxLength), this._startIndex = 0, this._length = 0;
           }
           get maxLength() {
             return this._maxLength;
           }
           set maxLength(g) {
             if (this._maxLength === g)
               return;
@@ -2377,25 +2377,25 @@
           }
           _getCyclicIndex(g) {
             return (this._startIndex + g) % this._maxLength;
           }
         }
         i.CircularList = d;
       }, 1439: (T, i) => {
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.clone = void 0, i.clone = function o(h, u = 5) {
-          if (typeof h != "object")
-            return h;
-          const d = Array.isArray(h) ? [] : {};
-          for (const _ in h)
-            d[_] = u <= 1 ? h[_] : h[_] && o(h[_], u - 1);
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.clone = void 0, i.clone = function h(a, u = 5) {
+          if (typeof a != "object")
+            return a;
+          const d = Array.isArray(a) ? [] : {};
+          for (const _ in a)
+            d[_] = u <= 1 ? a[_] : a[_] && h(a[_], u - 1);
           return d;
         };
-      }, 8055: (T, i, o) => {
+      }, 8055: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.contrastRatio = i.toPaddedHex = i.rgba = i.rgb = i.css = i.color = i.channels = i.NULL_COLOR = void 0;
-        const h = o(6114);
+        const a = h(6114);
         let u = 0, d = 0, _ = 0, g = 0;
         var v, c, e;
         function s(t) {
           const r = t.toString(16);
           return r.length < 2 ? "0" + r : r;
         }
         function n(t, r) {
@@ -2410,33 +2410,33 @@
         }(v = i.channels || (i.channels = {})), function(t) {
           function r(l, f) {
             return g = Math.round(255 * f), [u, d, _] = e.toChannels(l.rgba), { css: v.toCss(u, d, _, g), rgba: v.toRgba(u, d, _, g) };
           }
           t.blend = function(l, f) {
             if (g = (255 & f.rgba) / 255, g === 1)
               return { css: f.css, rgba: f.rgba };
-            const m = f.rgba >> 24 & 255, a = f.rgba >> 16 & 255, p = f.rgba >> 8 & 255, C = l.rgba >> 24 & 255, y = l.rgba >> 16 & 255, w = l.rgba >> 8 & 255;
-            return u = C + Math.round((m - C) * g), d = y + Math.round((a - y) * g), _ = w + Math.round((p - w) * g), { css: v.toCss(u, d, _), rgba: v.toRgba(u, d, _) };
+            const m = f.rgba >> 24 & 255, o = f.rgba >> 16 & 255, p = f.rgba >> 8 & 255, C = l.rgba >> 24 & 255, y = l.rgba >> 16 & 255, w = l.rgba >> 8 & 255;
+            return u = C + Math.round((m - C) * g), d = y + Math.round((o - y) * g), _ = w + Math.round((p - w) * g), { css: v.toCss(u, d, _), rgba: v.toRgba(u, d, _) };
           }, t.isOpaque = function(l) {
             return (255 & l.rgba) == 255;
           }, t.ensureContrastRatio = function(l, f, m) {
-            const a = e.ensureContrastRatio(l.rgba, f.rgba, m);
-            if (a)
-              return e.toColor(a >> 24 & 255, a >> 16 & 255, a >> 8 & 255);
+            const o = e.ensureContrastRatio(l.rgba, f.rgba, m);
+            if (o)
+              return e.toColor(o >> 24 & 255, o >> 16 & 255, o >> 8 & 255);
           }, t.opaque = function(l) {
             const f = (255 | l.rgba) >>> 0;
             return [u, d, _] = e.toChannels(f), { css: v.toCss(u, d, _), rgba: f };
           }, t.opacity = r, t.multiplyOpacity = function(l, f) {
             return g = 255 & l.rgba, r(l, g * f / 255);
           }, t.toColorRGB = function(l) {
             return [l.rgba >> 24 & 255, l.rgba >> 16 & 255, l.rgba >> 8 & 255];
           };
         }(i.color || (i.color = {})), function(t) {
           let r, l;
-          if (!h.isNode) {
+          if (!a.isNode) {
             const f = document.createElement("canvas");
             f.width = 1, f.height = 1;
             const m = f.getContext("2d", { willReadFrequently: !0 });
             m && (r = m, r.globalCompositeOperation = "copy", l = r.createLinearGradient(0, 0, 1, 1));
           }
           t.toColor = function(f) {
             if (f.match(/#[\da-f]{3,8}/i))
@@ -2459,70 +2459,70 @@
               throw new Error("css.toColor: Unsupported css format");
             if (r.fillRect(0, 0, 1, 1), [u, d, _, g] = r.getImageData(0, 0, 1, 1).data, g !== 255)
               throw new Error("css.toColor: Unsupported css format");
             return { rgba: v.toRgba(u, d, _, g), css: f };
           };
         }(i.css || (i.css = {})), function(t) {
           function r(l, f, m) {
-            const a = l / 255, p = f / 255, C = m / 255;
-            return 0.2126 * (a <= 0.03928 ? a / 12.92 : Math.pow((a + 0.055) / 1.055, 2.4)) + 0.7152 * (p <= 0.03928 ? p / 12.92 : Math.pow((p + 0.055) / 1.055, 2.4)) + 0.0722 * (C <= 0.03928 ? C / 12.92 : Math.pow((C + 0.055) / 1.055, 2.4));
+            const o = l / 255, p = f / 255, C = m / 255;
+            return 0.2126 * (o <= 0.03928 ? o / 12.92 : Math.pow((o + 0.055) / 1.055, 2.4)) + 0.7152 * (p <= 0.03928 ? p / 12.92 : Math.pow((p + 0.055) / 1.055, 2.4)) + 0.0722 * (C <= 0.03928 ? C / 12.92 : Math.pow((C + 0.055) / 1.055, 2.4));
           }
           t.relativeLuminance = function(l) {
             return r(l >> 16 & 255, l >> 8 & 255, 255 & l);
           }, t.relativeLuminance2 = r;
         }(c = i.rgb || (i.rgb = {})), function(t) {
-          function r(f, m, a) {
+          function r(f, m, o) {
             const p = f >> 24 & 255, C = f >> 16 & 255, y = f >> 8 & 255;
             let w = m >> 24 & 255, D = m >> 16 & 255, x = m >> 8 & 255, I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
-            for (; I < a && (w > 0 || D > 0 || x > 0); )
+            for (; I < o && (w > 0 || D > 0 || x > 0); )
               w -= Math.max(0, Math.ceil(0.1 * w)), D -= Math.max(0, Math.ceil(0.1 * D)), x -= Math.max(0, Math.ceil(0.1 * x)), I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
             return (w << 24 | D << 16 | x << 8 | 255) >>> 0;
           }
-          function l(f, m, a) {
+          function l(f, m, o) {
             const p = f >> 24 & 255, C = f >> 16 & 255, y = f >> 8 & 255;
             let w = m >> 24 & 255, D = m >> 16 & 255, x = m >> 8 & 255, I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
-            for (; I < a && (w < 255 || D < 255 || x < 255); )
+            for (; I < o && (w < 255 || D < 255 || x < 255); )
               w = Math.min(255, w + Math.ceil(0.1 * (255 - w))), D = Math.min(255, D + Math.ceil(0.1 * (255 - D))), x = Math.min(255, x + Math.ceil(0.1 * (255 - x))), I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
             return (w << 24 | D << 16 | x << 8 | 255) >>> 0;
           }
-          t.ensureContrastRatio = function(f, m, a) {
+          t.ensureContrastRatio = function(f, m, o) {
             const p = c.relativeLuminance(f >> 8), C = c.relativeLuminance(m >> 8);
-            if (n(p, C) < a) {
+            if (n(p, C) < o) {
               if (C < p) {
-                const D = r(f, m, a), x = n(p, c.relativeLuminance(D >> 8));
-                if (x < a) {
-                  const I = l(f, m, a);
+                const D = r(f, m, o), x = n(p, c.relativeLuminance(D >> 8));
+                if (x < o) {
+                  const I = l(f, m, o);
                   return x > n(p, c.relativeLuminance(I >> 8)) ? D : I;
                 }
                 return D;
               }
-              const y = l(f, m, a), w = n(p, c.relativeLuminance(y >> 8));
-              if (w < a) {
-                const D = r(f, m, a);
+              const y = l(f, m, o), w = n(p, c.relativeLuminance(y >> 8));
+              if (w < o) {
+                const D = r(f, m, o);
                 return w > n(p, c.relativeLuminance(D >> 8)) ? y : D;
               }
               return y;
             }
           }, t.reduceLuminance = r, t.increaseLuminance = l, t.toChannels = function(f) {
             return [f >> 24 & 255, f >> 16 & 255, f >> 8 & 255, 255 & f];
-          }, t.toColor = function(f, m, a, p) {
-            return { css: v.toCss(f, m, a, p), rgba: v.toRgba(f, m, a, p) };
+          }, t.toColor = function(f, m, o, p) {
+            return { css: v.toCss(f, m, o, p), rgba: v.toRgba(f, m, o, p) };
           };
         }(e = i.rgba || (i.rgba = {})), i.toPaddedHex = s, i.contrastRatio = n;
-      }, 8969: (T, i, o) => {
+      }, 8969: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CoreTerminal = void 0;
-        const h = o(844), u = o(2585), d = o(4348), _ = o(7866), g = o(744), v = o(7302), c = o(6975), e = o(8460), s = o(1753), n = o(1480), t = o(7994), r = o(9282), l = o(5435), f = o(5981), m = o(2660);
-        let a = !1;
-        class p extends h.Disposable {
+        const a = h(844), u = h(2585), d = h(4348), _ = h(7866), g = h(744), v = h(7302), c = h(6975), e = h(8460), s = h(1753), n = h(1480), t = h(7994), r = h(9282), l = h(5435), f = h(5981), m = h(2660);
+        let o = !1;
+        class p extends a.Disposable {
           constructor(y) {
             super(), this._onBinary = this.register(new e.EventEmitter()), this.onBinary = this._onBinary.event, this._onData = this.register(new e.EventEmitter()), this.onData = this._onData.event, this._onLineFeed = this.register(new e.EventEmitter()), this.onLineFeed = this._onLineFeed.event, this._onResize = this.register(new e.EventEmitter()), this.onResize = this._onResize.event, this._onWriteParsed = this.register(new e.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event, this._onScroll = this.register(new e.EventEmitter()), this._instantiationService = new d.InstantiationService(), this.optionsService = this.register(new v.OptionsService(y)), this._instantiationService.setService(u.IOptionsService, this.optionsService), this._bufferService = this.register(this._instantiationService.createInstance(g.BufferService)), this._instantiationService.setService(u.IBufferService, this._bufferService), this._logService = this.register(this._instantiationService.createInstance(_.LogService)), this._instantiationService.setService(u.ILogService, this._logService), this.coreService = this.register(this._instantiationService.createInstance(c.CoreService)), this._instantiationService.setService(u.ICoreService, this.coreService), this.coreMouseService = this.register(this._instantiationService.createInstance(s.CoreMouseService)), this._instantiationService.setService(u.ICoreMouseService, this.coreMouseService), this.unicodeService = this.register(this._instantiationService.createInstance(n.UnicodeService)), this._instantiationService.setService(u.IUnicodeService, this.unicodeService), this._charsetService = this._instantiationService.createInstance(t.CharsetService), this._instantiationService.setService(u.ICharsetService, this._charsetService), this._oscLinkService = this._instantiationService.createInstance(m.OscLinkService), this._instantiationService.setService(u.IOscLinkService, this._oscLinkService), this._inputHandler = this.register(new l.InputHandler(this._bufferService, this._charsetService, this.coreService, this._logService, this.optionsService, this._oscLinkService, this.coreMouseService, this.unicodeService)), this.register((0, e.forwardEvent)(this._inputHandler.onLineFeed, this._onLineFeed)), this.register(this._inputHandler), this.register((0, e.forwardEvent)(this._bufferService.onResize, this._onResize)), this.register((0, e.forwardEvent)(this.coreService.onData, this._onData)), this.register((0, e.forwardEvent)(this.coreService.onBinary, this._onBinary)), this.register(this.coreService.onRequestScrollToBottom(() => this.scrollToBottom())), this.register(this.coreService.onUserInput(() => this._writeBuffer.handleUserInput())), this.register(this.optionsService.onSpecificOptionChange("windowsMode", (w) => this._handleWindowsModeOptionChange(w))), this.register(this._bufferService.onScroll((w) => {
               this._onScroll.fire({ position: this._bufferService.buffer.ydisp, source: 0 }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom);
             })), this.register(this._inputHandler.onScroll((w) => {
               this._onScroll.fire({ position: this._bufferService.buffer.ydisp, source: 0 }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom);
-            })), this._writeBuffer = this.register(new f.WriteBuffer((w, D) => this._inputHandler.parse(w, D))), this.register((0, e.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed)), this.register((0, h.toDisposable)(() => {
+            })), this._writeBuffer = this.register(new f.WriteBuffer((w, D) => this._inputHandler.parse(w, D))), this.register((0, e.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed)), this.register((0, a.toDisposable)(() => {
               var w;
               (w = this._windowsMode) === null || w === void 0 || w.dispose(), this._windowsMode = void 0;
             }));
           }
           get onScroll() {
             return this._onScrollApi || (this._onScrollApi = this.register(new e.EventEmitter()), this._onScroll.event((y) => {
               var w;
@@ -2545,15 +2545,15 @@
             for (const w in y)
               this.optionsService.options[w] = y[w];
           }
           write(y, w) {
             this._writeBuffer.write(y, w);
           }
           writeSync(y, w) {
-            this._logService.logLevel <= u.LogLevelEnum.WARN && !a && (this._logService.warn("writeSync is unreliable and will be removed soon."), a = !0), this._writeBuffer.writeSync(y, w);
+            this._logService.logLevel <= u.LogLevelEnum.WARN && !o && (this._logService.warn("writeSync is unreliable and will be removed soon."), o = !0), this._writeBuffer.writeSync(y, w);
           }
           resize(y, w) {
             isNaN(y) || isNaN(w) || (y = Math.max(y, g.MINIMUM_COLS), w = Math.max(w, g.MINIMUM_ROWS), this._bufferService.resize(y, w));
           }
           scroll(y, w = !1) {
             this._bufferService.scroll(y, w);
           }
@@ -2607,51 +2607,51 @@
         i.CoreTerminal = p;
       }, 8460: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.forwardEvent = i.EventEmitter = void 0, i.EventEmitter = class {
           constructor() {
             this._listeners = [], this._disposed = !1;
           }
           get event() {
-            return this._event || (this._event = (o) => (this._listeners.push(o), { dispose: () => {
+            return this._event || (this._event = (h) => (this._listeners.push(h), { dispose: () => {
               if (!this._disposed) {
-                for (let h = 0; h < this._listeners.length; h++)
-                  if (this._listeners[h] === o)
-                    return void this._listeners.splice(h, 1);
+                for (let a = 0; a < this._listeners.length; a++)
+                  if (this._listeners[a] === h)
+                    return void this._listeners.splice(a, 1);
               }
             } })), this._event;
           }
-          fire(o, h) {
+          fire(h, a) {
             const u = [];
             for (let d = 0; d < this._listeners.length; d++)
               u.push(this._listeners[d]);
             for (let d = 0; d < u.length; d++)
-              u[d].call(void 0, o, h);
+              u[d].call(void 0, h, a);
           }
           dispose() {
             this._listeners && (this._listeners.length = 0), this._disposed = !0;
           }
-        }, i.forwardEvent = function(o, h) {
-          return o((u) => h.fire(u));
+        }, i.forwardEvent = function(h, a) {
+          return h((u) => a.fire(u));
         };
-      }, 5435: function(T, i, o) {
-        var h = this && this.__decorate || function(H, S, b, L) {
+      }, 5435: function(T, i, h) {
+        var a = this && this.__decorate || function(H, S, b, L) {
           var R, M = arguments.length, F = M < 3 ? S : L === null ? L = Object.getOwnPropertyDescriptor(S, b) : L;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             F = Reflect.decorate(H, S, b, L);
           else
             for (var $ = H.length - 1; $ >= 0; $--)
               (R = H[$]) && (F = (M < 3 ? R(F) : M > 3 ? R(S, b, F) : R(S, b)) || F);
           return M > 3 && F && Object.defineProperty(S, b, F), F;
         }, u = this && this.__param || function(H, S) {
           return function(b, L) {
             S(b, L, H);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.InputHandler = i.WindowsOptionsReportType = void 0;
-        const d = o(2584), _ = o(7116), g = o(2015), v = o(844), c = o(482), e = o(8437), s = o(8460), n = o(643), t = o(511), r = o(3734), l = o(2585), f = o(6242), m = o(6351), a = o(5941), p = { "(": 0, ")": 1, "*": 2, "+": 3, "-": 1, ".": 2 }, C = 131072;
+        const d = h(2584), _ = h(7116), g = h(2015), v = h(844), c = h(482), e = h(8437), s = h(8460), n = h(643), t = h(511), r = h(3734), l = h(2585), f = h(6242), m = h(6351), o = h(5941), p = { "(": 0, ")": 1, "*": 2, "+": 3, "-": 1, ".": 2 }, C = 131072;
         function y(H, S) {
           if (H > 24)
             return S.setWinLines || !1;
           switch (H) {
             case 1:
               return !!S.restoreWin;
             case 2:
@@ -3345,15 +3345,15 @@
               const R = L.shift(), M = L.shift();
               if (/^\d+$/.exec(R)) {
                 const F = parseInt(R);
                 if (0 <= F && F < 256)
                   if (M === "?")
                     b.push({ type: 0, index: F });
                   else {
-                    const $ = (0, a.parseColor)(M);
+                    const $ = (0, o.parseColor)(M);
                     $ && b.push({ type: 1, index: F, color: $ });
                   }
               }
             }
             return b.length && this._onColor.fire(b), !0;
           }
           setHyperlink(S) {
@@ -3372,15 +3372,15 @@
           }
           _setOrReportSpecialColor(S, b) {
             const L = S.split(";");
             for (let R = 0; R < L.length && !(b >= this._specialColors.length); ++R, ++b)
               if (L[R] === "?")
                 this._onColor.fire([{ type: 0, index: this._specialColors[b] }]);
               else {
-                const M = (0, a.parseColor)(L[R]);
+                const M = (0, o.parseColor)(L[R]);
                 M && this._onColor.fire([{ type: 1, index: this._specialColors[b], color: M }]);
               }
             return !0;
           }
           setOrReportFgColor(S) {
             return this._setOrReportSpecialColor(S, 0);
           }
@@ -3482,140 +3482,140 @@
           markRangeDirty(H, S) {
             H > S && (D = H, H = S, S = D), H < this.start && (this.start = H), S > this.end && (this.end = S);
           }
           markAllDirty() {
             this.markRangeDirty(0, this._bufferService.rows - 1);
           }
         };
-        I = h([u(0, l.IBufferService)], I);
+        I = a([u(0, l.IBufferService)], I);
       }, 844: (T, i) => {
-        function o(h) {
-          for (const u of h)
+        function h(a) {
+          for (const u of a)
             u.dispose();
-          h.length = 0;
+          a.length = 0;
         }
         Object.defineProperty(i, "__esModule", { value: !0 }), i.getDisposeArrayDisposable = i.disposeArray = i.toDisposable = i.Disposable = void 0, i.Disposable = class {
           constructor() {
             this._disposables = [], this._isDisposed = !1;
           }
           dispose() {
             this._isDisposed = !0;
-            for (const h of this._disposables)
-              h.dispose();
+            for (const a of this._disposables)
+              a.dispose();
             this._disposables.length = 0;
           }
-          register(h) {
-            return this._disposables.push(h), h;
+          register(a) {
+            return this._disposables.push(a), a;
           }
-          unregister(h) {
-            const u = this._disposables.indexOf(h);
+          unregister(a) {
+            const u = this._disposables.indexOf(a);
             u !== -1 && this._disposables.splice(u, 1);
           }
-        }, i.toDisposable = function(h) {
-          return { dispose: h };
-        }, i.disposeArray = o, i.getDisposeArrayDisposable = function(h) {
-          return { dispose: () => o(h) };
+        }, i.toDisposable = function(a) {
+          return { dispose: a };
+        }, i.disposeArray = h, i.getDisposeArrayDisposable = function(a) {
+          return { dispose: () => h(a) };
         };
       }, 1505: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.FourKeyMap = i.TwoKeyMap = void 0;
-        class o {
+        class h {
           constructor() {
             this._data = {};
           }
           set(u, d, _) {
             this._data[u] || (this._data[u] = {}), this._data[u][d] = _;
           }
           get(u, d) {
             return this._data[u] ? this._data[u][d] : void 0;
           }
           clear() {
             this._data = {};
           }
         }
-        i.TwoKeyMap = o, i.FourKeyMap = class {
+        i.TwoKeyMap = h, i.FourKeyMap = class {
           constructor() {
-            this._data = new o();
+            this._data = new h();
           }
-          set(h, u, d, _, g) {
-            this._data.get(h, u) || this._data.set(h, u, new o()), this._data.get(h, u).set(d, _, g);
+          set(a, u, d, _, g) {
+            this._data.get(a, u) || this._data.set(a, u, new h()), this._data.get(a, u).set(d, _, g);
           }
-          get(h, u, d, _) {
+          get(a, u, d, _) {
             var g;
-            return (g = this._data.get(h, u)) === null || g === void 0 ? void 0 : g.get(d, _);
+            return (g = this._data.get(a, u)) === null || g === void 0 ? void 0 : g.get(d, _);
           }
           clear() {
             this._data.clear();
           }
         };
       }, 6114: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.isChromeOS = i.isLinux = i.isWindows = i.isIphone = i.isIpad = i.isMac = i.getSafariVersion = i.isSafari = i.isLegacyEdge = i.isFirefox = i.isNode = void 0, i.isNode = typeof navigator > "u";
-        const o = i.isNode ? "node" : navigator.userAgent, h = i.isNode ? "node" : navigator.platform;
-        i.isFirefox = o.includes("Firefox"), i.isLegacyEdge = o.includes("Edge"), i.isSafari = /^((?!chrome|android).)*safari/i.test(o), i.getSafariVersion = function() {
+        const h = i.isNode ? "node" : navigator.userAgent, a = i.isNode ? "node" : navigator.platform;
+        i.isFirefox = h.includes("Firefox"), i.isLegacyEdge = h.includes("Edge"), i.isSafari = /^((?!chrome|android).)*safari/i.test(h), i.getSafariVersion = function() {
           if (!i.isSafari)
             return 0;
-          const u = o.match(/Version\/(\d+)/);
+          const u = h.match(/Version\/(\d+)/);
           return u === null || u.length < 2 ? 0 : parseInt(u[1]);
-        }, i.isMac = ["Macintosh", "MacIntel", "MacPPC", "Mac68K"].includes(h), i.isIpad = h === "iPad", i.isIphone = h === "iPhone", i.isWindows = ["Windows", "Win16", "Win32", "WinCE"].includes(h), i.isLinux = h.indexOf("Linux") >= 0, i.isChromeOS = /\bCrOS\b/.test(o);
+        }, i.isMac = ["Macintosh", "MacIntel", "MacPPC", "Mac68K"].includes(a), i.isIpad = a === "iPad", i.isIphone = a === "iPhone", i.isWindows = ["Windows", "Win16", "Win32", "WinCE"].includes(a), i.isLinux = a.indexOf("Linux") >= 0, i.isChromeOS = /\bCrOS\b/.test(h);
       }, 6106: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.SortedList = void 0;
-        let o = 0;
+        let h = 0;
         i.SortedList = class {
-          constructor(h) {
-            this._getKey = h, this._array = [];
+          constructor(a) {
+            this._getKey = a, this._array = [];
           }
           clear() {
             this._array.length = 0;
           }
-          insert(h) {
-            this._array.length !== 0 ? (o = this._search(this._getKey(h), 0, this._array.length - 1), this._array.splice(o, 0, h)) : this._array.push(h);
+          insert(a) {
+            this._array.length !== 0 ? (h = this._search(this._getKey(a), 0, this._array.length - 1), this._array.splice(h, 0, a)) : this._array.push(a);
           }
-          delete(h) {
+          delete(a) {
             if (this._array.length === 0)
               return !1;
-            const u = this._getKey(h);
-            if (u === void 0 || (o = this._search(u, 0, this._array.length - 1), o === -1) || this._getKey(this._array[o]) !== u)
+            const u = this._getKey(a);
+            if (u === void 0 || (h = this._search(u, 0, this._array.length - 1), h === -1) || this._getKey(this._array[h]) !== u)
               return !1;
             do
-              if (this._array[o] === h)
-                return this._array.splice(o, 1), !0;
-            while (++o < this._array.length && this._getKey(this._array[o]) === u);
+              if (this._array[h] === a)
+                return this._array.splice(h, 1), !0;
+            while (++h < this._array.length && this._getKey(this._array[h]) === u);
             return !1;
           }
-          *getKeyIterator(h) {
-            if (this._array.length !== 0 && (o = this._search(h, 0, this._array.length - 1), !(o < 0 || o >= this._array.length) && this._getKey(this._array[o]) === h))
+          *getKeyIterator(a) {
+            if (this._array.length !== 0 && (h = this._search(a, 0, this._array.length - 1), !(h < 0 || h >= this._array.length) && this._getKey(this._array[h]) === a))
               do
-                yield this._array[o];
-              while (++o < this._array.length && this._getKey(this._array[o]) === h);
+                yield this._array[h];
+              while (++h < this._array.length && this._getKey(this._array[h]) === a);
           }
-          forEachByKey(h, u) {
-            if (this._array.length !== 0 && (o = this._search(h, 0, this._array.length - 1), !(o < 0 || o >= this._array.length) && this._getKey(this._array[o]) === h))
+          forEachByKey(a, u) {
+            if (this._array.length !== 0 && (h = this._search(a, 0, this._array.length - 1), !(h < 0 || h >= this._array.length) && this._getKey(this._array[h]) === a))
               do
-                u(this._array[o]);
-              while (++o < this._array.length && this._getKey(this._array[o]) === h);
+                u(this._array[h]);
+              while (++h < this._array.length && this._getKey(this._array[h]) === a);
           }
           values() {
             return this._array.values();
           }
-          _search(h, u, d) {
+          _search(a, u, d) {
             if (d < u)
               return u;
             let _ = Math.floor((u + d) / 2);
             const g = this._getKey(this._array[_]);
-            if (g > h)
-              return this._search(h, u, _ - 1);
-            if (g < h)
-              return this._search(h, _ + 1, d);
-            for (; _ > 0 && this._getKey(this._array[_ - 1]) === h; )
+            if (g > a)
+              return this._search(a, u, _ - 1);
+            if (g < a)
+              return this._search(a, _ + 1, d);
+            for (; _ > 0 && this._getKey(this._array[_ - 1]) === a; )
               _--;
             return _;
           }
         };
-      }, 7226: (T, i, o) => {
+      }, 7226: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.DebouncedIdleTask = i.IdleTaskQueue = i.PriorityTaskQueue = void 0;
-        const h = o(6114);
+        const a = h(6114);
         class u {
           constructor() {
             this._tasks = [], this._i = 0;
           }
           enqueue(g) {
             this._tasks.push(g), this._start();
           }
@@ -3649,15 +3649,15 @@
             clearTimeout(g);
           }
           _createDeadline(g) {
             const v = Date.now() + g;
             return { timeRemaining: () => Math.max(0, v - Date.now()) };
           }
         }
-        i.PriorityTaskQueue = d, i.IdleTaskQueue = !h.isNode && "requestIdleCallback" in window ? class extends u {
+        i.PriorityTaskQueue = d, i.IdleTaskQueue = !a.isNode && "requestIdleCallback" in window ? class extends u {
           _requestCallback(_) {
             return requestIdleCallback(_);
           }
           _cancelCallback(_) {
             cancelIdleCallback(_);
           }
         } : d, i.DebouncedIdleTask = class {
@@ -3667,35 +3667,35 @@
           set(_) {
             this._queue.clear(), this._queue.enqueue(_);
           }
           flush() {
             this._queue.flush();
           }
         };
-      }, 9282: (T, i, o) => {
+      }, 9282: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.updateWindowsModeWrappedState = void 0;
-        const h = o(643);
+        const a = h(643);
         i.updateWindowsModeWrappedState = function(u) {
           const d = u.buffer.lines.get(u.buffer.ybase + u.buffer.y - 1), _ = d == null ? void 0 : d.get(u.cols - 1), g = u.buffer.lines.get(u.buffer.ybase + u.buffer.y);
-          g && _ && (g.isWrapped = _[h.CHAR_DATA_CODE_INDEX] !== h.NULL_CELL_CODE && _[h.CHAR_DATA_CODE_INDEX] !== h.WHITESPACE_CELL_CODE);
+          g && _ && (g.isWrapped = _[a.CHAR_DATA_CODE_INDEX] !== a.NULL_CELL_CODE && _[a.CHAR_DATA_CODE_INDEX] !== a.WHITESPACE_CELL_CODE);
         };
       }, 3734: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.ExtendedAttrs = i.AttributeData = void 0;
-        class o {
+        class h {
           constructor() {
-            this.fg = 0, this.bg = 0, this.extended = new h();
+            this.fg = 0, this.bg = 0, this.extended = new a();
           }
           static toColorRGB(d) {
             return [d >>> 16 & 255, d >>> 8 & 255, 255 & d];
           }
           static fromColorRGB(d) {
             return (255 & d[0]) << 16 | (255 & d[1]) << 8 | 255 & d[2];
           }
           clone() {
-            const d = new o();
+            const d = new h();
             return d.fg = this.fg, d.bg = this.bg, d.extended = this.extended.clone(), d;
           }
           isInverse() {
             return 67108864 & this.fg;
           }
           isBold() {
             return 134217728 & this.fg;
@@ -3801,16 +3801,16 @@
           isUnderlineColorDefault() {
             return 268435456 & this.bg && ~this.extended.underlineColor ? (50331648 & this.extended.underlineColor) == 0 : this.isFgDefault();
           }
           getUnderlineStyle() {
             return 268435456 & this.fg ? 268435456 & this.bg ? this.extended.underlineStyle : 1 : 0;
           }
         }
-        i.AttributeData = o;
-        class h {
+        i.AttributeData = h;
+        class a {
           constructor(d = 0, _ = 0) {
             this._ext = 0, this._urlId = 0, this._ext = d, this._urlId = _;
           }
           get ext() {
             return this._urlId ? -469762049 & this._ext | this.underlineStyle << 26 : this._ext;
           }
           set ext(d) {
@@ -3831,27 +3831,27 @@
           get urlId() {
             return this._urlId;
           }
           set urlId(d) {
             this._urlId = d;
           }
           clone() {
-            return new h(this._ext, this._urlId);
+            return new a(this._ext, this._urlId);
           }
           isEmpty() {
             return this.underlineStyle === 0 && this._urlId === 0;
           }
         }
-        i.ExtendedAttrs = h;
-      }, 9092: (T, i, o) => {
+        i.ExtendedAttrs = a;
+      }, 9092: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferStringIterator = i.Buffer = i.MAX_BUFFER_SIZE = void 0;
-        const h = o(6349), u = o(8437), d = o(511), _ = o(643), g = o(4634), v = o(4863), c = o(7116), e = o(3734), s = o(7226);
+        const a = h(6349), u = h(8437), d = h(511), _ = h(643), g = h(4634), v = h(4863), c = h(7116), e = h(3734), s = h(7226);
         i.MAX_BUFFER_SIZE = 4294967295, i.Buffer = class {
           constructor(t, r, l) {
-            this._hasScrollback = t, this._optionsService = r, this._bufferService = l, this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.tabs = {}, this.savedY = 0, this.savedX = 0, this.savedCurAttrData = u.DEFAULT_ATTR_DATA.clone(), this.savedCharset = c.DEFAULT_CHARSET, this.markers = [], this._nullCell = d.CellData.fromCharData([0, _.NULL_CELL_CHAR, _.NULL_CELL_WIDTH, _.NULL_CELL_CODE]), this._whitespaceCell = d.CellData.fromCharData([0, _.WHITESPACE_CELL_CHAR, _.WHITESPACE_CELL_WIDTH, _.WHITESPACE_CELL_CODE]), this._isClearing = !1, this._memoryCleanupQueue = new s.IdleTaskQueue(), this._memoryCleanupPosition = 0, this._cols = this._bufferService.cols, this._rows = this._bufferService.rows, this.lines = new h.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
+            this._hasScrollback = t, this._optionsService = r, this._bufferService = l, this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.tabs = {}, this.savedY = 0, this.savedX = 0, this.savedCurAttrData = u.DEFAULT_ATTR_DATA.clone(), this.savedCharset = c.DEFAULT_CHARSET, this.markers = [], this._nullCell = d.CellData.fromCharData([0, _.NULL_CELL_CHAR, _.NULL_CELL_WIDTH, _.NULL_CELL_CODE]), this._whitespaceCell = d.CellData.fromCharData([0, _.WHITESPACE_CELL_CHAR, _.WHITESPACE_CELL_WIDTH, _.WHITESPACE_CELL_CODE]), this._isClearing = !1, this._memoryCleanupQueue = new s.IdleTaskQueue(), this._memoryCleanupPosition = 0, this._cols = this._bufferService.cols, this._rows = this._bufferService.rows, this.lines = new a.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
           }
           getNullCell(t) {
             return t ? (this._nullCell.fg = t.fg, this._nullCell.bg = t.bg, this._nullCell.extended = t.extended) : (this._nullCell.fg = 0, this._nullCell.bg = 0, this._nullCell.extended = new e.ExtendedAttrs()), this._nullCell;
           }
           getWhitespaceCell(t) {
             return t ? (this._whitespaceCell.fg = t.fg, this._whitespaceCell.bg = t.bg, this._whitespaceCell.extended = t.extended) : (this._whitespaceCell.fg = 0, this._whitespaceCell.bg = 0, this._whitespaceCell.extended = new e.ExtendedAttrs()), this._whitespaceCell;
           }
@@ -3876,40 +3876,40 @@
               t === void 0 && (t = u.DEFAULT_ATTR_DATA);
               let r = this._rows;
               for (; r--; )
                 this.lines.push(this.getBlankLine(t));
             }
           }
           clear() {
-            this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.lines = new h.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
+            this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.lines = new a.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops();
           }
           resize(t, r) {
             const l = this.getNullCell(u.DEFAULT_ATTR_DATA);
             let f = 0;
             const m = this._getCorrectBufferLength(r);
             if (m > this.lines.maxLength && (this.lines.maxLength = m), this.lines.length > 0) {
               if (this._cols < t)
                 for (let p = 0; p < this.lines.length; p++)
                   f += +this.lines.get(p).resize(t, l);
-              let a = 0;
+              let o = 0;
               if (this._rows < r)
                 for (let p = this._rows; p < r; p++)
-                  this.lines.length < r + this.ybase && (this._optionsService.rawOptions.windowsMode ? this.lines.push(new u.BufferLine(t, l)) : this.ybase > 0 && this.lines.length <= this.ybase + this.y + a + 1 ? (this.ybase--, a++, this.ydisp > 0 && this.ydisp--) : this.lines.push(new u.BufferLine(t, l)));
+                  this.lines.length < r + this.ybase && (this._optionsService.rawOptions.windowsMode ? this.lines.push(new u.BufferLine(t, l)) : this.ybase > 0 && this.lines.length <= this.ybase + this.y + o + 1 ? (this.ybase--, o++, this.ydisp > 0 && this.ydisp--) : this.lines.push(new u.BufferLine(t, l)));
               else
                 for (let p = this._rows; p > r; p--)
                   this.lines.length > r + this.ybase && (this.lines.length > this.ybase + this.y + 1 ? this.lines.pop() : (this.ybase++, this.ydisp++));
               if (m < this.lines.maxLength) {
                 const p = this.lines.length - m;
                 p > 0 && (this.lines.trimStart(p), this.ybase = Math.max(this.ybase - p, 0), this.ydisp = Math.max(this.ydisp - p, 0), this.savedY = Math.max(this.savedY - p, 0)), this.lines.maxLength = m;
               }
-              this.x = Math.min(this.x, t - 1), this.y = Math.min(this.y, r - 1), a && (this.y += a), this.savedX = Math.min(this.savedX, t - 1), this.scrollTop = 0;
+              this.x = Math.min(this.x, t - 1), this.y = Math.min(this.y, r - 1), o && (this.y += o), this.savedX = Math.min(this.savedX, t - 1), this.scrollTop = 0;
             }
             if (this.scrollBottom = r - 1, this._isReflowEnabled && (this._reflow(t, r), this._cols > t))
-              for (let a = 0; a < this.lines.length; a++)
-                f += +this.lines.get(a).resize(t, l);
+              for (let o = 0; o < this.lines.length; o++)
+                f += +this.lines.get(o).resize(t, l);
             this._cols = t, this._rows = r, this._memoryCleanupQueue.clear(), f > 0.1 * this.lines.length && (this._memoryCleanupPosition = 0, this._memoryCleanupQueue.enqueue(() => this._batchedMemoryCleanup()));
           }
           _batchedMemoryCleanup() {
             let t = !0;
             this._memoryCleanupPosition >= this.lines.length && (this._memoryCleanupPosition = 0, t = !1);
             let r = 0;
             for (; this._memoryCleanupPosition < this.lines.length; )
@@ -3936,33 +3936,33 @@
             for (; m-- > 0; )
               this.ybase === 0 ? (this.y > 0 && this.y--, this.lines.length < r && this.lines.push(new u.BufferLine(t, f))) : (this.ydisp === this.ybase && this.ydisp--, this.ybase--);
             this.savedY = Math.max(this.savedY - l, 0);
           }
           _reflowSmaller(t, r) {
             const l = this.getNullCell(u.DEFAULT_ATTR_DATA), f = [];
             let m = 0;
-            for (let a = this.lines.length - 1; a >= 0; a--) {
-              let p = this.lines.get(a);
+            for (let o = this.lines.length - 1; o >= 0; o--) {
+              let p = this.lines.get(o);
               if (!p || !p.isWrapped && p.getTrimmedLength() <= t)
                 continue;
               const C = [p];
-              for (; p.isWrapped && a > 0; )
-                p = this.lines.get(--a), C.unshift(p);
+              for (; p.isWrapped && o > 0; )
+                p = this.lines.get(--o), C.unshift(p);
               const y = this.ybase + this.y;
-              if (y >= a && y < a + C.length)
+              if (y >= o && y < o + C.length)
                 continue;
               const w = C[C.length - 1].getTrimmedLength(), D = (0, g.reflowSmallerGetNewLineLengths)(C, this._cols, t), x = D.length - C.length;
               let I;
               I = this.ybase === 0 && this.y !== this.lines.length - 1 ? Math.max(0, this.y - this.lines.maxLength + x) : Math.max(0, this.lines.length - this.lines.maxLength + x);
               const H = [];
               for (let F = 0; F < x; F++) {
                 const $ = this.getBlankLine(u.DEFAULT_ATTR_DATA, !0);
                 H.push($);
               }
-              H.length > 0 && (f.push({ start: a + C.length + m, newLines: H }), m += H.length), C.push(...H);
+              H.length > 0 && (f.push({ start: o + C.length + m, newLines: H }), m += H.length), C.push(...H);
               let S = D.length - 1, b = D[S];
               b === 0 && (S--, b = D[S]);
               let L = C.length - x - 1, R = w;
               for (; L >= 0; ) {
                 const F = Math.min(R, b);
                 if (C[S] === void 0)
                   break;
@@ -3976,44 +3976,44 @@
                 D[F] < t && C[F].setCell(D[F], l);
               let M = x - I;
               for (; M-- > 0; )
                 this.ybase === 0 ? this.y < r - 1 ? (this.y++, this.lines.pop()) : (this.ybase++, this.ydisp++) : this.ybase < Math.min(this.lines.maxLength, this.lines.length + m) - r && (this.ybase === this.ydisp && this.ydisp++, this.ybase++);
               this.savedY = Math.min(this.savedY + x, this.ybase + r - 1);
             }
             if (f.length > 0) {
-              const a = [], p = [];
+              const o = [], p = [];
               for (let S = 0; S < this.lines.length; S++)
                 p.push(this.lines.get(S));
               const C = this.lines.length;
               let y = C - 1, w = 0, D = f[w];
               this.lines.length = Math.min(this.lines.maxLength, this.lines.length + m);
               let x = 0;
               for (let S = Math.min(this.lines.maxLength - 1, C + m - 1); S >= 0; S--)
                 if (D && D.start > y + x) {
                   for (let b = D.newLines.length - 1; b >= 0; b--)
                     this.lines.set(S--, D.newLines[b]);
-                  S++, a.push({ index: y + 1, amount: D.newLines.length }), x += D.newLines.length, D = f[++w];
+                  S++, o.push({ index: y + 1, amount: D.newLines.length }), x += D.newLines.length, D = f[++w];
                 } else
                   this.lines.set(S, p[y--]);
               let I = 0;
-              for (let S = a.length - 1; S >= 0; S--)
-                a[S].index += I, this.lines.onInsertEmitter.fire(a[S]), I += a[S].amount;
+              for (let S = o.length - 1; S >= 0; S--)
+                o[S].index += I, this.lines.onInsertEmitter.fire(o[S]), I += o[S].amount;
               const H = Math.max(0, C + m - this.lines.maxLength);
               H > 0 && this.lines.onTrimEmitter.fire(H);
             }
           }
           stringIndexToBufferIndex(t, r, l = !1) {
             for (; r; ) {
               const f = this.lines.get(t);
               if (!f)
                 return [-1, -1];
               const m = l ? f.getTrimmedLength() : f.length;
-              for (let a = 0; a < m; ++a)
-                if (f.get(a)[_.CHAR_DATA_WIDTH_INDEX] && (r -= f.get(a)[_.CHAR_DATA_CHAR_INDEX].length || 1), r < 0)
-                  return [t, a];
+              for (let o = 0; o < m; ++o)
+                if (f.get(o)[_.CHAR_DATA_WIDTH_INDEX] && (r -= f.get(o)[_.CHAR_DATA_CHAR_INDEX].length || 1), r < 0)
+                  return [t, o];
               t++;
             }
             return [t, 0];
           }
           translateBufferLineToString(t, r, l = 0, f) {
             const m = this.lines.get(t);
             return m ? m.translateToString(r, l, f) : "";
@@ -4066,46 +4066,46 @@
             this._isClearing || this.markers.splice(this.markers.indexOf(t), 1);
           }
           iterator(t, r, l, f, m) {
             return new n(this, t, r, l, f, m);
           }
         };
         class n {
-          constructor(r, l, f = 0, m = r.lines.length, a = 0, p = 0) {
-            this._buffer = r, this._trimRight = l, this._startIndex = f, this._endIndex = m, this._startOverscan = a, this._endOverscan = p, this._startIndex < 0 && (this._startIndex = 0), this._endIndex > this._buffer.lines.length && (this._endIndex = this._buffer.lines.length), this._current = this._startIndex;
+          constructor(r, l, f = 0, m = r.lines.length, o = 0, p = 0) {
+            this._buffer = r, this._trimRight = l, this._startIndex = f, this._endIndex = m, this._startOverscan = o, this._endOverscan = p, this._startIndex < 0 && (this._startIndex = 0), this._endIndex > this._buffer.lines.length && (this._endIndex = this._buffer.lines.length), this._current = this._startIndex;
           }
           hasNext() {
             return this._current < this._endIndex;
           }
           next() {
             const r = this._buffer.getWrappedRangeForLine(this._current);
             r.first < this._startIndex - this._startOverscan && (r.first = this._startIndex - this._startOverscan), r.last > this._endIndex + this._endOverscan && (r.last = this._endIndex + this._endOverscan), r.first = Math.max(r.first, 0), r.last = Math.min(r.last, this._buffer.lines.length);
             let l = "";
             for (let f = r.first; f <= r.last; ++f)
               l += this._buffer.translateBufferLineToString(f, this._trimRight);
             return this._current = r.last + 1, { range: r, content: l };
           }
         }
         i.BufferStringIterator = n;
-      }, 8437: (T, i, o) => {
+      }, 8437: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferLine = i.DEFAULT_ATTR_DATA = void 0;
-        const h = o(482), u = o(643), d = o(511), _ = o(3734);
+        const a = h(482), u = h(643), d = h(511), _ = h(3734);
         i.DEFAULT_ATTR_DATA = Object.freeze(new _.AttributeData());
         let g = 0;
         class v {
           constructor(e, s, n = !1) {
             this.isWrapped = n, this._combined = {}, this._extendedAttrs = {}, this._data = new Uint32Array(3 * e);
             const t = s || d.CellData.fromCharData([0, u.NULL_CELL_CHAR, u.NULL_CELL_WIDTH, u.NULL_CELL_CODE]);
             for (let r = 0; r < e; ++r)
               this.setCell(r, t);
             this.length = e;
           }
           get(e) {
             const s = this._data[3 * e + 0], n = 2097151 & s;
-            return [this._data[3 * e + 1], 2097152 & s ? this._combined[e] : n ? (0, h.stringFromCodePoint)(n) : "", s >> 22, 2097152 & s ? this._combined[e].charCodeAt(this._combined[e].length - 1) : n];
+            return [this._data[3 * e + 1], 2097152 & s ? this._combined[e] : n ? (0, a.stringFromCodePoint)(n) : "", s >> 22, 2097152 & s ? this._combined[e].charCodeAt(this._combined[e].length - 1) : n];
           }
           set(e, s) {
             this._data[3 * e + 1] = s[u.CHAR_DATA_ATTR_INDEX], s[u.CHAR_DATA_CHAR_INDEX].length > 1 ? (this._combined[e] = s[1], this._data[3 * e + 0] = 2097152 | e | s[u.CHAR_DATA_WIDTH_INDEX] << 22) : this._data[3 * e + 0] = s[u.CHAR_DATA_CHAR_INDEX].charCodeAt(0) | s[u.CHAR_DATA_WIDTH_INDEX] << 22;
           }
           getWidth(e) {
             return this._data[3 * e + 0] >> 22;
           }
@@ -4126,15 +4126,15 @@
             return 2097152 & s ? this._combined[e].charCodeAt(this._combined[e].length - 1) : 2097151 & s;
           }
           isCombined(e) {
             return 2097152 & this._data[3 * e + 0];
           }
           getString(e) {
             const s = this._data[3 * e + 0];
-            return 2097152 & s ? this._combined[e] : 2097151 & s ? (0, h.stringFromCodePoint)(2097151 & s) : "";
+            return 2097152 & s ? this._combined[e] : 2097151 & s ? (0, a.stringFromCodePoint)(2097151 & s) : "";
           }
           isProtected(e) {
             return 536870912 & this._data[3 * e + 2];
           }
           loadCell(e, s) {
             return g = 3 * e, s.content = this._data[g + 0], s.fg = this._data[g + 1], s.bg = this._data[g + 2], 2097152 & s.content && (s.combinedData = this._combined[e]), 268435456 & s.bg && (s.extended = this._extendedAttrs[e]), s;
           }
@@ -4142,15 +4142,15 @@
             2097152 & s.content && (this._combined[e] = s.combinedData), 268435456 & s.bg && (this._extendedAttrs[e] = s.extended), this._data[3 * e + 0] = s.content, this._data[3 * e + 1] = s.fg, this._data[3 * e + 2] = s.bg;
           }
           setCellFromCodePoint(e, s, n, t, r, l) {
             268435456 & r && (this._extendedAttrs[e] = l), this._data[3 * e + 0] = s | n << 22, this._data[3 * e + 1] = t, this._data[3 * e + 2] = r;
           }
           addCodepointToCell(e, s) {
             let n = this._data[3 * e + 0];
-            2097152 & n ? this._combined[e] += (0, h.stringFromCodePoint)(s) : (2097151 & n ? (this._combined[e] = (0, h.stringFromCodePoint)(2097151 & n) + (0, h.stringFromCodePoint)(s), n &= -2097152, n |= 2097152) : n = s | 4194304, this._data[3 * e + 0] = n);
+            2097152 & n ? this._combined[e] += (0, a.stringFromCodePoint)(s) : (2097151 & n ? (this._combined[e] = (0, a.stringFromCodePoint)(2097151 & n) + (0, a.stringFromCodePoint)(s), n &= -2097152, n |= 2097152) : n = s | 4194304, this._data[3 * e + 0] = n);
           }
           insertCells(e, s, n, t) {
             if ((e %= this.length) && this.getWidth(e - 1) === 2 && this.setCellFromCodePoint(e - 1, 0, 1, (t == null ? void 0 : t.fg) || 0, (t == null ? void 0 : t.bg) || 0, (t == null ? void 0 : t.extended) || new _.ExtendedAttrs()), s < this.length - e) {
               const r = new d.CellData();
               for (let l = this.length - e - s - 1; l >= 0; --l)
                 this.setCell(e + s + l, this.loadCell(e + l, r));
               for (let l = 0; l < s; ++l)
@@ -4249,123 +4249,123 @@
                 return e + (this._data[3 * e + 0] >> 22);
             return 0;
           }
           copyCellsFrom(e, s, n, t, r) {
             const l = e._data;
             if (r)
               for (let m = t - 1; m >= 0; m--) {
-                for (let a = 0; a < 3; a++)
-                  this._data[3 * (n + m) + a] = l[3 * (s + m) + a];
+                for (let o = 0; o < 3; o++)
+                  this._data[3 * (n + m) + o] = l[3 * (s + m) + o];
                 268435456 & l[3 * (s + m) + 2] && (this._extendedAttrs[n + m] = e._extendedAttrs[s + m]);
               }
             else
               for (let m = 0; m < t; m++) {
-                for (let a = 0; a < 3; a++)
-                  this._data[3 * (n + m) + a] = l[3 * (s + m) + a];
+                for (let o = 0; o < 3; o++)
+                  this._data[3 * (n + m) + o] = l[3 * (s + m) + o];
                 268435456 & l[3 * (s + m) + 2] && (this._extendedAttrs[n + m] = e._extendedAttrs[s + m]);
               }
             const f = Object.keys(e._combined);
             for (let m = 0; m < f.length; m++) {
-              const a = parseInt(f[m], 10);
-              a >= s && (this._combined[a - s + n] = e._combined[a]);
+              const o = parseInt(f[m], 10);
+              o >= s && (this._combined[o - s + n] = e._combined[o]);
             }
           }
           translateToString(e = !1, s = 0, n = this.length) {
             e && (n = Math.min(n, this.getTrimmedLength()));
             let t = "";
             for (; s < n; ) {
               const r = this._data[3 * s + 0], l = 2097151 & r;
-              t += 2097152 & r ? this._combined[s] : l ? (0, h.stringFromCodePoint)(l) : u.WHITESPACE_CELL_CHAR, s += r >> 22 || 1;
+              t += 2097152 & r ? this._combined[s] : l ? (0, a.stringFromCodePoint)(l) : u.WHITESPACE_CELL_CHAR, s += r >> 22 || 1;
             }
             return t;
           }
         }
         i.BufferLine = v;
       }, 4841: (T, i) => {
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.getRangeLength = void 0, i.getRangeLength = function(o, h) {
-          if (o.start.y > o.end.y)
-            throw new Error(`Buffer range end (${o.end.x}, ${o.end.y}) cannot be before start (${o.start.x}, ${o.start.y})`);
-          return h * (o.end.y - o.start.y) + (o.end.x - o.start.x + 1);
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.getRangeLength = void 0, i.getRangeLength = function(h, a) {
+          if (h.start.y > h.end.y)
+            throw new Error(`Buffer range end (${h.end.x}, ${h.end.y}) cannot be before start (${h.start.x}, ${h.start.y})`);
+          return a * (h.end.y - h.start.y) + (h.end.x - h.start.x + 1);
         };
       }, 4634: (T, i) => {
-        function o(h, u, d) {
-          if (u === h.length - 1)
-            return h[u].getTrimmedLength();
-          const _ = !h[u].hasContent(d - 1) && h[u].getWidth(d - 1) === 1, g = h[u + 1].getWidth(0) === 2;
+        function h(a, u, d) {
+          if (u === a.length - 1)
+            return a[u].getTrimmedLength();
+          const _ = !a[u].hasContent(d - 1) && a[u].getWidth(d - 1) === 1, g = a[u + 1].getWidth(0) === 2;
           return _ && g ? d - 1 : d;
         }
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.getWrappedLineTrimmedLength = i.reflowSmallerGetNewLineLengths = i.reflowLargerApplyNewLayout = i.reflowLargerCreateNewLayout = i.reflowLargerGetLinesToRemove = void 0, i.reflowLargerGetLinesToRemove = function(h, u, d, _, g) {
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.getWrappedLineTrimmedLength = i.reflowSmallerGetNewLineLengths = i.reflowLargerApplyNewLayout = i.reflowLargerCreateNewLayout = i.reflowLargerGetLinesToRemove = void 0, i.reflowLargerGetLinesToRemove = function(a, u, d, _, g) {
           const v = [];
-          for (let c = 0; c < h.length - 1; c++) {
-            let e = c, s = h.get(++e);
+          for (let c = 0; c < a.length - 1; c++) {
+            let e = c, s = a.get(++e);
             if (!s.isWrapped)
               continue;
-            const n = [h.get(c)];
-            for (; e < h.length && s.isWrapped; )
-              n.push(s), s = h.get(++e);
+            const n = [a.get(c)];
+            for (; e < a.length && s.isWrapped; )
+              n.push(s), s = a.get(++e);
             if (_ >= c && _ < e) {
               c += n.length - 1;
               continue;
             }
-            let t = 0, r = o(n, t, u), l = 1, f = 0;
+            let t = 0, r = h(n, t, u), l = 1, f = 0;
             for (; l < n.length; ) {
-              const a = o(n, l, u), p = a - f, C = d - r, y = Math.min(p, C);
-              n[t].copyCellsFrom(n[l], f, r, y, !1), r += y, r === d && (t++, r = 0), f += y, f === a && (l++, f = 0), r === 0 && t !== 0 && n[t - 1].getWidth(d - 1) === 2 && (n[t].copyCellsFrom(n[t - 1], d - 1, r++, 1, !1), n[t - 1].setCell(d - 1, g));
+              const o = h(n, l, u), p = o - f, C = d - r, y = Math.min(p, C);
+              n[t].copyCellsFrom(n[l], f, r, y, !1), r += y, r === d && (t++, r = 0), f += y, f === o && (l++, f = 0), r === 0 && t !== 0 && n[t - 1].getWidth(d - 1) === 2 && (n[t].copyCellsFrom(n[t - 1], d - 1, r++, 1, !1), n[t - 1].setCell(d - 1, g));
             }
             n[t].replaceCells(r, d, g);
             let m = 0;
-            for (let a = n.length - 1; a > 0 && (a > t || n[a].getTrimmedLength() === 0); a--)
+            for (let o = n.length - 1; o > 0 && (o > t || n[o].getTrimmedLength() === 0); o--)
               m++;
             m > 0 && (v.push(c + n.length - m), v.push(m)), c += n.length - 1;
           }
           return v;
-        }, i.reflowLargerCreateNewLayout = function(h, u) {
+        }, i.reflowLargerCreateNewLayout = function(a, u) {
           const d = [];
           let _ = 0, g = u[_], v = 0;
-          for (let c = 0; c < h.length; c++)
+          for (let c = 0; c < a.length; c++)
             if (g === c) {
               const e = u[++_];
-              h.onDeleteEmitter.fire({ index: c - v, amount: e }), c += e - 1, v += e, g = u[++_];
+              a.onDeleteEmitter.fire({ index: c - v, amount: e }), c += e - 1, v += e, g = u[++_];
             } else
               d.push(c);
           return { layout: d, countRemoved: v };
-        }, i.reflowLargerApplyNewLayout = function(h, u) {
+        }, i.reflowLargerApplyNewLayout = function(a, u) {
           const d = [];
           for (let _ = 0; _ < u.length; _++)
-            d.push(h.get(u[_]));
+            d.push(a.get(u[_]));
           for (let _ = 0; _ < d.length; _++)
-            h.set(_, d[_]);
-          h.length = u.length;
-        }, i.reflowSmallerGetNewLineLengths = function(h, u, d) {
-          const _ = [], g = h.map((s, n) => o(h, n, u)).reduce((s, n) => s + n);
+            a.set(_, d[_]);
+          a.length = u.length;
+        }, i.reflowSmallerGetNewLineLengths = function(a, u, d) {
+          const _ = [], g = a.map((s, n) => h(a, n, u)).reduce((s, n) => s + n);
           let v = 0, c = 0, e = 0;
           for (; e < g; ) {
             if (g - e < d) {
               _.push(g - e);
               break;
             }
             v += d;
-            const s = o(h, c, u);
+            const s = h(a, c, u);
             v > s && (v -= s, c++);
-            const n = h[c].getWidth(v - 1) === 2;
+            const n = a[c].getWidth(v - 1) === 2;
             n && v--;
             const t = n ? d - 1 : d;
             _.push(t), e += t;
           }
           return _;
-        }, i.getWrappedLineTrimmedLength = o;
-      }, 5295: (T, i, o) => {
+        }, i.getWrappedLineTrimmedLength = h;
+      }, 5295: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferSet = void 0;
-        const h = o(9092), u = o(8460), d = o(844);
+        const a = h(9092), u = h(8460), d = h(844);
         class _ extends d.Disposable {
           constructor(v, c) {
             super(), this._optionsService = v, this._bufferService = c, this._onBufferActivate = this.register(new u.EventEmitter()), this.onBufferActivate = this._onBufferActivate.event, this.reset(), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.resize(this._bufferService.cols, this._bufferService.rows))), this.register(this._optionsService.onSpecificOptionChange("tabStopWidth", () => this.setupTabStops()));
           }
           reset() {
-            this._normal = new h.Buffer(!0, this._optionsService, this._bufferService), this._normal.fillViewportRows(), this._alt = new h.Buffer(!1, this._optionsService, this._bufferService), this._activeBuffer = this._normal, this._onBufferActivate.fire({ activeBuffer: this._normal, inactiveBuffer: this._alt }), this.setupTabStops();
+            this._normal = new a.Buffer(!0, this._optionsService, this._bufferService), this._normal.fillViewportRows(), this._alt = new a.Buffer(!1, this._optionsService, this._bufferService), this._activeBuffer = this._normal, this._onBufferActivate.fire({ activeBuffer: this._normal, inactiveBuffer: this._alt }), this.setupTabStops();
           }
           get alt() {
             return this._alt;
           }
           get active() {
             return this._activeBuffer;
           }
@@ -4382,17 +4382,17 @@
             this._normal.resize(v, c), this._alt.resize(v, c), this.setupTabStops(v);
           }
           setupTabStops(v) {
             this._normal.setupTabStops(v), this._alt.setupTabStops(v);
           }
         }
         i.BufferSet = _;
-      }, 511: (T, i, o) => {
+      }, 511: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CellData = void 0;
-        const h = o(482), u = o(643), d = o(3734);
+        const a = h(482), u = h(643), d = h(3734);
         class _ extends d.AttributeData {
           constructor() {
             super(...arguments), this.content = 0, this.fg = 0, this.bg = 0, this.extended = new d.ExtendedAttrs(), this.combinedData = "";
           }
           static fromCharData(v) {
             const c = new _();
             return c.setFromCharData(v), c;
@@ -4400,15 +4400,15 @@
           isCombined() {
             return 2097152 & this.content;
           }
           getWidth() {
             return this.content >> 22;
           }
           getChars() {
-            return 2097152 & this.content ? this.combinedData : 2097151 & this.content ? (0, h.stringFromCodePoint)(2097151 & this.content) : "";
+            return 2097152 & this.content ? this.combinedData : 2097151 & this.content ? (0, a.stringFromCodePoint)(2097151 & this.content) : "";
           }
           getCode() {
             return this.isCombined() ? this.combinedData.charCodeAt(this.combinedData.length - 1) : 2097151 & this.content;
           }
           setFromCharData(v) {
             this.fg = v[u.CHAR_DATA_ATTR_INDEX], this.bg = 0;
             let c = !1;
@@ -4428,20 +4428,20 @@
           getAsCharData() {
             return [this.fg, this.getChars(), this.getWidth(), this.getCode()];
           }
         }
         i.CellData = _;
       }, 643: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.WHITESPACE_CELL_CODE = i.WHITESPACE_CELL_WIDTH = i.WHITESPACE_CELL_CHAR = i.NULL_CELL_CODE = i.NULL_CELL_WIDTH = i.NULL_CELL_CHAR = i.CHAR_DATA_CODE_INDEX = i.CHAR_DATA_WIDTH_INDEX = i.CHAR_DATA_CHAR_INDEX = i.CHAR_DATA_ATTR_INDEX = i.DEFAULT_EXT = i.DEFAULT_ATTR = i.DEFAULT_COLOR = void 0, i.DEFAULT_COLOR = 0, i.DEFAULT_ATTR = 256 | i.DEFAULT_COLOR << 9, i.DEFAULT_EXT = 0, i.CHAR_DATA_ATTR_INDEX = 0, i.CHAR_DATA_CHAR_INDEX = 1, i.CHAR_DATA_WIDTH_INDEX = 2, i.CHAR_DATA_CODE_INDEX = 3, i.NULL_CELL_CHAR = "", i.NULL_CELL_WIDTH = 1, i.NULL_CELL_CODE = 0, i.WHITESPACE_CELL_CHAR = " ", i.WHITESPACE_CELL_WIDTH = 1, i.WHITESPACE_CELL_CODE = 32;
-      }, 4863: (T, i, o) => {
+      }, 4863: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.Marker = void 0;
-        const h = o(8460), u = o(844);
+        const a = h(8460), u = h(844);
         class d {
           constructor(g) {
-            this.line = g, this.isDisposed = !1, this._disposables = [], this._id = d._nextId++, this._onDispose = this.register(new h.EventEmitter()), this.onDispose = this._onDispose.event;
+            this.line = g, this.isDisposed = !1, this._disposables = [], this._id = d._nextId++, this._onDispose = this.register(new a.EventEmitter()), this.onDispose = this._onDispose.event;
           }
           get id() {
             return this._id;
           }
           dispose() {
             this.isDisposed || (this.isDisposed = !0, this.line = -1, this._onDispose.fire(), (0, u.disposeArray)(this._disposables), this._disposables.length = 0);
           }
@@ -4449,286 +4449,286 @@
             return this._disposables.push(g), g;
           }
         }
         i.Marker = d, d._nextId = 1;
       }, 7116: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.DEFAULT_CHARSET = i.CHARSETS = void 0, i.CHARSETS = {}, i.DEFAULT_CHARSET = i.CHARSETS.B, i.CHARSETS[0] = { "`": "◆", a: "▒", b: "␉", c: "␌", d: "␍", e: "␊", f: "°", g: "±", h: "␤", i: "␋", j: "┘", k: "┐", l: "┌", m: "└", n: "┼", o: "⎺", p: "⎻", q: "─", r: "⎼", s: "⎽", t: "├", u: "┤", v: "┴", w: "┬", x: "│", y: "≤", z: "≥", "{": "π", "|": "≠", "}": "£", "~": "·" }, i.CHARSETS.A = { "#": "£" }, i.CHARSETS.B = void 0, i.CHARSETS[4] = { "#": "£", "@": "¾", "[": "ij", "\\": "½", "]": "|", "{": "¨", "|": "f", "}": "¼", "~": "´" }, i.CHARSETS.C = i.CHARSETS[5] = { "[": "Ä", "\\": "Ö", "]": "Å", "^": "Ü", "`": "é", "{": "ä", "|": "ö", "}": "å", "~": "ü" }, i.CHARSETS.R = { "#": "£", "@": "à", "[": "°", "\\": "ç", "]": "§", "{": "é", "|": "ù", "}": "è", "~": "¨" }, i.CHARSETS.Q = { "@": "à", "[": "â", "\\": "ç", "]": "ê", "^": "î", "`": "ô", "{": "é", "|": "ù", "}": "è", "~": "û" }, i.CHARSETS.K = { "@": "§", "[": "Ä", "\\": "Ö", "]": "Ü", "{": "ä", "|": "ö", "}": "ü", "~": "ß" }, i.CHARSETS.Y = { "#": "£", "@": "§", "[": "°", "\\": "ç", "]": "é", "`": "ù", "{": "à", "|": "ò", "}": "è", "~": "ì" }, i.CHARSETS.E = i.CHARSETS[6] = { "@": "Ä", "[": "Æ", "\\": "Ø", "]": "Å", "^": "Ü", "`": "ä", "{": "æ", "|": "ø", "}": "å", "~": "ü" }, i.CHARSETS.Z = { "#": "£", "@": "§", "[": "¡", "\\": "Ñ", "]": "¿", "{": "°", "|": "ñ", "}": "ç" }, i.CHARSETS.H = i.CHARSETS[7] = { "@": "É", "[": "Ä", "\\": "Ö", "]": "Å", "^": "Ü", "`": "é", "{": "ä", "|": "ö", "}": "å", "~": "ü" }, i.CHARSETS["="] = { "#": "ù", "@": "à", "[": "é", "\\": "ç", "]": "ê", "^": "î", _: "è", "`": "ô", "{": "ä", "|": "ö", "}": "ü", "~": "û" };
       }, 2584: (T, i) => {
-        var o, h;
+        var h, a;
         Object.defineProperty(i, "__esModule", { value: !0 }), i.C1_ESCAPED = i.C1 = i.C0 = void 0, function(u) {
           u.NUL = "\0", u.SOH = "", u.STX = "", u.ETX = "", u.EOT = "", u.ENQ = "", u.ACK = "", u.BEL = "\x07", u.BS = "\b", u.HT = "	", u.LF = `
 `, u.VT = "\v", u.FF = "\f", u.CR = "\r", u.SO = "", u.SI = "", u.DLE = "", u.DC1 = "", u.DC2 = "", u.DC3 = "", u.DC4 = "", u.NAK = "", u.SYN = "", u.ETB = "", u.CAN = "", u.EM = "", u.SUB = "", u.ESC = "\x1B", u.FS = "", u.GS = "", u.RS = "", u.US = "", u.SP = " ", u.DEL = "";
-        }(o = i.C0 || (i.C0 = {})), (h = i.C1 || (i.C1 = {})).PAD = "", h.HOP = "", h.BPH = "", h.NBH = "", h.IND = "", h.NEL = "", h.SSA = "", h.ESA = "", h.HTS = "", h.HTJ = "", h.VTS = "", h.PLD = "", h.PLU = "", h.RI = "", h.SS2 = "", h.SS3 = "", h.DCS = "", h.PU1 = "", h.PU2 = "", h.STS = "", h.CCH = "", h.MW = "", h.SPA = "", h.EPA = "", h.SOS = "", h.SGCI = "", h.SCI = "", h.CSI = "", h.ST = "", h.OSC = "", h.PM = "", h.APC = "", (i.C1_ESCAPED || (i.C1_ESCAPED = {})).ST = `${o.ESC}\\`;
-      }, 7399: (T, i, o) => {
+        }(h = i.C0 || (i.C0 = {})), (a = i.C1 || (i.C1 = {})).PAD = "", a.HOP = "", a.BPH = "", a.NBH = "", a.IND = "", a.NEL = "", a.SSA = "", a.ESA = "", a.HTS = "", a.HTJ = "", a.VTS = "", a.PLD = "", a.PLU = "", a.RI = "", a.SS2 = "", a.SS3 = "", a.DCS = "", a.PU1 = "", a.PU2 = "", a.STS = "", a.CCH = "", a.MW = "", a.SPA = "", a.EPA = "", a.SOS = "", a.SGCI = "", a.SCI = "", a.CSI = "", a.ST = "", a.OSC = "", a.PM = "", a.APC = "", (i.C1_ESCAPED || (i.C1_ESCAPED = {})).ST = `${h.ESC}\\`;
+      }, 7399: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.evaluateKeyboardEvent = void 0;
-        const h = o(2584), u = { 48: ["0", ")"], 49: ["1", "!"], 50: ["2", "@"], 51: ["3", "#"], 52: ["4", "$"], 53: ["5", "%"], 54: ["6", "^"], 55: ["7", "&"], 56: ["8", "*"], 57: ["9", "("], 186: [";", ":"], 187: ["=", "+"], 188: [",", "<"], 189: ["-", "_"], 190: [".", ">"], 191: ["/", "?"], 192: ["`", "~"], 219: ["[", "{"], 220: ["\\", "|"], 221: ["]", "}"], 222: ["'", '"'] };
+        const a = h(2584), u = { 48: ["0", ")"], 49: ["1", "!"], 50: ["2", "@"], 51: ["3", "#"], 52: ["4", "$"], 53: ["5", "%"], 54: ["6", "^"], 55: ["7", "&"], 56: ["8", "*"], 57: ["9", "("], 186: [";", ":"], 187: ["=", "+"], 188: [",", "<"], 189: ["-", "_"], 190: [".", ">"], 191: ["/", "?"], 192: ["`", "~"], 219: ["[", "{"], 220: ["\\", "|"], 221: ["]", "}"], 222: ["'", '"'] };
         i.evaluateKeyboardEvent = function(d, _, g, v) {
           const c = { type: 0, cancel: !1, key: void 0 }, e = (d.shiftKey ? 1 : 0) | (d.altKey ? 2 : 0) | (d.ctrlKey ? 4 : 0) | (d.metaKey ? 8 : 0);
           switch (d.keyCode) {
             case 0:
-              d.key === "UIKeyInputUpArrow" ? c.key = _ ? h.C0.ESC + "OA" : h.C0.ESC + "[A" : d.key === "UIKeyInputLeftArrow" ? c.key = _ ? h.C0.ESC + "OD" : h.C0.ESC + "[D" : d.key === "UIKeyInputRightArrow" ? c.key = _ ? h.C0.ESC + "OC" : h.C0.ESC + "[C" : d.key === "UIKeyInputDownArrow" && (c.key = _ ? h.C0.ESC + "OB" : h.C0.ESC + "[B");
+              d.key === "UIKeyInputUpArrow" ? c.key = _ ? a.C0.ESC + "OA" : a.C0.ESC + "[A" : d.key === "UIKeyInputLeftArrow" ? c.key = _ ? a.C0.ESC + "OD" : a.C0.ESC + "[D" : d.key === "UIKeyInputRightArrow" ? c.key = _ ? a.C0.ESC + "OC" : a.C0.ESC + "[C" : d.key === "UIKeyInputDownArrow" && (c.key = _ ? a.C0.ESC + "OB" : a.C0.ESC + "[B");
               break;
             case 8:
               if (d.altKey) {
-                c.key = h.C0.ESC + h.C0.DEL;
+                c.key = a.C0.ESC + a.C0.DEL;
                 break;
               }
-              c.key = h.C0.DEL;
+              c.key = a.C0.DEL;
               break;
             case 9:
               if (d.shiftKey) {
-                c.key = h.C0.ESC + "[Z";
+                c.key = a.C0.ESC + "[Z";
                 break;
               }
-              c.key = h.C0.HT, c.cancel = !0;
+              c.key = a.C0.HT, c.cancel = !0;
               break;
             case 13:
-              c.key = d.altKey ? h.C0.ESC + h.C0.CR : h.C0.CR, c.cancel = !0;
+              c.key = d.altKey ? a.C0.ESC + a.C0.CR : a.C0.CR, c.cancel = !0;
               break;
             case 27:
-              c.key = h.C0.ESC, d.altKey && (c.key = h.C0.ESC + h.C0.ESC), c.cancel = !0;
+              c.key = a.C0.ESC, d.altKey && (c.key = a.C0.ESC + a.C0.ESC), c.cancel = !0;
               break;
             case 37:
               if (d.metaKey)
                 break;
-              e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "D", c.key === h.C0.ESC + "[1;3D" && (c.key = h.C0.ESC + (g ? "b" : "[1;5D"))) : c.key = _ ? h.C0.ESC + "OD" : h.C0.ESC + "[D";
+              e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "D", c.key === a.C0.ESC + "[1;3D" && (c.key = a.C0.ESC + (g ? "b" : "[1;5D"))) : c.key = _ ? a.C0.ESC + "OD" : a.C0.ESC + "[D";
               break;
             case 39:
               if (d.metaKey)
                 break;
-              e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "C", c.key === h.C0.ESC + "[1;3C" && (c.key = h.C0.ESC + (g ? "f" : "[1;5C"))) : c.key = _ ? h.C0.ESC + "OC" : h.C0.ESC + "[C";
+              e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "C", c.key === a.C0.ESC + "[1;3C" && (c.key = a.C0.ESC + (g ? "f" : "[1;5C"))) : c.key = _ ? a.C0.ESC + "OC" : a.C0.ESC + "[C";
               break;
             case 38:
               if (d.metaKey)
                 break;
-              e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "A", g || c.key !== h.C0.ESC + "[1;3A" || (c.key = h.C0.ESC + "[1;5A")) : c.key = _ ? h.C0.ESC + "OA" : h.C0.ESC + "[A";
+              e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "A", g || c.key !== a.C0.ESC + "[1;3A" || (c.key = a.C0.ESC + "[1;5A")) : c.key = _ ? a.C0.ESC + "OA" : a.C0.ESC + "[A";
               break;
             case 40:
               if (d.metaKey)
                 break;
-              e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "B", g || c.key !== h.C0.ESC + "[1;3B" || (c.key = h.C0.ESC + "[1;5B")) : c.key = _ ? h.C0.ESC + "OB" : h.C0.ESC + "[B";
+              e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "B", g || c.key !== a.C0.ESC + "[1;3B" || (c.key = a.C0.ESC + "[1;5B")) : c.key = _ ? a.C0.ESC + "OB" : a.C0.ESC + "[B";
               break;
             case 45:
-              d.shiftKey || d.ctrlKey || (c.key = h.C0.ESC + "[2~");
+              d.shiftKey || d.ctrlKey || (c.key = a.C0.ESC + "[2~");
               break;
             case 46:
-              c.key = e ? h.C0.ESC + "[3;" + (e + 1) + "~" : h.C0.ESC + "[3~";
+              c.key = e ? a.C0.ESC + "[3;" + (e + 1) + "~" : a.C0.ESC + "[3~";
               break;
             case 36:
-              c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "H" : _ ? h.C0.ESC + "OH" : h.C0.ESC + "[H";
+              c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "H" : _ ? a.C0.ESC + "OH" : a.C0.ESC + "[H";
               break;
             case 35:
-              c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "F" : _ ? h.C0.ESC + "OF" : h.C0.ESC + "[F";
+              c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "F" : _ ? a.C0.ESC + "OF" : a.C0.ESC + "[F";
               break;
             case 33:
-              d.shiftKey ? c.type = 2 : d.ctrlKey ? c.key = h.C0.ESC + "[5;" + (e + 1) + "~" : c.key = h.C0.ESC + "[5~";
+              d.shiftKey ? c.type = 2 : d.ctrlKey ? c.key = a.C0.ESC + "[5;" + (e + 1) + "~" : c.key = a.C0.ESC + "[5~";
               break;
             case 34:
-              d.shiftKey ? c.type = 3 : d.ctrlKey ? c.key = h.C0.ESC + "[6;" + (e + 1) + "~" : c.key = h.C0.ESC + "[6~";
+              d.shiftKey ? c.type = 3 : d.ctrlKey ? c.key = a.C0.ESC + "[6;" + (e + 1) + "~" : c.key = a.C0.ESC + "[6~";
               break;
             case 112:
-              c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "P" : h.C0.ESC + "OP";
+              c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "P" : a.C0.ESC + "OP";
               break;
             case 113:
-              c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "Q" : h.C0.ESC + "OQ";
+              c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "Q" : a.C0.ESC + "OQ";
               break;
             case 114:
-              c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "R" : h.C0.ESC + "OR";
+              c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "R" : a.C0.ESC + "OR";
               break;
             case 115:
-              c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "S" : h.C0.ESC + "OS";
+              c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "S" : a.C0.ESC + "OS";
               break;
             case 116:
-              c.key = e ? h.C0.ESC + "[15;" + (e + 1) + "~" : h.C0.ESC + "[15~";
+              c.key = e ? a.C0.ESC + "[15;" + (e + 1) + "~" : a.C0.ESC + "[15~";
               break;
             case 117:
-              c.key = e ? h.C0.ESC + "[17;" + (e + 1) + "~" : h.C0.ESC + "[17~";
+              c.key = e ? a.C0.ESC + "[17;" + (e + 1) + "~" : a.C0.ESC + "[17~";
               break;
             case 118:
-              c.key = e ? h.C0.ESC + "[18;" + (e + 1) + "~" : h.C0.ESC + "[18~";
+              c.key = e ? a.C0.ESC + "[18;" + (e + 1) + "~" : a.C0.ESC + "[18~";
               break;
             case 119:
-              c.key = e ? h.C0.ESC + "[19;" + (e + 1) + "~" : h.C0.ESC + "[19~";
+              c.key = e ? a.C0.ESC + "[19;" + (e + 1) + "~" : a.C0.ESC + "[19~";
               break;
             case 120:
-              c.key = e ? h.C0.ESC + "[20;" + (e + 1) + "~" : h.C0.ESC + "[20~";
+              c.key = e ? a.C0.ESC + "[20;" + (e + 1) + "~" : a.C0.ESC + "[20~";
               break;
             case 121:
-              c.key = e ? h.C0.ESC + "[21;" + (e + 1) + "~" : h.C0.ESC + "[21~";
+              c.key = e ? a.C0.ESC + "[21;" + (e + 1) + "~" : a.C0.ESC + "[21~";
               break;
             case 122:
-              c.key = e ? h.C0.ESC + "[23;" + (e + 1) + "~" : h.C0.ESC + "[23~";
+              c.key = e ? a.C0.ESC + "[23;" + (e + 1) + "~" : a.C0.ESC + "[23~";
               break;
             case 123:
-              c.key = e ? h.C0.ESC + "[24;" + (e + 1) + "~" : h.C0.ESC + "[24~";
+              c.key = e ? a.C0.ESC + "[24;" + (e + 1) + "~" : a.C0.ESC + "[24~";
               break;
             default:
               if (!d.ctrlKey || d.shiftKey || d.altKey || d.metaKey)
                 if (g && !v || !d.altKey || d.metaKey)
-                  !g || d.altKey || d.ctrlKey || d.shiftKey || !d.metaKey ? d.key && !d.ctrlKey && !d.altKey && !d.metaKey && d.keyCode >= 48 && d.key.length === 1 ? c.key = d.key : d.key && d.ctrlKey && (d.key === "_" && (c.key = h.C0.US), d.key === "@" && (c.key = h.C0.NUL)) : d.keyCode === 65 && (c.type = 1);
+                  !g || d.altKey || d.ctrlKey || d.shiftKey || !d.metaKey ? d.key && !d.ctrlKey && !d.altKey && !d.metaKey && d.keyCode >= 48 && d.key.length === 1 ? c.key = d.key : d.key && d.ctrlKey && (d.key === "_" && (c.key = a.C0.US), d.key === "@" && (c.key = a.C0.NUL)) : d.keyCode === 65 && (c.type = 1);
                 else {
                   const s = u[d.keyCode], n = s == null ? void 0 : s[d.shiftKey ? 1 : 0];
                   if (n)
-                    c.key = h.C0.ESC + n;
+                    c.key = a.C0.ESC + n;
                   else if (d.keyCode >= 65 && d.keyCode <= 90) {
                     const t = d.ctrlKey ? d.keyCode - 64 : d.keyCode + 32;
                     let r = String.fromCharCode(t);
-                    d.shiftKey && (r = r.toUpperCase()), c.key = h.C0.ESC + r;
+                    d.shiftKey && (r = r.toUpperCase()), c.key = a.C0.ESC + r;
                   } else if (d.keyCode === 32)
-                    c.key = h.C0.ESC + (d.ctrlKey ? h.C0.NUL : " ");
+                    c.key = a.C0.ESC + (d.ctrlKey ? a.C0.NUL : " ");
                   else if (d.key === "Dead" && d.code.startsWith("Key")) {
                     let t = d.code.slice(3, 4);
-                    d.shiftKey || (t = t.toLowerCase()), c.key = h.C0.ESC + t, c.cancel = !0;
+                    d.shiftKey || (t = t.toLowerCase()), c.key = a.C0.ESC + t, c.cancel = !0;
                   }
                 }
               else
-                d.keyCode >= 65 && d.keyCode <= 90 ? c.key = String.fromCharCode(d.keyCode - 64) : d.keyCode === 32 ? c.key = h.C0.NUL : d.keyCode >= 51 && d.keyCode <= 55 ? c.key = String.fromCharCode(d.keyCode - 51 + 27) : d.keyCode === 56 ? c.key = h.C0.DEL : d.keyCode === 219 ? c.key = h.C0.ESC : d.keyCode === 220 ? c.key = h.C0.FS : d.keyCode === 221 && (c.key = h.C0.GS);
+                d.keyCode >= 65 && d.keyCode <= 90 ? c.key = String.fromCharCode(d.keyCode - 64) : d.keyCode === 32 ? c.key = a.C0.NUL : d.keyCode >= 51 && d.keyCode <= 55 ? c.key = String.fromCharCode(d.keyCode - 51 + 27) : d.keyCode === 56 ? c.key = a.C0.DEL : d.keyCode === 219 ? c.key = a.C0.ESC : d.keyCode === 220 ? c.key = a.C0.FS : d.keyCode === 221 && (c.key = a.C0.GS);
           }
           return c;
         };
       }, 482: (T, i) => {
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.Utf8ToUtf32 = i.StringToUtf32 = i.utf32ToString = i.stringFromCodePoint = void 0, i.stringFromCodePoint = function(o) {
-          return o > 65535 ? (o -= 65536, String.fromCharCode(55296 + (o >> 10)) + String.fromCharCode(o % 1024 + 56320)) : String.fromCharCode(o);
-        }, i.utf32ToString = function(o, h = 0, u = o.length) {
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.Utf8ToUtf32 = i.StringToUtf32 = i.utf32ToString = i.stringFromCodePoint = void 0, i.stringFromCodePoint = function(h) {
+          return h > 65535 ? (h -= 65536, String.fromCharCode(55296 + (h >> 10)) + String.fromCharCode(h % 1024 + 56320)) : String.fromCharCode(h);
+        }, i.utf32ToString = function(h, a = 0, u = h.length) {
           let d = "";
-          for (let _ = h; _ < u; ++_) {
-            let g = o[_];
+          for (let _ = a; _ < u; ++_) {
+            let g = h[_];
             g > 65535 ? (g -= 65536, d += String.fromCharCode(55296 + (g >> 10)) + String.fromCharCode(g % 1024 + 56320)) : d += String.fromCharCode(g);
           }
           return d;
         }, i.StringToUtf32 = class {
           constructor() {
             this._interim = 0;
           }
           clear() {
             this._interim = 0;
           }
-          decode(o, h) {
-            const u = o.length;
+          decode(h, a) {
+            const u = h.length;
             if (!u)
               return 0;
             let d = 0, _ = 0;
             if (this._interim) {
-              const g = o.charCodeAt(_++);
-              56320 <= g && g <= 57343 ? h[d++] = 1024 * (this._interim - 55296) + g - 56320 + 65536 : (h[d++] = this._interim, h[d++] = g), this._interim = 0;
+              const g = h.charCodeAt(_++);
+              56320 <= g && g <= 57343 ? a[d++] = 1024 * (this._interim - 55296) + g - 56320 + 65536 : (a[d++] = this._interim, a[d++] = g), this._interim = 0;
             }
             for (let g = _; g < u; ++g) {
-              const v = o.charCodeAt(g);
+              const v = h.charCodeAt(g);
               if (55296 <= v && v <= 56319) {
                 if (++g >= u)
                   return this._interim = v, d;
-                const c = o.charCodeAt(g);
-                56320 <= c && c <= 57343 ? h[d++] = 1024 * (v - 55296) + c - 56320 + 65536 : (h[d++] = v, h[d++] = c);
+                const c = h.charCodeAt(g);
+                56320 <= c && c <= 57343 ? a[d++] = 1024 * (v - 55296) + c - 56320 + 65536 : (a[d++] = v, a[d++] = c);
               } else
-                v !== 65279 && (h[d++] = v);
+                v !== 65279 && (a[d++] = v);
             }
             return d;
           }
         }, i.Utf8ToUtf32 = class {
           constructor() {
             this.interim = new Uint8Array(3);
           }
           clear() {
             this.interim.fill(0);
           }
-          decode(o, h) {
-            const u = o.length;
+          decode(h, a) {
+            const u = h.length;
             if (!u)
               return 0;
             let d, _, g, v, c = 0, e = 0, s = 0;
             if (this.interim[0]) {
               let r = !1, l = this.interim[0];
               l &= (224 & l) == 192 ? 31 : (240 & l) == 224 ? 15 : 7;
               let f, m = 0;
               for (; (f = 63 & this.interim[++m]) && m < 4; )
                 l <<= 6, l |= f;
-              const a = (224 & this.interim[0]) == 192 ? 2 : (240 & this.interim[0]) == 224 ? 3 : 4, p = a - m;
+              const o = (224 & this.interim[0]) == 192 ? 2 : (240 & this.interim[0]) == 224 ? 3 : 4, p = o - m;
               for (; s < p; ) {
                 if (s >= u)
                   return 0;
-                if (f = o[s++], (192 & f) != 128) {
+                if (f = h[s++], (192 & f) != 128) {
                   s--, r = !0;
                   break;
                 }
                 this.interim[m++] = f, l <<= 6, l |= 63 & f;
               }
-              r || (a === 2 ? l < 128 ? s-- : h[c++] = l : a === 3 ? l < 2048 || l >= 55296 && l <= 57343 || l === 65279 || (h[c++] = l) : l < 65536 || l > 1114111 || (h[c++] = l)), this.interim.fill(0);
+              r || (o === 2 ? l < 128 ? s-- : a[c++] = l : o === 3 ? l < 2048 || l >= 55296 && l <= 57343 || l === 65279 || (a[c++] = l) : l < 65536 || l > 1114111 || (a[c++] = l)), this.interim.fill(0);
             }
             const n = u - 4;
             let t = s;
             for (; t < u; ) {
-              for (; !(!(t < n) || 128 & (d = o[t]) || 128 & (_ = o[t + 1]) || 128 & (g = o[t + 2]) || 128 & (v = o[t + 3])); )
-                h[c++] = d, h[c++] = _, h[c++] = g, h[c++] = v, t += 4;
-              if (d = o[t++], d < 128)
-                h[c++] = d;
+              for (; !(!(t < n) || 128 & (d = h[t]) || 128 & (_ = h[t + 1]) || 128 & (g = h[t + 2]) || 128 & (v = h[t + 3])); )
+                a[c++] = d, a[c++] = _, a[c++] = g, a[c++] = v, t += 4;
+              if (d = h[t++], d < 128)
+                a[c++] = d;
               else if ((224 & d) == 192) {
                 if (t >= u)
                   return this.interim[0] = d, c;
-                if (_ = o[t++], (192 & _) != 128) {
+                if (_ = h[t++], (192 & _) != 128) {
                   t--;
                   continue;
                 }
                 if (e = (31 & d) << 6 | 63 & _, e < 128) {
                   t--;
                   continue;
                 }
-                h[c++] = e;
+                a[c++] = e;
               } else if ((240 & d) == 224) {
                 if (t >= u)
                   return this.interim[0] = d, c;
-                if (_ = o[t++], (192 & _) != 128) {
+                if (_ = h[t++], (192 & _) != 128) {
                   t--;
                   continue;
                 }
                 if (t >= u)
                   return this.interim[0] = d, this.interim[1] = _, c;
-                if (g = o[t++], (192 & g) != 128) {
+                if (g = h[t++], (192 & g) != 128) {
                   t--;
                   continue;
                 }
                 if (e = (15 & d) << 12 | (63 & _) << 6 | 63 & g, e < 2048 || e >= 55296 && e <= 57343 || e === 65279)
                   continue;
-                h[c++] = e;
+                a[c++] = e;
               } else if ((248 & d) == 240) {
                 if (t >= u)
                   return this.interim[0] = d, c;
-                if (_ = o[t++], (192 & _) != 128) {
+                if (_ = h[t++], (192 & _) != 128) {
                   t--;
                   continue;
                 }
                 if (t >= u)
                   return this.interim[0] = d, this.interim[1] = _, c;
-                if (g = o[t++], (192 & g) != 128) {
+                if (g = h[t++], (192 & g) != 128) {
                   t--;
                   continue;
                 }
                 if (t >= u)
                   return this.interim[0] = d, this.interim[1] = _, this.interim[2] = g, c;
-                if (v = o[t++], (192 & v) != 128) {
+                if (v = h[t++], (192 & v) != 128) {
                   t--;
                   continue;
                 }
                 if (e = (7 & d) << 18 | (63 & _) << 12 | (63 & g) << 6 | 63 & v, e < 65536 || e > 1114111)
                   continue;
-                h[c++] = e;
+                a[c++] = e;
               }
             }
             return c;
           }
         };
       }, 225: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.UnicodeV6 = void 0;
-        const o = [[768, 879], [1155, 1158], [1160, 1161], [1425, 1469], [1471, 1471], [1473, 1474], [1476, 1477], [1479, 1479], [1536, 1539], [1552, 1557], [1611, 1630], [1648, 1648], [1750, 1764], [1767, 1768], [1770, 1773], [1807, 1807], [1809, 1809], [1840, 1866], [1958, 1968], [2027, 2035], [2305, 2306], [2364, 2364], [2369, 2376], [2381, 2381], [2385, 2388], [2402, 2403], [2433, 2433], [2492, 2492], [2497, 2500], [2509, 2509], [2530, 2531], [2561, 2562], [2620, 2620], [2625, 2626], [2631, 2632], [2635, 2637], [2672, 2673], [2689, 2690], [2748, 2748], [2753, 2757], [2759, 2760], [2765, 2765], [2786, 2787], [2817, 2817], [2876, 2876], [2879, 2879], [2881, 2883], [2893, 2893], [2902, 2902], [2946, 2946], [3008, 3008], [3021, 3021], [3134, 3136], [3142, 3144], [3146, 3149], [3157, 3158], [3260, 3260], [3263, 3263], [3270, 3270], [3276, 3277], [3298, 3299], [3393, 3395], [3405, 3405], [3530, 3530], [3538, 3540], [3542, 3542], [3633, 3633], [3636, 3642], [3655, 3662], [3761, 3761], [3764, 3769], [3771, 3772], [3784, 3789], [3864, 3865], [3893, 3893], [3895, 3895], [3897, 3897], [3953, 3966], [3968, 3972], [3974, 3975], [3984, 3991], [3993, 4028], [4038, 4038], [4141, 4144], [4146, 4146], [4150, 4151], [4153, 4153], [4184, 4185], [4448, 4607], [4959, 4959], [5906, 5908], [5938, 5940], [5970, 5971], [6002, 6003], [6068, 6069], [6071, 6077], [6086, 6086], [6089, 6099], [6109, 6109], [6155, 6157], [6313, 6313], [6432, 6434], [6439, 6440], [6450, 6450], [6457, 6459], [6679, 6680], [6912, 6915], [6964, 6964], [6966, 6970], [6972, 6972], [6978, 6978], [7019, 7027], [7616, 7626], [7678, 7679], [8203, 8207], [8234, 8238], [8288, 8291], [8298, 8303], [8400, 8431], [12330, 12335], [12441, 12442], [43014, 43014], [43019, 43019], [43045, 43046], [64286, 64286], [65024, 65039], [65056, 65059], [65279, 65279], [65529, 65531]], h = [[68097, 68099], [68101, 68102], [68108, 68111], [68152, 68154], [68159, 68159], [119143, 119145], [119155, 119170], [119173, 119179], [119210, 119213], [119362, 119364], [917505, 917505], [917536, 917631], [917760, 917999]];
+        const h = [[768, 879], [1155, 1158], [1160, 1161], [1425, 1469], [1471, 1471], [1473, 1474], [1476, 1477], [1479, 1479], [1536, 1539], [1552, 1557], [1611, 1630], [1648, 1648], [1750, 1764], [1767, 1768], [1770, 1773], [1807, 1807], [1809, 1809], [1840, 1866], [1958, 1968], [2027, 2035], [2305, 2306], [2364, 2364], [2369, 2376], [2381, 2381], [2385, 2388], [2402, 2403], [2433, 2433], [2492, 2492], [2497, 2500], [2509, 2509], [2530, 2531], [2561, 2562], [2620, 2620], [2625, 2626], [2631, 2632], [2635, 2637], [2672, 2673], [2689, 2690], [2748, 2748], [2753, 2757], [2759, 2760], [2765, 2765], [2786, 2787], [2817, 2817], [2876, 2876], [2879, 2879], [2881, 2883], [2893, 2893], [2902, 2902], [2946, 2946], [3008, 3008], [3021, 3021], [3134, 3136], [3142, 3144], [3146, 3149], [3157, 3158], [3260, 3260], [3263, 3263], [3270, 3270], [3276, 3277], [3298, 3299], [3393, 3395], [3405, 3405], [3530, 3530], [3538, 3540], [3542, 3542], [3633, 3633], [3636, 3642], [3655, 3662], [3761, 3761], [3764, 3769], [3771, 3772], [3784, 3789], [3864, 3865], [3893, 3893], [3895, 3895], [3897, 3897], [3953, 3966], [3968, 3972], [3974, 3975], [3984, 3991], [3993, 4028], [4038, 4038], [4141, 4144], [4146, 4146], [4150, 4151], [4153, 4153], [4184, 4185], [4448, 4607], [4959, 4959], [5906, 5908], [5938, 5940], [5970, 5971], [6002, 6003], [6068, 6069], [6071, 6077], [6086, 6086], [6089, 6099], [6109, 6109], [6155, 6157], [6313, 6313], [6432, 6434], [6439, 6440], [6450, 6450], [6457, 6459], [6679, 6680], [6912, 6915], [6964, 6964], [6966, 6970], [6972, 6972], [6978, 6978], [7019, 7027], [7616, 7626], [7678, 7679], [8203, 8207], [8234, 8238], [8288, 8291], [8298, 8303], [8400, 8431], [12330, 12335], [12441, 12442], [43014, 43014], [43019, 43019], [43045, 43046], [64286, 64286], [65024, 65039], [65056, 65059], [65279, 65279], [65529, 65531]], a = [[68097, 68099], [68101, 68102], [68108, 68111], [68152, 68154], [68159, 68159], [119143, 119145], [119155, 119170], [119173, 119179], [119210, 119213], [119362, 119364], [917505, 917505], [917536, 917631], [917760, 917999]];
         let u;
         i.UnicodeV6 = class {
           constructor() {
             if (this.version = "6", !u) {
               u = new Uint8Array(65536), u.fill(1), u[0] = 0, u.fill(0, 1, 32), u.fill(0, 127, 160), u.fill(2, 4352, 4448), u[9001] = 2, u[9002] = 2, u.fill(2, 11904, 42192), u[12351] = 1, u.fill(2, 44032, 55204), u.fill(2, 63744, 64256), u.fill(2, 65040, 65050), u.fill(2, 65072, 65136), u.fill(2, 65280, 65377), u.fill(2, 65504, 65511);
-              for (let d = 0; d < o.length; ++d)
-                u.fill(0, o[d][0], o[d][1] + 1);
+              for (let d = 0; d < h.length; ++d)
+                u.fill(0, h[d][0], h[d][1] + 1);
             }
           }
           wcwidth(d) {
             return d < 32 ? 0 : d < 127 ? 1 : d < 65536 ? u[d] : function(_, g) {
               let v, c = 0, e = g.length - 1;
               if (_ < g[0][0] || _ > g[e][1])
                 return !1;
@@ -4737,23 +4737,23 @@
                   c = v + 1;
                 else {
                   if (!(_ < g[v][0]))
                     return !0;
                   e = v - 1;
                 }
               return !1;
-            }(d, h) ? 0 : d >= 131072 && d <= 196605 || d >= 196608 && d <= 262141 ? 2 : 1;
+            }(d, a) ? 0 : d >= 131072 && d <= 196605 || d >= 196608 && d <= 262141 ? 2 : 1;
           }
         };
-      }, 5981: (T, i, o) => {
+      }, 5981: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.WriteBuffer = void 0;
-        const h = o(8460), u = o(844);
+        const a = h(8460), u = h(844);
         class d extends u.Disposable {
           constructor(g) {
-            super(), this._action = g, this._writeBuffer = [], this._callbacks = [], this._pendingData = 0, this._bufferOffset = 0, this._isSyncWriting = !1, this._syncCalls = 0, this._didUserInput = !1, this._onWriteParsed = this.register(new h.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event;
+            super(), this._action = g, this._writeBuffer = [], this._callbacks = [], this._pendingData = 0, this._bufferOffset = 0, this._isSyncWriting = !1, this._syncCalls = 0, this._didUserInput = !1, this._onWriteParsed = this.register(new a.EventEmitter()), this.onWriteParsed = this._onWriteParsed.event;
           }
           handleUserInput() {
             this._didUserInput = !0;
           }
           writeSync(g, v) {
             if (v !== void 0 && this._syncCalls > v)
               return void (this._syncCalls = 0);
@@ -4793,15 +4793,15 @@
             }
             this._writeBuffer.length > this._bufferOffset ? (this._bufferOffset > 50 && (this._writeBuffer = this._writeBuffer.slice(this._bufferOffset), this._callbacks = this._callbacks.slice(this._bufferOffset), this._bufferOffset = 0), setTimeout(() => this._innerWrite())) : (this._writeBuffer.length = 0, this._callbacks.length = 0, this._pendingData = 0, this._bufferOffset = 0), this._onWriteParsed.fire();
           }
         }
         i.WriteBuffer = d;
       }, 5941: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.toRgbString = i.parseColor = void 0;
-        const o = /^([\da-f])\/([\da-f])\/([\da-f])$|^([\da-f]{2})\/([\da-f]{2})\/([\da-f]{2})$|^([\da-f]{3})\/([\da-f]{3})\/([\da-f]{3})$|^([\da-f]{4})\/([\da-f]{4})\/([\da-f]{4})$/, h = /^[\da-f]+$/;
+        const h = /^([\da-f])\/([\da-f])\/([\da-f])$|^([\da-f]{2})\/([\da-f]{2})\/([\da-f]{2})$|^([\da-f]{3})\/([\da-f]{3})\/([\da-f]{3})$|^([\da-f]{4})\/([\da-f]{4})\/([\da-f]{4})$/, a = /^[\da-f]+$/;
         function u(d, _) {
           const g = d.toString(16), v = g.length < 2 ? "0" + g : g;
           switch (_) {
             case 4:
               return g[0];
             case 8:
               return v;
@@ -4813,36 +4813,36 @@
         }
         i.parseColor = function(d) {
           if (!d)
             return;
           let _ = d.toLowerCase();
           if (_.indexOf("rgb:") === 0) {
             _ = _.slice(4);
-            const g = o.exec(_);
+            const g = h.exec(_);
             if (g) {
               const v = g[1] ? 15 : g[4] ? 255 : g[7] ? 4095 : 65535;
               return [Math.round(parseInt(g[1] || g[4] || g[7] || g[10], 16) / v * 255), Math.round(parseInt(g[2] || g[5] || g[8] || g[11], 16) / v * 255), Math.round(parseInt(g[3] || g[6] || g[9] || g[12], 16) / v * 255)];
             }
-          } else if (_.indexOf("#") === 0 && (_ = _.slice(1), h.exec(_) && [3, 6, 9, 12].includes(_.length))) {
+          } else if (_.indexOf("#") === 0 && (_ = _.slice(1), a.exec(_) && [3, 6, 9, 12].includes(_.length))) {
             const g = _.length / 3, v = [0, 0, 0];
             for (let c = 0; c < 3; ++c) {
               const e = parseInt(_.slice(g * c, g * c + g), 16);
               v[c] = g === 1 ? e << 4 : g === 2 ? e : g === 3 ? e >> 4 : e >> 8;
             }
             return v;
           }
         }, i.toRgbString = function(d, _ = 16) {
           const [g, v, c] = d;
           return `rgb:${u(g, _)}/${u(v, _)}/${u(c, _)}`;
         };
       }, 5770: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.PAYLOAD_LIMIT = void 0, i.PAYLOAD_LIMIT = 1e7;
-      }, 6351: (T, i, o) => {
+      }, 6351: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.DcsHandler = i.DcsParser = void 0;
-        const h = o(482), u = o(8742), d = o(5770), _ = [];
+        const a = h(482), u = h(8742), d = h(5770), _ = [];
         i.DcsParser = class {
           constructor() {
             this._handlers = /* @__PURE__ */ Object.create(null), this._active = _, this._ident = 0, this._handlerFb = () => {
             }, this._stack = { paused: !1, loopPosition: 0, fallThrough: !1 };
           }
           dispose() {
             this._handlers = /* @__PURE__ */ Object.create(null), this._handlerFb = () => {
@@ -4876,15 +4876,15 @@
               this._handlerFb(this._ident, "HOOK", c);
           }
           put(v, c, e) {
             if (this._active.length)
               for (let s = this._active.length - 1; s >= 0; s--)
                 this._active[s].put(v, c, e);
             else
-              this._handlerFb(this._ident, "PUT", (0, h.utf32ToString)(v, c, e));
+              this._handlerFb(this._ident, "PUT", (0, a.utf32ToString)(v, c, e));
           }
           unhook(v, c = !0) {
             if (this._active.length) {
               let e = !1, s = this._active.length - 1, n = !1;
               if (this._stack.paused && (s = this._stack.loopPosition - 1, e = c, n = this._stack.fallThrough, this._stack.paused = !1), !n && e === !1) {
                 for (; s >= 0 && (e = this._active[s].unhook(v), e !== !0); s--)
                   if (e instanceof Promise)
@@ -4904,28 +4904,28 @@
           constructor(v) {
             this._handler = v, this._data = "", this._params = g, this._hitLimit = !1;
           }
           hook(v) {
             this._params = v.length > 1 || v.params[0] ? v.clone() : g, this._data = "", this._hitLimit = !1;
           }
           put(v, c, e) {
-            this._hitLimit || (this._data += (0, h.utf32ToString)(v, c, e), this._data.length > d.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
+            this._hitLimit || (this._data += (0, a.utf32ToString)(v, c, e), this._data.length > d.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
           }
           unhook(v) {
             let c = !1;
             if (this._hitLimit)
               c = !1;
             else if (v && (c = this._handler(this._data, this._params), c instanceof Promise))
               return c.then((e) => (this._params = g, this._data = "", this._hitLimit = !1, e));
             return this._params = g, this._data = "", this._hitLimit = !1, c;
           }
         };
-      }, 2015: (T, i, o) => {
+      }, 2015: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.EscapeSequenceParser = i.VT500_TRANSITION_TABLE = i.TransitionTable = void 0;
-        const h = o(844), u = o(8742), d = o(6242), _ = o(6351);
+        const a = h(844), u = h(8742), d = h(6242), _ = h(6351);
         class g {
           constructor(s) {
             this.table = new Uint8Array(s);
           }
           setDefault(s, n) {
             this.table.fill(s << 4 | n);
           }
@@ -4936,29 +4936,29 @@
             for (let l = 0; l < s.length; l++)
               this.table[n << 8 | s[l]] = t << 4 | r;
           }
         }
         i.TransitionTable = g;
         const v = 160;
         i.VT500_TRANSITION_TABLE = function() {
-          const e = new g(4095), s = Array.apply(null, Array(256)).map((m, a) => a), n = (m, a) => s.slice(m, a), t = n(32, 127), r = n(0, 24);
+          const e = new g(4095), s = Array.apply(null, Array(256)).map((m, o) => o), n = (m, o) => s.slice(m, o), t = n(32, 127), r = n(0, 24);
           r.push(25), r.push.apply(r, n(28, 32));
           const l = n(0, 14);
           let f;
           for (f in e.setDefault(1, 0), e.addMany(t, 0, 2, 0), l)
             e.addMany([24, 26, 153, 154], f, 3, 0), e.addMany(n(128, 144), f, 3, 0), e.addMany(n(144, 152), f, 3, 0), e.add(156, f, 0, 0), e.add(27, f, 11, 1), e.add(157, f, 4, 8), e.addMany([152, 158, 159], f, 0, 7), e.add(155, f, 11, 3), e.add(144, f, 11, 9);
           return e.addMany(r, 0, 3, 0), e.addMany(r, 1, 3, 1), e.add(127, 1, 0, 1), e.addMany(r, 8, 0, 8), e.addMany(r, 3, 3, 3), e.add(127, 3, 0, 3), e.addMany(r, 4, 3, 4), e.add(127, 4, 0, 4), e.addMany(r, 6, 3, 6), e.addMany(r, 5, 3, 5), e.add(127, 5, 0, 5), e.addMany(r, 2, 3, 2), e.add(127, 2, 0, 2), e.add(93, 1, 4, 8), e.addMany(t, 8, 5, 8), e.add(127, 8, 5, 8), e.addMany([156, 27, 24, 26, 7], 8, 6, 0), e.addMany(n(28, 32), 8, 0, 8), e.addMany([88, 94, 95], 1, 0, 7), e.addMany(t, 7, 0, 7), e.addMany(r, 7, 0, 7), e.add(156, 7, 0, 0), e.add(127, 7, 0, 7), e.add(91, 1, 11, 3), e.addMany(n(64, 127), 3, 7, 0), e.addMany(n(48, 60), 3, 8, 4), e.addMany([60, 61, 62, 63], 3, 9, 4), e.addMany(n(48, 60), 4, 8, 4), e.addMany(n(64, 127), 4, 7, 0), e.addMany([60, 61, 62, 63], 4, 0, 6), e.addMany(n(32, 64), 6, 0, 6), e.add(127, 6, 0, 6), e.addMany(n(64, 127), 6, 0, 0), e.addMany(n(32, 48), 3, 9, 5), e.addMany(n(32, 48), 5, 9, 5), e.addMany(n(48, 64), 5, 0, 6), e.addMany(n(64, 127), 5, 7, 0), e.addMany(n(32, 48), 4, 9, 5), e.addMany(n(32, 48), 1, 9, 2), e.addMany(n(32, 48), 2, 9, 2), e.addMany(n(48, 127), 2, 10, 0), e.addMany(n(48, 80), 1, 10, 0), e.addMany(n(81, 88), 1, 10, 0), e.addMany([89, 90, 92], 1, 10, 0), e.addMany(n(96, 127), 1, 10, 0), e.add(80, 1, 11, 9), e.addMany(r, 9, 0, 9), e.add(127, 9, 0, 9), e.addMany(n(28, 32), 9, 0, 9), e.addMany(n(32, 48), 9, 9, 12), e.addMany(n(48, 60), 9, 8, 10), e.addMany([60, 61, 62, 63], 9, 9, 10), e.addMany(r, 11, 0, 11), e.addMany(n(32, 128), 11, 0, 11), e.addMany(n(28, 32), 11, 0, 11), e.addMany(r, 10, 0, 10), e.add(127, 10, 0, 10), e.addMany(n(28, 32), 10, 0, 10), e.addMany(n(48, 60), 10, 8, 10), e.addMany([60, 61, 62, 63], 10, 0, 11), e.addMany(n(32, 48), 10, 9, 12), e.addMany(r, 12, 0, 12), e.add(127, 12, 0, 12), e.addMany(n(28, 32), 12, 0, 12), e.addMany(n(32, 48), 12, 9, 12), e.addMany(n(48, 64), 12, 0, 11), e.addMany(n(64, 127), 12, 12, 13), e.addMany(n(64, 127), 10, 12, 13), e.addMany(n(64, 127), 9, 12, 13), e.addMany(r, 13, 13, 13), e.addMany(t, 13, 13, 13), e.add(127, 13, 0, 13), e.addMany([27, 156, 24, 26], 13, 14, 0), e.add(v, 0, 2, 0), e.add(v, 8, 5, 8), e.add(v, 6, 0, 6), e.add(v, 11, 0, 11), e.add(v, 13, 13, 13), e;
         }();
-        class c extends h.Disposable {
+        class c extends a.Disposable {
           constructor(s = i.VT500_TRANSITION_TABLE) {
             super(), this._transitions = s, this._parseStack = { state: 0, handlers: [], handlerPos: 0, transition: 0, chunkPos: 0 }, this.initialState = 0, this.currentState = this.initialState, this._params = new u.Params(), this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0, this._printHandlerFb = (n, t, r) => {
             }, this._executeHandlerFb = (n) => {
             }, this._csiHandlerFb = (n, t) => {
             }, this._escHandlerFb = (n) => {
-            }, this._errorHandlerFb = (n) => n, this._printHandler = this._printHandlerFb, this._executeHandlers = /* @__PURE__ */ Object.create(null), this._csiHandlers = /* @__PURE__ */ Object.create(null), this._escHandlers = /* @__PURE__ */ Object.create(null), this.register((0, h.toDisposable)(() => {
+            }, this._errorHandlerFb = (n) => n, this._printHandler = this._printHandlerFb, this._executeHandlers = /* @__PURE__ */ Object.create(null), this._csiHandlers = /* @__PURE__ */ Object.create(null), this._escHandlers = /* @__PURE__ */ Object.create(null), this.register((0, a.toDisposable)(() => {
               this._csiHandlers = /* @__PURE__ */ Object.create(null), this._executeHandlers = /* @__PURE__ */ Object.create(null), this._escHandlers = /* @__PURE__ */ Object.create(null);
             })), this._oscParser = this.register(new d.OscParser()), this._dcsParser = this.register(new _.DcsParser()), this._errorHandler = this._errorHandlerFb, this.registerEscHandler({ final: "\\" }, () => !0);
           }
           _identifier(s, n = [64, 126]) {
             let t = 0;
             if (s.prefix) {
               if (s.prefix.length > 1)
@@ -5068,28 +5068,28 @@
             let r, l = 0, f = 0, m = 0;
             if (this._parseStack.state)
               if (this._parseStack.state === 2)
                 this._parseStack.state = 0, m = this._parseStack.chunkPos + 1;
               else {
                 if (t === void 0 || this._parseStack.state === 1)
                   throw this._parseStack.state = 1, new Error("improper continuation due to previous async handler, giving up parsing");
-                const a = this._parseStack.handlers;
+                const o = this._parseStack.handlers;
                 let p = this._parseStack.handlerPos - 1;
                 switch (this._parseStack.state) {
                   case 3:
                     if (t === !1 && p > -1) {
-                      for (; p >= 0 && (r = a[p](this._params), r !== !0); p--)
+                      for (; p >= 0 && (r = o[p](this._params), r !== !0); p--)
                         if (r instanceof Promise)
                           return this._parseStack.handlerPos = p, r;
                     }
                     this._parseStack.handlers = [];
                     break;
                   case 4:
                     if (t === !1 && p > -1) {
-                      for (; p >= 0 && (r = a[p](), r !== !0); p--)
+                      for (; p >= 0 && (r = o[p](), r !== !0); p--)
                         if (r instanceof Promise)
                           return this._parseStack.handlerPos = p, r;
                     }
                     this._parseStack.handlers = [];
                     break;
                   case 6:
                     if (l = s[this._parseStack.chunkPos], r = this._dcsParser.unhook(l !== 24 && l !== 26, t), r)
@@ -5099,120 +5099,120 @@
                   case 5:
                     if (l = s[this._parseStack.chunkPos], r = this._oscParser.end(l !== 24 && l !== 26, t), r)
                       return r;
                     l === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0;
                 }
                 this._parseStack.state = 0, m = this._parseStack.chunkPos + 1, this.precedingCodepoint = 0, this.currentState = 15 & this._parseStack.transition;
               }
-            for (let a = m; a < n; ++a) {
-              switch (l = s[a], f = this._transitions.table[this.currentState << 8 | (l < 160 ? l : v)], f >> 4) {
+            for (let o = m; o < n; ++o) {
+              switch (l = s[o], f = this._transitions.table[this.currentState << 8 | (l < 160 ? l : v)], f >> 4) {
                 case 2:
-                  for (let D = a + 1; ; ++D) {
+                  for (let D = o + 1; ; ++D) {
                     if (D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                      this._printHandler(s, a, D), a = D - 1;
+                      this._printHandler(s, o, D), o = D - 1;
                       break;
                     }
                     if (++D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                      this._printHandler(s, a, D), a = D - 1;
+                      this._printHandler(s, o, D), o = D - 1;
                       break;
                     }
                     if (++D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                      this._printHandler(s, a, D), a = D - 1;
+                      this._printHandler(s, o, D), o = D - 1;
                       break;
                     }
                     if (++D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                      this._printHandler(s, a, D), a = D - 1;
+                      this._printHandler(s, o, D), o = D - 1;
                       break;
                     }
                   }
                   break;
                 case 3:
                   this._executeHandlers[l] ? this._executeHandlers[l]() : this._executeHandlerFb(l), this.precedingCodepoint = 0;
                   break;
                 case 0:
                   break;
                 case 1:
-                  if (this._errorHandler({ position: a, code: l, currentState: this.currentState, collect: this._collect, params: this._params, abort: !1 }).abort)
+                  if (this._errorHandler({ position: o, code: l, currentState: this.currentState, collect: this._collect, params: this._params, abort: !1 }).abort)
                     return;
                   break;
                 case 7:
                   const p = this._csiHandlers[this._collect << 8 | l];
                   let C = p ? p.length - 1 : -1;
                   for (; C >= 0 && (r = p[C](this._params), r !== !0); C--)
                     if (r instanceof Promise)
-                      return this._preserveStack(3, p, C, f, a), r;
+                      return this._preserveStack(3, p, C, f, o), r;
                   C < 0 && this._csiHandlerFb(this._collect << 8 | l, this._params), this.precedingCodepoint = 0;
                   break;
                 case 8:
                   do
                     switch (l) {
                       case 59:
                         this._params.addParam(0);
                         break;
                       case 58:
                         this._params.addSubParam(-1);
                         break;
                       default:
                         this._params.addDigit(l - 48);
                     }
-                  while (++a < n && (l = s[a]) > 47 && l < 60);
-                  a--;
+                  while (++o < n && (l = s[o]) > 47 && l < 60);
+                  o--;
                   break;
                 case 9:
                   this._collect <<= 8, this._collect |= l;
                   break;
                 case 10:
                   const y = this._escHandlers[this._collect << 8 | l];
                   let w = y ? y.length - 1 : -1;
                   for (; w >= 0 && (r = y[w](), r !== !0); w--)
                     if (r instanceof Promise)
-                      return this._preserveStack(4, y, w, f, a), r;
+                      return this._preserveStack(4, y, w, f, o), r;
                   w < 0 && this._escHandlerFb(this._collect << 8 | l), this.precedingCodepoint = 0;
                   break;
                 case 11:
                   this._params.reset(), this._params.addParam(0), this._collect = 0;
                   break;
                 case 12:
                   this._dcsParser.hook(this._collect << 8 | l, this._params);
                   break;
                 case 13:
-                  for (let D = a + 1; ; ++D)
+                  for (let D = o + 1; ; ++D)
                     if (D >= n || (l = s[D]) === 24 || l === 26 || l === 27 || l > 127 && l < v) {
-                      this._dcsParser.put(s, a, D), a = D - 1;
+                      this._dcsParser.put(s, o, D), o = D - 1;
                       break;
                     }
                   break;
                 case 14:
                   if (r = this._dcsParser.unhook(l !== 24 && l !== 26), r)
-                    return this._preserveStack(6, [], 0, f, a), r;
+                    return this._preserveStack(6, [], 0, f, o), r;
                   l === 27 && (f |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0;
                   break;
                 case 4:
                   this._oscParser.start();
                   break;
                 case 5:
-                  for (let D = a + 1; ; D++)
+                  for (let D = o + 1; ; D++)
                     if (D >= n || (l = s[D]) < 32 || l > 127 && l < v) {
-                      this._oscParser.put(s, a, D), a = D - 1;
+                      this._oscParser.put(s, o, D), o = D - 1;
                       break;
                     }
                   break;
                 case 6:
                   if (r = this._oscParser.end(l !== 24 && l !== 26), r)
-                    return this._preserveStack(5, [], 0, f, a), r;
+                    return this._preserveStack(5, [], 0, f, o), r;
                   l === 27 && (f |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0;
               }
               this.currentState = 15 & f;
             }
           }
         }
         i.EscapeSequenceParser = c;
-      }, 6242: (T, i, o) => {
+      }, 6242: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.OscHandler = i.OscParser = void 0;
-        const h = o(5770), u = o(482), d = [];
+        const a = h(5770), u = h(482), d = [];
         i.OscParser = class {
           constructor() {
             this._state = 0, this._active = d, this._id = -1, this._handlers = /* @__PURE__ */ Object.create(null), this._handlerFb = () => {
             }, this._stack = { paused: !1, loopPosition: 0, fallThrough: !1 };
           }
           registerHandler(_, g) {
             this._handlers[_] === void 0 && (this._handlers[_] = []);
@@ -5294,50 +5294,50 @@
           constructor(_) {
             this._handler = _, this._data = "", this._hitLimit = !1;
           }
           start() {
             this._data = "", this._hitLimit = !1;
           }
           put(_, g, v) {
-            this._hitLimit || (this._data += (0, u.utf32ToString)(_, g, v), this._data.length > h.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
+            this._hitLimit || (this._data += (0, u.utf32ToString)(_, g, v), this._data.length > a.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0));
           }
           end(_) {
             let g = !1;
             if (this._hitLimit)
               g = !1;
             else if (_ && (g = this._handler(this._data), g instanceof Promise))
               return g.then((v) => (this._data = "", this._hitLimit = !1, v));
             return this._data = "", this._hitLimit = !1, g;
           }
         };
       }, 8742: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.Params = void 0;
-        const o = 2147483647;
-        class h {
+        const h = 2147483647;
+        class a {
           constructor(d = 32, _ = 32) {
             if (this.maxLength = d, this.maxSubParamsLength = _, _ > 256)
               throw new Error("maxSubParamsLength must not be greater than 256");
             this.params = new Int32Array(d), this.length = 0, this._subParams = new Int32Array(_), this._subParamsLength = 0, this._subParamsIdx = new Uint16Array(d), this._rejectDigits = !1, this._rejectSubDigits = !1, this._digitIsSub = !1;
           }
           static fromArray(d) {
-            const _ = new h();
+            const _ = new a();
             if (!d.length)
               return _;
             for (let g = Array.isArray(d[0]) ? 1 : 0; g < d.length; ++g) {
               const v = d[g];
               if (Array.isArray(v))
                 for (let c = 0; c < v.length; ++c)
                   _.addSubParam(v[c]);
               else
                 _.addParam(v);
             }
             return _;
           }
           clone() {
-            const d = new h(this.maxLength, this.maxSubParamsLength);
+            const d = new a(this.maxLength, this.maxSubParamsLength);
             return d.params.set(this.params), d.length = this.length, d._subParams.set(this._subParams), d._subParamsLength = this._subParamsLength, d._subParamsIdx.set(this._subParamsIdx), d._rejectDigits = this._rejectDigits, d._rejectSubDigits = this._rejectSubDigits, d._digitIsSub = this._digitIsSub, d;
           }
           toArray() {
             const d = [];
             for (let _ = 0; _ < this.length; ++_) {
               d.push(this.params[_]);
               const g = this._subParamsIdx[_] >> 8, v = 255 & this._subParamsIdx[_];
@@ -5350,25 +5350,25 @@
           }
           addParam(d) {
             if (this._digitIsSub = !1, this.length >= this.maxLength)
               this._rejectDigits = !0;
             else {
               if (d < -1)
                 throw new Error("values lesser than -1 are not allowed");
-              this._subParamsIdx[this.length] = this._subParamsLength << 8 | this._subParamsLength, this.params[this.length++] = d > o ? o : d;
+              this._subParamsIdx[this.length] = this._subParamsLength << 8 | this._subParamsLength, this.params[this.length++] = d > h ? h : d;
             }
           }
           addSubParam(d) {
             if (this._digitIsSub = !0, this.length)
               if (this._rejectDigits || this._subParamsLength >= this.maxSubParamsLength)
                 this._rejectSubDigits = !0;
               else {
                 if (d < -1)
                   throw new Error("values lesser than -1 are not allowed");
-                this._subParams[this._subParamsLength++] = d > o ? o : d, this._subParamsIdx[this.length - 1]++;
+                this._subParams[this._subParamsLength++] = d > h ? h : d, this._subParamsIdx[this.length - 1]++;
               }
           }
           hasSubParams(d) {
             return (255 & this._subParamsIdx[d]) - (this._subParamsIdx[d] >> 8) > 0;
           }
           getSubParams(d) {
             const _ = this._subParamsIdx[d] >> 8, g = 255 & this._subParamsIdx[d];
@@ -5383,48 +5383,48 @@
             return d;
           }
           addDigit(d) {
             let _;
             if (this._rejectDigits || !(_ = this._digitIsSub ? this._subParamsLength : this.length) || this._digitIsSub && this._rejectSubDigits)
               return;
             const g = this._digitIsSub ? this._subParams : this.params, v = g[_ - 1];
-            g[_ - 1] = ~v ? Math.min(10 * v + d, o) : d;
+            g[_ - 1] = ~v ? Math.min(10 * v + d, h) : d;
           }
         }
-        i.Params = h;
+        i.Params = a;
       }, 5741: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.AddonManager = void 0, i.AddonManager = class {
           constructor() {
             this._addons = [];
           }
           dispose() {
-            for (let o = this._addons.length - 1; o >= 0; o--)
-              this._addons[o].instance.dispose();
+            for (let h = this._addons.length - 1; h >= 0; h--)
+              this._addons[h].instance.dispose();
           }
-          loadAddon(o, h) {
-            const u = { instance: h, dispose: h.dispose, isDisposed: !1 };
-            this._addons.push(u), h.dispose = () => this._wrappedAddonDispose(u), h.activate(o);
+          loadAddon(h, a) {
+            const u = { instance: a, dispose: a.dispose, isDisposed: !1 };
+            this._addons.push(u), a.dispose = () => this._wrappedAddonDispose(u), a.activate(h);
           }
-          _wrappedAddonDispose(o) {
-            if (o.isDisposed)
+          _wrappedAddonDispose(h) {
+            if (h.isDisposed)
               return;
-            let h = -1;
+            let a = -1;
             for (let u = 0; u < this._addons.length; u++)
-              if (this._addons[u] === o) {
-                h = u;
+              if (this._addons[u] === h) {
+                a = u;
                 break;
               }
-            if (h === -1)
+            if (a === -1)
               throw new Error("Could not dispose an addon that has not been loaded");
-            o.isDisposed = !0, o.dispose.apply(o.instance), this._addons.splice(h, 1);
+            h.isDisposed = !0, h.dispose.apply(h.instance), this._addons.splice(a, 1);
           }
         };
-      }, 8771: (T, i, o) => {
+      }, 8771: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferApiView = void 0;
-        const h = o(3785), u = o(511);
+        const a = h(3785), u = h(511);
         i.BufferApiView = class {
           constructor(d, _) {
             this._buffer = d, this.type = _;
           }
           init(d) {
             return this._buffer = d, this;
           }
@@ -5442,47 +5442,47 @@
           }
           get length() {
             return this._buffer.lines.length;
           }
           getLine(d) {
             const _ = this._buffer.lines.get(d);
             if (_)
-              return new h.BufferLineApiView(_);
+              return new a.BufferLineApiView(_);
           }
           getNullCell() {
             return new u.CellData();
           }
         };
-      }, 3785: (T, i, o) => {
+      }, 3785: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferLineApiView = void 0;
-        const h = o(511);
+        const a = h(511);
         i.BufferLineApiView = class {
           constructor(u) {
             this._line = u;
           }
           get isWrapped() {
             return this._line.isWrapped;
           }
           get length() {
             return this._line.length;
           }
           getCell(u, d) {
             if (!(u < 0 || u >= this._line.length))
-              return d ? (this._line.loadCell(u, d), d) : this._line.loadCell(u, new h.CellData());
+              return d ? (this._line.loadCell(u, d), d) : this._line.loadCell(u, new a.CellData());
           }
           translateToString(u, d, _) {
             return this._line.translateToString(u, d, _);
           }
         };
-      }, 8285: (T, i, o) => {
+      }, 8285: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferNamespaceApi = void 0;
-        const h = o(8771), u = o(8460);
+        const a = h(8771), u = h(8460);
         i.BufferNamespaceApi = class {
           constructor(d) {
-            this._core = d, this._onBufferChange = new u.EventEmitter(), this.onBufferChange = this._onBufferChange.event, this._normal = new h.BufferApiView(this._core.buffers.normal, "normal"), this._alternate = new h.BufferApiView(this._core.buffers.alt, "alternate"), this._core.buffers.onBufferActivate(() => this._onBufferChange.fire(this.active));
+            this._core = d, this._onBufferChange = new u.EventEmitter(), this.onBufferChange = this._onBufferChange.event, this._normal = new a.BufferApiView(this._core.buffers.normal, "normal"), this._alternate = new a.BufferApiView(this._core.buffers.alt, "alternate"), this._core.buffers.onBufferActivate(() => this._onBufferChange.fire(this.active));
           }
           get active() {
             if (this._core.buffers.active === this._core.buffers.normal)
               return this.normal;
             if (this._core.buffers.active === this._core.buffers.alt)
               return this.alternate;
             throw new Error("Active buffer is neither normal nor alternate");
@@ -5492,76 +5492,76 @@
           }
           get alternate() {
             return this._alternate.init(this._core.buffers.alt);
           }
         };
       }, 7975: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.ParserApi = void 0, i.ParserApi = class {
-          constructor(o) {
-            this._core = o;
+          constructor(h) {
+            this._core = h;
           }
-          registerCsiHandler(o, h) {
-            return this._core.registerCsiHandler(o, (u) => h(u.toArray()));
+          registerCsiHandler(h, a) {
+            return this._core.registerCsiHandler(h, (u) => a(u.toArray()));
           }
-          addCsiHandler(o, h) {
-            return this.registerCsiHandler(o, h);
+          addCsiHandler(h, a) {
+            return this.registerCsiHandler(h, a);
           }
-          registerDcsHandler(o, h) {
-            return this._core.registerDcsHandler(o, (u, d) => h(u, d.toArray()));
+          registerDcsHandler(h, a) {
+            return this._core.registerDcsHandler(h, (u, d) => a(u, d.toArray()));
           }
-          addDcsHandler(o, h) {
-            return this.registerDcsHandler(o, h);
+          addDcsHandler(h, a) {
+            return this.registerDcsHandler(h, a);
           }
-          registerEscHandler(o, h) {
-            return this._core.registerEscHandler(o, h);
+          registerEscHandler(h, a) {
+            return this._core.registerEscHandler(h, a);
           }
-          addEscHandler(o, h) {
-            return this.registerEscHandler(o, h);
+          addEscHandler(h, a) {
+            return this.registerEscHandler(h, a);
           }
-          registerOscHandler(o, h) {
-            return this._core.registerOscHandler(o, h);
+          registerOscHandler(h, a) {
+            return this._core.registerOscHandler(h, a);
           }
-          addOscHandler(o, h) {
-            return this.registerOscHandler(o, h);
+          addOscHandler(h, a) {
+            return this.registerOscHandler(h, a);
           }
         };
       }, 7090: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.UnicodeApi = void 0, i.UnicodeApi = class {
-          constructor(o) {
-            this._core = o;
+          constructor(h) {
+            this._core = h;
           }
-          register(o) {
-            this._core.unicodeService.register(o);
+          register(h) {
+            this._core.unicodeService.register(h);
           }
           get versions() {
             return this._core.unicodeService.versions;
           }
           get activeVersion() {
             return this._core.unicodeService.activeVersion;
           }
-          set activeVersion(o) {
-            this._core.unicodeService.activeVersion = o;
+          set activeVersion(h) {
+            this._core.unicodeService.activeVersion = h;
           }
         };
-      }, 744: function(T, i, o) {
-        var h = this && this.__decorate || function(e, s, n, t) {
+      }, 744: function(T, i, h) {
+        var a = this && this.__decorate || function(e, s, n, t) {
           var r, l = arguments.length, f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             f = Reflect.decorate(e, s, n, t);
           else
             for (var m = e.length - 1; m >= 0; m--)
               (r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
           return l > 3 && f && Object.defineProperty(s, n, f), f;
         }, u = this && this.__param || function(e, s) {
           return function(n, t) {
             s(n, t, e);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.BufferService = i.MINIMUM_ROWS = i.MINIMUM_COLS = void 0;
-        const d = o(2585), _ = o(5295), g = o(8460), v = o(844);
+        const d = h(2585), _ = h(5295), g = h(8460), v = h(844);
         i.MINIMUM_COLS = 2, i.MINIMUM_ROWS = 1;
         let c = class extends v.Disposable {
           constructor(e) {
             super(), this.isUserScrolling = !1, this._onResize = this.register(new g.EventEmitter()), this.onResize = this._onResize.event, this._onScroll = this.register(new g.EventEmitter()), this.onScroll = this._onScroll.event, this.cols = Math.max(e.rawOptions.cols || 0, i.MINIMUM_COLS), this.rows = Math.max(e.rawOptions.rows || 0, i.MINIMUM_ROWS), this.buffers = this.register(new _.BufferSet(e, this));
           }
           get buffer() {
             return this.buffers.active;
@@ -5607,46 +5607,46 @@
             this.scrollLines(this.buffer.ybase - this.buffer.ydisp);
           }
           scrollToLine(e) {
             const s = e - this.buffer.ydisp;
             s !== 0 && this.scrollLines(s);
           }
         };
-        c = h([u(0, d.IOptionsService)], c), i.BufferService = c;
+        c = a([u(0, d.IOptionsService)], c), i.BufferService = c;
       }, 7994: (T, i) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CharsetService = void 0, i.CharsetService = class {
           constructor() {
             this.glevel = 0, this._charsets = [];
           }
           reset() {
             this.charset = void 0, this._charsets = [], this.glevel = 0;
           }
-          setgLevel(o) {
-            this.glevel = o, this.charset = this._charsets[o];
+          setgLevel(h) {
+            this.glevel = h, this.charset = this._charsets[h];
           }
-          setgCharset(o, h) {
-            this._charsets[o] = h, this.glevel === o && (this.charset = h);
+          setgCharset(h, a) {
+            this._charsets[h] = a, this.glevel === h && (this.charset = a);
           }
         };
-      }, 1753: function(T, i, o) {
-        var h = this && this.__decorate || function(t, r, l, f) {
-          var m, a = arguments.length, p = a < 3 ? r : f === null ? f = Object.getOwnPropertyDescriptor(r, l) : f;
+      }, 1753: function(T, i, h) {
+        var a = this && this.__decorate || function(t, r, l, f) {
+          var m, o = arguments.length, p = o < 3 ? r : f === null ? f = Object.getOwnPropertyDescriptor(r, l) : f;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             p = Reflect.decorate(t, r, l, f);
           else
             for (var C = t.length - 1; C >= 0; C--)
-              (m = t[C]) && (p = (a < 3 ? m(p) : a > 3 ? m(r, l, p) : m(r, l)) || p);
-          return a > 3 && p && Object.defineProperty(r, l, p), p;
+              (m = t[C]) && (p = (o < 3 ? m(p) : o > 3 ? m(r, l, p) : m(r, l)) || p);
+          return o > 3 && p && Object.defineProperty(r, l, p), p;
         }, u = this && this.__param || function(t, r) {
           return function(l, f) {
             r(l, f, t);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CoreMouseService = void 0;
-        const d = o(2585), _ = o(8460), g = o(844), v = { NONE: { events: 0, restrict: () => !1 }, X10: { events: 1, restrict: (t) => t.button !== 4 && t.action === 1 && (t.ctrl = !1, t.alt = !1, t.shift = !1, !0) }, VT200: { events: 19, restrict: (t) => t.action !== 32 }, DRAG: { events: 23, restrict: (t) => t.action !== 32 || t.button !== 3 }, ANY: { events: 31, restrict: (t) => !0 } };
+        const d = h(2585), _ = h(8460), g = h(844), v = { NONE: { events: 0, restrict: () => !1 }, X10: { events: 1, restrict: (t) => t.button !== 4 && t.action === 1 && (t.ctrl = !1, t.alt = !1, t.shift = !1, !0) }, VT200: { events: 19, restrict: (t) => t.action !== 32 }, DRAG: { events: 23, restrict: (t) => t.action !== 32 || t.button !== 3 }, ANY: { events: 31, restrict: (t) => !0 } };
         function c(t, r) {
           let l = (t.ctrl ? 16 : 0) | (t.shift ? 4 : 0) | (t.alt ? 8 : 0);
           return t.button === 4 ? (l |= 64, l |= t.action) : (l |= 3 & t.button, 4 & t.button && (l |= 64), 8 & t.button && (l |= 128), t.action === 32 ? l |= 32 : t.action !== 0 || r || (l |= 3)), l;
         }
         const e = String.fromCharCode, s = { DEFAULT: (t) => {
           const r = [c(t, !1) + 32, t.col + 32, t.row + 32];
           return r[0] > 255 || r[1] > 255 || r[2] > 255 ? "" : `\x1B[M${e(r[0])}${e(r[1])}${e(r[2])}`;
@@ -5708,31 +5708,31 @@
               if (t.x !== r.x || t.y !== r.y)
                 return !1;
             } else if (t.col !== r.col || t.row !== r.row)
               return !1;
             return t.button === r.button && t.action === r.action && t.ctrl === r.ctrl && t.alt === r.alt && t.shift === r.shift;
           }
         };
-        n = h([u(0, d.IBufferService), u(1, d.ICoreService)], n), i.CoreMouseService = n;
-      }, 6975: function(T, i, o) {
-        var h = this && this.__decorate || function(n, t, r, l) {
-          var f, m = arguments.length, a = m < 3 ? t : l === null ? l = Object.getOwnPropertyDescriptor(t, r) : l;
+        n = a([u(0, d.IBufferService), u(1, d.ICoreService)], n), i.CoreMouseService = n;
+      }, 6975: function(T, i, h) {
+        var a = this && this.__decorate || function(n, t, r, l) {
+          var f, m = arguments.length, o = m < 3 ? t : l === null ? l = Object.getOwnPropertyDescriptor(t, r) : l;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
-            a = Reflect.decorate(n, t, r, l);
+            o = Reflect.decorate(n, t, r, l);
           else
             for (var p = n.length - 1; p >= 0; p--)
-              (f = n[p]) && (a = (m < 3 ? f(a) : m > 3 ? f(t, r, a) : f(t, r)) || a);
-          return m > 3 && a && Object.defineProperty(t, r, a), a;
+              (f = n[p]) && (o = (m < 3 ? f(o) : m > 3 ? f(t, r, o) : f(t, r)) || o);
+          return m > 3 && o && Object.defineProperty(t, r, o), o;
         }, u = this && this.__param || function(n, t) {
           return function(r, l) {
             t(r, l, n);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.CoreService = void 0;
-        const d = o(2585), _ = o(8460), g = o(1439), v = o(844), c = Object.freeze({ insertMode: !1 }), e = Object.freeze({ applicationCursorKeys: !1, applicationKeypad: !1, bracketedPasteMode: !1, origin: !1, reverseWraparound: !1, sendFocus: !1, wraparound: !0 });
+        const d = h(2585), _ = h(8460), g = h(1439), v = h(844), c = Object.freeze({ insertMode: !1 }), e = Object.freeze({ applicationCursorKeys: !1, applicationKeypad: !1, bracketedPasteMode: !1, origin: !1, reverseWraparound: !1, sendFocus: !1, wraparound: !0 });
         let s = class extends v.Disposable {
           constructor(n, t, r) {
             super(), this._bufferService = n, this._logService = t, this._optionsService = r, this.isCursorInitialized = !1, this.isCursorHidden = !1, this._onData = this.register(new _.EventEmitter()), this.onData = this._onData.event, this._onUserInput = this.register(new _.EventEmitter()), this.onUserInput = this._onUserInput.event, this._onBinary = this.register(new _.EventEmitter()), this.onBinary = this._onBinary.event, this._onRequestScrollToBottom = this.register(new _.EventEmitter()), this.onRequestScrollToBottom = this._onRequestScrollToBottom.event, this.modes = (0, g.clone)(c), this.decPrivateModes = (0, g.clone)(e);
           }
           reset() {
             this.modes = (0, g.clone)(c), this.decPrivateModes = (0, g.clone)(e);
           }
@@ -5742,18 +5742,18 @@
             const r = this._bufferService.buffer;
             t && this._optionsService.rawOptions.scrollOnUserInput && r.ybase !== r.ydisp && this._onRequestScrollToBottom.fire(), t && this._onUserInput.fire(), this._logService.debug(`sending data "${n}"`, () => n.split("").map((l) => l.charCodeAt(0))), this._onData.fire(n);
           }
           triggerBinaryEvent(n) {
             this._optionsService.rawOptions.disableStdin || (this._logService.debug(`sending binary "${n}"`, () => n.split("").map((t) => t.charCodeAt(0))), this._onBinary.fire(n));
           }
         };
-        s = h([u(0, d.IBufferService), u(1, d.ILogService), u(2, d.IOptionsService)], s), i.CoreService = s;
-      }, 9074: (T, i, o) => {
+        s = a([u(0, d.IBufferService), u(1, d.ILogService), u(2, d.IOptionsService)], s), i.CoreService = s;
+      }, 9074: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.DecorationService = void 0;
-        const h = o(8055), u = o(8460), d = o(844), _ = o(6106);
+        const a = h(8055), u = h(8460), d = h(844), _ = h(6106);
         let g = 0, v = 0;
         class c extends d.Disposable {
           constructor() {
             super(), this._decorations = new _.SortedList((n) => n == null ? void 0 : n.marker.line), this._onDecorationRegistered = this.register(new u.EventEmitter()), this.onDecorationRegistered = this._onDecorationRegistered.event, this._onDecorationRemoved = this.register(new u.EventEmitter()), this.onDecorationRemoved = this._onDecorationRemoved.event, this.register((0, d.toDisposable)(() => {
               for (const n of this._decorations.values())
                 this._onDecorationRemoved.fire(n);
               this.reset();
@@ -5777,48 +5777,48 @@
           reset() {
             for (const n of this._decorations.values())
               n.dispose();
             this._decorations.clear();
           }
           *getDecorationsAtCell(n, t, r) {
             var l, f, m;
-            let a = 0, p = 0;
+            let o = 0, p = 0;
             for (const C of this._decorations.getKeyIterator(t))
-              a = (l = C.options.x) !== null && l !== void 0 ? l : 0, p = a + ((f = C.options.width) !== null && f !== void 0 ? f : 1), n >= a && n < p && (!r || ((m = C.options.layer) !== null && m !== void 0 ? m : "bottom") === r) && (yield C);
+              o = (l = C.options.x) !== null && l !== void 0 ? l : 0, p = o + ((f = C.options.width) !== null && f !== void 0 ? f : 1), n >= o && n < p && (!r || ((m = C.options.layer) !== null && m !== void 0 ? m : "bottom") === r) && (yield C);
           }
           forEachDecorationAtCell(n, t, r, l) {
             this._decorations.forEachByKey(t, (f) => {
-              var m, a, p;
-              g = (m = f.options.x) !== null && m !== void 0 ? m : 0, v = g + ((a = f.options.width) !== null && a !== void 0 ? a : 1), n >= g && n < v && (!r || ((p = f.options.layer) !== null && p !== void 0 ? p : "bottom") === r) && l(f);
+              var m, o, p;
+              g = (m = f.options.x) !== null && m !== void 0 ? m : 0, v = g + ((o = f.options.width) !== null && o !== void 0 ? o : 1), n >= g && n < v && (!r || ((p = f.options.layer) !== null && p !== void 0 ? p : "bottom") === r) && l(f);
             });
           }
           dispose() {
             for (const n of this._decorations.values())
               this._onDecorationRemoved.fire(n);
             this.reset();
           }
         }
         i.DecorationService = c;
         class e extends d.Disposable {
           constructor(n) {
             super(), this.options = n, this.isDisposed = !1, this.onRenderEmitter = this.register(new u.EventEmitter()), this.onRender = this.onRenderEmitter.event, this._onDispose = this.register(new u.EventEmitter()), this.onDispose = this._onDispose.event, this._cachedBg = null, this._cachedFg = null, this.marker = n.marker, this.options.overviewRulerOptions && !this.options.overviewRulerOptions.position && (this.options.overviewRulerOptions.position = "full");
           }
           get backgroundColorRGB() {
-            return this._cachedBg === null && (this.options.backgroundColor ? this._cachedBg = h.css.toColor(this.options.backgroundColor) : this._cachedBg = void 0), this._cachedBg;
+            return this._cachedBg === null && (this.options.backgroundColor ? this._cachedBg = a.css.toColor(this.options.backgroundColor) : this._cachedBg = void 0), this._cachedBg;
           }
           get foregroundColorRGB() {
-            return this._cachedFg === null && (this.options.foregroundColor ? this._cachedFg = h.css.toColor(this.options.foregroundColor) : this._cachedFg = void 0), this._cachedFg;
+            return this._cachedFg === null && (this.options.foregroundColor ? this._cachedFg = a.css.toColor(this.options.foregroundColor) : this._cachedFg = void 0), this._cachedFg;
           }
           dispose() {
             this._onDispose.fire(), super.dispose();
           }
         }
-      }, 4348: (T, i, o) => {
+      }, 4348: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.InstantiationService = i.ServiceCollection = void 0;
-        const h = o(2585), u = o(8343);
+        const a = h(2585), u = h(8343);
         class d {
           constructor(...g) {
             this._entries = /* @__PURE__ */ new Map();
             for (const [v, c] of g)
               this.set(v, c);
           }
           set(g, v) {
@@ -5834,15 +5834,15 @@
           }
           get(g) {
             return this._entries.get(g);
           }
         }
         i.ServiceCollection = d, i.InstantiationService = class {
           constructor() {
-            this._services = new d(), this._services.set(h.IInstantiationService, this);
+            this._services = new d(), this._services.set(a.IInstantiationService, this);
           }
           setService(_, g) {
             this._services.set(_, g);
           }
           getService(_) {
             return this._services.get(_);
           }
@@ -5856,30 +5856,30 @@
             }
             const e = v.length > 0 ? v[0].index : g.length;
             if (g.length !== e)
               throw new Error(`[createInstance] First service dependency of ${_.name} at position ${e + 1} conflicts with ${g.length} static arguments`);
             return new _(...g, ...c);
           }
         };
-      }, 7866: function(T, i, o) {
-        var h = this && this.__decorate || function(c, e, s, n) {
+      }, 7866: function(T, i, h) {
+        var a = this && this.__decorate || function(c, e, s, n) {
           var t, r = arguments.length, l = r < 3 ? e : n === null ? n = Object.getOwnPropertyDescriptor(e, s) : n;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             l = Reflect.decorate(c, e, s, n);
           else
             for (var f = c.length - 1; f >= 0; f--)
               (t = c[f]) && (l = (r < 3 ? t(l) : r > 3 ? t(e, s, l) : t(e, s)) || l);
           return r > 3 && l && Object.defineProperty(e, s, l), l;
         }, u = this && this.__param || function(c, e) {
           return function(s, n) {
             e(s, n, c);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.LogService = void 0;
-        const d = o(844), _ = o(2585), g = { debug: _.LogLevelEnum.DEBUG, info: _.LogLevelEnum.INFO, warn: _.LogLevelEnum.WARN, error: _.LogLevelEnum.ERROR, off: _.LogLevelEnum.OFF };
+        const d = h(844), _ = h(2585), g = { debug: _.LogLevelEnum.DEBUG, info: _.LogLevelEnum.INFO, warn: _.LogLevelEnum.WARN, error: _.LogLevelEnum.ERROR, off: _.LogLevelEnum.OFF };
         let v = class extends d.Disposable {
           constructor(c) {
             super(), this._optionsService = c, this.logLevel = _.LogLevelEnum.OFF, this._updateLogLevel(), this.register(this._optionsService.onSpecificOptionChange("logLevel", () => this._updateLogLevel()));
           }
           _updateLogLevel() {
             this.logLevel = g[this._optionsService.rawOptions.logLevel];
           }
@@ -5899,23 +5899,23 @@
           warn(c, ...e) {
             this.logLevel <= _.LogLevelEnum.WARN && this._log(console.warn, c, e);
           }
           error(c, ...e) {
             this.logLevel <= _.LogLevelEnum.ERROR && this._log(console.error, c, e);
           }
         };
-        v = h([u(0, _.IOptionsService)], v), i.LogService = v;
-      }, 7302: (T, i, o) => {
+        v = a([u(0, _.IOptionsService)], v), i.LogService = v;
+      }, 7302: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.OptionsService = i.DEFAULT_OPTIONS = void 0;
-        const h = o(8460), u = o(6114), d = o(844);
+        const a = h(8460), u = h(6114), d = h(844);
         i.DEFAULT_OPTIONS = { cols: 80, rows: 24, cursorBlink: !1, cursorStyle: "block", cursorWidth: 1, customGlyphs: !0, drawBoldTextInBrightColors: !0, fastScrollModifier: "alt", fastScrollSensitivity: 5, fontFamily: "courier-new, courier, monospace", fontSize: 15, fontWeight: "normal", fontWeightBold: "bold", lineHeight: 1, letterSpacing: 0, linkHandler: null, logLevel: "info", scrollback: 1e3, scrollOnUserInput: !0, scrollSensitivity: 1, screenReaderMode: !1, smoothScrollDuration: 0, macOptionIsMeta: !1, macOptionClickForcesSelection: !1, minimumContrastRatio: 1, disableStdin: !1, allowProposedApi: !1, allowTransparency: !1, tabStopWidth: 8, theme: {}, rightClickSelectsWord: u.isMac, windowOptions: {}, windowsMode: !1, wordSeparator: " ()[]{}',\"`", altClickMovesCursor: !0, convertEol: !1, termName: "xterm", cancelEvents: !1, overviewRulerWidth: 0 };
         const _ = ["normal", "bold", "100", "200", "300", "400", "500", "600", "700", "800", "900"];
         class g extends d.Disposable {
           constructor(c) {
-            super(), this._onOptionChange = this.register(new h.EventEmitter()), this.onOptionChange = this._onOptionChange.event;
+            super(), this._onOptionChange = this.register(new a.EventEmitter()), this.onOptionChange = this._onOptionChange.event;
             const e = Object.assign({}, i.DEFAULT_OPTIONS);
             for (const s in c)
               if (s in e)
                 try {
                   const n = c[s];
                   e[s] = this._sanitizeAndValidateOption(s, n);
                 } catch (n) {
@@ -5988,30 +5988,30 @@
                 if (!e && e !== 0)
                   throw new Error(`${c} must be numeric, value: ${e}`);
             }
             return e;
           }
         }
         i.OptionsService = g;
-      }, 2660: function(T, i, o) {
-        var h = this && this.__decorate || function(g, v, c, e) {
+      }, 2660: function(T, i, h) {
+        var a = this && this.__decorate || function(g, v, c, e) {
           var s, n = arguments.length, t = n < 3 ? v : e === null ? e = Object.getOwnPropertyDescriptor(v, c) : e;
           if (typeof Reflect == "object" && typeof Reflect.decorate == "function")
             t = Reflect.decorate(g, v, c, e);
           else
             for (var r = g.length - 1; r >= 0; r--)
               (s = g[r]) && (t = (n < 3 ? s(t) : n > 3 ? s(v, c, t) : s(v, c)) || t);
           return n > 3 && t && Object.defineProperty(v, c, t), t;
         }, u = this && this.__param || function(g, v) {
           return function(c, e) {
             v(c, e, g);
           };
         };
         Object.defineProperty(i, "__esModule", { value: !0 }), i.OscLinkService = void 0;
-        const d = o(2585);
+        const d = h(2585);
         let _ = class {
           constructor(g) {
             this._bufferService = g, this._nextId = 1, this._entriesWithId = /* @__PURE__ */ new Map(), this._dataByLinkId = /* @__PURE__ */ new Map();
           }
           registerLink(g) {
             const v = this._bufferService.buffer;
             if (g.id === void 0) {
@@ -6039,42 +6039,42 @@
             return `${g.id};;${g.uri}`;
           }
           _removeMarkerFromLink(g, v) {
             const c = g.lines.indexOf(v);
             c !== -1 && (g.lines.splice(c, 1), g.lines.length === 0 && (g.data.id !== void 0 && this._entriesWithId.delete(g.key), this._dataByLinkId.delete(g.id)));
           }
         };
-        _ = h([u(0, d.IBufferService)], _), i.OscLinkService = _;
+        _ = a([u(0, d.IBufferService)], _), i.OscLinkService = _;
       }, 8343: (T, i) => {
-        function o(h, u, d) {
-          u.di$target === u ? u.di$dependencies.push({ id: h, index: d }) : (u.di$dependencies = [{ id: h, index: d }], u.di$target = u);
+        function h(a, u, d) {
+          u.di$target === u ? u.di$dependencies.push({ id: a, index: d }) : (u.di$dependencies = [{ id: a, index: d }], u.di$target = u);
         }
-        Object.defineProperty(i, "__esModule", { value: !0 }), i.createDecorator = i.getServiceDependencies = i.serviceRegistry = void 0, i.serviceRegistry = /* @__PURE__ */ new Map(), i.getServiceDependencies = function(h) {
-          return h.di$dependencies || [];
-        }, i.createDecorator = function(h) {
-          if (i.serviceRegistry.has(h))
-            return i.serviceRegistry.get(h);
+        Object.defineProperty(i, "__esModule", { value: !0 }), i.createDecorator = i.getServiceDependencies = i.serviceRegistry = void 0, i.serviceRegistry = /* @__PURE__ */ new Map(), i.getServiceDependencies = function(a) {
+          return a.di$dependencies || [];
+        }, i.createDecorator = function(a) {
+          if (i.serviceRegistry.has(a))
+            return i.serviceRegistry.get(a);
           const u = function(d, _, g) {
             if (arguments.length !== 3)
               throw new Error("@IServiceName-decorator can only be used to decorate a parameter");
-            o(u, d, g);
+            h(u, d, g);
           };
-          return u.toString = () => h, i.serviceRegistry.set(h, u), u;
+          return u.toString = () => a, i.serviceRegistry.set(a, u), u;
         };
-      }, 2585: (T, i, o) => {
+      }, 2585: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.IDecorationService = i.IUnicodeService = i.IOscLinkService = i.IOptionsService = i.ILogService = i.LogLevelEnum = i.IInstantiationService = i.ICharsetService = i.ICoreService = i.ICoreMouseService = i.IBufferService = void 0;
-        const h = o(8343);
+        const a = h(8343);
         var u;
-        i.IBufferService = (0, h.createDecorator)("BufferService"), i.ICoreMouseService = (0, h.createDecorator)("CoreMouseService"), i.ICoreService = (0, h.createDecorator)("CoreService"), i.ICharsetService = (0, h.createDecorator)("CharsetService"), i.IInstantiationService = (0, h.createDecorator)("InstantiationService"), (u = i.LogLevelEnum || (i.LogLevelEnum = {}))[u.DEBUG = 0] = "DEBUG", u[u.INFO = 1] = "INFO", u[u.WARN = 2] = "WARN", u[u.ERROR = 3] = "ERROR", u[u.OFF = 4] = "OFF", i.ILogService = (0, h.createDecorator)("LogService"), i.IOptionsService = (0, h.createDecorator)("OptionsService"), i.IOscLinkService = (0, h.createDecorator)("OscLinkService"), i.IUnicodeService = (0, h.createDecorator)("UnicodeService"), i.IDecorationService = (0, h.createDecorator)("DecorationService");
-      }, 1480: (T, i, o) => {
+        i.IBufferService = (0, a.createDecorator)("BufferService"), i.ICoreMouseService = (0, a.createDecorator)("CoreMouseService"), i.ICoreService = (0, a.createDecorator)("CoreService"), i.ICharsetService = (0, a.createDecorator)("CharsetService"), i.IInstantiationService = (0, a.createDecorator)("InstantiationService"), (u = i.LogLevelEnum || (i.LogLevelEnum = {}))[u.DEBUG = 0] = "DEBUG", u[u.INFO = 1] = "INFO", u[u.WARN = 2] = "WARN", u[u.ERROR = 3] = "ERROR", u[u.OFF = 4] = "OFF", i.ILogService = (0, a.createDecorator)("LogService"), i.IOptionsService = (0, a.createDecorator)("OptionsService"), i.IOscLinkService = (0, a.createDecorator)("OscLinkService"), i.IUnicodeService = (0, a.createDecorator)("UnicodeService"), i.IDecorationService = (0, a.createDecorator)("DecorationService");
+      }, 1480: (T, i, h) => {
         Object.defineProperty(i, "__esModule", { value: !0 }), i.UnicodeService = void 0;
-        const h = o(8460), u = o(225);
+        const a = h(8460), u = h(225);
         i.UnicodeService = class {
           constructor() {
-            this._providers = /* @__PURE__ */ Object.create(null), this._active = "", this._onChange = new h.EventEmitter(), this.onChange = this._onChange.event;
+            this._providers = /* @__PURE__ */ Object.create(null), this._active = "", this._onChange = new a.EventEmitter(), this.onChange = this._onChange.event;
             const d = new u.UnicodeV6();
             this.register(d), this._active = d.version, this._activeProvider = d;
           }
           dispose() {
             this._onChange.dispose();
           }
           get versions() {
@@ -6111,22 +6111,22 @@
           }
         };
       } }, G = {};
       function W(T) {
         var i = G[T];
         if (i !== void 0)
           return i.exports;
-        var o = G[T] = { exports: {} };
-        return Z[T].call(o.exports, o, o.exports, W), o.exports;
+        var h = G[T] = { exports: {} };
+        return Z[T].call(h.exports, h, h.exports, W), h.exports;
       }
       var Y = {};
       return (() => {
         var T = Y;
         Object.defineProperty(T, "__esModule", { value: !0 }), T.Terminal = void 0;
-        const i = W(3236), o = W(9042), h = W(7975), u = W(7090), d = W(5741), _ = W(8285), g = ["cols", "rows"];
+        const i = W(3236), h = W(9042), a = W(7975), u = W(7090), d = W(5741), _ = W(8285), g = ["cols", "rows"];
         T.Terminal = class {
           constructor(v) {
             this._core = new i.Terminal(v), this._addonManager = new d.AddonManager(), this._publicOptions = Object.assign({}, this._core.options);
             const c = (s) => this._core.options[s], e = (s, n) => {
               this._checkReadonlyOptions(s), this._core.options[s] = n;
             };
             for (const s in this._core.options) {
@@ -6178,15 +6178,15 @@
           get onWriteParsed() {
             return this._core.onWriteParsed;
           }
           get element() {
             return this._core.element;
           }
           get parser() {
-            return this._parser || (this._parser = new h.ParserApi(this._core)), this._parser;
+            return this._parser || (this._parser = new a.ParserApi(this._core)), this._parser;
           }
           get unicode() {
             return this._checkProposedApi(), new u.UnicodeApi(this._core);
           }
           get textarea() {
             return this._core.textarea;
           }
@@ -6319,15 +6319,15 @@
           clearTextureAtlas() {
             this._core.clearTextureAtlas();
           }
           loadAddon(v) {
             return this._addonManager.loadAddon(this, v);
           }
           static get strings() {
-            return o;
+            return h;
           }
           _verifyIntegers(...v) {
             for (const c of v)
               if (c === 1 / 0 || isNaN(c) || c % 1 != 0)
                 throw new Error("This API only accepts integers");
           }
           _verifyPositiveIntegers(...v) {
@@ -6373,15 +6373,15 @@
           }
           proposeDimensions() {
             if (!this._terminal || !this._terminal.element || !this._terminal.element.parentElement)
               return;
             const W = this._terminal._core, Y = W._renderService.dimensions;
             if (Y.css.cell.width === 0 || Y.css.cell.height === 0)
               return;
-            const T = this._terminal.options.scrollback === 0 ? 0 : W.viewport.scrollBarWidth, i = window.getComputedStyle(this._terminal.element.parentElement), o = parseInt(i.getPropertyValue("height")), h = Math.max(0, parseInt(i.getPropertyValue("width"))), u = window.getComputedStyle(this._terminal.element), d = o - (parseInt(u.getPropertyValue("padding-top")) + parseInt(u.getPropertyValue("padding-bottom"))), _ = h - (parseInt(u.getPropertyValue("padding-right")) + parseInt(u.getPropertyValue("padding-left"))) - T;
+            const T = this._terminal.options.scrollback === 0 ? 0 : W.viewport.scrollBarWidth, i = window.getComputedStyle(this._terminal.element.parentElement), h = parseInt(i.getPropertyValue("height")), a = Math.max(0, parseInt(i.getPropertyValue("width"))), u = window.getComputedStyle(this._terminal.element), d = h - (parseInt(u.getPropertyValue("padding-top")) + parseInt(u.getPropertyValue("padding-bottom"))), _ = a - (parseInt(u.getPropertyValue("padding-right")) + parseInt(u.getPropertyValue("padding-left"))) - T;
             return { cols: Math.max(2, Math.floor(_ / Y.css.cell.width)), rows: Math.max(1, Math.floor(d / Y.css.cell.height)) };
           }
         };
       })(), Z;
     })();
   });
 })(he);
@@ -6423,114 +6423,117 @@
     "writeParsed",
     "resize",
     "scroll",
     "selectionChange",
     "titleChange"
   ],
   setup(X, { emit: J, expose: Z }) {
-    const G = re(null), W = new Q.Terminal(X.options), Y = new ee.FitAddon(), T = new ResizeObserver(() => {
+    const G = re(null), W = new Q.Terminal(X.options), Y = new ee.FitAddon();
+    function T() {
       Y.fit();
-    });
+    }
+    const i = new ResizeObserver(T);
     W.loadAddon(Y);
-    for (let o = 0; o < X.listen.length; o++) {
-      const h = X.listen[o], u = ce[h];
-      h === "selectionChange" ? W[u](
-        () => J(h, {
+    for (let a = 0; a < X.listen.length; a++) {
+      const u = X.listen[a], d = ce[u];
+      u === "selectionChange" ? W[d](
+        () => J(u, {
           hasSelection: W.hasSelection() ? 1 : 0,
           selection: W.getSelection(),
           position: W.getSelectionPosition()
         })
-      ) : u && W[u]((d) => J(h, d));
+      ) : d && W[d]((_) => J(u, _));
     }
-    const i = {
+    const h = {
+      fit: T,
       // Skipped: open, dispose, loadAddon, +Experimental
       blur() {
         return W.blur();
       },
       focus() {
         return W.focus();
       },
-      resize(o, h) {
-        return W.resize(o, h);
+      resize(a, u) {
+        return W.resize(a, u);
       },
-      attachCustomKeyEventHandler(o) {
-        return W.attachCustomKeyEventHandler(o);
+      attachCustomKeyEventHandler(a) {
+        return W.attachCustomKeyEventHandler(a);
       },
-      registerLinkProvider(o) {
-        return W.registerLinkProvider(o);
+      registerLinkProvider(a) {
+        return W.registerLinkProvider(a);
       },
-      registerMarker(o) {
-        return W.registerMarker(o);
+      registerMarker(a) {
+        return W.registerMarker(a);
       },
-      registerDecoration(o) {
-        return W.registerDecoration(o);
+      registerDecoration(a) {
+        return W.registerDecoration(a);
       },
       hasSelection() {
         return W.hasSelection();
       },
       getSelection() {
         return W.getSelection();
       },
       getSelectionPosition() {
         return W.getSelectionPosition();
       },
       clearSelection() {
         return W.clearSelection();
       },
-      select(o, h, u) {
-        return W.select(o, h, u);
+      select(a, u, d) {
+        return W.select(a, u, d);
       },
       selectAll() {
         return W.selectAll();
       },
-      selectLines(o, h) {
-        return W.selectLines(o, h);
+      selectLines(a, u) {
+        return W.selectLines(a, u);
       },
-      scrollLines(o) {
-        return W.scrollLines(o);
+      scrollLines(a) {
+        return W.scrollLines(a);
       },
-      scrollPages(o) {
-        return W.scrollPages(o);
+      scrollPages(a) {
+        return W.scrollPages(a);
       },
       scrollToTop() {
         return W.scrollToTop();
       },
       scrollToBottom() {
         return W.scrollToBottom();
       },
-      scrollToLine(o) {
-        return W.scrollToLine(o);
+      scrollToLine(a) {
+        return W.scrollToLine(a);
       },
       clear() {
         return W.clear();
       },
-      write(o, h) {
-        return W.write(o, h);
+      write(a, u) {
+        return W.write(a, u);
       },
-      writeln(o, h) {
-        return W.writeln(o, h);
+      writeln(a, u) {
+        return W.writeln(a, u);
       },
-      paste(o) {
-        return W.paste(o);
+      paste(a) {
+        return W.paste(a);
       },
-      refresh(o, h) {
-        return W.refresh(o, h);
+      refresh(a, u) {
+        return W.refresh(a, u);
       },
       clearTextureAtlas() {
         return W.clearTextureAtlas();
       },
       reset() {
         return W.reset();
       }
     };
     return ne(() => {
-      W.open(G.value), T.observe(G.value), J("opened");
+      W.open(G.value), i.observe(G.value), J("opened");
     }), oe(() => {
-      T.unobserve(G.value), W.dispose(), J("disposed");
-    }), Z(i), { ...i, elem: G };
+      i.unobserve(G.value), W.dispose(), J("disposed");
+    }), Z(h), { ...h, elem: G };
   },
   template: `<div style="position: relative; width: 100%; height: 100%;" v-bind="$attrs">
       <div ref="elem" style="position: absolute; width: 100%; height: 100%;"></div>
     </div>
     `
 }, te = {
   XTerm: le
```

### Comparing `trame-xterm-0.1.1/trame_xterm/module/serve/trame-xterm.umd.js` & `trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.umd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -14,25 +14,25 @@
         };
     (function(X, J) {
         (function(Z, G) {
             X.exports = G()
         })(self, function() {
             return (() => {
                 var Z = {
-                        4567: (T, i, o) => {
+                        4567: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.AccessibilityManager = void 0;
-                            const h = o(9042),
-                                u = o(6114),
-                                d = o(9924),
-                                _ = o(3656),
-                                g = o(844),
-                                v = o(5596),
-                                c = o(9631);
+                            const a = h(9042),
+                                u = h(6114),
+                                d = h(9924),
+                                _ = h(3656),
+                                g = h(844),
+                                v = h(5596),
+                                c = h(9631);
                             class e extends g.Disposable {
                                 constructor(n, t) {
                                     super(), this._terminal = n, this._renderService = t, this._liveRegionLineCount = 0, this._charsToConsume = [], this._charsToAnnounce = "", this._accessibilityTreeRoot = document.createElement("div"), this._accessibilityTreeRoot.classList.add("xterm-accessibility"), this._accessibilityTreeRoot.tabIndex = 0, this._rowContainer = document.createElement("div"), this._rowContainer.setAttribute("role", "list"), this._rowContainer.classList.add("xterm-accessibility-tree"), this._rowElements = [];
                                     for (let r = 0; r < this._terminal.rows; r++) this._rowElements[r] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[r]);
                                     if (this._topBoundaryFocusListener = r => this._handleBoundaryFocus(r, 0), this._bottomBoundaryFocusListener = r => this._handleBoundaryFocus(r, 1), this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._refreshRowsDimensions(), this._accessibilityTreeRoot.appendChild(this._rowContainer), this._renderRowsDebouncer = new d.TimeBasedDebouncer(this._renderRows.bind(this)), this._refreshRows(), this._liveRegion = document.createElement("div"), this._liveRegion.classList.add("live-region"), this._liveRegion.setAttribute("aria-live", "assertive"), this._accessibilityTreeRoot.appendChild(this._liveRegion), !this._terminal.element) throw new Error("Cannot enable accessibility before Terminal.open");
                                     this._terminal.element.insertAdjacentElement("afterbegin", this._accessibilityTreeRoot), this.register(this._renderRowsDebouncer), this.register(this._terminal.onResize(r => this._handleResize(r.rows))), this.register(this._terminal.onRender(r => this._refreshRows(r.start, r.end))), this.register(this._terminal.onScroll(() => this._refreshRows())), this.register(this._terminal.onA11yChar(r => this._handleChar(r))), this.register(this._terminal.onLineFeed(() => this._handleChar(`
 `))), this.register(this._terminal.onA11yTab(r => this._handleTab(r))), this.register(this._terminal.onKey(r => this._handleKey(r.key))), this.register(this._terminal.onBlur(() => this._clearLiveRegion())), this.register(this._renderService.onDimensionsChange(() => this._refreshRowsDimensions())), this._screenDprMonitor = new v.ScreenDprMonitor(window), this.register(this._screenDprMonitor), this._screenDprMonitor.setListener(() => this._refreshRowsDimensions()), this.register((0, _.addDisposableDomListener)(window, "resize", () => this._refreshRowsDimensions())), this.register((0, g.toDisposable)(() => {
@@ -41,19 +41,19 @@
                                 }
                                 _handleBoundaryFocus(n, t) {
                                     const r = n.target,
                                         l = this._rowElements[t === 0 ? 1 : this._rowElements.length - 2];
                                     if (r.getAttribute("aria-posinset") === (t === 0 ? "1" : `${this._terminal.buffer.lines.length}`) || n.relatedTarget !== l) return;
                                     let f, m;
                                     if (t === 0 ? (f = r, m = this._rowElements.pop(), this._rowContainer.removeChild(m)) : (f = this._rowElements.shift(), m = r, this._rowContainer.removeChild(f)), f.removeEventListener("focus", this._topBoundaryFocusListener), m.removeEventListener("focus", this._bottomBoundaryFocusListener), t === 0) {
-                                        const a = this._createAccessibilityTreeNode();
-                                        this._rowElements.unshift(a), this._rowContainer.insertAdjacentElement("afterbegin", a)
+                                        const o = this._createAccessibilityTreeNode();
+                                        this._rowElements.unshift(o), this._rowContainer.insertAdjacentElement("afterbegin", o)
                                     } else {
-                                        const a = this._createAccessibilityTreeNode();
-                                        this._rowElements.push(a), this._rowContainer.appendChild(a)
+                                        const o = this._createAccessibilityTreeNode();
+                                        this._rowElements.push(o), this._rowContainer.appendChild(o)
                                     }
                                     this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._terminal.scrollLines(t === 0 ? -1 : 1), this._rowElements[t === 0 ? 1 : this._rowElements.length - 2].focus(), n.preventDefault(), n.stopImmediatePropagation()
                                 }
                                 _handleResize(n) {
                                     this._rowElements[this._rowElements.length - 1].removeEventListener("focus", this._bottomBoundaryFocusListener);
                                     for (let t = this._rowContainer.children.length; t < this._terminal.rows; t++) this._rowElements[t] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[t]);
                                     for (; this._rowElements.length > n;) this._rowContainer.removeChild(this._rowElements.pop());
@@ -64,15 +64,15 @@
                                     return n.setAttribute("role", "listitem"), n.tabIndex = -1, this._refreshRowDimensions(n), n
                                 }
                                 _handleTab(n) {
                                     for (let t = 0; t < n; t++) this._handleChar(" ")
                                 }
                                 _handleChar(n) {
                                     this._liveRegionLineCount < 21 && (this._charsToConsume.length > 0 ? this._charsToConsume.shift() !== n && (this._charsToAnnounce += n) : this._charsToAnnounce += n, n === `
-` && (this._liveRegionLineCount++, this._liveRegionLineCount === 21 && (this._liveRegion.textContent += h.tooMuchOutput)), u.isMac && this._liveRegion.textContent && this._liveRegion.textContent.length > 0 && !this._liveRegion.parentNode && setTimeout(() => {
+` && (this._liveRegionLineCount++, this._liveRegionLineCount === 21 && (this._liveRegion.textContent += a.tooMuchOutput)), u.isMac && this._liveRegion.textContent && this._liveRegion.textContent.length > 0 && !this._liveRegion.parentNode && setTimeout(() => {
                                         this._accessibilityTreeRoot.appendChild(this._liveRegion)
                                     }, 0))
                                 }
                                 _clearLiveRegion() {
                                     this._liveRegion.textContent = "", this._liveRegionLineCount = 0, u.isMac && (0, c.removeElementFromParent)(this._liveRegion)
                                 }
                                 _handleKey(n) {
@@ -82,17 +82,17 @@
                                     this._renderRowsDebouncer.refresh(n, t, this._terminal.rows)
                                 }
                                 _renderRows(n, t) {
                                     const r = this._terminal.buffer,
                                         l = r.lines.length.toString();
                                     for (let f = n; f <= t; f++) {
                                         const m = r.translateBufferLineToString(r.ydisp + f, !0),
-                                            a = (r.ydisp + f + 1).toString(),
+                                            o = (r.ydisp + f + 1).toString(),
                                             p = this._rowElements[f];
-                                        p && (m.length === 0 ? p.innerText = " " : p.textContent = m, p.setAttribute("aria-posinset", a), p.setAttribute("aria-setsize", l))
+                                        p && (m.length === 0 ? p.innerText = " " : p.textContent = m, p.setAttribute("aria-posinset", o), p.setAttribute("aria-setsize", l))
                                     }
                                     this._announceCharacters()
                                 }
                                 _refreshRowsDimensions() {
                                     if (this._renderService.dimensions.css.cell.height) {
                                         this._accessibilityTreeRoot.style.width = `${this._renderService.dimensions.css.canvas.width}px`, this._rowElements.length !== this._terminal.rows && this._handleResize(this._terminal.rows);
                                         for (let n = 0; n < this._terminal.rows; n++) this._refreshRowDimensions(this._rowElements[n])
@@ -104,50 +104,50 @@
                                 _announceCharacters() {
                                     this._charsToAnnounce.length !== 0 && (this._liveRegion.textContent += this._charsToAnnounce, this._charsToAnnounce = "")
                                 }
                             }
                             i.AccessibilityManager = e
                         },
                         3614: (T, i) => {
-                            function o(_) {
+                            function h(_) {
                                 return _.replace(/\r?\n/g, "\r")
                             }
 
-                            function h(_, g) {
+                            function a(_, g) {
                                 return g ? "\x1B[200~" + _ + "\x1B[201~" : _
                             }
 
                             function u(_, g, v) {
-                                _ = h(_ = o(_), v.decPrivateModes.bracketedPasteMode), v.triggerDataEvent(_, !0), g.value = ""
+                                _ = a(_ = h(_), v.decPrivateModes.bracketedPasteMode), v.triggerDataEvent(_, !0), g.value = ""
                             }
 
                             function d(_, g, v) {
                                 const c = v.getBoundingClientRect(),
                                     e = _.clientX - c.left - 10,
                                     s = _.clientY - c.top - 10;
                                 g.style.width = "20px", g.style.height = "20px", g.style.left = `${e}px`, g.style.top = `${s}px`, g.style.zIndex = "1000", g.focus()
                             }
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.rightClickHandler = i.moveTextAreaUnderMouseCursor = i.paste = i.handlePasteEvent = i.copyHandler = i.bracketTextForPaste = i.prepareTextForTerminal = void 0, i.prepareTextForTerminal = o, i.bracketTextForPaste = h, i.copyHandler = function(_, g) {
+                            }), i.rightClickHandler = i.moveTextAreaUnderMouseCursor = i.paste = i.handlePasteEvent = i.copyHandler = i.bracketTextForPaste = i.prepareTextForTerminal = void 0, i.prepareTextForTerminal = h, i.bracketTextForPaste = a, i.copyHandler = function(_, g) {
                                 _.clipboardData && _.clipboardData.setData("text/plain", g.selectionText), _.preventDefault()
                             }, i.handlePasteEvent = function(_, g, v) {
                                 _.stopPropagation(), _.clipboardData && u(_.clipboardData.getData("text/plain"), g, v)
                             }, i.paste = u, i.moveTextAreaUnderMouseCursor = d, i.rightClickHandler = function(_, g, v, c, e) {
                                 d(_, g, v), e && c.rightClickSelect(_), g.value = c.selectionText, g.select()
                             }
                         },
-                        7239: (T, i, o) => {
+                        7239: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.ColorContrastCache = void 0;
-                            const h = o(1505);
+                            const a = h(1505);
                             i.ColorContrastCache = class {
                                 constructor() {
-                                    this._color = new h.TwoKeyMap, this._css = new h.TwoKeyMap
+                                    this._color = new a.TwoKeyMap, this._css = new a.TwoKeyMap
                                 }
                                 setCss(u, d, _) {
                                     this._css.set(u, d, _)
                                 }
                                 getCss(u, d) {
                                     return this._css.get(u, d)
                                 }
@@ -161,34 +161,34 @@
                                     this._color.clear(), this._css.clear()
                                 }
                             }
                         },
                         9631: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.removeElementFromParent = void 0, i.removeElementFromParent = function(...o) {
-                                var h;
-                                for (const u of o)(h = u == null ? void 0 : u.parentElement) === null || h === void 0 || h.removeChild(u)
+                            }), i.removeElementFromParent = void 0, i.removeElementFromParent = function(...h) {
+                                var a;
+                                for (const u of h)(a = u == null ? void 0 : u.parentElement) === null || a === void 0 || a.removeChild(u)
                             }
                         },
                         3656: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.addDisposableDomListener = void 0, i.addDisposableDomListener = function(o, h, u, d) {
-                                o.addEventListener(h, u, d);
+                            }), i.addDisposableDomListener = void 0, i.addDisposableDomListener = function(h, a, u, d) {
+                                h.addEventListener(a, u, d);
                                 let _ = !1;
                                 return {
                                     dispose: () => {
-                                        _ || (_ = !0, o.removeEventListener(h, u, d))
+                                        _ || (_ = !0, h.removeEventListener(a, u, d))
                                     }
                                 }
                             }
                         },
-                        6465: function(T, i, o) {
-                            var h = this && this.__decorate || function(e, s, n, t) {
+                        6465: function(T, i, h) {
+                            var a = this && this.__decorate || function(e, s, n, t) {
                                     var r, l = arguments.length,
                                         f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") f = Reflect.decorate(e, s, n, t);
                                     else
                                         for (var m = e.length - 1; m >= 0; m--)(r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
                                     return l > 3 && f && Object.defineProperty(s, n, f), f
                                 },
@@ -196,18 +196,18 @@
                                     return function(n, t) {
                                         s(n, t, e)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.Linkifier2 = void 0;
-                            const d = o(2585),
-                                _ = o(8460),
-                                g = o(844),
-                                v = o(3656);
+                            const d = h(2585),
+                                _ = h(8460),
+                                g = h(844),
+                                v = h(3656);
                             let c = class extends g.Disposable {
                                 constructor(e) {
                                     super(), this._bufferService = e, this._linkProviders = [], this._linkCacheDisposables = [], this._isMouseOut = !0, this._activeLine = -1, this._onShowLinkUnderline = this.register(new _.EventEmitter), this.onShowLinkUnderline = this._onShowLinkUnderline.event, this._onHideLinkUnderline = this.register(new _.EventEmitter), this.onHideLinkUnderline = this._onHideLinkUnderline.event, this.register((0, g.getDisposeArrayDisposable)(this._linkCacheDisposables)), this.register((0, g.toDisposable)(() => {
                                         this._lastMouseEvent = void 0
                                     }))
                                 }
                                 get currentLink() {
@@ -248,32 +248,32 @@
                                     this._activeProviderReplies && s || ((n = this._activeProviderReplies) === null || n === void 0 || n.forEach(l => {
                                         l == null || l.forEach(f => {
                                             f.link.dispose && f.link.dispose()
                                         })
                                     }), this._activeProviderReplies = new Map, this._activeLine = e.y);
                                     let r = !1;
                                     for (const [l, f] of this._linkProviders.entries()) s ? !((t = this._activeProviderReplies) === null || t === void 0) && t.get(l) && (r = this._checkLinkProviderResult(l, e, r)) : f.provideLinks(e.y, m => {
-                                        var a, p;
+                                        var o, p;
                                         if (this._isMouseOut) return;
                                         const C = m == null ? void 0 : m.map(y => ({
                                             link: y
                                         }));
-                                        (a = this._activeProviderReplies) === null || a === void 0 || a.set(l, C), r = this._checkLinkProviderResult(l, e, r), ((p = this._activeProviderReplies) === null || p === void 0 ? void 0 : p.size) === this._linkProviders.length && this._removeIntersectingLinks(e.y, this._activeProviderReplies)
+                                        (o = this._activeProviderReplies) === null || o === void 0 || o.set(l, C), r = this._checkLinkProviderResult(l, e, r), ((p = this._activeProviderReplies) === null || p === void 0 ? void 0 : p.size) === this._linkProviders.length && this._removeIntersectingLinks(e.y, this._activeProviderReplies)
                                     })
                                 }
                                 _removeIntersectingLinks(e, s) {
                                     const n = new Set;
                                     for (let t = 0; t < s.size; t++) {
                                         const r = s.get(t);
                                         if (r)
                                             for (let l = 0; l < r.length; l++) {
                                                 const f = r[l],
                                                     m = f.link.range.start.y < e ? 0 : f.link.range.start.x,
-                                                    a = f.link.range.end.y > e ? this._bufferService.cols : f.link.range.end.x;
-                                                for (let p = m; p <= a; p++) {
+                                                    o = f.link.range.end.y > e ? this._bufferService.cols : f.link.range.end.x;
+                                                for (let p = m; p <= o; p++) {
                                                     if (n.has(p)) {
                                                         r.splice(l--, 1);
                                                         break
                                                     }
                                                     n.add(p)
                                                 }
                                             }
@@ -287,15 +287,15 @@
                                     for (let f = 0; f < e; f++) this._activeProviderReplies.has(f) && !this._activeProviderReplies.get(f) || (l = !0);
                                     if (!l && r) {
                                         const f = r.find(m => this._linkAtPosition(m.link, s));
                                         f && (n = !0, this._handleNewLink(f))
                                     }
                                     if (this._activeProviderReplies.size === this._linkProviders.length && !n)
                                         for (let f = 0; f < this._activeProviderReplies.size; f++) {
-                                            const m = (t = this._activeProviderReplies.get(f)) === null || t === void 0 ? void 0 : t.find(a => this._linkAtPosition(a.link, s));
+                                            const m = (t = this._activeProviderReplies.get(f)) === null || t === void 0 ? void 0 : t.find(o => this._linkAtPosition(o.link, s));
                                             if (m) {
                                                 n = !0, this._handleNewLink(m);
                                                 break
                                             }
                                         }
                                     return n
                                 }
@@ -383,23 +383,23 @@
                                         x2: n,
                                         y2: t,
                                         cols: this._bufferService.cols,
                                         fg: r
                                     }
                                 }
                             };
-                            c = h([u(0, d.IBufferService)], c), i.Linkifier2 = c
+                            c = a([u(0, d.IBufferService)], c), i.Linkifier2 = c
                         },
                         9042: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.tooMuchOutput = i.promptLabel = void 0, i.promptLabel = "Terminal input", i.tooMuchOutput = "Too much output to announce, navigate to rows manually to read"
                         },
-                        3730: function(T, i, o) {
-                            var h = this && this.__decorate || function(c, e, s, n) {
+                        3730: function(T, i, h) {
+                            var a = this && this.__decorate || function(c, e, s, n) {
                                     var t, r = arguments.length,
                                         l = r < 3 ? e : n === null ? n = Object.getOwnPropertyDescriptor(e, s) : n;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") l = Reflect.decorate(c, e, s, n);
                                     else
                                         for (var f = c.length - 1; f >= 0; f--)(t = c[f]) && (l = (r < 3 ? t(l) : r > 3 ? t(e, s, l) : t(e, s)) || l);
                                     return r > 3 && l && Object.defineProperty(e, s, l), l
                                 },
@@ -407,46 +407,46 @@
                                     return function(s, n) {
                                         e(s, n, c)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.OscLinkProvider = void 0;
-                            const d = o(511),
-                                _ = o(2585);
+                            const d = h(511),
+                                _ = h(2585);
                             let g = class {
                                 constructor(c, e, s) {
                                     this._bufferService = c, this._optionsService = e, this._oscLinkService = s
                                 }
                                 provideLinks(c, e) {
                                     var s;
                                     const n = this._bufferService.buffer.lines.get(c - 1);
                                     if (!n) return void e(void 0);
                                     const t = [],
                                         r = this._optionsService.rawOptions.linkHandler,
                                         l = new d.CellData,
                                         f = n.getTrimmedLength();
                                     let m = -1,
-                                        a = -1,
+                                        o = -1,
                                         p = !1;
                                     for (let C = 0; C < f; C++)
-                                        if (a !== -1 || n.hasContent(C)) {
+                                        if (o !== -1 || n.hasContent(C)) {
                                             if (n.loadCell(C, l), l.hasExtendedAttrs() && l.extended.urlId) {
-                                                if (a === -1) {
-                                                    a = C, m = l.extended.urlId;
+                                                if (o === -1) {
+                                                    o = C, m = l.extended.urlId;
                                                     continue
                                                 }
                                                 p = l.extended.urlId !== m
-                                            } else a !== -1 && (p = !0);
-                                            if (p || a !== -1 && C === f - 1) {
+                                            } else o !== -1 && (p = !0);
+                                            if (p || o !== -1 && C === f - 1) {
                                                 const y = (s = this._oscLinkService.getLinkData(m)) === null || s === void 0 ? void 0 : s.uri;
                                                 if (y) {
                                                     const w = {
                                                         start: {
-                                                            x: a + 1,
+                                                            x: o + 1,
                                                             y: c
                                                         },
                                                         end: {
                                                             x: C + (p || C !== f - 1 ? 0 : 1),
                                                             y: c
                                                         }
                                                     };
@@ -467,15 +467,15 @@
                                                         },
                                                         leave: (x, I) => {
                                                             var H;
                                                             return (H = r == null ? void 0 : r.leave) === null || H === void 0 ? void 0 : H.call(r, x, I, w)
                                                         }
                                                     })
                                                 }
-                                                p = !1, l.hasExtendedAttrs() && l.extended.urlId ? (a = C, m = l.extended.urlId) : (a = -1, m = -1)
+                                                p = !1, l.hasExtendedAttrs() && l.extended.urlId ? (o = C, m = l.extended.urlId) : (o = -1, m = -1)
                                             }
                                         } e(t)
                                 }
                             };
 
                             function v(c, e) {
                                 if (confirm(`Do you want to navigate to ${e}?
@@ -486,52 +486,52 @@
                                         try {
                                             s.opener = null
                                         } catch {}
                                         s.location.href = e
                                     } else console.warn("Opening link blocked as opener could not be cleared")
                                 }
                             }
-                            g = h([u(0, _.IBufferService), u(1, _.IOptionsService), u(2, _.IOscLinkService)], g), i.OscLinkProvider = g
+                            g = a([u(0, _.IBufferService), u(1, _.IOptionsService), u(2, _.IOscLinkService)], g), i.OscLinkProvider = g
                         },
                         6193: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.RenderDebouncer = void 0, i.RenderDebouncer = class {
-                                constructor(o, h) {
-                                    this._parentWindow = o, this._renderCallback = h, this._refreshCallbacks = []
+                                constructor(h, a) {
+                                    this._parentWindow = h, this._renderCallback = a, this._refreshCallbacks = []
                                 }
                                 dispose() {
                                     this._animationFrame && (this._parentWindow.cancelAnimationFrame(this._animationFrame), this._animationFrame = void 0)
                                 }
-                                addRefreshCallback(o) {
-                                    return this._refreshCallbacks.push(o), this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh())), this._animationFrame
+                                addRefreshCallback(h) {
+                                    return this._refreshCallbacks.push(h), this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh())), this._animationFrame
                                 }
-                                refresh(o, h, u) {
-                                    this._rowCount = u, o = o !== void 0 ? o : 0, h = h !== void 0 ? h : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, o) : o, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, h) : h, this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh()))
+                                refresh(h, a, u) {
+                                    this._rowCount = u, h = h !== void 0 ? h : 0, a = a !== void 0 ? a : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, h) : h, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, a) : a, this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame(() => this._innerRefresh()))
                                 }
                                 _innerRefresh() {
                                     if (this._animationFrame = void 0, this._rowStart === void 0 || this._rowEnd === void 0 || this._rowCount === void 0) return void this._runRefreshCallbacks();
-                                    const o = Math.max(this._rowStart, 0),
-                                        h = Math.min(this._rowEnd, this._rowCount - 1);
-                                    this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(o, h), this._runRefreshCallbacks()
+                                    const h = Math.max(this._rowStart, 0),
+                                        a = Math.min(this._rowEnd, this._rowCount - 1);
+                                    this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(h, a), this._runRefreshCallbacks()
                                 }
                                 _runRefreshCallbacks() {
-                                    for (const o of this._refreshCallbacks) o(0);
+                                    for (const h of this._refreshCallbacks) h(0);
                                     this._refreshCallbacks = []
                                 }
                             }
                         },
-                        5596: (T, i, o) => {
+                        5596: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.ScreenDprMonitor = void 0;
-                            const h = o(844);
-                            class u extends h.Disposable {
+                            const a = h(844);
+                            class u extends a.Disposable {
                                 constructor(_) {
-                                    super(), this._parentWindow = _, this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this.register((0, h.toDisposable)(() => {
+                                    super(), this._parentWindow = _, this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this.register((0, a.toDisposable)(() => {
                                         this.clearListener()
                                     }))
                                 }
                                 setListener(_) {
                                     this._listener && this.clearListener(), this._listener = _, this._outerListener = () => {
                                         this._listener && (this._listener(this._parentWindow.devicePixelRatio, this._currentDevicePixelRatio), this._updateDpr())
                                     }, this._updateDpr()
@@ -542,49 +542,49 @@
                                 }
                                 clearListener() {
                                     this._resolutionMediaMatchList && this._listener && this._outerListener && (this._resolutionMediaMatchList.removeListener(this._outerListener), this._resolutionMediaMatchList = void 0, this._listener = void 0, this._outerListener = void 0)
                                 }
                             }
                             i.ScreenDprMonitor = u
                         },
-                        3236: (T, i, o) => {
+                        3236: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.Terminal = void 0;
-                            const h = o(2950),
-                                u = o(1680),
-                                d = o(3614),
-                                _ = o(2584),
-                                g = o(5435),
-                                v = o(9312),
-                                c = o(6114),
-                                e = o(3656),
-                                s = o(9042),
-                                n = o(4567),
-                                t = o(1296),
-                                r = o(7399),
-                                l = o(8460),
-                                f = o(8437),
-                                m = o(3230),
-                                a = o(4725),
-                                p = o(428),
-                                C = o(8934),
-                                y = o(6465),
-                                w = o(5114),
-                                D = o(8969),
-                                x = o(8055),
-                                I = o(4269),
-                                H = o(5941),
-                                S = o(3107),
-                                b = o(5744),
-                                L = o(9074),
-                                R = o(2585),
-                                M = o(3730),
-                                F = o(844),
-                                j = o(6731),
+                            const a = h(2950),
+                                u = h(1680),
+                                d = h(3614),
+                                _ = h(2584),
+                                g = h(5435),
+                                v = h(9312),
+                                c = h(6114),
+                                e = h(3656),
+                                s = h(9042),
+                                n = h(4567),
+                                t = h(1296),
+                                r = h(7399),
+                                l = h(8460),
+                                f = h(8437),
+                                m = h(3230),
+                                o = h(4725),
+                                p = h(428),
+                                C = h(8934),
+                                y = h(6465),
+                                w = h(5114),
+                                D = h(8969),
+                                x = h(8055),
+                                I = h(4269),
+                                H = h(5941),
+                                S = h(3107),
+                                b = h(5744),
+                                L = h(9074),
+                                R = h(2585),
+                                M = h(3730),
+                                F = h(844),
+                                j = h(6731),
                                 O = typeof window < "u" ? window.document : null;
                             class N extends D.CoreTerminal {
                                 constructor(E = {}) {
                                     super(E), this.browser = c, this._keyDownHandled = !1, this._keyDownSeen = !1, this._keyPressHandled = !1, this._unprocessedDeadKey = !1, this._onCursorMove = this.register(new l.EventEmitter), this.onCursorMove = this._onCursorMove.event, this._onKey = this.register(new l.EventEmitter), this.onKey = this._onKey.event, this._onRender = this.register(new l.EventEmitter), this.onRender = this._onRender.event, this._onSelectionChange = this.register(new l.EventEmitter), this.onSelectionChange = this._onSelectionChange.event, this._onTitleChange = this.register(new l.EventEmitter), this.onTitleChange = this._onTitleChange.event, this._onBell = this.register(new l.EventEmitter), this.onBell = this._onBell.event, this._onFocus = this.register(new l.EventEmitter), this._onBlur = this.register(new l.EventEmitter), this._onA11yCharEmitter = this.register(new l.EventEmitter), this._onA11yTabEmitter = this.register(new l.EventEmitter), this._onWillOpen = this.register(new l.EventEmitter), this._setup(), this.linkifier2 = this.register(this._instantiationService.createInstance(y.Linkifier2)), this.linkifier2.registerLinkProvider(this._instantiationService.createInstance(M.OscLinkProvider)), this._decorationService = this._instantiationService.createInstance(L.DecorationService), this._instantiationService.setService(R.IDecorationService, this._decorationService), this.register(this._inputHandler.onRequestBell(() => this._onBell.fire())), this.register(this._inputHandler.onRequestRefreshRows((A, B) => this.refresh(A, B))), this.register(this._inputHandler.onRequestSendFocus(() => this._reportFocus())), this.register(this._inputHandler.onRequestReset(() => this.reset())), this.register(this._inputHandler.onRequestWindowsOptionsReport(A => this._reportWindowsOptions(A))), this.register(this._inputHandler.onColor(A => this._handleColorEvent(A))), this.register((0, l.forwardEvent)(this._inputHandler.onCursorMove, this._onCursorMove)), this.register((0, l.forwardEvent)(this._inputHandler.onTitleChange, this._onTitleChange)), this.register((0, l.forwardEvent)(this._inputHandler.onA11yChar, this._onA11yCharEmitter)), this.register((0, l.forwardEvent)(this._inputHandler.onA11yTab, this._onA11yTabEmitter)), this.register(this._bufferService.onResize(A => this._afterResize(A.cols, A.rows))), this.register((0, F.toDisposable)(() => {
                                         var A, B;
                                         this._customKeyEventHandler = void 0, (B = (A = this.element) === null || A === void 0 ? void 0 : A.parentNode) === null || B === void 0 || B.removeChild(this.element)
                                     }))
@@ -693,21 +693,21 @@
                                     this.register((0, e.addDisposableDomListener)(this.textarea, "keyup", E => this._keyUp(E), !0)), this.register((0, e.addDisposableDomListener)(this.textarea, "keydown", E => this._keyDown(E), !0)), this.register((0, e.addDisposableDomListener)(this.textarea, "keypress", E => this._keyPress(E), !0)), this.register((0, e.addDisposableDomListener)(this.textarea, "compositionstart", () => this._compositionHelper.compositionstart())), this.register((0, e.addDisposableDomListener)(this.textarea, "compositionupdate", E => this._compositionHelper.compositionupdate(E))), this.register((0, e.addDisposableDomListener)(this.textarea, "compositionend", () => this._compositionHelper.compositionend())), this.register((0, e.addDisposableDomListener)(this.textarea, "input", E => this._inputEvent(E), !0)), this.register(this.onRender(() => this._compositionHelper.updateCompositionElements()))
                                 }
                                 open(E) {
                                     var A;
                                     if (!E) throw new Error("Terminal requires a parent element.");
                                     E.isConnected || this._logService.debug("Terminal.open was called on an element that was not attached to the DOM"), this._document = E.ownerDocument, this.element = this._document.createElement("div"), this.element.dir = "ltr", this.element.classList.add("terminal"), this.element.classList.add("xterm"), this.element.setAttribute("tabindex", "0"), E.appendChild(this.element);
                                     const B = O.createDocumentFragment();
-                                    this._viewportElement = O.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), B.appendChild(this._viewportElement), this._viewportScrollArea = O.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = O.createElement("div"), this.screenElement.classList.add("xterm-screen"), this._helperContainer = O.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), B.appendChild(this.screenElement), this.textarea = O.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", s.promptLabel), c.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this._instantiationService.createInstance(w.CoreBrowserService, this.textarea, (A = this._document.defaultView) !== null && A !== void 0 ? A : window), this._instantiationService.setService(a.ICoreBrowserService, this._coreBrowserService), this.register((0, e.addDisposableDomListener)(this.textarea, "focus", P => this._handleTextAreaFocus(P))), this.register((0, e.addDisposableDomListener)(this.textarea, "blur", () => this._handleTextAreaBlur())), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(p.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(a.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance(j.ThemeService), this._instantiationService.setService(a.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(I.CharacterJoinerService), this._instantiationService.setService(a.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(m.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(a.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange(P => this._onRender.fire(P))), this.onResize(P => this._renderService.resize(P.cols, P.rows)), this._compositionView = O.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(h.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this.element.appendChild(B);
+                                    this._viewportElement = O.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), B.appendChild(this._viewportElement), this._viewportScrollArea = O.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = O.createElement("div"), this.screenElement.classList.add("xterm-screen"), this._helperContainer = O.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), B.appendChild(this.screenElement), this.textarea = O.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", s.promptLabel), c.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this._instantiationService.createInstance(w.CoreBrowserService, this.textarea, (A = this._document.defaultView) !== null && A !== void 0 ? A : window), this._instantiationService.setService(o.ICoreBrowserService, this._coreBrowserService), this.register((0, e.addDisposableDomListener)(this.textarea, "focus", P => this._handleTextAreaFocus(P))), this.register((0, e.addDisposableDomListener)(this.textarea, "blur", () => this._handleTextAreaBlur())), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(p.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(o.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance(j.ThemeService), this._instantiationService.setService(o.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(I.CharacterJoinerService), this._instantiationService.setService(o.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(m.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(o.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange(P => this._onRender.fire(P))), this.onResize(P => this._renderService.resize(P.cols, P.rows)), this._compositionView = O.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(a.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this.element.appendChild(B);
                                     try {
                                         this._onWillOpen.fire(this.element)
                                     } catch {}
-                                    this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this._mouseService = this._instantiationService.createInstance(C.MouseService), this._instantiationService.setService(a.IMouseService, this._mouseService), this.viewport = this._instantiationService.createInstance(u.Viewport, P => this.scrollLines(P, !0, 1), this._viewportElement, this._viewportScrollArea), this.register(this._inputHandler.onRequestSyncScrollBar(() => this.viewport.syncScrollArea())), this.register(this.viewport), this.register(this.onCursorMove(() => {
+                                    this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this._mouseService = this._instantiationService.createInstance(C.MouseService), this._instantiationService.setService(o.IMouseService, this._mouseService), this.viewport = this._instantiationService.createInstance(u.Viewport, P => this.scrollLines(P, !0, 1), this._viewportElement, this._viewportScrollArea), this.register(this._inputHandler.onRequestSyncScrollBar(() => this.viewport.syncScrollArea())), this.register(this.viewport), this.register(this.onCursorMove(() => {
                                         this._renderService.handleCursorMove(), this._syncTextArea()
-                                    })), this.register(this.onResize(() => this._renderService.handleResize(this.cols, this.rows))), this.register(this.onBlur(() => this._renderService.handleBlur())), this.register(this.onFocus(() => this._renderService.handleFocus())), this.register(this._renderService.onDimensionsChange(() => this.viewport.syncScrollArea())), this._selectionService = this.register(this._instantiationService.createInstance(v.SelectionService, this.element, this.screenElement, this.linkifier2)), this._instantiationService.setService(a.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines(P => this.scrollLines(P.amount, P.suppressScrollEvent))), this.register(this._selectionService.onSelectionChange(() => this._onSelectionChange.fire())), this.register(this._selectionService.onRequestRedraw(P => this._renderService.handleSelectionChanged(P.start, P.end, P.columnSelectMode))), this.register(this._selectionService.onLinuxMouseSelection(P => {
+                                    })), this.register(this.onResize(() => this._renderService.handleResize(this.cols, this.rows))), this.register(this.onBlur(() => this._renderService.handleBlur())), this.register(this.onFocus(() => this._renderService.handleFocus())), this.register(this._renderService.onDimensionsChange(() => this.viewport.syncScrollArea())), this._selectionService = this.register(this._instantiationService.createInstance(v.SelectionService, this.element, this.screenElement, this.linkifier2)), this._instantiationService.setService(o.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines(P => this.scrollLines(P.amount, P.suppressScrollEvent))), this.register(this._selectionService.onSelectionChange(() => this._onSelectionChange.fire())), this.register(this._selectionService.onRequestRedraw(P => this._renderService.handleSelectionChanged(P.start, P.end, P.columnSelectMode))), this.register(this._selectionService.onLinuxMouseSelection(P => {
                                         this.textarea.value = P, this.textarea.focus(), this.textarea.select()
                                     })), this.register(this._onScroll.event(P => {
                                         this.viewport.syncScrollArea(), this._selectionService.refresh()
                                     })), this.register((0, e.addDisposableDomListener)(this._viewportElement, "scroll", () => this._selectionService.refresh())), this.linkifier2.attachToDom(this.screenElement, this._mouseService, this._renderService), this.register(this._instantiationService.createInstance(S.BufferDecorationRenderer, this.screenElement)), this.register((0, e.addDisposableDomListener)(this.element, "mousedown", P => this._selectionService.handleMouseDown(P))), this.coreMouseService.areMouseEventsActive ? (this._selectionService.disable(), this.element.classList.add("enable-mouse-events")) : this._selectionService.enable(), this.options.screenReaderMode && (this._accessibilityManager = new n.AccessibilityManager(this, this._renderService)), this.register(this.optionsService.onSpecificOptionChange("screenReaderMode", P => this._handleScreenReaderModeOptionChange(P))), this.options.overviewRulerWidth && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(b.OverviewRulerRenderer, this._viewportElement, this.screenElement))), this.optionsService.onSpecificOptionChange("overviewRulerWidth", P => {
                                         !this._overviewRulerRenderer && P && this._viewportElement && this.screenElement && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(b.OverviewRulerRenderer, this._viewportElement, this.screenElement)))
                                     }), this._charSizeService.measure(), this.refresh(0, this.rows - 1), this._initGlobal(), this.bindMouse()
                                 }
@@ -968,42 +968,42 @@
                             }
                             i.Terminal = N
                         },
                         9924: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.TimeBasedDebouncer = void 0, i.TimeBasedDebouncer = class {
-                                constructor(o, h = 1e3) {
-                                    this._renderCallback = o, this._debounceThresholdMS = h, this._lastRefreshMs = 0, this._additionalRefreshRequested = !1
+                                constructor(h, a = 1e3) {
+                                    this._renderCallback = h, this._debounceThresholdMS = a, this._lastRefreshMs = 0, this._additionalRefreshRequested = !1
                                 }
                                 dispose() {
                                     this._refreshTimeoutID && clearTimeout(this._refreshTimeoutID)
                                 }
-                                refresh(o, h, u) {
-                                    this._rowCount = u, o = o !== void 0 ? o : 0, h = h !== void 0 ? h : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, o) : o, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, h) : h;
+                                refresh(h, a, u) {
+                                    this._rowCount = u, h = h !== void 0 ? h : 0, a = a !== void 0 ? a : this._rowCount - 1, this._rowStart = this._rowStart !== void 0 ? Math.min(this._rowStart, h) : h, this._rowEnd = this._rowEnd !== void 0 ? Math.max(this._rowEnd, a) : a;
                                     const d = Date.now();
                                     if (d - this._lastRefreshMs >= this._debounceThresholdMS) this._lastRefreshMs = d, this._innerRefresh();
                                     else if (!this._additionalRefreshRequested) {
                                         const _ = d - this._lastRefreshMs,
                                             g = this._debounceThresholdMS - _;
                                         this._additionalRefreshRequested = !0, this._refreshTimeoutID = window.setTimeout(() => {
                                             this._lastRefreshMs = Date.now(), this._innerRefresh(), this._additionalRefreshRequested = !1, this._refreshTimeoutID = void 0
                                         }, g)
                                     }
                                 }
                                 _innerRefresh() {
                                     if (this._rowStart === void 0 || this._rowEnd === void 0 || this._rowCount === void 0) return;
-                                    const o = Math.max(this._rowStart, 0),
-                                        h = Math.min(this._rowEnd, this._rowCount - 1);
-                                    this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(o, h)
+                                    const h = Math.max(this._rowStart, 0),
+                                        a = Math.min(this._rowEnd, this._rowCount - 1);
+                                    this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(h, a)
                                 }
                             }
                         },
-                        1680: function(T, i, o) {
-                            var h = this && this.__decorate || function(e, s, n, t) {
+                        1680: function(T, i, h) {
+                            var a = this && this.__decorate || function(e, s, n, t) {
                                     var r, l = arguments.length,
                                         f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") f = Reflect.decorate(e, s, n, t);
                                     else
                                         for (var m = e.length - 1; m >= 0; m--)(r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
                                     return l > 3 && f && Object.defineProperty(s, n, f), f
                                 },
@@ -1011,25 +1011,25 @@
                                     return function(n, t) {
                                         s(n, t, e)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.Viewport = void 0;
-                            const d = o(844),
-                                _ = o(3656),
-                                g = o(4725),
-                                v = o(2585);
+                            const d = h(844),
+                                _ = h(3656),
+                                g = h(4725),
+                                v = h(2585);
                             let c = class extends d.Disposable {
-                                constructor(e, s, n, t, r, l, f, m, a) {
+                                constructor(e, s, n, t, r, l, f, m, o) {
                                     super(), this._scrollLines = e, this._viewportElement = s, this._scrollArea = n, this._bufferService = t, this._optionsService = r, this._charSizeService = l, this._renderService = f, this._coreBrowserService = m, this.scrollBarWidth = 0, this._currentRowHeight = 0, this._currentDeviceCellHeight = 0, this._lastRecordedBufferLength = 0, this._lastRecordedViewportHeight = 0, this._lastRecordedBufferHeight = 0, this._lastTouchY = 0, this._lastScrollTop = 0, this._wheelPartialScroll = 0, this._refreshAnimationFrame = null, this._ignoreNextScrollEvent = !1, this._smoothScrollState = {
                                         startTime: 0,
                                         origin: -1,
                                         target: -1
-                                    }, this.scrollBarWidth = this._viewportElement.offsetWidth - this._scrollArea.offsetWidth || 15, this.register((0, _.addDisposableDomListener)(this._viewportElement, "scroll", this._handleScroll.bind(this))), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate(p => this._activeBuffer = p.activeBuffer)), this._renderDimensions = this._renderService.dimensions, this.register(this._renderService.onDimensionsChange(p => this._renderDimensions = p)), this._handleThemeChange(a.colors), this.register(a.onChangeColors(p => this._handleThemeChange(p))), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.syncScrollArea())), setTimeout(() => this.syncScrollArea(), 0)
+                                    }, this.scrollBarWidth = this._viewportElement.offsetWidth - this._scrollArea.offsetWidth || 15, this.register((0, _.addDisposableDomListener)(this._viewportElement, "scroll", this._handleScroll.bind(this))), this._activeBuffer = this._bufferService.buffer, this.register(this._bufferService.buffers.onBufferActivate(p => this._activeBuffer = p.activeBuffer)), this._renderDimensions = this._renderService.dimensions, this.register(this._renderService.onDimensionsChange(p => this._renderDimensions = p)), this._handleThemeChange(o.colors), this.register(o.onChangeColors(p => this._handleThemeChange(p))), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.syncScrollArea())), setTimeout(() => this.syncScrollArea(), 0)
                                 }
                                 _handleThemeChange(e) {
                                     this._viewportElement.style.backgroundColor = e.background.css
                                 }
                                 _refresh(e) {
                                     if (e) return this._innerRefresh(), void(this._refreshAnimationFrame !== null && this._coreBrowserService.window.cancelAnimationFrame(this._refreshAnimationFrame));
                                     this._refreshAnimationFrame === null && (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame(() => this._innerRefresh()))
@@ -1090,18 +1090,18 @@
                                     this._lastTouchY = e.touches[0].pageY
                                 }
                                 handleTouchMove(e) {
                                     const s = this._lastTouchY - e.touches[0].pageY;
                                     return this._lastTouchY = e.touches[0].pageY, s !== 0 && (this._viewportElement.scrollTop += s, this._bubbleScroll(e, s))
                                 }
                             };
-                            c = h([u(3, v.IBufferService), u(4, v.IOptionsService), u(5, g.ICharSizeService), u(6, g.IRenderService), u(7, g.ICoreBrowserService), u(8, g.IThemeService)], c), i.Viewport = c
+                            c = a([u(3, v.IBufferService), u(4, v.IOptionsService), u(5, g.ICharSizeService), u(6, g.IRenderService), u(7, g.ICoreBrowserService), u(8, g.IThemeService)], c), i.Viewport = c
                         },
-                        3107: function(T, i, o) {
-                            var h = this && this.__decorate || function(e, s, n, t) {
+                        3107: function(T, i, h) {
+                            var a = this && this.__decorate || function(e, s, n, t) {
                                     var r, l = arguments.length,
                                         f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") f = Reflect.decorate(e, s, n, t);
                                     else
                                         for (var m = e.length - 1; m >= 0; m--)(r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
                                     return l > 3 && f && Object.defineProperty(s, n, f), f
                                 },
@@ -1109,18 +1109,18 @@
                                     return function(n, t) {
                                         s(n, t, e)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferDecorationRenderer = void 0;
-                            const d = o(3656),
-                                _ = o(4725),
-                                g = o(844),
-                                v = o(2585);
+                            const d = h(3656),
+                                _ = h(4725),
+                                g = h(844),
+                                v = h(2585);
                             let c = class extends g.Disposable {
                                 constructor(e, s, n, t) {
                                     super(), this._screenElement = e, this._bufferService = s, this._decorationService = n, this._renderService = t, this._decorationElements = new Map, this._altBufferIsActive = !1, this._dimensionsChanged = !1, this._container = document.createElement("div"), this._container.classList.add("xterm-decoration-container"), this._screenElement.appendChild(this._container), this.register(this._renderService.onRenderedViewportChange(() => this._doRefreshDecorations())), this.register(this._renderService.onDimensionsChange(() => {
                                         this._dimensionsChanged = !0, this._queueRefresh()
                                     })), this.register((0, d.addDisposableDomListener)(window, "resize", () => this._queueRefresh())), this.register(this._bufferService.buffers.onBufferActivate(() => {
                                         this._altBufferIsActive = this._bufferService.buffer === this._bufferService.buffers.alt
                                     })), this.register(this._decorationService.onDecorationRegistered(() => this._queueRefresh())), this.register(this._decorationService.onDecorationRemoved(r => this._removeDecoration(r))), this.register((0, g.toDisposable)(() => {
@@ -1161,15 +1161,15 @@
                                     (e.options.anchor || "left") === "right" ? s.style.right = t ? t * this._renderService.dimensions.css.cell.width + "px" : "": s.style.left = t ? t * this._renderService.dimensions.css.cell.width + "px" : ""
                                 }
                                 _removeDecoration(e) {
                                     var s;
                                     (s = this._decorationElements.get(e)) === null || s === void 0 || s.remove(), this._decorationElements.delete(e), e.dispose()
                                 }
                             };
-                            c = h([u(1, v.IBufferService), u(2, v.IDecorationService), u(3, _.IRenderService)], c), i.BufferDecorationRenderer = c
+                            c = a([u(1, v.IBufferService), u(2, v.IDecorationService), u(3, _.IRenderService)], c), i.BufferDecorationRenderer = c
                         },
                         5871: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.ColorZoneStore = void 0, i.ColorZoneStore = class {
                                 constructor() {
                                     this._zones = [], this._zonePool = [], this._zonePoolIndex = 0, this._linePadding = {
@@ -1181,65 +1181,65 @@
                                 }
                                 get zones() {
                                     return this._zonePool.length = Math.min(this._zonePool.length, this._zones.length), this._zones
                                 }
                                 clear() {
                                     this._zones.length = 0, this._zonePoolIndex = 0
                                 }
-                                addDecoration(o) {
-                                    if (o.options.overviewRulerOptions) {
-                                        for (const h of this._zones)
-                                            if (h.color === o.options.overviewRulerOptions.color && h.position === o.options.overviewRulerOptions.position) {
-                                                if (this._lineIntersectsZone(h, o.marker.line)) return;
-                                                if (this._lineAdjacentToZone(h, o.marker.line, o.options.overviewRulerOptions.position)) return void this._addLineToZone(h, o.marker.line)
-                                            } if (this._zonePoolIndex < this._zonePool.length) return this._zonePool[this._zonePoolIndex].color = o.options.overviewRulerOptions.color, this._zonePool[this._zonePoolIndex].position = o.options.overviewRulerOptions.position, this._zonePool[this._zonePoolIndex].startBufferLine = o.marker.line, this._zonePool[this._zonePoolIndex].endBufferLine = o.marker.line, void this._zones.push(this._zonePool[this._zonePoolIndex++]);
+                                addDecoration(h) {
+                                    if (h.options.overviewRulerOptions) {
+                                        for (const a of this._zones)
+                                            if (a.color === h.options.overviewRulerOptions.color && a.position === h.options.overviewRulerOptions.position) {
+                                                if (this._lineIntersectsZone(a, h.marker.line)) return;
+                                                if (this._lineAdjacentToZone(a, h.marker.line, h.options.overviewRulerOptions.position)) return void this._addLineToZone(a, h.marker.line)
+                                            } if (this._zonePoolIndex < this._zonePool.length) return this._zonePool[this._zonePoolIndex].color = h.options.overviewRulerOptions.color, this._zonePool[this._zonePoolIndex].position = h.options.overviewRulerOptions.position, this._zonePool[this._zonePoolIndex].startBufferLine = h.marker.line, this._zonePool[this._zonePoolIndex].endBufferLine = h.marker.line, void this._zones.push(this._zonePool[this._zonePoolIndex++]);
                                         this._zones.push({
-                                            color: o.options.overviewRulerOptions.color,
-                                            position: o.options.overviewRulerOptions.position,
-                                            startBufferLine: o.marker.line,
-                                            endBufferLine: o.marker.line
+                                            color: h.options.overviewRulerOptions.color,
+                                            position: h.options.overviewRulerOptions.position,
+                                            startBufferLine: h.marker.line,
+                                            endBufferLine: h.marker.line
                                         }), this._zonePool.push(this._zones[this._zones.length - 1]), this._zonePoolIndex++
                                     }
                                 }
-                                setPadding(o) {
-                                    this._linePadding = o
+                                setPadding(h) {
+                                    this._linePadding = h
                                 }
-                                _lineIntersectsZone(o, h) {
-                                    return h >= o.startBufferLine && h <= o.endBufferLine
+                                _lineIntersectsZone(h, a) {
+                                    return a >= h.startBufferLine && a <= h.endBufferLine
                                 }
-                                _lineAdjacentToZone(o, h, u) {
-                                    return h >= o.startBufferLine - this._linePadding[u || "full"] && h <= o.endBufferLine + this._linePadding[u || "full"]
+                                _lineAdjacentToZone(h, a, u) {
+                                    return a >= h.startBufferLine - this._linePadding[u || "full"] && a <= h.endBufferLine + this._linePadding[u || "full"]
                                 }
-                                _addLineToZone(o, h) {
-                                    o.startBufferLine = Math.min(o.startBufferLine, h), o.endBufferLine = Math.max(o.endBufferLine, h)
+                                _addLineToZone(h, a) {
+                                    h.startBufferLine = Math.min(h.startBufferLine, a), h.endBufferLine = Math.max(h.endBufferLine, a)
                                 }
                             }
                         },
-                        5744: function(T, i, o) {
-                            var h = this && this.__decorate || function(r, l, f, m) {
-                                    var a, p = arguments.length,
+                        5744: function(T, i, h) {
+                            var a = this && this.__decorate || function(r, l, f, m) {
+                                    var o, p = arguments.length,
                                         C = p < 3 ? l : m === null ? m = Object.getOwnPropertyDescriptor(l, f) : m;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") C = Reflect.decorate(r, l, f, m);
                                     else
-                                        for (var y = r.length - 1; y >= 0; y--)(a = r[y]) && (C = (p < 3 ? a(C) : p > 3 ? a(l, f, C) : a(l, f)) || C);
+                                        for (var y = r.length - 1; y >= 0; y--)(o = r[y]) && (C = (p < 3 ? o(C) : p > 3 ? o(l, f, C) : o(l, f)) || C);
                                     return p > 3 && C && Object.defineProperty(l, f, C), C
                                 },
                                 u = this && this.__param || function(r, l) {
                                     return function(f, m) {
                                         l(f, m, r)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.OverviewRulerRenderer = void 0;
-                            const d = o(5871),
-                                _ = o(3656),
-                                g = o(4725),
-                                v = o(844),
-                                c = o(2585),
+                            const d = h(5871),
+                                _ = h(3656),
+                                g = h(4725),
+                                v = h(844),
+                                c = h(2585),
                                 e = {
                                     full: 0,
                                     left: 0,
                                     center: 0,
                                     right: 0
                                 },
                                 s = {
@@ -1251,17 +1251,17 @@
                                 n = {
                                     full: 0,
                                     left: 0,
                                     center: 0,
                                     right: 0
                                 };
                             let t = class extends v.Disposable {
-                                constructor(r, l, f, m, a, p, C) {
+                                constructor(r, l, f, m, o, p, C) {
                                     var y;
-                                    super(), this._viewportElement = r, this._screenElement = l, this._bufferService = f, this._decorationService = m, this._renderService = a, this._optionsService = p, this._coreBrowseService = C, this._colorZoneStore = new d.ColorZoneStore, this._shouldUpdateDimensions = !0, this._shouldUpdateAnchor = !0, this._lastKnownBufferLength = 0, this._canvas = document.createElement("canvas"), this._canvas.classList.add("xterm-decoration-overview-ruler"), this._refreshCanvasDimensions(), (y = this._viewportElement.parentElement) === null || y === void 0 || y.insertBefore(this._canvas, this._viewportElement);
+                                    super(), this._viewportElement = r, this._screenElement = l, this._bufferService = f, this._decorationService = m, this._renderService = o, this._optionsService = p, this._coreBrowseService = C, this._colorZoneStore = new d.ColorZoneStore, this._shouldUpdateDimensions = !0, this._shouldUpdateAnchor = !0, this._lastKnownBufferLength = 0, this._canvas = document.createElement("canvas"), this._canvas.classList.add("xterm-decoration-overview-ruler"), this._refreshCanvasDimensions(), (y = this._viewportElement.parentElement) === null || y === void 0 || y.insertBefore(this._canvas, this._viewportElement);
                                     const w = this._canvas.getContext("2d");
                                     if (!w) throw new Error("Ctx cannot be null");
                                     this._ctx = w, this._registerDecorationListeners(), this._registerBufferChangeListeners(), this._registerDimensionChangeListeners(), this.register((0, v.toDisposable)(() => {
                                         var D;
                                         (D = this._canvas) === null || D === void 0 || D.remove()
                                     }))
                                 }
@@ -1319,18 +1319,18 @@
                                 }
                                 _queueRefresh(r, l) {
                                     this._shouldUpdateDimensions = r || this._shouldUpdateDimensions, this._shouldUpdateAnchor = l || this._shouldUpdateAnchor, this._animationFrame === void 0 && (this._animationFrame = this._coreBrowseService.window.requestAnimationFrame(() => {
                                         this._refreshDecorations(), this._animationFrame = void 0
                                     }))
                                 }
                             };
-                            t = h([u(2, c.IBufferService), u(3, c.IDecorationService), u(4, g.IRenderService), u(5, c.IOptionsService), u(6, g.ICoreBrowserService)], t), i.OverviewRulerRenderer = t
+                            t = a([u(2, c.IBufferService), u(3, c.IDecorationService), u(4, g.IRenderService), u(5, c.IOptionsService), u(6, g.ICoreBrowserService)], t), i.OverviewRulerRenderer = t
                         },
-                        2950: function(T, i, o) {
-                            var h = this && this.__decorate || function(c, e, s, n) {
+                        2950: function(T, i, h) {
+                            var a = this && this.__decorate || function(c, e, s, n) {
                                     var t, r = arguments.length,
                                         l = r < 3 ? e : n === null ? n = Object.getOwnPropertyDescriptor(e, s) : n;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") l = Reflect.decorate(c, e, s, n);
                                     else
                                         for (var f = c.length - 1; f >= 0; f--)(t = c[f]) && (l = (r < 3 ? t(l) : r > 3 ? t(e, s, l) : t(e, s)) || l);
                                     return r > 3 && l && Object.defineProperty(e, s, l), l
                                 },
@@ -1338,17 +1338,17 @@
                                     return function(s, n) {
                                         e(s, n, c)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CompositionHelper = void 0;
-                            const d = o(4725),
-                                _ = o(2585),
-                                g = o(2584);
+                            const d = h(4725),
+                                _ = h(2585),
+                                g = h(2584);
                             let v = class {
                                 constructor(c, e, s, n, t, r) {
                                     this._textarea = c, this._compositionView = e, this._bufferService = s, this._optionsService = n, this._coreService = t, this._renderService = r, this._isComposing = !1, this._isSendingComposition = !1, this._compositionPosition = {
                                         start: 0,
                                         end: 0
                                     }, this._dataAlreadySent = ""
                                 }
@@ -1412,47 +1412,47 @@
                                             const r = this._compositionView.getBoundingClientRect();
                                             this._textarea.style.left = t + "px", this._textarea.style.top = n + "px", this._textarea.style.width = Math.max(r.width, 1) + "px", this._textarea.style.height = Math.max(r.height, 1) + "px", this._textarea.style.lineHeight = r.height + "px"
                                         }
                                         c || setTimeout(() => this.updateCompositionElements(!0), 0)
                                     }
                                 }
                             };
-                            v = h([u(2, _.IBufferService), u(3, _.IOptionsService), u(4, _.ICoreService), u(5, d.IRenderService)], v), i.CompositionHelper = v
+                            v = a([u(2, _.IBufferService), u(3, _.IOptionsService), u(4, _.ICoreService), u(5, d.IRenderService)], v), i.CompositionHelper = v
                         },
                         9806: (T, i) => {
-                            function o(h, u, d) {
+                            function h(a, u, d) {
                                 const _ = d.getBoundingClientRect(),
-                                    g = h.getComputedStyle(d),
+                                    g = a.getComputedStyle(d),
                                     v = parseInt(g.getPropertyValue("padding-left")),
                                     c = parseInt(g.getPropertyValue("padding-top"));
                                 return [u.clientX - _.left - v, u.clientY - _.top - c]
                             }
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.getCoords = i.getCoordsRelativeToElement = void 0, i.getCoordsRelativeToElement = o, i.getCoords = function(h, u, d, _, g, v, c, e, s) {
+                            }), i.getCoords = i.getCoordsRelativeToElement = void 0, i.getCoordsRelativeToElement = h, i.getCoords = function(a, u, d, _, g, v, c, e, s) {
                                 if (!v) return;
-                                const n = o(h, u, d);
+                                const n = h(a, u, d);
                                 return n ? (n[0] = Math.ceil((n[0] + (s ? c / 2 : 0)) / c), n[1] = Math.ceil(n[1] / e), n[0] = Math.min(Math.max(n[0], 1), _ + (s ? 1 : 0)), n[1] = Math.min(Math.max(n[1], 1), g), n) : void 0
                             }
                         },
-                        9504: (T, i, o) => {
+                        9504: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.moveToCellSequence = void 0;
-                            const h = o(2584);
+                            const a = h(2584);
 
                             function u(e, s, n, t) {
                                 const r = e - d(e, n),
                                     l = s - d(s, n),
-                                    f = Math.abs(r - l) - function(m, a, p) {
+                                    f = Math.abs(r - l) - function(m, o, p) {
                                         let C = 0;
                                         const y = m - d(m, p),
-                                            w = a - d(a, p);
+                                            w = o - d(o, p);
                                         for (let D = 0; D < Math.abs(y - w); D++) {
-                                            const x = _(m, a) === "A" ? -1 : 1,
+                                            const x = _(m, o) === "A" ? -1 : 1,
                                                 I = p.buffer.lines.get(y + x * D);
                                             I != null && I.isWrapped && C++
                                         }
                                         return C
                                     }(e, s, n);
                                 return c(f, v(_(e, s), t))
                             }
@@ -1468,234 +1468,234 @@
                             function _(e, s) {
                                 return e > s ? "A" : "B"
                             }
 
                             function g(e, s, n, t, r, l) {
                                 let f = e,
                                     m = s,
-                                    a = "";
-                                for (; f !== n || m !== t;) f += r ? 1 : -1, r && f > l.cols - 1 ? (a += l.buffer.translateBufferLineToString(m, !1, e, f), f = 0, e = 0, m++) : !r && f < 0 && (a += l.buffer.translateBufferLineToString(m, !1, 0, e + 1), f = l.cols - 1, e = f, m--);
-                                return a + l.buffer.translateBufferLineToString(m, !1, e, f)
+                                    o = "";
+                                for (; f !== n || m !== t;) f += r ? 1 : -1, r && f > l.cols - 1 ? (o += l.buffer.translateBufferLineToString(m, !1, e, f), f = 0, e = 0, m++) : !r && f < 0 && (o += l.buffer.translateBufferLineToString(m, !1, 0, e + 1), f = l.cols - 1, e = f, m--);
+                                return o + l.buffer.translateBufferLineToString(m, !1, e, f)
                             }
 
                             function v(e, s) {
                                 const n = s ? "O" : "[";
-                                return h.C0.ESC + n + e
+                                return a.C0.ESC + n + e
                             }
 
                             function c(e, s) {
                                 e = Math.floor(e);
                                 let n = "";
                                 for (let t = 0; t < e; t++) n += s;
                                 return n
                             }
                             i.moveToCellSequence = function(e, s, n, t) {
                                 const r = n.buffer.x,
                                     l = n.buffer.y;
-                                if (!n.buffer.hasScrollback) return function(a, p, C, y, w, D) {
-                                    return u(p, y, w, D).length === 0 ? "" : c(g(a, p, a, p - d(p, w), !1, w).length, v("D", D))
-                                }(r, l, 0, s, n, t) + u(l, s, n, t) + function(a, p, C, y, w, D) {
+                                if (!n.buffer.hasScrollback) return function(o, p, C, y, w, D) {
+                                    return u(p, y, w, D).length === 0 ? "" : c(g(o, p, o, p - d(p, w), !1, w).length, v("D", D))
+                                }(r, l, 0, s, n, t) + u(l, s, n, t) + function(o, p, C, y, w, D) {
                                     let x;
                                     x = u(p, y, w, D).length > 0 ? y - d(y, w) : p;
                                     const I = y,
                                         H = function(S, b, L, R, M, F) {
                                             let j;
                                             return j = u(L, R, M, F).length > 0 ? R - d(R, M) : b, S < L && j <= R || S >= L && j < R ? "C" : "D"
-                                        }(a, p, C, y, w, D);
-                                    return c(g(a, x, C, I, H === "C", w).length, v(H, D))
+                                        }(o, p, C, y, w, D);
+                                    return c(g(o, x, C, I, H === "C", w).length, v(H, D))
                                 }(r, l, e, s, n, t);
                                 let f;
                                 if (l === s) return f = r > e ? "D" : "C", c(Math.abs(r - e), v(f, t));
                                 f = l > s ? "D" : "C";
                                 const m = Math.abs(l - s);
-                                return c(function(a, p) {
-                                    return p.cols - a
+                                return c(function(o, p) {
+                                    return p.cols - o
                                 }(l > s ? e : r, n) + (m - 1) * n.cols + 1 + ((l > s ? r : e) - 1), v(f, t))
                             }
                         },
-                        1296: function(T, i, o) {
-                            var h = this && this.__decorate || function(a, p, C, y) {
+                        1296: function(T, i, h) {
+                            var a = this && this.__decorate || function(o, p, C, y) {
                                     var w, D = arguments.length,
                                         x = D < 3 ? p : y === null ? y = Object.getOwnPropertyDescriptor(p, C) : y;
-                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") x = Reflect.decorate(a, p, C, y);
+                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") x = Reflect.decorate(o, p, C, y);
                                     else
-                                        for (var I = a.length - 1; I >= 0; I--)(w = a[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
+                                        for (var I = o.length - 1; I >= 0; I--)(w = o[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
                                     return D > 3 && x && Object.defineProperty(p, C, x), x
                                 },
-                                u = this && this.__param || function(a, p) {
+                                u = this && this.__param || function(o, p) {
                                     return function(C, y) {
-                                        p(C, y, a)
+                                        p(C, y, o)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.DomRenderer = void 0;
-                            const d = o(9631),
-                                _ = o(3787),
-                                g = o(2223),
-                                v = o(6171),
-                                c = o(4725),
-                                e = o(8055),
-                                s = o(8460),
-                                n = o(844),
-                                t = o(2585),
+                            const d = h(9631),
+                                _ = h(3787),
+                                g = h(2223),
+                                v = h(6171),
+                                c = h(4725),
+                                e = h(8055),
+                                s = h(8460),
+                                n = h(844),
+                                t = h(2585),
                                 r = "xterm-dom-renderer-owner-",
                                 l = "xterm-focus";
                             let f = 1,
                                 m = class extends n.Disposable {
-                                    constructor(a, p, C, y, w, D, x, I, H, S) {
-                                        super(), this._element = a, this._screenElement = p, this._viewportElement = C, this._linkifier2 = y, this._charSizeService = D, this._optionsService = x, this._bufferService = I, this._coreBrowserService = H, this._terminalClass = f++, this._rowElements = [], this._cellToRowElements = [], this.onRequestRedraw = this.register(new s.EventEmitter).event, this._rowContainer = document.createElement("div"), this._rowContainer.classList.add("xterm-rows"), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = document.createElement("div"), this._selectionContainer.classList.add("xterm-selection"), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, v.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange(() => this._handleOptionsChanged())), this.register(S.onChangeColors(b => this._injectCss(b))), this._injectCss(S.colors), this._rowFactory = w.createInstance(_.DomRendererRowFactory, document), this._element.classList.add(r + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline(b => this._handleLinkHover(b))), this.register(this._linkifier2.onHideLinkUnderline(b => this._handleLinkLeave(b))), this.register((0, n.toDisposable)(() => {
+                                    constructor(o, p, C, y, w, D, x, I, H, S) {
+                                        super(), this._element = o, this._screenElement = p, this._viewportElement = C, this._linkifier2 = y, this._charSizeService = D, this._optionsService = x, this._bufferService = I, this._coreBrowserService = H, this._terminalClass = f++, this._rowElements = [], this._cellToRowElements = [], this.onRequestRedraw = this.register(new s.EventEmitter).event, this._rowContainer = document.createElement("div"), this._rowContainer.classList.add("xterm-rows"), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = document.createElement("div"), this._selectionContainer.classList.add("xterm-selection"), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, v.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange(() => this._handleOptionsChanged())), this.register(S.onChangeColors(b => this._injectCss(b))), this._injectCss(S.colors), this._rowFactory = w.createInstance(_.DomRendererRowFactory, document), this._element.classList.add(r + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline(b => this._handleLinkHover(b))), this.register(this._linkifier2.onHideLinkUnderline(b => this._handleLinkLeave(b))), this.register((0, n.toDisposable)(() => {
                                             this._element.classList.remove(r + this._terminalClass), (0, d.removeElementFromParent)(this._rowContainer, this._selectionContainer, this._themeStyleElement, this._dimensionsStyleElement)
                                         }))
                                     }
                                     _updateDimensions() {
-                                        const a = this._coreBrowserService.dpr;
-                                        this.dimensions.device.char.width = this._charSizeService.width * a, this.dimensions.device.char.height = Math.ceil(this._charSizeService.height * a), this.dimensions.device.cell.width = this.dimensions.device.char.width + Math.round(this._optionsService.rawOptions.letterSpacing), this.dimensions.device.cell.height = Math.floor(this.dimensions.device.char.height * this._optionsService.rawOptions.lineHeight), this.dimensions.device.char.left = 0, this.dimensions.device.char.top = 0, this.dimensions.device.canvas.width = this.dimensions.device.cell.width * this._bufferService.cols, this.dimensions.device.canvas.height = this.dimensions.device.cell.height * this._bufferService.rows, this.dimensions.css.canvas.width = Math.round(this.dimensions.device.canvas.width / a), this.dimensions.css.canvas.height = Math.round(this.dimensions.device.canvas.height / a), this.dimensions.css.cell.width = this.dimensions.css.canvas.width / this._bufferService.cols, this.dimensions.css.cell.height = this.dimensions.css.canvas.height / this._bufferService.rows;
+                                        const o = this._coreBrowserService.dpr;
+                                        this.dimensions.device.char.width = this._charSizeService.width * o, this.dimensions.device.char.height = Math.ceil(this._charSizeService.height * o), this.dimensions.device.cell.width = this.dimensions.device.char.width + Math.round(this._optionsService.rawOptions.letterSpacing), this.dimensions.device.cell.height = Math.floor(this.dimensions.device.char.height * this._optionsService.rawOptions.lineHeight), this.dimensions.device.char.left = 0, this.dimensions.device.char.top = 0, this.dimensions.device.canvas.width = this.dimensions.device.cell.width * this._bufferService.cols, this.dimensions.device.canvas.height = this.dimensions.device.cell.height * this._bufferService.rows, this.dimensions.css.canvas.width = Math.round(this.dimensions.device.canvas.width / o), this.dimensions.css.canvas.height = Math.round(this.dimensions.device.canvas.height / o), this.dimensions.css.cell.width = this.dimensions.css.canvas.width / this._bufferService.cols, this.dimensions.css.cell.height = this.dimensions.css.canvas.height / this._bufferService.rows;
                                         for (const C of this._rowElements) C.style.width = `${this.dimensions.css.canvas.width}px`, C.style.height = `${this.dimensions.css.cell.height}px`, C.style.lineHeight = `${this.dimensions.css.cell.height}px`, C.style.overflow = "hidden";
                                         this._dimensionsStyleElement || (this._dimensionsStyleElement = document.createElement("style"), this._screenElement.appendChild(this._dimensionsStyleElement));
                                         const p = `${this._terminalSelector} .xterm-rows span { display: inline-block; height: 100%; vertical-align: top; width: ${this.dimensions.css.cell.width}px}`;
                                         this._dimensionsStyleElement.textContent = p, this._selectionContainer.style.height = this._viewportElement.style.height, this._screenElement.style.width = `${this.dimensions.css.canvas.width}px`, this._screenElement.style.height = `${this.dimensions.css.canvas.height}px`
                                     }
-                                    _injectCss(a) {
+                                    _injectCss(o) {
                                         this._themeStyleElement || (this._themeStyleElement = document.createElement("style"), this._screenElement.appendChild(this._themeStyleElement));
-                                        let p = `${this._terminalSelector} .xterm-rows { color: ${a.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px;}`;
-                                        p += `${this._terminalSelector} span:not(.${_.BOLD_CLASS}) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.${_.BOLD_CLASS} { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.${_.ITALIC_CLASS} { font-style: italic;}`, p += "@keyframes blink_box_shadow_" + this._terminalClass + " { 50% {  box-shadow: none; }}", p += "@keyframes blink_block_" + this._terminalClass + ` { 0% {  background-color: ${a.cursor.css};  color: ${a.cursorAccent.css}; } 50% {  background-color: ${a.cursorAccent.css};  color: ${a.cursor.css}; }}`, p += `${this._terminalSelector} .xterm-rows:not(.xterm-focus) .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { outline: 1px solid ${a.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}:not(.${_.CURSOR_STYLE_BLOCK_CLASS}) { animation: blink_box_shadow_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { animation: blink_block_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { background-color: ${a.cursor.css}; color: ${a.cursorAccent.css};}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BAR_CLASS} { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${a.cursor.css} inset;}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_UNDERLINE_CLASS} { box-shadow: 0 -1px 0 ${a.cursor.css} inset;}`, p += `${this._terminalSelector} .xterm-selection { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .xterm-selection div { position: absolute; background-color: ${a.selectionBackgroundOpaque.css};}${this._terminalSelector} .xterm-selection div { position: absolute; background-color: ${a.selectionInactiveBackgroundOpaque.css};}`;
-                                        for (const [C, y] of a.ansi.entries()) p += `${this._terminalSelector} .xterm-fg-${C} { color: ${y.css}; }${this._terminalSelector} .xterm-bg-${C} { background-color: ${y.css}; }`;
-                                        p += `${this._terminalSelector} .xterm-fg-${g.INVERTED_DEFAULT_COLOR} { color: ${e.color.opaque(a.background).css}; }${this._terminalSelector} .xterm-bg-${g.INVERTED_DEFAULT_COLOR} { background-color: ${a.foreground.css}; }`, this._themeStyleElement.textContent = p
+                                        let p = `${this._terminalSelector} .xterm-rows { color: ${o.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px;}`;
+                                        p += `${this._terminalSelector} span:not(.${_.BOLD_CLASS}) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.${_.BOLD_CLASS} { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.${_.ITALIC_CLASS} { font-style: italic;}`, p += "@keyframes blink_box_shadow_" + this._terminalClass + " { 50% {  box-shadow: none; }}", p += "@keyframes blink_block_" + this._terminalClass + ` { 0% {  background-color: ${o.cursor.css};  color: ${o.cursorAccent.css}; } 50% {  background-color: ${o.cursorAccent.css};  color: ${o.cursor.css}; }}`, p += `${this._terminalSelector} .xterm-rows:not(.xterm-focus) .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { outline: 1px solid ${o.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}:not(.${_.CURSOR_STYLE_BLOCK_CLASS}) { animation: blink_box_shadow_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_BLINK_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { animation: blink_block_` + this._terminalClass + ` 1s step-end infinite;}${this._terminalSelector} .xterm-rows.xterm-focus .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BLOCK_CLASS} { background-color: ${o.cursor.css}; color: ${o.cursorAccent.css};}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_BAR_CLASS} { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${o.cursor.css} inset;}${this._terminalSelector} .xterm-rows .${_.CURSOR_CLASS}.${_.CURSOR_STYLE_UNDERLINE_CLASS} { box-shadow: 0 -1px 0 ${o.cursor.css} inset;}`, p += `${this._terminalSelector} .xterm-selection { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .xterm-selection div { position: absolute; background-color: ${o.selectionBackgroundOpaque.css};}${this._terminalSelector} .xterm-selection div { position: absolute; background-color: ${o.selectionInactiveBackgroundOpaque.css};}`;
+                                        for (const [C, y] of o.ansi.entries()) p += `${this._terminalSelector} .xterm-fg-${C} { color: ${y.css}; }${this._terminalSelector} .xterm-bg-${C} { background-color: ${y.css}; }`;
+                                        p += `${this._terminalSelector} .xterm-fg-${g.INVERTED_DEFAULT_COLOR} { color: ${e.color.opaque(o.background).css}; }${this._terminalSelector} .xterm-bg-${g.INVERTED_DEFAULT_COLOR} { background-color: ${o.foreground.css}; }`, this._themeStyleElement.textContent = p
                                     }
                                     handleDevicePixelRatioChange() {
                                         this._updateDimensions()
                                     }
-                                    _refreshRowElements(a, p) {
+                                    _refreshRowElements(o, p) {
                                         for (let C = this._rowElements.length; C <= p; C++) {
                                             const y = document.createElement("div");
                                             this._rowContainer.appendChild(y), this._rowElements.push(y)
                                         }
                                         for (; this._rowElements.length > p;) this._rowContainer.removeChild(this._rowElements.pop())
                                     }
-                                    handleResize(a, p) {
-                                        this._refreshRowElements(a, p), this._updateDimensions()
+                                    handleResize(o, p) {
+                                        this._refreshRowElements(o, p), this._updateDimensions()
                                     }
                                     handleCharSizeChanged() {
                                         this._updateDimensions()
                                     }
                                     handleBlur() {
                                         this._rowContainer.classList.remove(l)
                                     }
                                     handleFocus() {
                                         this._rowContainer.classList.add(l)
                                     }
-                                    handleSelectionChanged(a, p, C) {
+                                    handleSelectionChanged(o, p, C) {
                                         for (; this._selectionContainer.children.length;) this._selectionContainer.removeChild(this._selectionContainer.children[0]);
-                                        if (this._rowFactory.handleSelectionChanged(a, p, C), this.renderRows(0, this._bufferService.rows - 1), !a || !p) return;
-                                        const y = a[1] - this._bufferService.buffer.ydisp,
+                                        if (this._rowFactory.handleSelectionChanged(o, p, C), this.renderRows(0, this._bufferService.rows - 1), !o || !p) return;
+                                        const y = o[1] - this._bufferService.buffer.ydisp,
                                             w = p[1] - this._bufferService.buffer.ydisp,
                                             D = Math.max(y, 0),
                                             x = Math.min(w, this._bufferService.rows - 1);
                                         if (D >= this._bufferService.rows || x < 0) return;
                                         const I = document.createDocumentFragment();
                                         if (C) {
-                                            const H = a[0] > p[0];
-                                            I.appendChild(this._createSelectionElement(D, H ? p[0] : a[0], H ? a[0] : p[0], x - D + 1))
+                                            const H = o[0] > p[0];
+                                            I.appendChild(this._createSelectionElement(D, H ? p[0] : o[0], H ? o[0] : p[0], x - D + 1))
                                         } else {
-                                            const H = y === D ? a[0] : 0,
+                                            const H = y === D ? o[0] : 0,
                                                 S = D === w ? p[0] : this._bufferService.cols;
                                             I.appendChild(this._createSelectionElement(D, H, S));
                                             const b = x - D - 1;
                                             if (I.appendChild(this._createSelectionElement(D + 1, 0, this._bufferService.cols, b)), D !== x) {
                                                 const L = w === x ? p[0] : this._bufferService.cols;
                                                 I.appendChild(this._createSelectionElement(x, 0, L))
                                             }
                                         }
                                         this._selectionContainer.appendChild(I)
                                     }
-                                    _createSelectionElement(a, p, C, y = 1) {
+                                    _createSelectionElement(o, p, C, y = 1) {
                                         const w = document.createElement("div");
-                                        return w.style.height = y * this.dimensions.css.cell.height + "px", w.style.top = a * this.dimensions.css.cell.height + "px", w.style.left = p * this.dimensions.css.cell.width + "px", w.style.width = this.dimensions.css.cell.width * (C - p) + "px", w
+                                        return w.style.height = y * this.dimensions.css.cell.height + "px", w.style.top = o * this.dimensions.css.cell.height + "px", w.style.left = p * this.dimensions.css.cell.width + "px", w.style.width = this.dimensions.css.cell.width * (C - p) + "px", w
                                     }
                                     handleCursorMove() {}
                                     _handleOptionsChanged() {
                                         this._updateDimensions()
                                     }
                                     clear() {
-                                        for (const a of this._rowElements) a.replaceChildren()
+                                        for (const o of this._rowElements) o.replaceChildren()
                                     }
-                                    renderRows(a, p) {
+                                    renderRows(o, p) {
                                         const C = this._bufferService.buffer.ybase + this._bufferService.buffer.y,
                                             y = Math.min(this._bufferService.buffer.x, this._bufferService.cols - 1),
                                             w = this._optionsService.rawOptions.cursorBlink;
-                                        for (let D = a; D <= p; D++) {
+                                        for (let D = o; D <= p; D++) {
                                             const x = this._rowElements[D],
                                                 I = D + this._bufferService.buffer.ydisp,
                                                 H = this._bufferService.buffer.lines.get(I),
                                                 S = this._optionsService.rawOptions.cursorStyle;
                                             this._cellToRowElements[D] && this._cellToRowElements[D].length === this._bufferService.cols || (this._cellToRowElements[D] = new Int16Array(this._bufferService.cols)), x.replaceChildren(this._rowFactory.createRow(H, I, I === C, S, y, w, this.dimensions.css.cell.width, this._bufferService.cols, this._cellToRowElements[D]))
                                         }
                                     }
                                     get _terminalSelector() {
                                         return `.${r}${this._terminalClass}`
                                     }
-                                    _handleLinkHover(a) {
-                                        this._setCellUnderline(a.x1, a.x2, a.y1, a.y2, a.cols, !0)
+                                    _handleLinkHover(o) {
+                                        this._setCellUnderline(o.x1, o.x2, o.y1, o.y2, o.cols, !0)
                                     }
-                                    _handleLinkLeave(a) {
-                                        this._setCellUnderline(a.x1, a.x2, a.y1, a.y2, a.cols, !1)
+                                    _handleLinkLeave(o) {
+                                        this._setCellUnderline(o.x1, o.x2, o.y1, o.y2, o.cols, !1)
                                     }
-                                    _setCellUnderline(a, p, C, y, w, D) {
-                                        if (a = this._cellToRowElements[C][a], p = this._cellToRowElements[y][p], a !== -1 && p !== -1)
-                                            for (; a !== p || C !== y;) {
+                                    _setCellUnderline(o, p, C, y, w, D) {
+                                        if (o = this._cellToRowElements[C][o], p = this._cellToRowElements[y][p], o !== -1 && p !== -1)
+                                            for (; o !== p || C !== y;) {
                                                 const x = this._rowElements[C];
                                                 if (!x) return;
-                                                const I = x.children[a];
-                                                I && (I.style.textDecoration = D ? "underline" : "none"), ++a >= w && (a = 0, C++)
+                                                const I = x.children[o];
+                                                I && (I.style.textDecoration = D ? "underline" : "none"), ++o >= w && (o = 0, C++)
                                             }
                                     }
                                 };
-                            m = h([u(4, t.IInstantiationService), u(5, c.ICharSizeService), u(6, t.IOptionsService), u(7, t.IBufferService), u(8, c.ICoreBrowserService), u(9, c.IThemeService)], m), i.DomRenderer = m
+                            m = a([u(4, t.IInstantiationService), u(5, c.ICharSizeService), u(6, t.IOptionsService), u(7, t.IBufferService), u(8, c.ICoreBrowserService), u(9, c.IThemeService)], m), i.DomRenderer = m
                         },
-                        3787: function(T, i, o) {
-                            var h = this && this.__decorate || function(f, m, a, p) {
+                        3787: function(T, i, h) {
+                            var a = this && this.__decorate || function(f, m, o, p) {
                                     var C, y = arguments.length,
-                                        w = y < 3 ? m : p === null ? p = Object.getOwnPropertyDescriptor(m, a) : p;
-                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") w = Reflect.decorate(f, m, a, p);
+                                        w = y < 3 ? m : p === null ? p = Object.getOwnPropertyDescriptor(m, o) : p;
+                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") w = Reflect.decorate(f, m, o, p);
                                     else
-                                        for (var D = f.length - 1; D >= 0; D--)(C = f[D]) && (w = (y < 3 ? C(w) : y > 3 ? C(m, a, w) : C(m, a)) || w);
-                                    return y > 3 && w && Object.defineProperty(m, a, w), w
+                                        for (var D = f.length - 1; D >= 0; D--)(C = f[D]) && (w = (y < 3 ? C(w) : y > 3 ? C(m, o, w) : C(m, o)) || w);
+                                    return y > 3 && w && Object.defineProperty(m, o, w), w
                                 },
                                 u = this && this.__param || function(f, m) {
-                                    return function(a, p) {
-                                        m(a, p, f)
+                                    return function(o, p) {
+                                        m(o, p, f)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.DomRendererRowFactory = i.CURSOR_STYLE_UNDERLINE_CLASS = i.CURSOR_STYLE_BAR_CLASS = i.CURSOR_STYLE_BLOCK_CLASS = i.CURSOR_BLINK_CLASS = i.CURSOR_CLASS = i.STRIKETHROUGH_CLASS = i.UNDERLINE_CLASS = i.ITALIC_CLASS = i.DIM_CLASS = i.BOLD_CLASS = void 0;
-                            const d = o(2223),
-                                _ = o(643),
-                                g = o(511),
-                                v = o(2585),
-                                c = o(8055),
-                                e = o(4725),
-                                s = o(4269),
-                                n = o(6171),
-                                t = o(3734);
+                            const d = h(2223),
+                                _ = h(643),
+                                g = h(511),
+                                v = h(2585),
+                                c = h(8055),
+                                e = h(4725),
+                                s = h(4269),
+                                n = h(6171),
+                                t = h(3734);
                             i.BOLD_CLASS = "xterm-bold", i.DIM_CLASS = "xterm-dim", i.ITALIC_CLASS = "xterm-italic", i.UNDERLINE_CLASS = "xterm-underline", i.STRIKETHROUGH_CLASS = "xterm-strikethrough", i.CURSOR_CLASS = "xterm-cursor", i.CURSOR_BLINK_CLASS = "xterm-cursor-blink", i.CURSOR_STYLE_BLOCK_CLASS = "xterm-cursor-block", i.CURSOR_STYLE_BAR_CLASS = "xterm-cursor-bar", i.CURSOR_STYLE_UNDERLINE_CLASS = "xterm-cursor-underline";
                             let r = class {
-                                constructor(f, m, a, p, C, y, w) {
-                                    this._document = f, this._characterJoinerService = m, this._optionsService = a, this._coreBrowserService = p, this._coreService = C, this._decorationService = y, this._themeService = w, this._workCell = new g.CellData, this._columnSelectMode = !1
+                                constructor(f, m, o, p, C, y, w) {
+                                    this._document = f, this._characterJoinerService = m, this._optionsService = o, this._coreBrowserService = p, this._coreService = C, this._decorationService = y, this._themeService = w, this._workCell = new g.CellData, this._columnSelectMode = !1
                                 }
-                                handleSelectionChanged(f, m, a) {
-                                    this._selectionStart = f, this._selectionEnd = m, this._columnSelectMode = a
+                                handleSelectionChanged(f, m, o) {
+                                    this._selectionStart = f, this._selectionEnd = m, this._columnSelectMode = o
                                 }
-                                createRow(f, m, a, p, C, y, w, D, x) {
+                                createRow(f, m, o, p, C, y, w, D, x) {
                                     const I = this._document.createDocumentFragment(),
                                         H = this._characterJoinerService.getJoinedCharacters(m);
                                     let S = 0;
                                     for (let M = Math.min(f.length, D) - 1; M >= 0; M--)
-                                        if (f.loadCell(M, this._workCell).getCode() !== _.NULL_CELL_CODE || a && M === C) {
+                                        if (f.loadCell(M, this._workCell).getCode() !== _.NULL_CELL_CODE || o && M === C) {
                                             S = M + 1;
                                             break
                                         } const b = this._themeService.colors;
                                     let L = -1,
                                         R = 0;
                                     for (; R < S; R++) {
                                         f.loadCell(R, this._workCell);
@@ -1709,15 +1709,15 @@
                                             O = this._workCell;
                                         if (H.length > 0 && R === H[0][0]) {
                                             F = !0;
                                             const $ = H.shift();
                                             O = new s.JoinedCellData(this._workCell, f.translateToString(!0, $[0], $[1]), $[1] - $[0]), j = $[1] - 1, M = O.getWidth()
                                         }
                                         const N = this._document.createElement("span");
-                                        if (M > 1 && (N.style.width = w * M + "px"), F && (N.style.display = "inline", C >= R && C <= j && (C = R)), !this._coreService.isCursorHidden && a && R === C) switch (N.classList.add(i.CURSOR_CLASS), y && N.classList.add(i.CURSOR_BLINK_CLASS), p) {
+                                        if (M > 1 && (N.style.width = w * M + "px"), F && (N.style.display = "inline", C >= R && C <= j && (C = R)), !this._coreService.isCursorHidden && o && R === C) switch (N.classList.add(i.CURSOR_CLASS), y && N.classList.add(i.CURSOR_BLINK_CLASS), p) {
                                             case "bar":
                                                 N.classList.add(i.CURSOR_STYLE_BAR_CLASS);
                                                 break;
                                             case "underline":
                                                 N.classList.add(i.CURSOR_STYLE_UNDERLINE_CLASS);
                                                 break;
                                             default:
@@ -1769,57 +1769,57 @@
                                             default:
                                                 this._applyMinimumContrast(N, q, b.foreground, O, z, void 0) || P && N.classList.add(`xterm-fg-${d.INVERTED_DEFAULT_COLOR}`)
                                         }
                                         I.appendChild(N), x[R] = ++L, R = j
                                     }
                                     return R < D - 1 && x.subarray(R).fill(++L), I
                                 }
-                                _applyMinimumContrast(f, m, a, p, C, y) {
+                                _applyMinimumContrast(f, m, o, p, C, y) {
                                     if (this._optionsService.rawOptions.minimumContrastRatio === 1 || (0, n.excludeFromContrastRatioDemands)(p.getCode())) return !1;
                                     let w;
-                                    return C || y || (w = this._themeService.colors.contrastCache.getColor(m.rgba, a.rgba)), w === void 0 && (w = c.color.ensureContrastRatio(C || m, y || a, this._optionsService.rawOptions.minimumContrastRatio), this._themeService.colors.contrastCache.setColor((C || m).rgba, (y || a).rgba, w ?? null)), !!w && (this._addStyle(f, `color:${w.css}`), !0)
+                                    return C || y || (w = this._themeService.colors.contrastCache.getColor(m.rgba, o.rgba)), w === void 0 && (w = c.color.ensureContrastRatio(C || m, y || o, this._optionsService.rawOptions.minimumContrastRatio), this._themeService.colors.contrastCache.setColor((C || m).rgba, (y || o).rgba, w ?? null)), !!w && (this._addStyle(f, `color:${w.css}`), !0)
                                 }
                                 _addStyle(f, m) {
                                     f.setAttribute("style", `${f.getAttribute("style")||""}${m};`)
                                 }
                                 _isCellInSelection(f, m) {
-                                    const a = this._selectionStart,
+                                    const o = this._selectionStart,
                                         p = this._selectionEnd;
-                                    return !(!a || !p) && (this._columnSelectMode ? a[0] <= p[0] ? f >= a[0] && m >= a[1] && f < p[0] && m <= p[1] : f < a[0] && m >= a[1] && f >= p[0] && m <= p[1] : m > a[1] && m < p[1] || a[1] === p[1] && m === a[1] && f >= a[0] && f < p[0] || a[1] < p[1] && m === p[1] && f < p[0] || a[1] < p[1] && m === a[1] && f >= a[0])
+                                    return !(!o || !p) && (this._columnSelectMode ? o[0] <= p[0] ? f >= o[0] && m >= o[1] && f < p[0] && m <= p[1] : f < o[0] && m >= o[1] && f >= p[0] && m <= p[1] : m > o[1] && m < p[1] || o[1] === p[1] && m === o[1] && f >= o[0] && f < p[0] || o[1] < p[1] && m === p[1] && f < p[0] || o[1] < p[1] && m === o[1] && f >= o[0])
                                 }
                             };
 
-                            function l(f, m, a) {
-                                for (; f.length < a;) f = m + f;
+                            function l(f, m, o) {
+                                for (; f.length < o;) f = m + f;
                                 return f
                             }
-                            r = h([u(1, e.ICharacterJoinerService), u(2, v.IOptionsService), u(3, e.ICoreBrowserService), u(4, v.ICoreService), u(5, v.IDecorationService), u(6, e.IThemeService)], r), i.DomRendererRowFactory = r
+                            r = a([u(1, e.ICharacterJoinerService), u(2, v.IOptionsService), u(3, e.ICoreBrowserService), u(4, v.ICoreService), u(5, v.IDecorationService), u(6, e.IThemeService)], r), i.DomRendererRowFactory = r
                         },
-                        2223: (T, i, o) => {
+                        2223: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.TEXT_BASELINE = i.DIM_OPACITY = i.INVERTED_DEFAULT_COLOR = void 0;
-                            const h = o(6114);
-                            i.INVERTED_DEFAULT_COLOR = 257, i.DIM_OPACITY = .5, i.TEXT_BASELINE = h.isFirefox || h.isLegacyEdge ? "bottom" : "ideographic"
+                            const a = h(6114);
+                            i.INVERTED_DEFAULT_COLOR = 257, i.DIM_OPACITY = .5, i.TEXT_BASELINE = a.isFirefox || a.isLegacyEdge ? "bottom" : "ideographic"
                         },
                         6171: (T, i) => {
-                            function o(h) {
-                                return 57508 <= h && h <= 57558
+                            function h(a) {
+                                return 57508 <= a && a <= 57558
                             }
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.createRenderDimensions = i.excludeFromContrastRatioDemands = i.isRestrictedPowerlineGlyph = i.isPowerlineGlyph = i.throwIfFalsy = void 0, i.throwIfFalsy = function(h) {
-                                if (!h) throw new Error("value must not be falsy");
-                                return h
-                            }, i.isPowerlineGlyph = o, i.isRestrictedPowerlineGlyph = function(h) {
-                                return 57520 <= h && h <= 57527
-                            }, i.excludeFromContrastRatioDemands = function(h) {
-                                return o(h) || function(u) {
+                            }), i.createRenderDimensions = i.excludeFromContrastRatioDemands = i.isRestrictedPowerlineGlyph = i.isPowerlineGlyph = i.throwIfFalsy = void 0, i.throwIfFalsy = function(a) {
+                                if (!a) throw new Error("value must not be falsy");
+                                return a
+                            }, i.isPowerlineGlyph = h, i.isRestrictedPowerlineGlyph = function(a) {
+                                return 57520 <= a && a <= 57527
+                            }, i.excludeFromContrastRatioDemands = function(a) {
+                                return h(a) || function(u) {
                                     return 9472 <= u && u <= 9631
-                                }(h)
+                                }(a)
                             }, i.createRenderDimensions = function() {
                                 return {
                                     css: {
                                         canvas: {
                                             width: 0,
                                             height: 0
                                         },
@@ -1847,49 +1847,49 @@
                                 }
                             }
                         },
                         456: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.SelectionModel = void 0, i.SelectionModel = class {
-                                constructor(o) {
-                                    this._bufferService = o, this.isSelectAllActive = !1, this.selectionStartLength = 0
+                                constructor(h) {
+                                    this._bufferService = h, this.isSelectAllActive = !1, this.selectionStartLength = 0
                                 }
                                 clearSelection() {
                                     this.selectionStart = void 0, this.selectionEnd = void 0, this.isSelectAllActive = !1, this.selectionStartLength = 0
                                 }
                                 get finalSelectionStart() {
                                     return this.isSelectAllActive ? [0, 0] : this.selectionEnd && this.selectionStart && this.areSelectionValuesReversed() ? this.selectionEnd : this.selectionStart
                                 }
                                 get finalSelectionEnd() {
                                     if (this.isSelectAllActive) return [this._bufferService.cols, this._bufferService.buffer.ybase + this._bufferService.rows - 1];
                                     if (this.selectionStart) {
                                         if (!this.selectionEnd || this.areSelectionValuesReversed()) {
-                                            const o = this.selectionStart[0] + this.selectionStartLength;
-                                            return o > this._bufferService.cols ? o % this._bufferService.cols == 0 ? [this._bufferService.cols, this.selectionStart[1] + Math.floor(o / this._bufferService.cols) - 1] : [o % this._bufferService.cols, this.selectionStart[1] + Math.floor(o / this._bufferService.cols)] : [o, this.selectionStart[1]]
+                                            const h = this.selectionStart[0] + this.selectionStartLength;
+                                            return h > this._bufferService.cols ? h % this._bufferService.cols == 0 ? [this._bufferService.cols, this.selectionStart[1] + Math.floor(h / this._bufferService.cols) - 1] : [h % this._bufferService.cols, this.selectionStart[1] + Math.floor(h / this._bufferService.cols)] : [h, this.selectionStart[1]]
                                         }
                                         if (this.selectionStartLength && this.selectionEnd[1] === this.selectionStart[1]) {
-                                            const o = this.selectionStart[0] + this.selectionStartLength;
-                                            return o > this._bufferService.cols ? [o % this._bufferService.cols, this.selectionStart[1] + Math.floor(o / this._bufferService.cols)] : [Math.max(o, this.selectionEnd[0]), this.selectionEnd[1]]
+                                            const h = this.selectionStart[0] + this.selectionStartLength;
+                                            return h > this._bufferService.cols ? [h % this._bufferService.cols, this.selectionStart[1] + Math.floor(h / this._bufferService.cols)] : [Math.max(h, this.selectionEnd[0]), this.selectionEnd[1]]
                                         }
                                         return this.selectionEnd
                                     }
                                 }
                                 areSelectionValuesReversed() {
-                                    const o = this.selectionStart,
-                                        h = this.selectionEnd;
-                                    return !(!o || !h) && (o[1] > h[1] || o[1] === h[1] && o[0] > h[0])
+                                    const h = this.selectionStart,
+                                        a = this.selectionEnd;
+                                    return !(!h || !a) && (h[1] > a[1] || h[1] === a[1] && h[0] > a[0])
                                 }
-                                handleTrim(o) {
-                                    return this.selectionStart && (this.selectionStart[1] -= o), this.selectionEnd && (this.selectionEnd[1] -= o), this.selectionEnd && this.selectionEnd[1] < 0 ? (this.clearSelection(), !0) : (this.selectionStart && this.selectionStart[1] < 0 && (this.selectionStart[1] = 0), !1)
+                                handleTrim(h) {
+                                    return this.selectionStart && (this.selectionStart[1] -= h), this.selectionEnd && (this.selectionEnd[1] -= h), this.selectionEnd && this.selectionEnd[1] < 0 ? (this.clearSelection(), !0) : (this.selectionStart && this.selectionStart[1] < 0 && (this.selectionStart[1] = 0), !1)
                                 }
                             }
                         },
-                        428: function(T, i, o) {
-                            var h = this && this.__decorate || function(e, s, n, t) {
+                        428: function(T, i, h) {
+                            var a = this && this.__decorate || function(e, s, n, t) {
                                     var r, l = arguments.length,
                                         f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") f = Reflect.decorate(e, s, n, t);
                                     else
                                         for (var m = e.length - 1; m >= 0; m--)(r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
                                     return l > 3 && f && Object.defineProperty(s, n, f), f
                                 },
@@ -1897,65 +1897,65 @@
                                     return function(n, t) {
                                         s(n, t, e)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CharSizeService = void 0;
-                            const d = o(2585),
-                                _ = o(8460),
-                                g = o(844);
+                            const d = h(2585),
+                                _ = h(8460),
+                                g = h(844);
                             let v = class extends g.Disposable {
                                 constructor(e, s, n) {
                                     super(), this._optionsService = n, this.width = 0, this.height = 0, this._onCharSizeChange = this.register(new _.EventEmitter), this.onCharSizeChange = this._onCharSizeChange.event, this._measureStrategy = new c(e, s, this._optionsService), this.register(this._optionsService.onMultipleOptionChange(["fontFamily", "fontSize"], () => this.measure()))
                                 }
                                 get hasValidSize() {
                                     return this.width > 0 && this.height > 0
                                 }
                                 measure() {
                                     const e = this._measureStrategy.measure();
                                     e.width === this.width && e.height === this.height || (this.width = e.width, this.height = e.height, this._onCharSizeChange.fire())
                                 }
                             };
-                            v = h([u(2, d.IOptionsService)], v), i.CharSizeService = v;
+                            v = a([u(2, d.IOptionsService)], v), i.CharSizeService = v;
                             class c {
                                 constructor(s, n, t) {
                                     this._document = s, this._parentElement = n, this._optionsService = t, this._result = {
                                         width: 0,
                                         height: 0
                                     }, this._measureElement = this._document.createElement("span"), this._measureElement.classList.add("xterm-char-measure-element"), this._measureElement.textContent = "W", this._measureElement.setAttribute("aria-hidden", "true"), this._parentElement.appendChild(this._measureElement)
                                 }
                                 measure() {
                                     this._measureElement.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._measureElement.style.fontSize = `${this._optionsService.rawOptions.fontSize}px`;
                                     const s = this._measureElement.getBoundingClientRect();
                                     return s.width !== 0 && s.height !== 0 && (this._result.width = s.width, this._result.height = Math.ceil(s.height)), this._result
                                 }
                             }
                         },
-                        4269: function(T, i, o) {
-                            var h = this && this.__decorate || function(s, n, t, r) {
+                        4269: function(T, i, h) {
+                            var a = this && this.__decorate || function(s, n, t, r) {
                                     var l, f = arguments.length,
                                         m = f < 3 ? n : r === null ? r = Object.getOwnPropertyDescriptor(n, t) : r;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") m = Reflect.decorate(s, n, t, r);
                                     else
-                                        for (var a = s.length - 1; a >= 0; a--)(l = s[a]) && (m = (f < 3 ? l(m) : f > 3 ? l(n, t, m) : l(n, t)) || m);
+                                        for (var o = s.length - 1; o >= 0; o--)(l = s[o]) && (m = (f < 3 ? l(m) : f > 3 ? l(n, t, m) : l(n, t)) || m);
                                     return f > 3 && m && Object.defineProperty(n, t, m), m
                                 },
                                 u = this && this.__param || function(s, n) {
                                     return function(t, r) {
                                         n(t, r, s)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CharacterJoinerService = i.JoinedCellData = void 0;
-                            const d = o(3734),
-                                _ = o(643),
-                                g = o(511),
-                                v = o(2585);
+                            const d = h(3734),
+                                _ = h(643),
+                                g = h(511),
+                                v = h(2585);
                             class c extends d.AttributeData {
                                 constructor(n, t, r) {
                                     super(), this.content = 0, this.combinedData = "", this.fg = n.fg, this.bg = n.bg, this.combinedData = t, this._width = r
                                 }
                                 isCombined() {
                                     return 2097152
                                 }
@@ -1996,67 +1996,67 @@
                                     if (this._characterJoiners.length === 0) return [];
                                     const t = this._bufferService.buffer.lines.get(n);
                                     if (!t || t.length === 0) return [];
                                     const r = [],
                                         l = t.translateToString(!0);
                                     let f = 0,
                                         m = 0,
-                                        a = 0,
+                                        o = 0,
                                         p = t.getFg(0),
                                         C = t.getBg(0);
                                     for (let y = 0; y < t.getTrimmedLength(); y++)
                                         if (t.loadCell(y, this._workCell), this._workCell.getWidth() !== 0) {
                                             if (this._workCell.fg !== p || this._workCell.bg !== C) {
                                                 if (y - f > 1) {
-                                                    const w = this._getJoinedRanges(l, a, m, t, f);
+                                                    const w = this._getJoinedRanges(l, o, m, t, f);
                                                     for (let D = 0; D < w.length; D++) r.push(w[D])
                                                 }
-                                                f = y, a = m, p = this._workCell.fg, C = this._workCell.bg
+                                                f = y, o = m, p = this._workCell.fg, C = this._workCell.bg
                                             }
                                             m += this._workCell.getChars().length || _.WHITESPACE_CELL_CHAR.length
                                         } if (this._bufferService.cols - f > 1) {
-                                        const y = this._getJoinedRanges(l, a, m, t, f);
+                                        const y = this._getJoinedRanges(l, o, m, t, f);
                                         for (let w = 0; w < y.length; w++) r.push(y[w])
                                     }
                                     return r
                                 }
                                 _getJoinedRanges(n, t, r, l, f) {
                                     const m = n.substring(t, r);
-                                    let a = [];
+                                    let o = [];
                                     try {
-                                        a = this._characterJoiners[0].handler(m)
+                                        o = this._characterJoiners[0].handler(m)
                                     } catch (p) {
                                         console.error(p)
                                     }
                                     for (let p = 1; p < this._characterJoiners.length; p++) try {
                                         const C = this._characterJoiners[p].handler(m);
-                                        for (let y = 0; y < C.length; y++) re._mergeRanges(a, C[y])
+                                        for (let y = 0; y < C.length; y++) re._mergeRanges(o, C[y])
                                     } catch (C) {
                                         console.error(C)
                                     }
-                                    return this._stringRangesToCellRanges(a, l, f), a
+                                    return this._stringRangesToCellRanges(o, l, f), o
                                 }
                                 _stringRangesToCellRanges(n, t, r) {
                                     let l = 0,
                                         f = !1,
                                         m = 0,
-                                        a = n[l];
-                                    if (a) {
+                                        o = n[l];
+                                    if (o) {
                                         for (let p = r; p < this._bufferService.cols; p++) {
                                             const C = t.getWidth(p),
                                                 y = t.getString(p).length || _.WHITESPACE_CELL_CHAR.length;
                                             if (C !== 0) {
-                                                if (!f && a[0] <= m && (a[0] = p, f = !0), a[1] <= m) {
-                                                    if (a[1] = p, a = n[++l], !a) break;
-                                                    a[0] <= m ? (a[0] = p, f = !0) : f = !1
+                                                if (!f && o[0] <= m && (o[0] = p, f = !0), o[1] <= m) {
+                                                    if (o[1] = p, o = n[++l], !o) break;
+                                                    o[0] <= m ? (o[0] = p, f = !0) : f = !1
                                                 }
                                                 m += y
                                             }
                                         }
-                                        a && (a[1] = this._bufferService.cols)
+                                        o && (o[1] = this._bufferService.cols)
                                     }
                                 }
                                 static _mergeRanges(n, t) {
                                     let r = !1;
                                     for (let l = 0; l < n.length; l++) {
                                         const f = n[l];
                                         if (r) {
@@ -2068,33 +2068,33 @@
                                             if (t[1] <= f[1]) return f[0] = Math.min(t[0], f[0]), n;
                                             t[0] < f[1] && (f[0] = Math.min(t[0], f[0]), r = !0)
                                         }
                                     }
                                     return r ? n[n.length - 1][1] = t[1] : n.push(t), n
                                 }
                             };
-                            e = h([u(0, v.IBufferService)], e), i.CharacterJoinerService = e
+                            e = a([u(0, v.IBufferService)], e), i.CharacterJoinerService = e
                         },
                         5114: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CoreBrowserService = void 0, i.CoreBrowserService = class {
-                                constructor(o, h) {
-                                    this._textarea = o, this.window = h, this._isFocused = !1, this._cachedIsFocused = void 0, this._textarea.addEventListener("focus", () => this._isFocused = !0), this._textarea.addEventListener("blur", () => this._isFocused = !1)
+                                constructor(h, a) {
+                                    this._textarea = h, this.window = a, this._isFocused = !1, this._cachedIsFocused = void 0, this._textarea.addEventListener("focus", () => this._isFocused = !0), this._textarea.addEventListener("blur", () => this._isFocused = !1)
                                 }
                                 get dpr() {
                                     return this.window.devicePixelRatio
                                 }
                                 get isFocused() {
                                     return this._cachedIsFocused === void 0 && (this._cachedIsFocused = this._isFocused && this._textarea.ownerDocument.hasFocus(), queueMicrotask(() => this._cachedIsFocused = void 0)), this._cachedIsFocused
                                 }
                             }
                         },
-                        8934: function(T, i, o) {
-                            var h = this && this.__decorate || function(v, c, e, s) {
+                        8934: function(T, i, h) {
+                            var a = this && this.__decorate || function(v, c, e, s) {
                                     var n, t = arguments.length,
                                         r = t < 3 ? c : s === null ? s = Object.getOwnPropertyDescriptor(c, e) : s;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") r = Reflect.decorate(v, c, e, s);
                                     else
                                         for (var l = v.length - 1; l >= 0; l--)(n = v[l]) && (r = (t < 3 ? n(r) : t > 3 ? n(c, e, r) : n(c, e)) || r);
                                     return t > 3 && r && Object.defineProperty(c, e, r), r
                                 },
@@ -2102,16 +2102,16 @@
                                     return function(e, s) {
                                         c(e, s, v)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.MouseService = void 0;
-                            const d = o(4725),
-                                _ = o(9806);
+                            const d = h(4725),
+                                _ = h(9806);
                             let g = class {
                                 constructor(v, c) {
                                     this._renderService = v, this._charSizeService = c
                                 }
                                 getCoords(v, c, e, s, n) {
                                     return (0, _.getCoords)(window, v, c, e, s, this._charSizeService.hasValidSize, this._renderService.dimensions.css.cell.width, this._renderService.dimensions.css.cell.height, n)
                                 }
@@ -2121,56 +2121,56 @@
                                         col: Math.floor(e[0] / this._renderService.dimensions.css.cell.width),
                                         row: Math.floor(e[1] / this._renderService.dimensions.css.cell.height),
                                         x: Math.floor(e[0]),
                                         y: Math.floor(e[1])
                                     }
                                 }
                             };
-                            g = h([u(0, d.IRenderService), u(1, d.ICharSizeService)], g), i.MouseService = g
+                            g = a([u(0, d.IRenderService), u(1, d.ICharSizeService)], g), i.MouseService = g
                         },
-                        3230: function(T, i, o) {
-                            var h = this && this.__decorate || function(r, l, f, m) {
-                                    var a, p = arguments.length,
+                        3230: function(T, i, h) {
+                            var a = this && this.__decorate || function(r, l, f, m) {
+                                    var o, p = arguments.length,
                                         C = p < 3 ? l : m === null ? m = Object.getOwnPropertyDescriptor(l, f) : m;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") C = Reflect.decorate(r, l, f, m);
                                     else
-                                        for (var y = r.length - 1; y >= 0; y--)(a = r[y]) && (C = (p < 3 ? a(C) : p > 3 ? a(l, f, C) : a(l, f)) || C);
+                                        for (var y = r.length - 1; y >= 0; y--)(o = r[y]) && (C = (p < 3 ? o(C) : p > 3 ? o(l, f, C) : o(l, f)) || C);
                                     return p > 3 && C && Object.defineProperty(l, f, C), C
                                 },
                                 u = this && this.__param || function(r, l) {
                                     return function(f, m) {
                                         l(f, m, r)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.RenderService = void 0;
-                            const d = o(6193),
-                                _ = o(8460),
-                                g = o(844),
-                                v = o(5596),
-                                c = o(3656),
-                                e = o(2585),
-                                s = o(4725),
-                                n = o(7226);
+                            const d = h(6193),
+                                _ = h(8460),
+                                g = h(844),
+                                v = h(5596),
+                                c = h(3656),
+                                e = h(2585),
+                                s = h(4725),
+                                n = h(7226);
                             let t = class extends g.Disposable {
-                                constructor(r, l, f, m, a, p, C, y) {
+                                constructor(r, l, f, m, o, p, C, y) {
                                     if (super(), this._rowCount = r, this._charSizeService = m, this._pausedResizeTask = new n.DebouncedIdleTask, this._isPaused = !1, this._needsFullRefresh = !1, this._isNextRenderRedrawOnly = !0, this._needsSelectionRefresh = !1, this._canvasWidth = 0, this._canvasHeight = 0, this._selectionState = {
                                             start: void 0,
                                             end: void 0,
                                             columnSelectMode: !1
                                         }, this._onDimensionsChange = this.register(new _.EventEmitter), this.onDimensionsChange = this._onDimensionsChange.event, this._onRenderedViewportChange = this.register(new _.EventEmitter), this.onRenderedViewportChange = this._onRenderedViewportChange.event, this._onRender = this.register(new _.EventEmitter), this.onRender = this._onRender.event, this._onRefreshRequest = this.register(new _.EventEmitter), this.onRefreshRequest = this._onRefreshRequest.event, this.register({
                                             dispose: () => {
                                                 var w;
                                                 return (w = this._renderer) === null || w === void 0 ? void 0 : w.dispose()
                                             }
                                         }), this._renderDebouncer = new d.RenderDebouncer(C.window, (w, D) => this._renderRows(w, D)), this.register(this._renderDebouncer), this._screenDprMonitor = new v.ScreenDprMonitor(C.window), this._screenDprMonitor.setListener(() => this.handleDevicePixelRatioChange()), this.register(this._screenDprMonitor), this.register(p.onResize(() => this._fullRefresh())), this.register(p.buffers.onBufferActivate(() => {
                                             var w;
                                             return (w = this._renderer) === null || w === void 0 ? void 0 : w.clear()
-                                        })), this.register(f.onOptionChange(() => this._handleOptionsChanged())), this.register(this._charSizeService.onCharSizeChange(() => this.handleCharSizeChanged())), this.register(a.onDecorationRegistered(() => this._fullRefresh())), this.register(a.onDecorationRemoved(() => this._fullRefresh())), this.register(f.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio"], () => {
+                                        })), this.register(f.onOptionChange(() => this._handleOptionsChanged())), this.register(this._charSizeService.onCharSizeChange(() => this.handleCharSizeChanged())), this.register(o.onDecorationRegistered(() => this._fullRefresh())), this.register(o.onDecorationRemoved(() => this._fullRefresh())), this.register(f.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio"], () => {
                                             this.clear(), this.handleResize(p.cols, p.rows), this._fullRefresh()
                                         })), this.register(f.onMultipleOptionChange(["cursorBlink", "cursorStyle"], () => this.refreshRows(p.buffer.y, p.buffer.y, !0))), this.register((0, c.addDisposableDomListener)(C.window, "resize", () => this.handleDevicePixelRatioChange())), this.register(y.onChangeColors(() => this._fullRefresh())), "IntersectionObserver" in C.window) {
                                         const w = new C.window.IntersectionObserver(D => this._handleIntersectionChange(D[D.length - 1]), {
                                             threshold: 0
                                         });
                                         w.observe(l), this.register({
                                             dispose: () => w.disconnect()
@@ -2248,48 +2248,48 @@
                                     (r = this._renderer) === null || r === void 0 || r.handleCursorMove()
                                 }
                                 clear() {
                                     var r;
                                     (r = this._renderer) === null || r === void 0 || r.clear()
                                 }
                             };
-                            t = h([u(2, e.IOptionsService), u(3, s.ICharSizeService), u(4, e.IDecorationService), u(5, e.IBufferService), u(6, s.ICoreBrowserService), u(7, s.IThemeService)], t), i.RenderService = t
+                            t = a([u(2, e.IOptionsService), u(3, s.ICharSizeService), u(4, e.IDecorationService), u(5, e.IBufferService), u(6, s.ICoreBrowserService), u(7, s.IThemeService)], t), i.RenderService = t
                         },
-                        9312: function(T, i, o) {
-                            var h = this && this.__decorate || function(a, p, C, y) {
+                        9312: function(T, i, h) {
+                            var a = this && this.__decorate || function(o, p, C, y) {
                                     var w, D = arguments.length,
                                         x = D < 3 ? p : y === null ? y = Object.getOwnPropertyDescriptor(p, C) : y;
-                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") x = Reflect.decorate(a, p, C, y);
+                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") x = Reflect.decorate(o, p, C, y);
                                     else
-                                        for (var I = a.length - 1; I >= 0; I--)(w = a[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
+                                        for (var I = o.length - 1; I >= 0; I--)(w = o[I]) && (x = (D < 3 ? w(x) : D > 3 ? w(p, C, x) : w(p, C)) || x);
                                     return D > 3 && x && Object.defineProperty(p, C, x), x
                                 },
-                                u = this && this.__param || function(a, p) {
+                                u = this && this.__param || function(o, p) {
                                     return function(C, y) {
-                                        p(C, y, a)
+                                        p(C, y, o)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.SelectionService = void 0;
-                            const d = o(6114),
-                                _ = o(456),
-                                g = o(511),
-                                v = o(8460),
-                                c = o(4725),
-                                e = o(2585),
-                                s = o(9806),
-                                n = o(9504),
-                                t = o(844),
-                                r = o(4841),
+                            const d = h(6114),
+                                _ = h(456),
+                                g = h(511),
+                                v = h(8460),
+                                c = h(4725),
+                                e = h(2585),
+                                s = h(9806),
+                                n = h(9504),
+                                t = h(844),
+                                r = h(4841),
                                 l = String.fromCharCode(160),
                                 f = new RegExp(l, "g");
                             let m = class extends t.Disposable {
-                                constructor(a, p, C, y, w, D, x, I, H) {
-                                    super(), this._element = a, this._screenElement = p, this._linkifier = C, this._bufferService = y, this._coreService = w, this._mouseService = D, this._optionsService = x, this._renderService = I, this._coreBrowserService = H, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new g.CellData, this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new v.EventEmitter), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new v.EventEmitter), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new v.EventEmitter), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new v.EventEmitter), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = S => this._handleMouseMove(S), this._mouseUpListener = S => this._handleMouseUp(S), this._coreService.onUserInput(() => {
+                                constructor(o, p, C, y, w, D, x, I, H) {
+                                    super(), this._element = o, this._screenElement = p, this._linkifier = C, this._bufferService = y, this._coreService = w, this._mouseService = D, this._optionsService = x, this._renderService = I, this._coreBrowserService = H, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new g.CellData, this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new v.EventEmitter), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new v.EventEmitter), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new v.EventEmitter), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new v.EventEmitter), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = S => this._handleMouseMove(S), this._mouseUpListener = S => this._handleMouseUp(S), this._coreService.onUserInput(() => {
                                         this.hasSelection && this.clearSelection()
                                     }), this._trimListener = this._bufferService.buffer.lines.onTrim(S => this._handleTrim(S)), this.register(this._bufferService.buffers.onBufferActivate(S => this._handleBufferActivate(S))), this.enable(), this._model = new _.SelectionModel(this._bufferService), this._activeSelectionMode = 0, this.register((0, t.toDisposable)(() => {
                                         this._removeMouseDownListeners()
                                     }))
                                 }
                                 reset() {
                                     this.clearSelection()
@@ -2303,218 +2303,218 @@
                                 get selectionStart() {
                                     return this._model.finalSelectionStart
                                 }
                                 get selectionEnd() {
                                     return this._model.finalSelectionEnd
                                 }
                                 get hasSelection() {
-                                    const a = this._model.finalSelectionStart,
+                                    const o = this._model.finalSelectionStart,
                                         p = this._model.finalSelectionEnd;
-                                    return !(!a || !p || a[0] === p[0] && a[1] === p[1])
+                                    return !(!o || !p || o[0] === p[0] && o[1] === p[1])
                                 }
                                 get selectionText() {
-                                    const a = this._model.finalSelectionStart,
+                                    const o = this._model.finalSelectionStart,
                                         p = this._model.finalSelectionEnd;
-                                    if (!a || !p) return "";
+                                    if (!o || !p) return "";
                                     const C = this._bufferService.buffer,
                                         y = [];
                                     if (this._activeSelectionMode === 3) {
-                                        if (a[0] === p[0]) return "";
-                                        const w = a[0] < p[0] ? a[0] : p[0],
-                                            D = a[0] < p[0] ? p[0] : a[0];
-                                        for (let x = a[1]; x <= p[1]; x++) {
+                                        if (o[0] === p[0]) return "";
+                                        const w = o[0] < p[0] ? o[0] : p[0],
+                                            D = o[0] < p[0] ? p[0] : o[0];
+                                        for (let x = o[1]; x <= p[1]; x++) {
                                             const I = C.translateBufferLineToString(x, !0, w, D);
                                             y.push(I)
                                         }
                                     } else {
-                                        const w = a[1] === p[1] ? p[0] : void 0;
-                                        y.push(C.translateBufferLineToString(a[1], !0, a[0], w));
-                                        for (let D = a[1] + 1; D <= p[1] - 1; D++) {
+                                        const w = o[1] === p[1] ? p[0] : void 0;
+                                        y.push(C.translateBufferLineToString(o[1], !0, o[0], w));
+                                        for (let D = o[1] + 1; D <= p[1] - 1; D++) {
                                             const x = C.lines.get(D),
                                                 I = C.translateBufferLineToString(D, !0);
                                             x != null && x.isWrapped ? y[y.length - 1] += I : y.push(I)
                                         }
-                                        if (a[1] !== p[1]) {
+                                        if (o[1] !== p[1]) {
                                             const D = C.lines.get(p[1]),
                                                 x = C.translateBufferLineToString(p[1], !0, 0, p[0]);
                                             D && D.isWrapped ? y[y.length - 1] += x : y.push(x)
                                         }
                                     }
                                     return y.map(w => w.replace(f, " ")).join(d.isWindows ? `\r
 ` : `
 `)
                                 }
                                 clearSelection() {
                                     this._model.clearSelection(), this._removeMouseDownListeners(), this.refresh(), this._onSelectionChange.fire()
                                 }
-                                refresh(a) {
-                                    this._refreshAnimationFrame || (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame(() => this._refresh())), d.isLinux && a && this.selectionText.length && this._onLinuxMouseSelection.fire(this.selectionText)
+                                refresh(o) {
+                                    this._refreshAnimationFrame || (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame(() => this._refresh())), d.isLinux && o && this.selectionText.length && this._onLinuxMouseSelection.fire(this.selectionText)
                                 }
                                 _refresh() {
                                     this._refreshAnimationFrame = void 0, this._onRedrawRequest.fire({
                                         start: this._model.finalSelectionStart,
                                         end: this._model.finalSelectionEnd,
                                         columnSelectMode: this._activeSelectionMode === 3
                                     })
                                 }
-                                _isClickInSelection(a) {
-                                    const p = this._getMouseBufferCoords(a),
+                                _isClickInSelection(o) {
+                                    const p = this._getMouseBufferCoords(o),
                                         C = this._model.finalSelectionStart,
                                         y = this._model.finalSelectionEnd;
                                     return !!(C && y && p) && this._areCoordsInSelection(p, C, y)
                                 }
-                                isCellInSelection(a, p) {
+                                isCellInSelection(o, p) {
                                     const C = this._model.finalSelectionStart,
                                         y = this._model.finalSelectionEnd;
-                                    return !(!C || !y) && this._areCoordsInSelection([a, p], C, y)
+                                    return !(!C || !y) && this._areCoordsInSelection([o, p], C, y)
                                 }
-                                _areCoordsInSelection(a, p, C) {
-                                    return a[1] > p[1] && a[1] < C[1] || p[1] === C[1] && a[1] === p[1] && a[0] >= p[0] && a[0] < C[0] || p[1] < C[1] && a[1] === C[1] && a[0] < C[0] || p[1] < C[1] && a[1] === p[1] && a[0] >= p[0]
+                                _areCoordsInSelection(o, p, C) {
+                                    return o[1] > p[1] && o[1] < C[1] || p[1] === C[1] && o[1] === p[1] && o[0] >= p[0] && o[0] < C[0] || p[1] < C[1] && o[1] === C[1] && o[0] < C[0] || p[1] < C[1] && o[1] === p[1] && o[0] >= p[0]
                                 }
-                                _selectWordAtCursor(a, p) {
+                                _selectWordAtCursor(o, p) {
                                     var C, y;
                                     const w = (y = (C = this._linkifier.currentLink) === null || C === void 0 ? void 0 : C.link) === null || y === void 0 ? void 0 : y.range;
                                     if (w) return this._model.selectionStart = [w.start.x - 1, w.start.y - 1], this._model.selectionStartLength = (0, r.getRangeLength)(w, this._bufferService.cols), this._model.selectionEnd = void 0, !0;
-                                    const D = this._getMouseBufferCoords(a);
+                                    const D = this._getMouseBufferCoords(o);
                                     return !!D && (this._selectWordAt(D, p), this._model.selectionEnd = void 0, !0)
                                 }
                                 selectAll() {
                                     this._model.isSelectAllActive = !0, this.refresh(), this._onSelectionChange.fire()
                                 }
-                                selectLines(a, p) {
-                                    this._model.clearSelection(), a = Math.max(a, 0), p = Math.min(p, this._bufferService.buffer.lines.length - 1), this._model.selectionStart = [0, a], this._model.selectionEnd = [this._bufferService.cols, p], this.refresh(), this._onSelectionChange.fire()
+                                selectLines(o, p) {
+                                    this._model.clearSelection(), o = Math.max(o, 0), p = Math.min(p, this._bufferService.buffer.lines.length - 1), this._model.selectionStart = [0, o], this._model.selectionEnd = [this._bufferService.cols, p], this.refresh(), this._onSelectionChange.fire()
                                 }
-                                _handleTrim(a) {
-                                    this._model.handleTrim(a) && this.refresh()
+                                _handleTrim(o) {
+                                    this._model.handleTrim(o) && this.refresh()
                                 }
-                                _getMouseBufferCoords(a) {
-                                    const p = this._mouseService.getCoords(a, this._screenElement, this._bufferService.cols, this._bufferService.rows, !0);
+                                _getMouseBufferCoords(o) {
+                                    const p = this._mouseService.getCoords(o, this._screenElement, this._bufferService.cols, this._bufferService.rows, !0);
                                     if (p) return p[0]--, p[1]--, p[1] += this._bufferService.buffer.ydisp, p
                                 }
-                                _getMouseEventScrollAmount(a) {
-                                    let p = (0, s.getCoordsRelativeToElement)(this._coreBrowserService.window, a, this._screenElement)[1];
+                                _getMouseEventScrollAmount(o) {
+                                    let p = (0, s.getCoordsRelativeToElement)(this._coreBrowserService.window, o, this._screenElement)[1];
                                     const C = this._renderService.dimensions.css.canvas.height;
                                     return p >= 0 && p <= C ? 0 : (p > C && (p -= C), p = Math.min(Math.max(p, -50), 50), p /= 50, p / Math.abs(p) + Math.round(14 * p))
                                 }
-                                shouldForceSelection(a) {
-                                    return d.isMac ? a.altKey && this._optionsService.rawOptions.macOptionClickForcesSelection : a.shiftKey
+                                shouldForceSelection(o) {
+                                    return d.isMac ? o.altKey && this._optionsService.rawOptions.macOptionClickForcesSelection : o.shiftKey
                                 }
-                                handleMouseDown(a) {
-                                    if (this._mouseDownTimeStamp = a.timeStamp, (a.button !== 2 || !this.hasSelection) && a.button === 0) {
+                                handleMouseDown(o) {
+                                    if (this._mouseDownTimeStamp = o.timeStamp, (o.button !== 2 || !this.hasSelection) && o.button === 0) {
                                         if (!this._enabled) {
-                                            if (!this.shouldForceSelection(a)) return;
-                                            a.stopPropagation()
+                                            if (!this.shouldForceSelection(o)) return;
+                                            o.stopPropagation()
                                         }
-                                        a.preventDefault(), this._dragScrollAmount = 0, this._enabled && a.shiftKey ? this._handleIncrementalClick(a) : a.detail === 1 ? this._handleSingleClick(a) : a.detail === 2 ? this._handleDoubleClick(a) : a.detail === 3 && this._handleTripleClick(a), this._addMouseDownListeners(), this.refresh(!0)
+                                        o.preventDefault(), this._dragScrollAmount = 0, this._enabled && o.shiftKey ? this._handleIncrementalClick(o) : o.detail === 1 ? this._handleSingleClick(o) : o.detail === 2 ? this._handleDoubleClick(o) : o.detail === 3 && this._handleTripleClick(o), this._addMouseDownListeners(), this.refresh(!0)
                                     }
                                 }
                                 _addMouseDownListeners() {
                                     this._screenElement.ownerDocument && (this._screenElement.ownerDocument.addEventListener("mousemove", this._mouseMoveListener), this._screenElement.ownerDocument.addEventListener("mouseup", this._mouseUpListener)), this._dragScrollIntervalTimer = this._coreBrowserService.window.setInterval(() => this._dragScroll(), 50)
                                 }
                                 _removeMouseDownListeners() {
                                     this._screenElement.ownerDocument && (this._screenElement.ownerDocument.removeEventListener("mousemove", this._mouseMoveListener), this._screenElement.ownerDocument.removeEventListener("mouseup", this._mouseUpListener)), this._coreBrowserService.window.clearInterval(this._dragScrollIntervalTimer), this._dragScrollIntervalTimer = void 0
                                 }
-                                _handleIncrementalClick(a) {
-                                    this._model.selectionStart && (this._model.selectionEnd = this._getMouseBufferCoords(a))
+                                _handleIncrementalClick(o) {
+                                    this._model.selectionStart && (this._model.selectionEnd = this._getMouseBufferCoords(o))
                                 }
-                                _handleSingleClick(a) {
-                                    if (this._model.selectionStartLength = 0, this._model.isSelectAllActive = !1, this._activeSelectionMode = this.shouldColumnSelect(a) ? 3 : 0, this._model.selectionStart = this._getMouseBufferCoords(a), !this._model.selectionStart) return;
+                                _handleSingleClick(o) {
+                                    if (this._model.selectionStartLength = 0, this._model.isSelectAllActive = !1, this._activeSelectionMode = this.shouldColumnSelect(o) ? 3 : 0, this._model.selectionStart = this._getMouseBufferCoords(o), !this._model.selectionStart) return;
                                     this._model.selectionEnd = void 0;
                                     const p = this._bufferService.buffer.lines.get(this._model.selectionStart[1]);
                                     p && p.length !== this._model.selectionStart[0] && p.hasWidth(this._model.selectionStart[0]) === 0 && this._model.selectionStart[0]++
                                 }
-                                _handleDoubleClick(a) {
-                                    this._selectWordAtCursor(a, !0) && (this._activeSelectionMode = 1)
+                                _handleDoubleClick(o) {
+                                    this._selectWordAtCursor(o, !0) && (this._activeSelectionMode = 1)
                                 }
-                                _handleTripleClick(a) {
-                                    const p = this._getMouseBufferCoords(a);
+                                _handleTripleClick(o) {
+                                    const p = this._getMouseBufferCoords(o);
                                     p && (this._activeSelectionMode = 2, this._selectLineAt(p[1]))
                                 }
-                                shouldColumnSelect(a) {
-                                    return a.altKey && !(d.isMac && this._optionsService.rawOptions.macOptionClickForcesSelection)
+                                shouldColumnSelect(o) {
+                                    return o.altKey && !(d.isMac && this._optionsService.rawOptions.macOptionClickForcesSelection)
                                 }
-                                _handleMouseMove(a) {
-                                    if (a.stopImmediatePropagation(), !this._model.selectionStart) return;
+                                _handleMouseMove(o) {
+                                    if (o.stopImmediatePropagation(), !this._model.selectionStart) return;
                                     const p = this._model.selectionEnd ? [this._model.selectionEnd[0], this._model.selectionEnd[1]] : null;
-                                    if (this._model.selectionEnd = this._getMouseBufferCoords(a), !this._model.selectionEnd) return void this.refresh(!0);
-                                    this._activeSelectionMode === 2 ? this._model.selectionEnd[1] < this._model.selectionStart[1] ? this._model.selectionEnd[0] = 0 : this._model.selectionEnd[0] = this._bufferService.cols : this._activeSelectionMode === 1 && this._selectToWordAt(this._model.selectionEnd), this._dragScrollAmount = this._getMouseEventScrollAmount(a), this._activeSelectionMode !== 3 && (this._dragScrollAmount > 0 ? this._model.selectionEnd[0] = this._bufferService.cols : this._dragScrollAmount < 0 && (this._model.selectionEnd[0] = 0));
+                                    if (this._model.selectionEnd = this._getMouseBufferCoords(o), !this._model.selectionEnd) return void this.refresh(!0);
+                                    this._activeSelectionMode === 2 ? this._model.selectionEnd[1] < this._model.selectionStart[1] ? this._model.selectionEnd[0] = 0 : this._model.selectionEnd[0] = this._bufferService.cols : this._activeSelectionMode === 1 && this._selectToWordAt(this._model.selectionEnd), this._dragScrollAmount = this._getMouseEventScrollAmount(o), this._activeSelectionMode !== 3 && (this._dragScrollAmount > 0 ? this._model.selectionEnd[0] = this._bufferService.cols : this._dragScrollAmount < 0 && (this._model.selectionEnd[0] = 0));
                                     const C = this._bufferService.buffer;
                                     if (this._model.selectionEnd[1] < C.lines.length) {
                                         const y = C.lines.get(this._model.selectionEnd[1]);
                                         y && y.hasWidth(this._model.selectionEnd[0]) === 0 && this._model.selectionEnd[0]++
                                     }
                                     p && p[0] === this._model.selectionEnd[0] && p[1] === this._model.selectionEnd[1] || this.refresh(!0)
                                 }
                                 _dragScroll() {
                                     if (this._model.selectionEnd && this._model.selectionStart && this._dragScrollAmount) {
                                         this._onRequestScrollLines.fire({
                                             amount: this._dragScrollAmount,
                                             suppressScrollEvent: !1
                                         });
-                                        const a = this._bufferService.buffer;
-                                        this._dragScrollAmount > 0 ? (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = this._bufferService.cols), this._model.selectionEnd[1] = Math.min(a.ydisp + this._bufferService.rows, a.lines.length - 1)) : (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = 0), this._model.selectionEnd[1] = a.ydisp), this.refresh()
+                                        const o = this._bufferService.buffer;
+                                        this._dragScrollAmount > 0 ? (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = this._bufferService.cols), this._model.selectionEnd[1] = Math.min(o.ydisp + this._bufferService.rows, o.lines.length - 1)) : (this._activeSelectionMode !== 3 && (this._model.selectionEnd[0] = 0), this._model.selectionEnd[1] = o.ydisp), this.refresh()
                                     }
                                 }
-                                _handleMouseUp(a) {
-                                    const p = a.timeStamp - this._mouseDownTimeStamp;
-                                    if (this._removeMouseDownListeners(), this.selectionText.length <= 1 && p < 500 && a.altKey && this._optionsService.rawOptions.altClickMovesCursor) {
+                                _handleMouseUp(o) {
+                                    const p = o.timeStamp - this._mouseDownTimeStamp;
+                                    if (this._removeMouseDownListeners(), this.selectionText.length <= 1 && p < 500 && o.altKey && this._optionsService.rawOptions.altClickMovesCursor) {
                                         if (this._bufferService.buffer.ybase === this._bufferService.buffer.ydisp) {
-                                            const C = this._mouseService.getCoords(a, this._element, this._bufferService.cols, this._bufferService.rows, !1);
+                                            const C = this._mouseService.getCoords(o, this._element, this._bufferService.cols, this._bufferService.rows, !1);
                                             if (C && C[0] !== void 0 && C[1] !== void 0) {
                                                 const y = (0, n.moveToCellSequence)(C[0] - 1, C[1] - 1, this._bufferService, this._coreService.decPrivateModes.applicationCursorKeys);
                                                 this._coreService.triggerDataEvent(y, !0)
                                             }
                                         }
                                     } else this._fireEventIfSelectionChanged()
                                 }
                                 _fireEventIfSelectionChanged() {
-                                    const a = this._model.finalSelectionStart,
+                                    const o = this._model.finalSelectionStart,
                                         p = this._model.finalSelectionEnd,
-                                        C = !(!a || !p || a[0] === p[0] && a[1] === p[1]);
-                                    C ? a && p && (this._oldSelectionStart && this._oldSelectionEnd && a[0] === this._oldSelectionStart[0] && a[1] === this._oldSelectionStart[1] && p[0] === this._oldSelectionEnd[0] && p[1] === this._oldSelectionEnd[1] || this._fireOnSelectionChange(a, p, C)) : this._oldHasSelection && this._fireOnSelectionChange(a, p, C)
+                                        C = !(!o || !p || o[0] === p[0] && o[1] === p[1]);
+                                    C ? o && p && (this._oldSelectionStart && this._oldSelectionEnd && o[0] === this._oldSelectionStart[0] && o[1] === this._oldSelectionStart[1] && p[0] === this._oldSelectionEnd[0] && p[1] === this._oldSelectionEnd[1] || this._fireOnSelectionChange(o, p, C)) : this._oldHasSelection && this._fireOnSelectionChange(o, p, C)
                                 }
-                                _fireOnSelectionChange(a, p, C) {
-                                    this._oldSelectionStart = a, this._oldSelectionEnd = p, this._oldHasSelection = C, this._onSelectionChange.fire()
+                                _fireOnSelectionChange(o, p, C) {
+                                    this._oldSelectionStart = o, this._oldSelectionEnd = p, this._oldHasSelection = C, this._onSelectionChange.fire()
                                 }
-                                _handleBufferActivate(a) {
-                                    this.clearSelection(), this._trimListener.dispose(), this._trimListener = a.activeBuffer.lines.onTrim(p => this._handleTrim(p))
+                                _handleBufferActivate(o) {
+                                    this.clearSelection(), this._trimListener.dispose(), this._trimListener = o.activeBuffer.lines.onTrim(p => this._handleTrim(p))
                                 }
-                                _convertViewportColToCharacterIndex(a, p) {
+                                _convertViewportColToCharacterIndex(o, p) {
                                     let C = p;
                                     for (let y = 0; p >= y; y++) {
-                                        const w = a.loadCell(y, this._workCell).getChars().length;
+                                        const w = o.loadCell(y, this._workCell).getChars().length;
                                         this._workCell.getWidth() === 0 ? C-- : w > 1 && p !== y && (C += w - 1)
                                     }
                                     return C
                                 }
-                                setSelection(a, p, C) {
-                                    this._model.clearSelection(), this._removeMouseDownListeners(), this._model.selectionStart = [a, p], this._model.selectionStartLength = C, this.refresh(), this._fireEventIfSelectionChanged()
+                                setSelection(o, p, C) {
+                                    this._model.clearSelection(), this._removeMouseDownListeners(), this._model.selectionStart = [o, p], this._model.selectionStartLength = C, this.refresh(), this._fireEventIfSelectionChanged()
                                 }
-                                rightClickSelect(a) {
-                                    this._isClickInSelection(a) || (this._selectWordAtCursor(a, !1) && this.refresh(!0), this._fireEventIfSelectionChanged())
+                                rightClickSelect(o) {
+                                    this._isClickInSelection(o) || (this._selectWordAtCursor(o, !1) && this.refresh(!0), this._fireEventIfSelectionChanged())
                                 }
-                                _getWordAt(a, p, C = !0, y = !0) {
-                                    if (a[0] >= this._bufferService.cols) return;
+                                _getWordAt(o, p, C = !0, y = !0) {
+                                    if (o[0] >= this._bufferService.cols) return;
                                     const w = this._bufferService.buffer,
-                                        D = w.lines.get(a[1]);
+                                        D = w.lines.get(o[1]);
                                     if (!D) return;
-                                    const x = w.translateBufferLineToString(a[1], !1);
-                                    let I = this._convertViewportColToCharacterIndex(D, a[0]),
+                                    const x = w.translateBufferLineToString(o[1], !1);
+                                    let I = this._convertViewportColToCharacterIndex(D, o[0]),
                                         H = I;
-                                    const S = a[0] - I;
+                                    const S = o[0] - I;
                                     let b = 0,
                                         L = 0,
                                         R = 0,
                                         M = 0;
                                     if (x.charAt(I) === " ") {
                                         for (; I > 0 && x.charAt(I - 1) === " ";) I--;
                                         for (; H < x.length && x.charAt(H + 1) === " ";) H++
                                     } else {
-                                        let O = a[0],
-                                            N = a[0];
+                                        let O = o[0],
+                                            N = o[0];
                                         D.getWidth(O) === 0 && (b++, O--), D.getWidth(N) === 2 && (L++, N++);
                                         const k = D.getString(N).length;
                                         for (k > 1 && (M += k - 1, H += k - 1); O > 0 && I > 0 && !this._isCharWordSeparator(D.loadCell(O - 1, this._workCell));) {
                                             D.loadCell(O - 1, this._workCell);
                                             const E = this._workCell.getChars().length;
                                             this._workCell.getWidth() === 0 ? (b++, O--) : E > 1 && (R += E - 1, I -= E - 1), I--, O--
                                         }
@@ -2525,117 +2525,117 @@
                                         }
                                     }
                                     H++;
                                     let F = I + S - b + R,
                                         j = Math.min(this._bufferService.cols, H - I + b + L - R - M);
                                     if (p || x.slice(I, H).trim() !== "") {
                                         if (C && F === 0 && D.getCodePoint(0) !== 32) {
-                                            const O = w.lines.get(a[1] - 1);
+                                            const O = w.lines.get(o[1] - 1);
                                             if (O && D.isWrapped && O.getCodePoint(this._bufferService.cols - 1) !== 32) {
-                                                const N = this._getWordAt([this._bufferService.cols - 1, a[1] - 1], !1, !0, !1);
+                                                const N = this._getWordAt([this._bufferService.cols - 1, o[1] - 1], !1, !0, !1);
                                                 if (N) {
                                                     const k = this._bufferService.cols - N.start;
                                                     F -= k, j += k
                                                 }
                                             }
                                         }
                                         if (y && F + j === this._bufferService.cols && D.getCodePoint(this._bufferService.cols - 1) !== 32) {
-                                            const O = w.lines.get(a[1] + 1);
+                                            const O = w.lines.get(o[1] + 1);
                                             if (O != null && O.isWrapped && O.getCodePoint(0) !== 32) {
-                                                const N = this._getWordAt([0, a[1] + 1], !1, !1, !0);
+                                                const N = this._getWordAt([0, o[1] + 1], !1, !1, !0);
                                                 N && (j += N.length)
                                             }
                                         }
                                         return {
                                             start: F,
                                             length: j
                                         }
                                     }
                                 }
-                                _selectWordAt(a, p) {
-                                    const C = this._getWordAt(a, p);
+                                _selectWordAt(o, p) {
+                                    const C = this._getWordAt(o, p);
                                     if (C) {
-                                        for (; C.start < 0;) C.start += this._bufferService.cols, a[1]--;
-                                        this._model.selectionStart = [C.start, a[1]], this._model.selectionStartLength = C.length
+                                        for (; C.start < 0;) C.start += this._bufferService.cols, o[1]--;
+                                        this._model.selectionStart = [C.start, o[1]], this._model.selectionStartLength = C.length
                                     }
                                 }
-                                _selectToWordAt(a) {
-                                    const p = this._getWordAt(a, !0);
+                                _selectToWordAt(o) {
+                                    const p = this._getWordAt(o, !0);
                                     if (p) {
-                                        let C = a[1];
+                                        let C = o[1];
                                         for (; p.start < 0;) p.start += this._bufferService.cols, C--;
                                         if (!this._model.areSelectionValuesReversed())
                                             for (; p.start + p.length > this._bufferService.cols;) p.length -= this._bufferService.cols, C++;
                                         this._model.selectionEnd = [this._model.areSelectionValuesReversed() ? p.start : p.start + p.length, C]
                                     }
                                 }
-                                _isCharWordSeparator(a) {
-                                    return a.getWidth() !== 0 && this._optionsService.rawOptions.wordSeparator.indexOf(a.getChars()) >= 0
+                                _isCharWordSeparator(o) {
+                                    return o.getWidth() !== 0 && this._optionsService.rawOptions.wordSeparator.indexOf(o.getChars()) >= 0
                                 }
-                                _selectLineAt(a) {
-                                    const p = this._bufferService.buffer.getWrappedRangeForLine(a),
+                                _selectLineAt(o) {
+                                    const p = this._bufferService.buffer.getWrappedRangeForLine(o),
                                         C = {
                                             start: {
                                                 x: 0,
                                                 y: p.first
                                             },
                                             end: {
                                                 x: this._bufferService.cols - 1,
                                                 y: p.last
                                             }
                                         };
                                     this._model.selectionStart = [0, p.first], this._model.selectionEnd = void 0, this._model.selectionStartLength = (0, r.getRangeLength)(C, this._bufferService.cols)
                                 }
                             };
-                            m = h([u(3, e.IBufferService), u(4, e.ICoreService), u(5, c.IMouseService), u(6, e.IOptionsService), u(7, c.IRenderService), u(8, c.ICoreBrowserService)], m), i.SelectionService = m
+                            m = a([u(3, e.IBufferService), u(4, e.ICoreService), u(5, c.IMouseService), u(6, e.IOptionsService), u(7, c.IRenderService), u(8, c.ICoreBrowserService)], m), i.SelectionService = m
                         },
-                        4725: (T, i, o) => {
+                        4725: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.IThemeService = i.ICharacterJoinerService = i.ISelectionService = i.IRenderService = i.IMouseService = i.ICoreBrowserService = i.ICharSizeService = void 0;
-                            const h = o(8343);
-                            i.ICharSizeService = (0, h.createDecorator)("CharSizeService"), i.ICoreBrowserService = (0, h.createDecorator)("CoreBrowserService"), i.IMouseService = (0, h.createDecorator)("MouseService"), i.IRenderService = (0, h.createDecorator)("RenderService"), i.ISelectionService = (0, h.createDecorator)("SelectionService"), i.ICharacterJoinerService = (0, h.createDecorator)("CharacterJoinerService"), i.IThemeService = (0, h.createDecorator)("ThemeService")
+                            const a = h(8343);
+                            i.ICharSizeService = (0, a.createDecorator)("CharSizeService"), i.ICoreBrowserService = (0, a.createDecorator)("CoreBrowserService"), i.IMouseService = (0, a.createDecorator)("MouseService"), i.IRenderService = (0, a.createDecorator)("RenderService"), i.ISelectionService = (0, a.createDecorator)("SelectionService"), i.ICharacterJoinerService = (0, a.createDecorator)("CharacterJoinerService"), i.IThemeService = (0, a.createDecorator)("ThemeService")
                         },
-                        6731: function(T, i, o) {
-                            var h = this && this.__decorate || function(m, a, p, C) {
+                        6731: function(T, i, h) {
+                            var a = this && this.__decorate || function(m, o, p, C) {
                                     var y, w = arguments.length,
-                                        D = w < 3 ? a : C === null ? C = Object.getOwnPropertyDescriptor(a, p) : C;
-                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") D = Reflect.decorate(m, a, p, C);
+                                        D = w < 3 ? o : C === null ? C = Object.getOwnPropertyDescriptor(o, p) : C;
+                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") D = Reflect.decorate(m, o, p, C);
                                     else
-                                        for (var x = m.length - 1; x >= 0; x--)(y = m[x]) && (D = (w < 3 ? y(D) : w > 3 ? y(a, p, D) : y(a, p)) || D);
-                                    return w > 3 && D && Object.defineProperty(a, p, D), D
+                                        for (var x = m.length - 1; x >= 0; x--)(y = m[x]) && (D = (w < 3 ? y(D) : w > 3 ? y(o, p, D) : y(o, p)) || D);
+                                    return w > 3 && D && Object.defineProperty(o, p, D), D
                                 },
-                                u = this && this.__param || function(m, a) {
+                                u = this && this.__param || function(m, o) {
                                     return function(p, C) {
-                                        a(p, C, m)
+                                        o(p, C, m)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.ThemeService = i.DEFAULT_ANSI_COLORS = void 0;
-                            const d = o(7239),
-                                _ = o(8055),
-                                g = o(8460),
-                                v = o(844),
-                                c = o(2585),
+                            const d = h(7239),
+                                _ = h(8055),
+                                g = h(8460),
+                                v = h(844),
+                                c = h(2585),
                                 e = _.css.toColor("#ffffff"),
                                 s = _.css.toColor("#000000"),
                                 n = _.css.toColor("#ffffff"),
                                 t = _.css.toColor("#000000"),
                                 r = {
                                     css: "rgba(255, 255, 255, 0.3)",
                                     rgba: 4294967117
                                 };
                             i.DEFAULT_ANSI_COLORS = Object.freeze((() => {
                                 const m = [_.css.toColor("#2e3436"), _.css.toColor("#cc0000"), _.css.toColor("#4e9a06"), _.css.toColor("#c4a000"), _.css.toColor("#3465a4"), _.css.toColor("#75507b"), _.css.toColor("#06989a"), _.css.toColor("#d3d7cf"), _.css.toColor("#555753"), _.css.toColor("#ef2929"), _.css.toColor("#8ae234"), _.css.toColor("#fce94f"), _.css.toColor("#729fcf"), _.css.toColor("#ad7fa8"), _.css.toColor("#34e2e2"), _.css.toColor("#eeeeec")],
-                                    a = [0, 95, 135, 175, 215, 255];
+                                    o = [0, 95, 135, 175, 215, 255];
                                 for (let p = 0; p < 216; p++) {
-                                    const C = a[p / 36 % 6 | 0],
-                                        y = a[p / 6 % 6 | 0],
-                                        w = a[p % 6];
+                                    const C = o[p / 36 % 6 | 0],
+                                        y = o[p / 6 % 6 | 0],
+                                        w = o[p % 6];
                                     m.push({
                                         css: _.channels.toCss(C, y, w),
                                         rgba: _.channels.toRgba(C, y, w)
                                     })
                                 }
                                 for (let p = 0; p < 24; p++) {
                                     const C = 8 + 10 * p;
@@ -2662,18 +2662,18 @@
                                         contrastCache: this._contrastCache
                                     }, this._updateRestoreColors(), this._setTheme(this._optionsService.rawOptions.theme), this.register(this._optionsService.onSpecificOptionChange("minimumContrastRatio", () => this._contrastCache.clear())), this.register(this._optionsService.onSpecificOptionChange("theme", () => this._setTheme(this._optionsService.rawOptions.theme)))
                                 }
                                 get colors() {
                                     return this._colors
                                 }
                                 _setTheme(m = {}) {
-                                    const a = this._colors;
-                                    if (a.foreground = f(m.foreground, e), a.background = f(m.background, s), a.cursor = f(m.cursor, n), a.cursorAccent = f(m.cursorAccent, t), a.selectionBackgroundTransparent = f(m.selectionBackground, r), a.selectionBackgroundOpaque = _.color.blend(a.background, a.selectionBackgroundTransparent), a.selectionInactiveBackgroundTransparent = f(m.selectionInactiveBackground, a.selectionBackgroundTransparent), a.selectionInactiveBackgroundOpaque = _.color.blend(a.background, a.selectionInactiveBackgroundTransparent), a.selectionForeground = m.selectionForeground ? f(m.selectionForeground, _.NULL_COLOR) : void 0, a.selectionForeground === _.NULL_COLOR && (a.selectionForeground = void 0), _.color.isOpaque(a.selectionBackgroundTransparent) && (a.selectionBackgroundTransparent = _.color.opacity(a.selectionBackgroundTransparent, .3)), _.color.isOpaque(a.selectionInactiveBackgroundTransparent) && (a.selectionInactiveBackgroundTransparent = _.color.opacity(a.selectionInactiveBackgroundTransparent, .3)), a.ansi = i.DEFAULT_ANSI_COLORS.slice(), a.ansi[0] = f(m.black, i.DEFAULT_ANSI_COLORS[0]), a.ansi[1] = f(m.red, i.DEFAULT_ANSI_COLORS[1]), a.ansi[2] = f(m.green, i.DEFAULT_ANSI_COLORS[2]), a.ansi[3] = f(m.yellow, i.DEFAULT_ANSI_COLORS[3]), a.ansi[4] = f(m.blue, i.DEFAULT_ANSI_COLORS[4]), a.ansi[5] = f(m.magenta, i.DEFAULT_ANSI_COLORS[5]), a.ansi[6] = f(m.cyan, i.DEFAULT_ANSI_COLORS[6]), a.ansi[7] = f(m.white, i.DEFAULT_ANSI_COLORS[7]), a.ansi[8] = f(m.brightBlack, i.DEFAULT_ANSI_COLORS[8]), a.ansi[9] = f(m.brightRed, i.DEFAULT_ANSI_COLORS[9]), a.ansi[10] = f(m.brightGreen, i.DEFAULT_ANSI_COLORS[10]), a.ansi[11] = f(m.brightYellow, i.DEFAULT_ANSI_COLORS[11]), a.ansi[12] = f(m.brightBlue, i.DEFAULT_ANSI_COLORS[12]), a.ansi[13] = f(m.brightMagenta, i.DEFAULT_ANSI_COLORS[13]), a.ansi[14] = f(m.brightCyan, i.DEFAULT_ANSI_COLORS[14]), a.ansi[15] = f(m.brightWhite, i.DEFAULT_ANSI_COLORS[15]), m.extendedAnsi) {
-                                        const p = Math.min(a.ansi.length - 16, m.extendedAnsi.length);
-                                        for (let C = 0; C < p; C++) a.ansi[C + 16] = f(m.extendedAnsi[C], i.DEFAULT_ANSI_COLORS[C + 16])
+                                    const o = this._colors;
+                                    if (o.foreground = f(m.foreground, e), o.background = f(m.background, s), o.cursor = f(m.cursor, n), o.cursorAccent = f(m.cursorAccent, t), o.selectionBackgroundTransparent = f(m.selectionBackground, r), o.selectionBackgroundOpaque = _.color.blend(o.background, o.selectionBackgroundTransparent), o.selectionInactiveBackgroundTransparent = f(m.selectionInactiveBackground, o.selectionBackgroundTransparent), o.selectionInactiveBackgroundOpaque = _.color.blend(o.background, o.selectionInactiveBackgroundTransparent), o.selectionForeground = m.selectionForeground ? f(m.selectionForeground, _.NULL_COLOR) : void 0, o.selectionForeground === _.NULL_COLOR && (o.selectionForeground = void 0), _.color.isOpaque(o.selectionBackgroundTransparent) && (o.selectionBackgroundTransparent = _.color.opacity(o.selectionBackgroundTransparent, .3)), _.color.isOpaque(o.selectionInactiveBackgroundTransparent) && (o.selectionInactiveBackgroundTransparent = _.color.opacity(o.selectionInactiveBackgroundTransparent, .3)), o.ansi = i.DEFAULT_ANSI_COLORS.slice(), o.ansi[0] = f(m.black, i.DEFAULT_ANSI_COLORS[0]), o.ansi[1] = f(m.red, i.DEFAULT_ANSI_COLORS[1]), o.ansi[2] = f(m.green, i.DEFAULT_ANSI_COLORS[2]), o.ansi[3] = f(m.yellow, i.DEFAULT_ANSI_COLORS[3]), o.ansi[4] = f(m.blue, i.DEFAULT_ANSI_COLORS[4]), o.ansi[5] = f(m.magenta, i.DEFAULT_ANSI_COLORS[5]), o.ansi[6] = f(m.cyan, i.DEFAULT_ANSI_COLORS[6]), o.ansi[7] = f(m.white, i.DEFAULT_ANSI_COLORS[7]), o.ansi[8] = f(m.brightBlack, i.DEFAULT_ANSI_COLORS[8]), o.ansi[9] = f(m.brightRed, i.DEFAULT_ANSI_COLORS[9]), o.ansi[10] = f(m.brightGreen, i.DEFAULT_ANSI_COLORS[10]), o.ansi[11] = f(m.brightYellow, i.DEFAULT_ANSI_COLORS[11]), o.ansi[12] = f(m.brightBlue, i.DEFAULT_ANSI_COLORS[12]), o.ansi[13] = f(m.brightMagenta, i.DEFAULT_ANSI_COLORS[13]), o.ansi[14] = f(m.brightCyan, i.DEFAULT_ANSI_COLORS[14]), o.ansi[15] = f(m.brightWhite, i.DEFAULT_ANSI_COLORS[15]), m.extendedAnsi) {
+                                        const p = Math.min(o.ansi.length - 16, m.extendedAnsi.length);
+                                        for (let C = 0; C < p; C++) o.ansi[C + 16] = f(m.extendedAnsi[C], i.DEFAULT_ANSI_COLORS[C + 16])
                                     }
                                     this._contrastCache.clear(), this._updateRestoreColors(), this._onChangeColors.fire(this.colors)
                                 }
                                 restoreColor(m) {
                                     this._restoreColor(m), this._onChangeColors.fire(this.colors)
                                 }
                                 _restoreColor(m) {
@@ -2686,46 +2686,46 @@
                                             break;
                                         case 258:
                                             this._colors.cursor = this._restoreColors.cursor;
                                             break;
                                         default:
                                             this._colors.ansi[m] = this._restoreColors.ansi[m]
                                     } else
-                                        for (let a = 0; a < this._restoreColors.ansi.length; ++a) this._colors.ansi[a] = this._restoreColors.ansi[a]
+                                        for (let o = 0; o < this._restoreColors.ansi.length; ++o) this._colors.ansi[o] = this._restoreColors.ansi[o]
                                 }
                                 modifyColors(m) {
                                     m(this._colors), this._onChangeColors.fire(this.colors)
                                 }
                                 _updateRestoreColors() {
                                     this._restoreColors = {
                                         foreground: this._colors.foreground,
                                         background: this._colors.background,
                                         cursor: this._colors.cursor,
                                         ansi: this._colors.ansi.slice()
                                     }
                                 }
                             };
 
-                            function f(m, a) {
+                            function f(m, o) {
                                 if (m !== void 0) try {
                                     return _.css.toColor(m)
                                 } catch {}
-                                return a
+                                return o
                             }
-                            l = h([u(0, c.IOptionsService)], l), i.ThemeService = l
+                            l = a([u(0, c.IOptionsService)], l), i.ThemeService = l
                         },
-                        6349: (T, i, o) => {
+                        6349: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CircularList = void 0;
-                            const h = o(8460),
-                                u = o(844);
+                            const a = h(8460),
+                                u = h(844);
                             class d extends u.Disposable {
                                 constructor(g) {
-                                    super(), this._maxLength = g, this.onDeleteEmitter = this.register(new h.EventEmitter), this.onDelete = this.onDeleteEmitter.event, this.onInsertEmitter = this.register(new h.EventEmitter), this.onInsert = this.onInsertEmitter.event, this.onTrimEmitter = this.register(new h.EventEmitter), this.onTrim = this.onTrimEmitter.event, this._array = new Array(this._maxLength), this._startIndex = 0, this._length = 0
+                                    super(), this._maxLength = g, this.onDeleteEmitter = this.register(new a.EventEmitter), this.onDelete = this.onDeleteEmitter.event, this.onInsertEmitter = this.register(new a.EventEmitter), this.onInsert = this.onInsertEmitter.event, this.onTrimEmitter = this.register(new a.EventEmitter), this.onTrim = this.onTrimEmitter.event, this._array = new Array(this._maxLength), this._startIndex = 0, this._length = 0
                                 }
                                 get maxLength() {
                                     return this._maxLength
                                 }
                                 set maxLength(g) {
                                     if (this._maxLength === g) return;
                                     const v = new Array(g);
@@ -2798,26 +2798,26 @@
                                 }
                             }
                             i.CircularList = d
                         },
                         1439: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.clone = void 0, i.clone = function o(h, u = 5) {
-                                if (typeof h != "object") return h;
-                                const d = Array.isArray(h) ? [] : {};
-                                for (const _ in h) d[_] = u <= 1 ? h[_] : h[_] && o(h[_], u - 1);
+                            }), i.clone = void 0, i.clone = function h(a, u = 5) {
+                                if (typeof a != "object") return a;
+                                const d = Array.isArray(a) ? [] : {};
+                                for (const _ in a) d[_] = u <= 1 ? a[_] : a[_] && h(a[_], u - 1);
                                 return d
                             }
                         },
-                        8055: (T, i, o) => {
+                        8055: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.contrastRatio = i.toPaddedHex = i.rgba = i.rgb = i.css = i.color = i.channels = i.NULL_COLOR = void 0;
-                            const h = o(6114);
+                            const a = h(6114);
                             let u = 0,
                                 d = 0,
                                 _ = 0,
                                 g = 0;
                             var v, c, e;
 
                             function s(t) {
@@ -2848,43 +2848,43 @@
                                     }
                                     t.blend = function(l, f) {
                                         if (g = (255 & f.rgba) / 255, g === 1) return {
                                             css: f.css,
                                             rgba: f.rgba
                                         };
                                         const m = f.rgba >> 24 & 255,
-                                            a = f.rgba >> 16 & 255,
+                                            o = f.rgba >> 16 & 255,
                                             p = f.rgba >> 8 & 255,
                                             C = l.rgba >> 24 & 255,
                                             y = l.rgba >> 16 & 255,
                                             w = l.rgba >> 8 & 255;
-                                        return u = C + Math.round((m - C) * g), d = y + Math.round((a - y) * g), _ = w + Math.round((p - w) * g), {
+                                        return u = C + Math.round((m - C) * g), d = y + Math.round((o - y) * g), _ = w + Math.round((p - w) * g), {
                                             css: v.toCss(u, d, _),
                                             rgba: v.toRgba(u, d, _)
                                         }
                                     }, t.isOpaque = function(l) {
                                         return (255 & l.rgba) == 255
                                     }, t.ensureContrastRatio = function(l, f, m) {
-                                        const a = e.ensureContrastRatio(l.rgba, f.rgba, m);
-                                        if (a) return e.toColor(a >> 24 & 255, a >> 16 & 255, a >> 8 & 255)
+                                        const o = e.ensureContrastRatio(l.rgba, f.rgba, m);
+                                        if (o) return e.toColor(o >> 24 & 255, o >> 16 & 255, o >> 8 & 255)
                                     }, t.opaque = function(l) {
                                         const f = (255 | l.rgba) >>> 0;
                                         return [u, d, _] = e.toChannels(f), {
                                             css: v.toCss(u, d, _),
                                             rgba: f
                                         }
                                     }, t.opacity = r, t.multiplyOpacity = function(l, f) {
                                         return g = 255 & l.rgba, r(l, g * f / 255)
                                     }, t.toColorRGB = function(l) {
                                         return [l.rgba >> 24 & 255, l.rgba >> 16 & 255, l.rgba >> 8 & 255]
                                     }
                                 }(i.color || (i.color = {})),
                                 function(t) {
                                     let r, l;
-                                    if (!h.isNode) {
+                                    if (!a.isNode) {
                                         const f = document.createElement("canvas");
                                         f.width = 1, f.height = 1;
                                         const m = f.getContext("2d", {
                                             willReadFrequently: !0
                                         });
                                         m && (r = m, r.globalCompositeOperation = "copy", l = r.createLinearGradient(0, 0, 1, 1))
                                     }
@@ -2912,111 +2912,111 @@
                                             rgba: v.toRgba(u, d, _, g),
                                             css: f
                                         }
                                     }
                                 }(i.css || (i.css = {})),
                                 function(t) {
                                     function r(l, f, m) {
-                                        const a = l / 255,
+                                        const o = l / 255,
                                             p = f / 255,
                                             C = m / 255;
-                                        return .2126 * (a <= .03928 ? a / 12.92 : Math.pow((a + .055) / 1.055, 2.4)) + .7152 * (p <= .03928 ? p / 12.92 : Math.pow((p + .055) / 1.055, 2.4)) + .0722 * (C <= .03928 ? C / 12.92 : Math.pow((C + .055) / 1.055, 2.4))
+                                        return .2126 * (o <= .03928 ? o / 12.92 : Math.pow((o + .055) / 1.055, 2.4)) + .7152 * (p <= .03928 ? p / 12.92 : Math.pow((p + .055) / 1.055, 2.4)) + .0722 * (C <= .03928 ? C / 12.92 : Math.pow((C + .055) / 1.055, 2.4))
                                     }
                                     t.relativeLuminance = function(l) {
                                         return r(l >> 16 & 255, l >> 8 & 255, 255 & l)
                                     }, t.relativeLuminance2 = r
                                 }(c = i.rgb || (i.rgb = {})),
                                 function(t) {
-                                    function r(f, m, a) {
+                                    function r(f, m, o) {
                                         const p = f >> 24 & 255,
                                             C = f >> 16 & 255,
                                             y = f >> 8 & 255;
                                         let w = m >> 24 & 255,
                                             D = m >> 16 & 255,
                                             x = m >> 8 & 255,
                                             I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
-                                        for (; I < a && (w > 0 || D > 0 || x > 0);) w -= Math.max(0, Math.ceil(.1 * w)), D -= Math.max(0, Math.ceil(.1 * D)), x -= Math.max(0, Math.ceil(.1 * x)), I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
+                                        for (; I < o && (w > 0 || D > 0 || x > 0);) w -= Math.max(0, Math.ceil(.1 * w)), D -= Math.max(0, Math.ceil(.1 * D)), x -= Math.max(0, Math.ceil(.1 * x)), I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
                                         return (w << 24 | D << 16 | x << 8 | 255) >>> 0
                                     }
 
-                                    function l(f, m, a) {
+                                    function l(f, m, o) {
                                         const p = f >> 24 & 255,
                                             C = f >> 16 & 255,
                                             y = f >> 8 & 255;
                                         let w = m >> 24 & 255,
                                             D = m >> 16 & 255,
                                             x = m >> 8 & 255,
                                             I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
-                                        for (; I < a && (w < 255 || D < 255 || x < 255);) w = Math.min(255, w + Math.ceil(.1 * (255 - w))), D = Math.min(255, D + Math.ceil(.1 * (255 - D))), x = Math.min(255, x + Math.ceil(.1 * (255 - x))), I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
+                                        for (; I < o && (w < 255 || D < 255 || x < 255);) w = Math.min(255, w + Math.ceil(.1 * (255 - w))), D = Math.min(255, D + Math.ceil(.1 * (255 - D))), x = Math.min(255, x + Math.ceil(.1 * (255 - x))), I = n(c.relativeLuminance2(w, D, x), c.relativeLuminance2(p, C, y));
                                         return (w << 24 | D << 16 | x << 8 | 255) >>> 0
                                     }
-                                    t.ensureContrastRatio = function(f, m, a) {
+                                    t.ensureContrastRatio = function(f, m, o) {
                                         const p = c.relativeLuminance(f >> 8),
                                             C = c.relativeLuminance(m >> 8);
-                                        if (n(p, C) < a) {
+                                        if (n(p, C) < o) {
                                             if (C < p) {
-                                                const D = r(f, m, a),
+                                                const D = r(f, m, o),
                                                     x = n(p, c.relativeLuminance(D >> 8));
-                                                if (x < a) {
-                                                    const I = l(f, m, a);
+                                                if (x < o) {
+                                                    const I = l(f, m, o);
                                                     return x > n(p, c.relativeLuminance(I >> 8)) ? D : I
                                                 }
                                                 return D
                                             }
-                                            const y = l(f, m, a),
+                                            const y = l(f, m, o),
                                                 w = n(p, c.relativeLuminance(y >> 8));
-                                            if (w < a) {
-                                                const D = r(f, m, a);
+                                            if (w < o) {
+                                                const D = r(f, m, o);
                                                 return w > n(p, c.relativeLuminance(D >> 8)) ? y : D
                                             }
                                             return y
                                         }
                                     }, t.reduceLuminance = r, t.increaseLuminance = l, t.toChannels = function(f) {
                                         return [f >> 24 & 255, f >> 16 & 255, f >> 8 & 255, 255 & f]
-                                    }, t.toColor = function(f, m, a, p) {
+                                    }, t.toColor = function(f, m, o, p) {
                                         return {
-                                            css: v.toCss(f, m, a, p),
-                                            rgba: v.toRgba(f, m, a, p)
+                                            css: v.toCss(f, m, o, p),
+                                            rgba: v.toRgba(f, m, o, p)
                                         }
                                     }
                                 }(e = i.rgba || (i.rgba = {})), i.toPaddedHex = s, i.contrastRatio = n
                         },
-                        8969: (T, i, o) => {
+                        8969: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CoreTerminal = void 0;
-                            const h = o(844),
-                                u = o(2585),
-                                d = o(4348),
-                                _ = o(7866),
-                                g = o(744),
-                                v = o(7302),
-                                c = o(6975),
-                                e = o(8460),
-                                s = o(1753),
-                                n = o(1480),
-                                t = o(7994),
-                                r = o(9282),
-                                l = o(5435),
-                                f = o(5981),
-                                m = o(2660);
-                            let a = !1;
-                            class p extends h.Disposable {
+                            const a = h(844),
+                                u = h(2585),
+                                d = h(4348),
+                                _ = h(7866),
+                                g = h(744),
+                                v = h(7302),
+                                c = h(6975),
+                                e = h(8460),
+                                s = h(1753),
+                                n = h(1480),
+                                t = h(7994),
+                                r = h(9282),
+                                l = h(5435),
+                                f = h(5981),
+                                m = h(2660);
+                            let o = !1;
+                            class p extends a.Disposable {
                                 constructor(y) {
                                     super(), this._onBinary = this.register(new e.EventEmitter), this.onBinary = this._onBinary.event, this._onData = this.register(new e.EventEmitter), this.onData = this._onData.event, this._onLineFeed = this.register(new e.EventEmitter), this.onLineFeed = this._onLineFeed.event, this._onResize = this.register(new e.EventEmitter), this.onResize = this._onResize.event, this._onWriteParsed = this.register(new e.EventEmitter), this.onWriteParsed = this._onWriteParsed.event, this._onScroll = this.register(new e.EventEmitter), this._instantiationService = new d.InstantiationService, this.optionsService = this.register(new v.OptionsService(y)), this._instantiationService.setService(u.IOptionsService, this.optionsService), this._bufferService = this.register(this._instantiationService.createInstance(g.BufferService)), this._instantiationService.setService(u.IBufferService, this._bufferService), this._logService = this.register(this._instantiationService.createInstance(_.LogService)), this._instantiationService.setService(u.ILogService, this._logService), this.coreService = this.register(this._instantiationService.createInstance(c.CoreService)), this._instantiationService.setService(u.ICoreService, this.coreService), this.coreMouseService = this.register(this._instantiationService.createInstance(s.CoreMouseService)), this._instantiationService.setService(u.ICoreMouseService, this.coreMouseService), this.unicodeService = this.register(this._instantiationService.createInstance(n.UnicodeService)), this._instantiationService.setService(u.IUnicodeService, this.unicodeService), this._charsetService = this._instantiationService.createInstance(t.CharsetService), this._instantiationService.setService(u.ICharsetService, this._charsetService), this._oscLinkService = this._instantiationService.createInstance(m.OscLinkService), this._instantiationService.setService(u.IOscLinkService, this._oscLinkService), this._inputHandler = this.register(new l.InputHandler(this._bufferService, this._charsetService, this.coreService, this._logService, this.optionsService, this._oscLinkService, this.coreMouseService, this.unicodeService)), this.register((0, e.forwardEvent)(this._inputHandler.onLineFeed, this._onLineFeed)), this.register(this._inputHandler), this.register((0, e.forwardEvent)(this._bufferService.onResize, this._onResize)), this.register((0, e.forwardEvent)(this.coreService.onData, this._onData)), this.register((0, e.forwardEvent)(this.coreService.onBinary, this._onBinary)), this.register(this.coreService.onRequestScrollToBottom(() => this.scrollToBottom())), this.register(this.coreService.onUserInput(() => this._writeBuffer.handleUserInput())), this.register(this.optionsService.onSpecificOptionChange("windowsMode", w => this._handleWindowsModeOptionChange(w))), this.register(this._bufferService.onScroll(w => {
                                         this._onScroll.fire({
                                             position: this._bufferService.buffer.ydisp,
                                             source: 0
                                         }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom)
                                     })), this.register(this._inputHandler.onScroll(w => {
                                         this._onScroll.fire({
                                             position: this._bufferService.buffer.ydisp,
                                             source: 0
                                         }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom)
-                                    })), this._writeBuffer = this.register(new f.WriteBuffer((w, D) => this._inputHandler.parse(w, D))), this.register((0, e.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed)), this.register((0, h.toDisposable)(() => {
+                                    })), this._writeBuffer = this.register(new f.WriteBuffer((w, D) => this._inputHandler.parse(w, D))), this.register((0, e.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed)), this.register((0, a.toDisposable)(() => {
                                         var w;
                                         (w = this._windowsMode) === null || w === void 0 || w.dispose(), this._windowsMode = void 0
                                     }))
                                 }
                                 get onScroll() {
                                     return this._onScrollApi || (this._onScrollApi = this.register(new e.EventEmitter), this._onScroll.event(y => {
                                         var w;
@@ -3038,15 +3038,15 @@
                                 set options(y) {
                                     for (const w in y) this.optionsService.options[w] = y[w]
                                 }
                                 write(y, w) {
                                     this._writeBuffer.write(y, w)
                                 }
                                 writeSync(y, w) {
-                                    this._logService.logLevel <= u.LogLevelEnum.WARN && !a && (this._logService.warn("writeSync is unreliable and will be removed soon."), a = !0), this._writeBuffer.writeSync(y, w)
+                                    this._logService.logLevel <= u.LogLevelEnum.WARN && !o && (this._logService.warn("writeSync is unreliable and will be removed soon."), o = !0), this._writeBuffer.writeSync(y, w)
                                 }
                                 resize(y, w) {
                                     isNaN(y) || isNaN(w) || (y = Math.max(y, g.MINIMUM_COLS), w = Math.max(w, g.MINIMUM_ROWS), this._bufferService.resize(y, w))
                                 }
                                 scroll(y, w = !1) {
                                     this._bufferService.scroll(y, w)
                                 }
@@ -3106,37 +3106,37 @@
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.forwardEvent = i.EventEmitter = void 0, i.EventEmitter = class {
                                 constructor() {
                                     this._listeners = [], this._disposed = !1
                                 }
                                 get event() {
-                                    return this._event || (this._event = o => (this._listeners.push(o), {
+                                    return this._event || (this._event = h => (this._listeners.push(h), {
                                         dispose: () => {
                                             if (!this._disposed) {
-                                                for (let h = 0; h < this._listeners.length; h++)
-                                                    if (this._listeners[h] === o) return void this._listeners.splice(h, 1)
+                                                for (let a = 0; a < this._listeners.length; a++)
+                                                    if (this._listeners[a] === h) return void this._listeners.splice(a, 1)
                                             }
                                         }
                                     })), this._event
                                 }
-                                fire(o, h) {
+                                fire(h, a) {
                                     const u = [];
                                     for (let d = 0; d < this._listeners.length; d++) u.push(this._listeners[d]);
-                                    for (let d = 0; d < u.length; d++) u[d].call(void 0, o, h)
+                                    for (let d = 0; d < u.length; d++) u[d].call(void 0, h, a)
                                 }
                                 dispose() {
                                     this._listeners && (this._listeners.length = 0), this._disposed = !0
                                 }
-                            }, i.forwardEvent = function(o, h) {
-                                return o(u => h.fire(u))
+                            }, i.forwardEvent = function(h, a) {
+                                return h(u => a.fire(u))
                             }
                         },
-                        5435: function(T, i, o) {
-                            var h = this && this.__decorate || function(H, S, b, L) {
+                        5435: function(T, i, h) {
+                            var a = this && this.__decorate || function(H, S, b, L) {
                                     var R, M = arguments.length,
                                         F = M < 3 ? S : L === null ? L = Object.getOwnPropertyDescriptor(S, b) : L;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") F = Reflect.decorate(H, S, b, L);
                                     else
                                         for (var j = H.length - 1; j >= 0; j--)(R = H[j]) && (F = (M < 3 ? R(F) : M > 3 ? R(S, b, F) : R(S, b)) || F);
                                     return M > 3 && F && Object.defineProperty(S, b, F), F
                                 },
@@ -3144,28 +3144,28 @@
                                     return function(b, L) {
                                         S(b, L, H)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.InputHandler = i.WindowsOptionsReportType = void 0;
-                            const d = o(2584),
-                                _ = o(7116),
-                                g = o(2015),
-                                v = o(844),
-                                c = o(482),
-                                e = o(8437),
-                                s = o(8460),
-                                n = o(643),
-                                t = o(511),
-                                r = o(3734),
-                                l = o(2585),
-                                f = o(6242),
-                                m = o(6351),
-                                a = o(5941),
+                            const d = h(2584),
+                                _ = h(7116),
+                                g = h(2015),
+                                v = h(844),
+                                c = h(482),
+                                e = h(8437),
+                                s = h(8460),
+                                n = h(643),
+                                t = h(511),
+                                r = h(3734),
+                                l = h(2585),
+                                f = h(6242),
+                                m = h(6351),
+                                o = h(5941),
                                 p = {
                                     "(": 0,
                                     ")": 1,
                                     "*": 2,
                                     "+": 3,
                                     "-": 1,
                                     ".": 2
@@ -4056,15 +4056,15 @@
                                             const F = parseInt(R);
                                             if (0 <= F && F < 256)
                                                 if (M === "?") b.push({
                                                     type: 0,
                                                     index: F
                                                 });
                                                 else {
-                                                    const j = (0, a.parseColor)(M);
+                                                    const j = (0, o.parseColor)(M);
                                                     j && b.push({
                                                         type: 1,
                                                         index: F,
                                                         color: j
                                                     })
                                                 }
                                         }
@@ -4092,15 +4092,15 @@
                                     const L = S.split(";");
                                     for (let R = 0; R < L.length && !(b >= this._specialColors.length); ++R, ++b)
                                         if (L[R] === "?") this._onColor.fire([{
                                             type: 0,
                                             index: this._specialColors[b]
                                         }]);
                                         else {
-                                            const M = (0, a.parseColor)(L[R]);
+                                            const M = (0, o.parseColor)(L[R]);
                                             M && this._onColor.fire([{
                                                 type: 1,
                                                 index: this._specialColors[b],
                                                 color: M
                                             }])
                                         } return !0
                                 }
@@ -4219,144 +4219,144 @@
                                 markRangeDirty(H, S) {
                                     H > S && (D = H, H = S, S = D), H < this.start && (this.start = H), S > this.end && (this.end = S)
                                 }
                                 markAllDirty() {
                                     this.markRangeDirty(0, this._bufferService.rows - 1)
                                 }
                             };
-                            I = h([u(0, l.IBufferService)], I)
+                            I = a([u(0, l.IBufferService)], I)
                         },
                         844: (T, i) => {
-                            function o(h) {
-                                for (const u of h) u.dispose();
-                                h.length = 0
+                            function h(a) {
+                                for (const u of a) u.dispose();
+                                a.length = 0
                             }
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.getDisposeArrayDisposable = i.disposeArray = i.toDisposable = i.Disposable = void 0, i.Disposable = class {
                                 constructor() {
                                     this._disposables = [], this._isDisposed = !1
                                 }
                                 dispose() {
                                     this._isDisposed = !0;
-                                    for (const h of this._disposables) h.dispose();
+                                    for (const a of this._disposables) a.dispose();
                                     this._disposables.length = 0
                                 }
-                                register(h) {
-                                    return this._disposables.push(h), h
+                                register(a) {
+                                    return this._disposables.push(a), a
                                 }
-                                unregister(h) {
-                                    const u = this._disposables.indexOf(h);
+                                unregister(a) {
+                                    const u = this._disposables.indexOf(a);
                                     u !== -1 && this._disposables.splice(u, 1)
                                 }
-                            }, i.toDisposable = function(h) {
+                            }, i.toDisposable = function(a) {
                                 return {
-                                    dispose: h
+                                    dispose: a
                                 }
-                            }, i.disposeArray = o, i.getDisposeArrayDisposable = function(h) {
+                            }, i.disposeArray = h, i.getDisposeArrayDisposable = function(a) {
                                 return {
-                                    dispose: () => o(h)
+                                    dispose: () => h(a)
                                 }
                             }
                         },
                         1505: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.FourKeyMap = i.TwoKeyMap = void 0;
-                            class o {
+                            class h {
                                 constructor() {
                                     this._data = {}
                                 }
                                 set(u, d, _) {
                                     this._data[u] || (this._data[u] = {}), this._data[u][d] = _
                                 }
                                 get(u, d) {
                                     return this._data[u] ? this._data[u][d] : void 0
                                 }
                                 clear() {
                                     this._data = {}
                                 }
                             }
-                            i.TwoKeyMap = o, i.FourKeyMap = class {
+                            i.TwoKeyMap = h, i.FourKeyMap = class {
                                 constructor() {
-                                    this._data = new o
+                                    this._data = new h
                                 }
-                                set(h, u, d, _, g) {
-                                    this._data.get(h, u) || this._data.set(h, u, new o), this._data.get(h, u).set(d, _, g)
+                                set(a, u, d, _, g) {
+                                    this._data.get(a, u) || this._data.set(a, u, new h), this._data.get(a, u).set(d, _, g)
                                 }
-                                get(h, u, d, _) {
+                                get(a, u, d, _) {
                                     var g;
-                                    return (g = this._data.get(h, u)) === null || g === void 0 ? void 0 : g.get(d, _)
+                                    return (g = this._data.get(a, u)) === null || g === void 0 ? void 0 : g.get(d, _)
                                 }
                                 clear() {
                                     this._data.clear()
                                 }
                             }
                         },
                         6114: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.isChromeOS = i.isLinux = i.isWindows = i.isIphone = i.isIpad = i.isMac = i.getSafariVersion = i.isSafari = i.isLegacyEdge = i.isFirefox = i.isNode = void 0, i.isNode = typeof navigator > "u";
-                            const o = i.isNode ? "node" : navigator.userAgent,
-                                h = i.isNode ? "node" : navigator.platform;
-                            i.isFirefox = o.includes("Firefox"), i.isLegacyEdge = o.includes("Edge"), i.isSafari = /^((?!chrome|android).)*safari/i.test(o), i.getSafariVersion = function() {
+                            const h = i.isNode ? "node" : navigator.userAgent,
+                                a = i.isNode ? "node" : navigator.platform;
+                            i.isFirefox = h.includes("Firefox"), i.isLegacyEdge = h.includes("Edge"), i.isSafari = /^((?!chrome|android).)*safari/i.test(h), i.getSafariVersion = function() {
                                 if (!i.isSafari) return 0;
-                                const u = o.match(/Version\/(\d+)/);
+                                const u = h.match(/Version\/(\d+)/);
                                 return u === null || u.length < 2 ? 0 : parseInt(u[1])
-                            }, i.isMac = ["Macintosh", "MacIntel", "MacPPC", "Mac68K"].includes(h), i.isIpad = h === "iPad", i.isIphone = h === "iPhone", i.isWindows = ["Windows", "Win16", "Win32", "WinCE"].includes(h), i.isLinux = h.indexOf("Linux") >= 0, i.isChromeOS = /\bCrOS\b/.test(o)
+                            }, i.isMac = ["Macintosh", "MacIntel", "MacPPC", "Mac68K"].includes(a), i.isIpad = a === "iPad", i.isIphone = a === "iPhone", i.isWindows = ["Windows", "Win16", "Win32", "WinCE"].includes(a), i.isLinux = a.indexOf("Linux") >= 0, i.isChromeOS = /\bCrOS\b/.test(h)
                         },
                         6106: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.SortedList = void 0;
-                            let o = 0;
+                            let h = 0;
                             i.SortedList = class {
-                                constructor(h) {
-                                    this._getKey = h, this._array = []
+                                constructor(a) {
+                                    this._getKey = a, this._array = []
                                 }
                                 clear() {
                                     this._array.length = 0
                                 }
-                                insert(h) {
-                                    this._array.length !== 0 ? (o = this._search(this._getKey(h), 0, this._array.length - 1), this._array.splice(o, 0, h)) : this._array.push(h)
+                                insert(a) {
+                                    this._array.length !== 0 ? (h = this._search(this._getKey(a), 0, this._array.length - 1), this._array.splice(h, 0, a)) : this._array.push(a)
                                 }
-                                delete(h) {
+                                delete(a) {
                                     if (this._array.length === 0) return !1;
-                                    const u = this._getKey(h);
-                                    if (u === void 0 || (o = this._search(u, 0, this._array.length - 1), o === -1) || this._getKey(this._array[o]) !== u) return !1;
+                                    const u = this._getKey(a);
+                                    if (u === void 0 || (h = this._search(u, 0, this._array.length - 1), h === -1) || this._getKey(this._array[h]) !== u) return !1;
                                     do
-                                        if (this._array[o] === h) return this._array.splice(o, 1), !0; while (++o < this._array.length && this._getKey(this._array[o]) === u);
+                                        if (this._array[h] === a) return this._array.splice(h, 1), !0; while (++h < this._array.length && this._getKey(this._array[h]) === u);
                                     return !1
-                                }* getKeyIterator(h) {
-                                    if (this._array.length !== 0 && (o = this._search(h, 0, this._array.length - 1), !(o < 0 || o >= this._array.length) && this._getKey(this._array[o]) === h))
-                                        do yield this._array[o]; while (++o < this._array.length && this._getKey(this._array[o]) === h)
-                                }
-                                forEachByKey(h, u) {
-                                    if (this._array.length !== 0 && (o = this._search(h, 0, this._array.length - 1), !(o < 0 || o >= this._array.length) && this._getKey(this._array[o]) === h))
-                                        do u(this._array[o]); while (++o < this._array.length && this._getKey(this._array[o]) === h)
+                                }* getKeyIterator(a) {
+                                    if (this._array.length !== 0 && (h = this._search(a, 0, this._array.length - 1), !(h < 0 || h >= this._array.length) && this._getKey(this._array[h]) === a))
+                                        do yield this._array[h]; while (++h < this._array.length && this._getKey(this._array[h]) === a)
+                                }
+                                forEachByKey(a, u) {
+                                    if (this._array.length !== 0 && (h = this._search(a, 0, this._array.length - 1), !(h < 0 || h >= this._array.length) && this._getKey(this._array[h]) === a))
+                                        do u(this._array[h]); while (++h < this._array.length && this._getKey(this._array[h]) === a)
                                 }
                                 values() {
                                     return this._array.values()
                                 }
-                                _search(h, u, d) {
+                                _search(a, u, d) {
                                     if (d < u) return u;
                                     let _ = Math.floor((u + d) / 2);
                                     const g = this._getKey(this._array[_]);
-                                    if (g > h) return this._search(h, u, _ - 1);
-                                    if (g < h) return this._search(h, _ + 1, d);
-                                    for (; _ > 0 && this._getKey(this._array[_ - 1]) === h;) _--;
+                                    if (g > a) return this._search(a, u, _ - 1);
+                                    if (g < a) return this._search(a, _ + 1, d);
+                                    for (; _ > 0 && this._getKey(this._array[_ - 1]) === a;) _--;
                                     return _
                                 }
                             }
                         },
-                        7226: (T, i, o) => {
+                        7226: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.DebouncedIdleTask = i.IdleTaskQueue = i.PriorityTaskQueue = void 0;
-                            const h = o(6114);
+                            const a = h(6114);
                             class u {
                                 constructor() {
                                     this._tasks = [], this._i = 0
                                 }
                                 enqueue(g) {
                                     this._tasks.push(g), this._start()
                                 }
@@ -4393,15 +4393,15 @@
                                 _createDeadline(g) {
                                     const v = Date.now() + g;
                                     return {
                                         timeRemaining: () => Math.max(0, v - Date.now())
                                     }
                                 }
                             }
-                            i.PriorityTaskQueue = d, i.IdleTaskQueue = !h.isNode && "requestIdleCallback" in window ? class extends u {
+                            i.PriorityTaskQueue = d, i.IdleTaskQueue = !a.isNode && "requestIdleCallback" in window ? class extends u {
                                 _requestCallback(_) {
                                     return requestIdleCallback(_)
                                 }
                                 _cancelCallback(_) {
                                     cancelIdleCallback(_)
                                 }
                             } : d, i.DebouncedIdleTask = class {
@@ -4412,42 +4412,42 @@
                                     this._queue.clear(), this._queue.enqueue(_)
                                 }
                                 flush() {
                                     this._queue.flush()
                                 }
                             }
                         },
-                        9282: (T, i, o) => {
+                        9282: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.updateWindowsModeWrappedState = void 0;
-                            const h = o(643);
+                            const a = h(643);
                             i.updateWindowsModeWrappedState = function(u) {
                                 const d = u.buffer.lines.get(u.buffer.ybase + u.buffer.y - 1),
                                     _ = d == null ? void 0 : d.get(u.cols - 1),
                                     g = u.buffer.lines.get(u.buffer.ybase + u.buffer.y);
-                                g && _ && (g.isWrapped = _[h.CHAR_DATA_CODE_INDEX] !== h.NULL_CELL_CODE && _[h.CHAR_DATA_CODE_INDEX] !== h.WHITESPACE_CELL_CODE)
+                                g && _ && (g.isWrapped = _[a.CHAR_DATA_CODE_INDEX] !== a.NULL_CELL_CODE && _[a.CHAR_DATA_CODE_INDEX] !== a.WHITESPACE_CELL_CODE)
                             }
                         },
                         3734: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.ExtendedAttrs = i.AttributeData = void 0;
-                            class o {
+                            class h {
                                 constructor() {
-                                    this.fg = 0, this.bg = 0, this.extended = new h
+                                    this.fg = 0, this.bg = 0, this.extended = new a
                                 }
                                 static toColorRGB(d) {
                                     return [d >>> 16 & 255, d >>> 8 & 255, 255 & d]
                                 }
                                 static fromColorRGB(d) {
                                     return (255 & d[0]) << 16 | (255 & d[1]) << 8 | 255 & d[2]
                                 }
                                 clone() {
-                                    const d = new o;
+                                    const d = new h;
                                     return d.fg = this.fg, d.bg = this.bg, d.extended = this.extended.clone(), d
                                 }
                                 isInverse() {
                                     return 67108864 & this.fg
                                 }
                                 isBold() {
                                     return 134217728 & this.fg
@@ -4552,16 +4552,16 @@
                                 isUnderlineColorDefault() {
                                     return 268435456 & this.bg && ~this.extended.underlineColor ? (50331648 & this.extended.underlineColor) == 0 : this.isFgDefault()
                                 }
                                 getUnderlineStyle() {
                                     return 268435456 & this.fg ? 268435456 & this.bg ? this.extended.underlineStyle : 1 : 0
                                 }
                             }
-                            i.AttributeData = o;
-                            class h {
+                            i.AttributeData = h;
+                            class a {
                                 constructor(d = 0, _ = 0) {
                                     this._ext = 0, this._urlId = 0, this._ext = d, this._urlId = _
                                 }
                                 get ext() {
                                     return this._urlId ? -469762049 & this._ext | this.underlineStyle << 26 : this._ext
                                 }
                                 set ext(d) {
@@ -4582,38 +4582,38 @@
                                 get urlId() {
                                     return this._urlId
                                 }
                                 set urlId(d) {
                                     this._urlId = d
                                 }
                                 clone() {
-                                    return new h(this._ext, this._urlId)
+                                    return new a(this._ext, this._urlId)
                                 }
                                 isEmpty() {
                                     return this.underlineStyle === 0 && this._urlId === 0
                                 }
                             }
-                            i.ExtendedAttrs = h
+                            i.ExtendedAttrs = a
                         },
-                        9092: (T, i, o) => {
+                        9092: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferStringIterator = i.Buffer = i.MAX_BUFFER_SIZE = void 0;
-                            const h = o(6349),
-                                u = o(8437),
-                                d = o(511),
-                                _ = o(643),
-                                g = o(4634),
-                                v = o(4863),
-                                c = o(7116),
-                                e = o(3734),
-                                s = o(7226);
+                            const a = h(6349),
+                                u = h(8437),
+                                d = h(511),
+                                _ = h(643),
+                                g = h(4634),
+                                v = h(4863),
+                                c = h(7116),
+                                e = h(3734),
+                                s = h(7226);
                             i.MAX_BUFFER_SIZE = 4294967295, i.Buffer = class {
                                 constructor(t, r, l) {
-                                    this._hasScrollback = t, this._optionsService = r, this._bufferService = l, this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.tabs = {}, this.savedY = 0, this.savedX = 0, this.savedCurAttrData = u.DEFAULT_ATTR_DATA.clone(), this.savedCharset = c.DEFAULT_CHARSET, this.markers = [], this._nullCell = d.CellData.fromCharData([0, _.NULL_CELL_CHAR, _.NULL_CELL_WIDTH, _.NULL_CELL_CODE]), this._whitespaceCell = d.CellData.fromCharData([0, _.WHITESPACE_CELL_CHAR, _.WHITESPACE_CELL_WIDTH, _.WHITESPACE_CELL_CODE]), this._isClearing = !1, this._memoryCleanupQueue = new s.IdleTaskQueue, this._memoryCleanupPosition = 0, this._cols = this._bufferService.cols, this._rows = this._bufferService.rows, this.lines = new h.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops()
+                                    this._hasScrollback = t, this._optionsService = r, this._bufferService = l, this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.tabs = {}, this.savedY = 0, this.savedX = 0, this.savedCurAttrData = u.DEFAULT_ATTR_DATA.clone(), this.savedCharset = c.DEFAULT_CHARSET, this.markers = [], this._nullCell = d.CellData.fromCharData([0, _.NULL_CELL_CHAR, _.NULL_CELL_WIDTH, _.NULL_CELL_CODE]), this._whitespaceCell = d.CellData.fromCharData([0, _.WHITESPACE_CELL_CHAR, _.WHITESPACE_CELL_WIDTH, _.WHITESPACE_CELL_CODE]), this._isClearing = !1, this._memoryCleanupQueue = new s.IdleTaskQueue, this._memoryCleanupPosition = 0, this._cols = this._bufferService.cols, this._rows = this._bufferService.rows, this.lines = new a.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops()
                                 }
                                 getNullCell(t) {
                                     return t ? (this._nullCell.fg = t.fg, this._nullCell.bg = t.bg, this._nullCell.extended = t.extended) : (this._nullCell.fg = 0, this._nullCell.bg = 0, this._nullCell.extended = new e.ExtendedAttrs), this._nullCell
                                 }
                                 getWhitespaceCell(t) {
                                     return t ? (this._whitespaceCell.fg = t.fg, this._whitespaceCell.bg = t.bg, this._whitespaceCell.extended = t.extended) : (this._whitespaceCell.fg = 0, this._whitespaceCell.bg = 0, this._whitespaceCell.extended = new e.ExtendedAttrs), this._whitespaceCell
                                 }
@@ -4636,36 +4636,36 @@
                                     if (this.lines.length === 0) {
                                         t === void 0 && (t = u.DEFAULT_ATTR_DATA);
                                         let r = this._rows;
                                         for (; r--;) this.lines.push(this.getBlankLine(t))
                                     }
                                 }
                                 clear() {
-                                    this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.lines = new h.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops()
+                                    this.ydisp = 0, this.ybase = 0, this.y = 0, this.x = 0, this.lines = new a.CircularList(this._getCorrectBufferLength(this._rows)), this.scrollTop = 0, this.scrollBottom = this._rows - 1, this.setupTabStops()
                                 }
                                 resize(t, r) {
                                     const l = this.getNullCell(u.DEFAULT_ATTR_DATA);
                                     let f = 0;
                                     const m = this._getCorrectBufferLength(r);
                                     if (m > this.lines.maxLength && (this.lines.maxLength = m), this.lines.length > 0) {
                                         if (this._cols < t)
                                             for (let p = 0; p < this.lines.length; p++) f += +this.lines.get(p).resize(t, l);
-                                        let a = 0;
+                                        let o = 0;
                                         if (this._rows < r)
-                                            for (let p = this._rows; p < r; p++) this.lines.length < r + this.ybase && (this._optionsService.rawOptions.windowsMode ? this.lines.push(new u.BufferLine(t, l)) : this.ybase > 0 && this.lines.length <= this.ybase + this.y + a + 1 ? (this.ybase--, a++, this.ydisp > 0 && this.ydisp--) : this.lines.push(new u.BufferLine(t, l)));
+                                            for (let p = this._rows; p < r; p++) this.lines.length < r + this.ybase && (this._optionsService.rawOptions.windowsMode ? this.lines.push(new u.BufferLine(t, l)) : this.ybase > 0 && this.lines.length <= this.ybase + this.y + o + 1 ? (this.ybase--, o++, this.ydisp > 0 && this.ydisp--) : this.lines.push(new u.BufferLine(t, l)));
                                         else
                                             for (let p = this._rows; p > r; p--) this.lines.length > r + this.ybase && (this.lines.length > this.ybase + this.y + 1 ? this.lines.pop() : (this.ybase++, this.ydisp++));
                                         if (m < this.lines.maxLength) {
                                             const p = this.lines.length - m;
                                             p > 0 && (this.lines.trimStart(p), this.ybase = Math.max(this.ybase - p, 0), this.ydisp = Math.max(this.ydisp - p, 0), this.savedY = Math.max(this.savedY - p, 0)), this.lines.maxLength = m
                                         }
-                                        this.x = Math.min(this.x, t - 1), this.y = Math.min(this.y, r - 1), a && (this.y += a), this.savedX = Math.min(this.savedX, t - 1), this.scrollTop = 0
+                                        this.x = Math.min(this.x, t - 1), this.y = Math.min(this.y, r - 1), o && (this.y += o), this.savedX = Math.min(this.savedX, t - 1), this.scrollTop = 0
                                     }
                                     if (this.scrollBottom = r - 1, this._isReflowEnabled && (this._reflow(t, r), this._cols > t))
-                                        for (let a = 0; a < this.lines.length; a++) f += +this.lines.get(a).resize(t, l);
+                                        for (let o = 0; o < this.lines.length; o++) f += +this.lines.get(o).resize(t, l);
                                     this._cols = t, this._rows = r, this._memoryCleanupQueue.clear(), f > .1 * this.lines.length && (this._memoryCleanupPosition = 0, this._memoryCleanupQueue.enqueue(() => this._batchedMemoryCleanup()))
                                 }
                                 _batchedMemoryCleanup() {
                                     let t = !0;
                                     this._memoryCleanupPosition >= this.lines.length && (this._memoryCleanupPosition = 0, t = !1);
                                     let r = 0;
                                     for (; this._memoryCleanupPosition < this.lines.length;)
@@ -4691,33 +4691,33 @@
                                     for (; m-- > 0;) this.ybase === 0 ? (this.y > 0 && this.y--, this.lines.length < r && this.lines.push(new u.BufferLine(t, f))) : (this.ydisp === this.ybase && this.ydisp--, this.ybase--);
                                     this.savedY = Math.max(this.savedY - l, 0)
                                 }
                                 _reflowSmaller(t, r) {
                                     const l = this.getNullCell(u.DEFAULT_ATTR_DATA),
                                         f = [];
                                     let m = 0;
-                                    for (let a = this.lines.length - 1; a >= 0; a--) {
-                                        let p = this.lines.get(a);
+                                    for (let o = this.lines.length - 1; o >= 0; o--) {
+                                        let p = this.lines.get(o);
                                         if (!p || !p.isWrapped && p.getTrimmedLength() <= t) continue;
                                         const C = [p];
-                                        for (; p.isWrapped && a > 0;) p = this.lines.get(--a), C.unshift(p);
+                                        for (; p.isWrapped && o > 0;) p = this.lines.get(--o), C.unshift(p);
                                         const y = this.ybase + this.y;
-                                        if (y >= a && y < a + C.length) continue;
+                                        if (y >= o && y < o + C.length) continue;
                                         const w = C[C.length - 1].getTrimmedLength(),
                                             D = (0, g.reflowSmallerGetNewLineLengths)(C, this._cols, t),
                                             x = D.length - C.length;
                                         let I;
                                         I = this.ybase === 0 && this.y !== this.lines.length - 1 ? Math.max(0, this.y - this.lines.maxLength + x) : Math.max(0, this.lines.length - this.lines.maxLength + x);
                                         const H = [];
                                         for (let F = 0; F < x; F++) {
                                             const j = this.getBlankLine(u.DEFAULT_ATTR_DATA, !0);
                                             H.push(j)
                                         }
                                         H.length > 0 && (f.push({
-                                            start: a + C.length + m,
+                                            start: o + C.length + m,
                                             newLines: H
                                         }), m += H.length), C.push(...H);
                                         let S = D.length - 1,
                                             b = D[S];
                                         b === 0 && (S--, b = D[S]);
                                         let L = C.length - x - 1,
                                             R = w;
@@ -4732,44 +4732,44 @@
                                         }
                                         for (let F = 0; F < C.length; F++) D[F] < t && C[F].setCell(D[F], l);
                                         let M = x - I;
                                         for (; M-- > 0;) this.ybase === 0 ? this.y < r - 1 ? (this.y++, this.lines.pop()) : (this.ybase++, this.ydisp++) : this.ybase < Math.min(this.lines.maxLength, this.lines.length + m) - r && (this.ybase === this.ydisp && this.ydisp++, this.ybase++);
                                         this.savedY = Math.min(this.savedY + x, this.ybase + r - 1)
                                     }
                                     if (f.length > 0) {
-                                        const a = [],
+                                        const o = [],
                                             p = [];
                                         for (let S = 0; S < this.lines.length; S++) p.push(this.lines.get(S));
                                         const C = this.lines.length;
                                         let y = C - 1,
                                             w = 0,
                                             D = f[w];
                                         this.lines.length = Math.min(this.lines.maxLength, this.lines.length + m);
                                         let x = 0;
                                         for (let S = Math.min(this.lines.maxLength - 1, C + m - 1); S >= 0; S--)
                                             if (D && D.start > y + x) {
                                                 for (let b = D.newLines.length - 1; b >= 0; b--) this.lines.set(S--, D.newLines[b]);
-                                                S++, a.push({
+                                                S++, o.push({
                                                     index: y + 1,
                                                     amount: D.newLines.length
                                                 }), x += D.newLines.length, D = f[++w]
                                             } else this.lines.set(S, p[y--]);
                                         let I = 0;
-                                        for (let S = a.length - 1; S >= 0; S--) a[S].index += I, this.lines.onInsertEmitter.fire(a[S]), I += a[S].amount;
+                                        for (let S = o.length - 1; S >= 0; S--) o[S].index += I, this.lines.onInsertEmitter.fire(o[S]), I += o[S].amount;
                                         const H = Math.max(0, C + m - this.lines.maxLength);
                                         H > 0 && this.lines.onTrimEmitter.fire(H)
                                     }
                                 }
                                 stringIndexToBufferIndex(t, r, l = !1) {
                                     for (; r;) {
                                         const f = this.lines.get(t);
                                         if (!f) return [-1, -1];
                                         const m = l ? f.getTrimmedLength() : f.length;
-                                        for (let a = 0; a < m; ++a)
-                                            if (f.get(a)[_.CHAR_DATA_WIDTH_INDEX] && (r -= f.get(a)[_.CHAR_DATA_CHAR_INDEX].length || 1), r < 0) return [t, a];
+                                        for (let o = 0; o < m; ++o)
+                                            if (f.get(o)[_.CHAR_DATA_WIDTH_INDEX] && (r -= f.get(o)[_.CHAR_DATA_CHAR_INDEX].length || 1), r < 0) return [t, o];
                                         t++
                                     }
                                     return [t, 0]
                                 }
                                 translateBufferLineToString(t, r, l = 0, f) {
                                     const m = this.lines.get(t);
                                     return m ? m.translateToString(r, l, f) : ""
@@ -4819,16 +4819,16 @@
                                     this._isClearing || this.markers.splice(this.markers.indexOf(t), 1)
                                 }
                                 iterator(t, r, l, f, m) {
                                     return new n(this, t, r, l, f, m)
                                 }
                             };
                             class n {
-                                constructor(r, l, f = 0, m = r.lines.length, a = 0, p = 0) {
-                                    this._buffer = r, this._trimRight = l, this._startIndex = f, this._endIndex = m, this._startOverscan = a, this._endOverscan = p, this._startIndex < 0 && (this._startIndex = 0), this._endIndex > this._buffer.lines.length && (this._endIndex = this._buffer.lines.length), this._current = this._startIndex
+                                constructor(r, l, f = 0, m = r.lines.length, o = 0, p = 0) {
+                                    this._buffer = r, this._trimRight = l, this._startIndex = f, this._endIndex = m, this._startOverscan = o, this._endOverscan = p, this._startIndex < 0 && (this._startIndex = 0), this._endIndex > this._buffer.lines.length && (this._endIndex = this._buffer.lines.length), this._current = this._startIndex
                                 }
                                 hasNext() {
                                     return this._current < this._endIndex
                                 }
                                 next() {
                                     const r = this._buffer.getWrappedRangeForLine(this._current);
                                     r.first < this._startIndex - this._startOverscan && (r.first = this._startIndex - this._startOverscan), r.last > this._endIndex + this._endOverscan && (r.last = this._endIndex + this._endOverscan), r.first = Math.max(r.first, 0), r.last = Math.min(r.last, this._buffer.lines.length);
@@ -4838,35 +4838,35 @@
                                         range: r,
                                         content: l
                                     }
                                 }
                             }
                             i.BufferStringIterator = n
                         },
-                        8437: (T, i, o) => {
+                        8437: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferLine = i.DEFAULT_ATTR_DATA = void 0;
-                            const h = o(482),
-                                u = o(643),
-                                d = o(511),
-                                _ = o(3734);
+                            const a = h(482),
+                                u = h(643),
+                                d = h(511),
+                                _ = h(3734);
                             i.DEFAULT_ATTR_DATA = Object.freeze(new _.AttributeData);
                             let g = 0;
                             class v {
                                 constructor(e, s, n = !1) {
                                     this.isWrapped = n, this._combined = {}, this._extendedAttrs = {}, this._data = new Uint32Array(3 * e);
                                     const t = s || d.CellData.fromCharData([0, u.NULL_CELL_CHAR, u.NULL_CELL_WIDTH, u.NULL_CELL_CODE]);
                                     for (let r = 0; r < e; ++r) this.setCell(r, t);
                                     this.length = e
                                 }
                                 get(e) {
                                     const s = this._data[3 * e + 0],
                                         n = 2097151 & s;
-                                    return [this._data[3 * e + 1], 2097152 & s ? this._combined[e] : n ? (0, h.stringFromCodePoint)(n) : "", s >> 22, 2097152 & s ? this._combined[e].charCodeAt(this._combined[e].length - 1) : n]
+                                    return [this._data[3 * e + 1], 2097152 & s ? this._combined[e] : n ? (0, a.stringFromCodePoint)(n) : "", s >> 22, 2097152 & s ? this._combined[e].charCodeAt(this._combined[e].length - 1) : n]
                                 }
                                 set(e, s) {
                                     this._data[3 * e + 1] = s[u.CHAR_DATA_ATTR_INDEX], s[u.CHAR_DATA_CHAR_INDEX].length > 1 ? (this._combined[e] = s[1], this._data[3 * e + 0] = 2097152 | e | s[u.CHAR_DATA_WIDTH_INDEX] << 22) : this._data[3 * e + 0] = s[u.CHAR_DATA_CHAR_INDEX].charCodeAt(0) | s[u.CHAR_DATA_WIDTH_INDEX] << 22
                                 }
                                 getWidth(e) {
                                     return this._data[3 * e + 0] >> 22
                                 }
@@ -4887,15 +4887,15 @@
                                     return 2097152 & s ? this._combined[e].charCodeAt(this._combined[e].length - 1) : 2097151 & s
                                 }
                                 isCombined(e) {
                                     return 2097152 & this._data[3 * e + 0]
                                 }
                                 getString(e) {
                                     const s = this._data[3 * e + 0];
-                                    return 2097152 & s ? this._combined[e] : 2097151 & s ? (0, h.stringFromCodePoint)(2097151 & s) : ""
+                                    return 2097152 & s ? this._combined[e] : 2097151 & s ? (0, a.stringFromCodePoint)(2097151 & s) : ""
                                 }
                                 isProtected(e) {
                                     return 536870912 & this._data[3 * e + 2]
                                 }
                                 loadCell(e, s) {
                                     return g = 3 * e, s.content = this._data[g + 0], s.fg = this._data[g + 1], s.bg = this._data[g + 2], 2097152 & s.content && (s.combinedData = this._combined[e]), 268435456 & s.bg && (s.extended = this._extendedAttrs[e]), s
                                 }
@@ -4903,15 +4903,15 @@
                                     2097152 & s.content && (this._combined[e] = s.combinedData), 268435456 & s.bg && (this._extendedAttrs[e] = s.extended), this._data[3 * e + 0] = s.content, this._data[3 * e + 1] = s.fg, this._data[3 * e + 2] = s.bg
                                 }
                                 setCellFromCodePoint(e, s, n, t, r, l) {
                                     268435456 & r && (this._extendedAttrs[e] = l), this._data[3 * e + 0] = s | n << 22, this._data[3 * e + 1] = t, this._data[3 * e + 2] = r
                                 }
                                 addCodepointToCell(e, s) {
                                     let n = this._data[3 * e + 0];
-                                    2097152 & n ? this._combined[e] += (0, h.stringFromCodePoint)(s) : (2097151 & n ? (this._combined[e] = (0, h.stringFromCodePoint)(2097151 & n) + (0, h.stringFromCodePoint)(s), n &= -2097152, n |= 2097152) : n = s | 4194304, this._data[3 * e + 0] = n)
+                                    2097152 & n ? this._combined[e] += (0, a.stringFromCodePoint)(s) : (2097151 & n ? (this._combined[e] = (0, a.stringFromCodePoint)(2097151 & n) + (0, a.stringFromCodePoint)(s), n &= -2097152, n |= 2097152) : n = s | 4194304, this._data[3 * e + 0] = n)
                                 }
                                 insertCells(e, s, n, t) {
                                     if ((e %= this.length) && this.getWidth(e - 1) === 2 && this.setCellFromCodePoint(e - 1, 0, 1, (t == null ? void 0 : t.fg) || 0, (t == null ? void 0 : t.bg) || 0, (t == null ? void 0 : t.extended) || new _.ExtendedAttrs), s < this.length - e) {
                                         const r = new d.CellData;
                                         for (let l = this.length - e - s - 1; l >= 0; --l) this.setCell(e + s + l, this.loadCell(e + l, r));
                                         for (let l = 0; l < s; ++l) this.setCell(e + l, n)
                                     } else
@@ -4992,143 +4992,143 @@
                                         if (4194303 & this._data[3 * e + 0]) return e + (this._data[3 * e + 0] >> 22);
                                     return 0
                                 }
                                 copyCellsFrom(e, s, n, t, r) {
                                     const l = e._data;
                                     if (r)
                                         for (let m = t - 1; m >= 0; m--) {
-                                            for (let a = 0; a < 3; a++) this._data[3 * (n + m) + a] = l[3 * (s + m) + a];
+                                            for (let o = 0; o < 3; o++) this._data[3 * (n + m) + o] = l[3 * (s + m) + o];
                                             268435456 & l[3 * (s + m) + 2] && (this._extendedAttrs[n + m] = e._extendedAttrs[s + m])
                                         } else
                                             for (let m = 0; m < t; m++) {
-                                                for (let a = 0; a < 3; a++) this._data[3 * (n + m) + a] = l[3 * (s + m) + a];
+                                                for (let o = 0; o < 3; o++) this._data[3 * (n + m) + o] = l[3 * (s + m) + o];
                                                 268435456 & l[3 * (s + m) + 2] && (this._extendedAttrs[n + m] = e._extendedAttrs[s + m])
                                             }
                                     const f = Object.keys(e._combined);
                                     for (let m = 0; m < f.length; m++) {
-                                        const a = parseInt(f[m], 10);
-                                        a >= s && (this._combined[a - s + n] = e._combined[a])
+                                        const o = parseInt(f[m], 10);
+                                        o >= s && (this._combined[o - s + n] = e._combined[o])
                                     }
                                 }
                                 translateToString(e = !1, s = 0, n = this.length) {
                                     e && (n = Math.min(n, this.getTrimmedLength()));
                                     let t = "";
                                     for (; s < n;) {
                                         const r = this._data[3 * s + 0],
                                             l = 2097151 & r;
-                                        t += 2097152 & r ? this._combined[s] : l ? (0, h.stringFromCodePoint)(l) : u.WHITESPACE_CELL_CHAR, s += r >> 22 || 1
+                                        t += 2097152 & r ? this._combined[s] : l ? (0, a.stringFromCodePoint)(l) : u.WHITESPACE_CELL_CHAR, s += r >> 22 || 1
                                     }
                                     return t
                                 }
                             }
                             i.BufferLine = v
                         },
                         4841: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.getRangeLength = void 0, i.getRangeLength = function(o, h) {
-                                if (o.start.y > o.end.y) throw new Error(`Buffer range end (${o.end.x}, ${o.end.y}) cannot be before start (${o.start.x}, ${o.start.y})`);
-                                return h * (o.end.y - o.start.y) + (o.end.x - o.start.x + 1)
+                            }), i.getRangeLength = void 0, i.getRangeLength = function(h, a) {
+                                if (h.start.y > h.end.y) throw new Error(`Buffer range end (${h.end.x}, ${h.end.y}) cannot be before start (${h.start.x}, ${h.start.y})`);
+                                return a * (h.end.y - h.start.y) + (h.end.x - h.start.x + 1)
                             }
                         },
                         4634: (T, i) => {
-                            function o(h, u, d) {
-                                if (u === h.length - 1) return h[u].getTrimmedLength();
-                                const _ = !h[u].hasContent(d - 1) && h[u].getWidth(d - 1) === 1,
-                                    g = h[u + 1].getWidth(0) === 2;
+                            function h(a, u, d) {
+                                if (u === a.length - 1) return a[u].getTrimmedLength();
+                                const _ = !a[u].hasContent(d - 1) && a[u].getWidth(d - 1) === 1,
+                                    g = a[u + 1].getWidth(0) === 2;
                                 return _ && g ? d - 1 : d
                             }
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.getWrappedLineTrimmedLength = i.reflowSmallerGetNewLineLengths = i.reflowLargerApplyNewLayout = i.reflowLargerCreateNewLayout = i.reflowLargerGetLinesToRemove = void 0, i.reflowLargerGetLinesToRemove = function(h, u, d, _, g) {
+                            }), i.getWrappedLineTrimmedLength = i.reflowSmallerGetNewLineLengths = i.reflowLargerApplyNewLayout = i.reflowLargerCreateNewLayout = i.reflowLargerGetLinesToRemove = void 0, i.reflowLargerGetLinesToRemove = function(a, u, d, _, g) {
                                 const v = [];
-                                for (let c = 0; c < h.length - 1; c++) {
+                                for (let c = 0; c < a.length - 1; c++) {
                                     let e = c,
-                                        s = h.get(++e);
+                                        s = a.get(++e);
                                     if (!s.isWrapped) continue;
-                                    const n = [h.get(c)];
-                                    for (; e < h.length && s.isWrapped;) n.push(s), s = h.get(++e);
+                                    const n = [a.get(c)];
+                                    for (; e < a.length && s.isWrapped;) n.push(s), s = a.get(++e);
                                     if (_ >= c && _ < e) {
                                         c += n.length - 1;
                                         continue
                                     }
                                     let t = 0,
-                                        r = o(n, t, u),
+                                        r = h(n, t, u),
                                         l = 1,
                                         f = 0;
                                     for (; l < n.length;) {
-                                        const a = o(n, l, u),
-                                            p = a - f,
+                                        const o = h(n, l, u),
+                                            p = o - f,
                                             C = d - r,
                                             y = Math.min(p, C);
-                                        n[t].copyCellsFrom(n[l], f, r, y, !1), r += y, r === d && (t++, r = 0), f += y, f === a && (l++, f = 0), r === 0 && t !== 0 && n[t - 1].getWidth(d - 1) === 2 && (n[t].copyCellsFrom(n[t - 1], d - 1, r++, 1, !1), n[t - 1].setCell(d - 1, g))
+                                        n[t].copyCellsFrom(n[l], f, r, y, !1), r += y, r === d && (t++, r = 0), f += y, f === o && (l++, f = 0), r === 0 && t !== 0 && n[t - 1].getWidth(d - 1) === 2 && (n[t].copyCellsFrom(n[t - 1], d - 1, r++, 1, !1), n[t - 1].setCell(d - 1, g))
                                     }
                                     n[t].replaceCells(r, d, g);
                                     let m = 0;
-                                    for (let a = n.length - 1; a > 0 && (a > t || n[a].getTrimmedLength() === 0); a--) m++;
+                                    for (let o = n.length - 1; o > 0 && (o > t || n[o].getTrimmedLength() === 0); o--) m++;
                                     m > 0 && (v.push(c + n.length - m), v.push(m)), c += n.length - 1
                                 }
                                 return v
-                            }, i.reflowLargerCreateNewLayout = function(h, u) {
+                            }, i.reflowLargerCreateNewLayout = function(a, u) {
                                 const d = [];
                                 let _ = 0,
                                     g = u[_],
                                     v = 0;
-                                for (let c = 0; c < h.length; c++)
+                                for (let c = 0; c < a.length; c++)
                                     if (g === c) {
                                         const e = u[++_];
-                                        h.onDeleteEmitter.fire({
+                                        a.onDeleteEmitter.fire({
                                             index: c - v,
                                             amount: e
                                         }), c += e - 1, v += e, g = u[++_]
                                     } else d.push(c);
                                 return {
                                     layout: d,
                                     countRemoved: v
                                 }
-                            }, i.reflowLargerApplyNewLayout = function(h, u) {
+                            }, i.reflowLargerApplyNewLayout = function(a, u) {
                                 const d = [];
-                                for (let _ = 0; _ < u.length; _++) d.push(h.get(u[_]));
-                                for (let _ = 0; _ < d.length; _++) h.set(_, d[_]);
-                                h.length = u.length
-                            }, i.reflowSmallerGetNewLineLengths = function(h, u, d) {
+                                for (let _ = 0; _ < u.length; _++) d.push(a.get(u[_]));
+                                for (let _ = 0; _ < d.length; _++) a.set(_, d[_]);
+                                a.length = u.length
+                            }, i.reflowSmallerGetNewLineLengths = function(a, u, d) {
                                 const _ = [],
-                                    g = h.map((s, n) => o(h, n, u)).reduce((s, n) => s + n);
+                                    g = a.map((s, n) => h(a, n, u)).reduce((s, n) => s + n);
                                 let v = 0,
                                     c = 0,
                                     e = 0;
                                 for (; e < g;) {
                                     if (g - e < d) {
                                         _.push(g - e);
                                         break
                                     }
                                     v += d;
-                                    const s = o(h, c, u);
+                                    const s = h(a, c, u);
                                     v > s && (v -= s, c++);
-                                    const n = h[c].getWidth(v - 1) === 2;
+                                    const n = a[c].getWidth(v - 1) === 2;
                                     n && v--;
                                     const t = n ? d - 1 : d;
                                     _.push(t), e += t
                                 }
                                 return _
-                            }, i.getWrappedLineTrimmedLength = o
+                            }, i.getWrappedLineTrimmedLength = h
                         },
-                        5295: (T, i, o) => {
+                        5295: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferSet = void 0;
-                            const h = o(9092),
-                                u = o(8460),
-                                d = o(844);
+                            const a = h(9092),
+                                u = h(8460),
+                                d = h(844);
                             class _ extends d.Disposable {
                                 constructor(v, c) {
                                     super(), this._optionsService = v, this._bufferService = c, this._onBufferActivate = this.register(new u.EventEmitter), this.onBufferActivate = this._onBufferActivate.event, this.reset(), this.register(this._optionsService.onSpecificOptionChange("scrollback", () => this.resize(this._bufferService.cols, this._bufferService.rows))), this.register(this._optionsService.onSpecificOptionChange("tabStopWidth", () => this.setupTabStops()))
                                 }
                                 reset() {
-                                    this._normal = new h.Buffer(!0, this._optionsService, this._bufferService), this._normal.fillViewportRows(), this._alt = new h.Buffer(!1, this._optionsService, this._bufferService), this._activeBuffer = this._normal, this._onBufferActivate.fire({
+                                    this._normal = new a.Buffer(!0, this._optionsService, this._bufferService), this._normal.fillViewportRows(), this._alt = new a.Buffer(!1, this._optionsService, this._bufferService), this._activeBuffer = this._normal, this._onBufferActivate.fire({
                                         activeBuffer: this._normal,
                                         inactiveBuffer: this._alt
                                     }), this.setupTabStops()
                                 }
                                 get alt() {
                                     return this._alt
                                 }
@@ -5155,21 +5155,21 @@
                                 }
                                 setupTabStops(v) {
                                     this._normal.setupTabStops(v), this._alt.setupTabStops(v)
                                 }
                             }
                             i.BufferSet = _
                         },
-                        511: (T, i, o) => {
+                        511: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CellData = void 0;
-                            const h = o(482),
-                                u = o(643),
-                                d = o(3734);
+                            const a = h(482),
+                                u = h(643),
+                                d = h(3734);
                             class _ extends d.AttributeData {
                                 constructor() {
                                     super(...arguments), this.content = 0, this.fg = 0, this.bg = 0, this.extended = new d.ExtendedAttrs, this.combinedData = ""
                                 }
                                 static fromCharData(v) {
                                     const c = new _;
                                     return c.setFromCharData(v), c
@@ -5177,15 +5177,15 @@
                                 isCombined() {
                                     return 2097152 & this.content
                                 }
                                 getWidth() {
                                     return this.content >> 22
                                 }
                                 getChars() {
-                                    return 2097152 & this.content ? this.combinedData : 2097151 & this.content ? (0, h.stringFromCodePoint)(2097151 & this.content) : ""
+                                    return 2097152 & this.content ? this.combinedData : 2097151 & this.content ? (0, a.stringFromCodePoint)(2097151 & this.content) : ""
                                 }
                                 getCode() {
                                     return this.isCombined() ? this.combinedData.charCodeAt(this.combinedData.length - 1) : 2097151 & this.content
                                 }
                                 setFromCharData(v) {
                                     this.fg = v[u.CHAR_DATA_ATTR_INDEX], this.bg = 0;
                                     let c = !1;
@@ -5206,23 +5206,23 @@
                             i.CellData = _
                         },
                         643: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.WHITESPACE_CELL_CODE = i.WHITESPACE_CELL_WIDTH = i.WHITESPACE_CELL_CHAR = i.NULL_CELL_CODE = i.NULL_CELL_WIDTH = i.NULL_CELL_CHAR = i.CHAR_DATA_CODE_INDEX = i.CHAR_DATA_WIDTH_INDEX = i.CHAR_DATA_CHAR_INDEX = i.CHAR_DATA_ATTR_INDEX = i.DEFAULT_EXT = i.DEFAULT_ATTR = i.DEFAULT_COLOR = void 0, i.DEFAULT_COLOR = 0, i.DEFAULT_ATTR = 256 | i.DEFAULT_COLOR << 9, i.DEFAULT_EXT = 0, i.CHAR_DATA_ATTR_INDEX = 0, i.CHAR_DATA_CHAR_INDEX = 1, i.CHAR_DATA_WIDTH_INDEX = 2, i.CHAR_DATA_CODE_INDEX = 3, i.NULL_CELL_CHAR = "", i.NULL_CELL_WIDTH = 1, i.NULL_CELL_CODE = 0, i.WHITESPACE_CELL_CHAR = " ", i.WHITESPACE_CELL_WIDTH = 1, i.WHITESPACE_CELL_CODE = 32
                         },
-                        4863: (T, i, o) => {
+                        4863: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.Marker = void 0;
-                            const h = o(8460),
-                                u = o(844);
+                            const a = h(8460),
+                                u = h(844);
                             class d {
                                 constructor(g) {
-                                    this.line = g, this.isDisposed = !1, this._disposables = [], this._id = d._nextId++, this._onDispose = this.register(new h.EventEmitter), this.onDispose = this._onDispose.event
+                                    this.line = g, this.isDisposed = !1, this._disposables = [], this._id = d._nextId++, this._onDispose = this.register(new a.EventEmitter), this.onDispose = this._onDispose.event
                                 }
                                 get id() {
                                     return this._id
                                 }
                                 dispose() {
                                     this.isDisposed || (this.isDisposed = !0, this.line = -1, this._onDispose.fire(), (0, u.disposeArray)(this._disposables), this._disposables.length = 0)
                                 }
@@ -5373,28 +5373,28 @@
                                 "{": "ä",
                                 "|": "ö",
                                 "}": "ü",
                                 "~": "û"
                             }
                         },
                         2584: (T, i) => {
-                            var o, h;
+                            var h, a;
                             Object.defineProperty(i, "__esModule", {
                                     value: !0
                                 }), i.C1_ESCAPED = i.C1 = i.C0 = void 0,
                                 function(u) {
                                     u.NUL = "\0", u.SOH = "", u.STX = "", u.ETX = "", u.EOT = "", u.ENQ = "", u.ACK = "", u.BEL = "\x07", u.BS = "\b", u.HT = "	", u.LF = `
 `, u.VT = "\v", u.FF = "\f", u.CR = "\r", u.SO = "", u.SI = "", u.DLE = "", u.DC1 = "", u.DC2 = "", u.DC3 = "", u.DC4 = "", u.NAK = "", u.SYN = "", u.ETB = "", u.CAN = "", u.EM = "", u.SUB = "", u.ESC = "\x1B", u.FS = "", u.GS = "", u.RS = "", u.US = "", u.SP = " ", u.DEL = ""
-                                }(o = i.C0 || (i.C0 = {})), (h = i.C1 || (i.C1 = {})).PAD = "", h.HOP = "", h.BPH = "", h.NBH = "", h.IND = "", h.NEL = "", h.SSA = "", h.ESA = "", h.HTS = "", h.HTJ = "", h.VTS = "", h.PLD = "", h.PLU = "", h.RI = "", h.SS2 = "", h.SS3 = "", h.DCS = "", h.PU1 = "", h.PU2 = "", h.STS = "", h.CCH = "", h.MW = "", h.SPA = "", h.EPA = "", h.SOS = "", h.SGCI = "", h.SCI = "", h.CSI = "", h.ST = "", h.OSC = "", h.PM = "", h.APC = "", (i.C1_ESCAPED || (i.C1_ESCAPED = {})).ST = `${o.ESC}\\`
+                                }(h = i.C0 || (i.C0 = {})), (a = i.C1 || (i.C1 = {})).PAD = "", a.HOP = "", a.BPH = "", a.NBH = "", a.IND = "", a.NEL = "", a.SSA = "", a.ESA = "", a.HTS = "", a.HTJ = "", a.VTS = "", a.PLD = "", a.PLU = "", a.RI = "", a.SS2 = "", a.SS3 = "", a.DCS = "", a.PU1 = "", a.PU2 = "", a.STS = "", a.CCH = "", a.MW = "", a.SPA = "", a.EPA = "", a.SOS = "", a.SGCI = "", a.SCI = "", a.CSI = "", a.ST = "", a.OSC = "", a.PM = "", a.APC = "", (i.C1_ESCAPED || (i.C1_ESCAPED = {})).ST = `${h.ESC}\\`
                         },
-                        7399: (T, i, o) => {
+                        7399: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.evaluateKeyboardEvent = void 0;
-                            const h = o(2584),
+                            const a = h(2584),
                                 u = {
                                     48: ["0", ")"],
                                     49: ["1", "!"],
                                     50: ["2", "@"],
                                     51: ["3", "#"],
                                     52: ["4", "$"],
                                     53: ["5", "%"],
@@ -5419,256 +5419,256 @@
                                         type: 0,
                                         cancel: !1,
                                         key: void 0
                                     },
                                     e = (d.shiftKey ? 1 : 0) | (d.altKey ? 2 : 0) | (d.ctrlKey ? 4 : 0) | (d.metaKey ? 8 : 0);
                                 switch (d.keyCode) {
                                     case 0:
-                                        d.key === "UIKeyInputUpArrow" ? c.key = _ ? h.C0.ESC + "OA" : h.C0.ESC + "[A" : d.key === "UIKeyInputLeftArrow" ? c.key = _ ? h.C0.ESC + "OD" : h.C0.ESC + "[D" : d.key === "UIKeyInputRightArrow" ? c.key = _ ? h.C0.ESC + "OC" : h.C0.ESC + "[C" : d.key === "UIKeyInputDownArrow" && (c.key = _ ? h.C0.ESC + "OB" : h.C0.ESC + "[B");
+                                        d.key === "UIKeyInputUpArrow" ? c.key = _ ? a.C0.ESC + "OA" : a.C0.ESC + "[A" : d.key === "UIKeyInputLeftArrow" ? c.key = _ ? a.C0.ESC + "OD" : a.C0.ESC + "[D" : d.key === "UIKeyInputRightArrow" ? c.key = _ ? a.C0.ESC + "OC" : a.C0.ESC + "[C" : d.key === "UIKeyInputDownArrow" && (c.key = _ ? a.C0.ESC + "OB" : a.C0.ESC + "[B");
                                         break;
                                     case 8:
                                         if (d.altKey) {
-                                            c.key = h.C0.ESC + h.C0.DEL;
+                                            c.key = a.C0.ESC + a.C0.DEL;
                                             break
                                         }
-                                        c.key = h.C0.DEL;
+                                        c.key = a.C0.DEL;
                                         break;
                                     case 9:
                                         if (d.shiftKey) {
-                                            c.key = h.C0.ESC + "[Z";
+                                            c.key = a.C0.ESC + "[Z";
                                             break
                                         }
-                                        c.key = h.C0.HT, c.cancel = !0;
+                                        c.key = a.C0.HT, c.cancel = !0;
                                         break;
                                     case 13:
-                                        c.key = d.altKey ? h.C0.ESC + h.C0.CR : h.C0.CR, c.cancel = !0;
+                                        c.key = d.altKey ? a.C0.ESC + a.C0.CR : a.C0.CR, c.cancel = !0;
                                         break;
                                     case 27:
-                                        c.key = h.C0.ESC, d.altKey && (c.key = h.C0.ESC + h.C0.ESC), c.cancel = !0;
+                                        c.key = a.C0.ESC, d.altKey && (c.key = a.C0.ESC + a.C0.ESC), c.cancel = !0;
                                         break;
                                     case 37:
                                         if (d.metaKey) break;
-                                        e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "D", c.key === h.C0.ESC + "[1;3D" && (c.key = h.C0.ESC + (g ? "b" : "[1;5D"))) : c.key = _ ? h.C0.ESC + "OD" : h.C0.ESC + "[D";
+                                        e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "D", c.key === a.C0.ESC + "[1;3D" && (c.key = a.C0.ESC + (g ? "b" : "[1;5D"))) : c.key = _ ? a.C0.ESC + "OD" : a.C0.ESC + "[D";
                                         break;
                                     case 39:
                                         if (d.metaKey) break;
-                                        e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "C", c.key === h.C0.ESC + "[1;3C" && (c.key = h.C0.ESC + (g ? "f" : "[1;5C"))) : c.key = _ ? h.C0.ESC + "OC" : h.C0.ESC + "[C";
+                                        e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "C", c.key === a.C0.ESC + "[1;3C" && (c.key = a.C0.ESC + (g ? "f" : "[1;5C"))) : c.key = _ ? a.C0.ESC + "OC" : a.C0.ESC + "[C";
                                         break;
                                     case 38:
                                         if (d.metaKey) break;
-                                        e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "A", g || c.key !== h.C0.ESC + "[1;3A" || (c.key = h.C0.ESC + "[1;5A")) : c.key = _ ? h.C0.ESC + "OA" : h.C0.ESC + "[A";
+                                        e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "A", g || c.key !== a.C0.ESC + "[1;3A" || (c.key = a.C0.ESC + "[1;5A")) : c.key = _ ? a.C0.ESC + "OA" : a.C0.ESC + "[A";
                                         break;
                                     case 40:
                                         if (d.metaKey) break;
-                                        e ? (c.key = h.C0.ESC + "[1;" + (e + 1) + "B", g || c.key !== h.C0.ESC + "[1;3B" || (c.key = h.C0.ESC + "[1;5B")) : c.key = _ ? h.C0.ESC + "OB" : h.C0.ESC + "[B";
+                                        e ? (c.key = a.C0.ESC + "[1;" + (e + 1) + "B", g || c.key !== a.C0.ESC + "[1;3B" || (c.key = a.C0.ESC + "[1;5B")) : c.key = _ ? a.C0.ESC + "OB" : a.C0.ESC + "[B";
                                         break;
                                     case 45:
-                                        d.shiftKey || d.ctrlKey || (c.key = h.C0.ESC + "[2~");
+                                        d.shiftKey || d.ctrlKey || (c.key = a.C0.ESC + "[2~");
                                         break;
                                     case 46:
-                                        c.key = e ? h.C0.ESC + "[3;" + (e + 1) + "~" : h.C0.ESC + "[3~";
+                                        c.key = e ? a.C0.ESC + "[3;" + (e + 1) + "~" : a.C0.ESC + "[3~";
                                         break;
                                     case 36:
-                                        c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "H" : _ ? h.C0.ESC + "OH" : h.C0.ESC + "[H";
+                                        c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "H" : _ ? a.C0.ESC + "OH" : a.C0.ESC + "[H";
                                         break;
                                     case 35:
-                                        c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "F" : _ ? h.C0.ESC + "OF" : h.C0.ESC + "[F";
+                                        c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "F" : _ ? a.C0.ESC + "OF" : a.C0.ESC + "[F";
                                         break;
                                     case 33:
-                                        d.shiftKey ? c.type = 2 : d.ctrlKey ? c.key = h.C0.ESC + "[5;" + (e + 1) + "~" : c.key = h.C0.ESC + "[5~";
+                                        d.shiftKey ? c.type = 2 : d.ctrlKey ? c.key = a.C0.ESC + "[5;" + (e + 1) + "~" : c.key = a.C0.ESC + "[5~";
                                         break;
                                     case 34:
-                                        d.shiftKey ? c.type = 3 : d.ctrlKey ? c.key = h.C0.ESC + "[6;" + (e + 1) + "~" : c.key = h.C0.ESC + "[6~";
+                                        d.shiftKey ? c.type = 3 : d.ctrlKey ? c.key = a.C0.ESC + "[6;" + (e + 1) + "~" : c.key = a.C0.ESC + "[6~";
                                         break;
                                     case 112:
-                                        c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "P" : h.C0.ESC + "OP";
+                                        c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "P" : a.C0.ESC + "OP";
                                         break;
                                     case 113:
-                                        c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "Q" : h.C0.ESC + "OQ";
+                                        c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "Q" : a.C0.ESC + "OQ";
                                         break;
                                     case 114:
-                                        c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "R" : h.C0.ESC + "OR";
+                                        c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "R" : a.C0.ESC + "OR";
                                         break;
                                     case 115:
-                                        c.key = e ? h.C0.ESC + "[1;" + (e + 1) + "S" : h.C0.ESC + "OS";
+                                        c.key = e ? a.C0.ESC + "[1;" + (e + 1) + "S" : a.C0.ESC + "OS";
                                         break;
                                     case 116:
-                                        c.key = e ? h.C0.ESC + "[15;" + (e + 1) + "~" : h.C0.ESC + "[15~";
+                                        c.key = e ? a.C0.ESC + "[15;" + (e + 1) + "~" : a.C0.ESC + "[15~";
                                         break;
                                     case 117:
-                                        c.key = e ? h.C0.ESC + "[17;" + (e + 1) + "~" : h.C0.ESC + "[17~";
+                                        c.key = e ? a.C0.ESC + "[17;" + (e + 1) + "~" : a.C0.ESC + "[17~";
                                         break;
                                     case 118:
-                                        c.key = e ? h.C0.ESC + "[18;" + (e + 1) + "~" : h.C0.ESC + "[18~";
+                                        c.key = e ? a.C0.ESC + "[18;" + (e + 1) + "~" : a.C0.ESC + "[18~";
                                         break;
                                     case 119:
-                                        c.key = e ? h.C0.ESC + "[19;" + (e + 1) + "~" : h.C0.ESC + "[19~";
+                                        c.key = e ? a.C0.ESC + "[19;" + (e + 1) + "~" : a.C0.ESC + "[19~";
                                         break;
                                     case 120:
-                                        c.key = e ? h.C0.ESC + "[20;" + (e + 1) + "~" : h.C0.ESC + "[20~";
+                                        c.key = e ? a.C0.ESC + "[20;" + (e + 1) + "~" : a.C0.ESC + "[20~";
                                         break;
                                     case 121:
-                                        c.key = e ? h.C0.ESC + "[21;" + (e + 1) + "~" : h.C0.ESC + "[21~";
+                                        c.key = e ? a.C0.ESC + "[21;" + (e + 1) + "~" : a.C0.ESC + "[21~";
                                         break;
                                     case 122:
-                                        c.key = e ? h.C0.ESC + "[23;" + (e + 1) + "~" : h.C0.ESC + "[23~";
+                                        c.key = e ? a.C0.ESC + "[23;" + (e + 1) + "~" : a.C0.ESC + "[23~";
                                         break;
                                     case 123:
-                                        c.key = e ? h.C0.ESC + "[24;" + (e + 1) + "~" : h.C0.ESC + "[24~";
+                                        c.key = e ? a.C0.ESC + "[24;" + (e + 1) + "~" : a.C0.ESC + "[24~";
                                         break;
                                     default:
                                         if (!d.ctrlKey || d.shiftKey || d.altKey || d.metaKey)
-                                            if (g && !v || !d.altKey || d.metaKey) !g || d.altKey || d.ctrlKey || d.shiftKey || !d.metaKey ? d.key && !d.ctrlKey && !d.altKey && !d.metaKey && d.keyCode >= 48 && d.key.length === 1 ? c.key = d.key : d.key && d.ctrlKey && (d.key === "_" && (c.key = h.C0.US), d.key === "@" && (c.key = h.C0.NUL)) : d.keyCode === 65 && (c.type = 1);
+                                            if (g && !v || !d.altKey || d.metaKey) !g || d.altKey || d.ctrlKey || d.shiftKey || !d.metaKey ? d.key && !d.ctrlKey && !d.altKey && !d.metaKey && d.keyCode >= 48 && d.key.length === 1 ? c.key = d.key : d.key && d.ctrlKey && (d.key === "_" && (c.key = a.C0.US), d.key === "@" && (c.key = a.C0.NUL)) : d.keyCode === 65 && (c.type = 1);
                                             else {
                                                 const s = u[d.keyCode],
                                                     n = s == null ? void 0 : s[d.shiftKey ? 1 : 0];
-                                                if (n) c.key = h.C0.ESC + n;
+                                                if (n) c.key = a.C0.ESC + n;
                                                 else if (d.keyCode >= 65 && d.keyCode <= 90) {
                                                     const t = d.ctrlKey ? d.keyCode - 64 : d.keyCode + 32;
                                                     let r = String.fromCharCode(t);
-                                                    d.shiftKey && (r = r.toUpperCase()), c.key = h.C0.ESC + r
-                                                } else if (d.keyCode === 32) c.key = h.C0.ESC + (d.ctrlKey ? h.C0.NUL : " ");
+                                                    d.shiftKey && (r = r.toUpperCase()), c.key = a.C0.ESC + r
+                                                } else if (d.keyCode === 32) c.key = a.C0.ESC + (d.ctrlKey ? a.C0.NUL : " ");
                                                 else if (d.key === "Dead" && d.code.startsWith("Key")) {
                                                     let t = d.code.slice(3, 4);
-                                                    d.shiftKey || (t = t.toLowerCase()), c.key = h.C0.ESC + t, c.cancel = !0
+                                                    d.shiftKey || (t = t.toLowerCase()), c.key = a.C0.ESC + t, c.cancel = !0
                                                 }
                                             }
-                                        else d.keyCode >= 65 && d.keyCode <= 90 ? c.key = String.fromCharCode(d.keyCode - 64) : d.keyCode === 32 ? c.key = h.C0.NUL : d.keyCode >= 51 && d.keyCode <= 55 ? c.key = String.fromCharCode(d.keyCode - 51 + 27) : d.keyCode === 56 ? c.key = h.C0.DEL : d.keyCode === 219 ? c.key = h.C0.ESC : d.keyCode === 220 ? c.key = h.C0.FS : d.keyCode === 221 && (c.key = h.C0.GS)
+                                        else d.keyCode >= 65 && d.keyCode <= 90 ? c.key = String.fromCharCode(d.keyCode - 64) : d.keyCode === 32 ? c.key = a.C0.NUL : d.keyCode >= 51 && d.keyCode <= 55 ? c.key = String.fromCharCode(d.keyCode - 51 + 27) : d.keyCode === 56 ? c.key = a.C0.DEL : d.keyCode === 219 ? c.key = a.C0.ESC : d.keyCode === 220 ? c.key = a.C0.FS : d.keyCode === 221 && (c.key = a.C0.GS)
                                 }
                                 return c
                             }
                         },
                         482: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.Utf8ToUtf32 = i.StringToUtf32 = i.utf32ToString = i.stringFromCodePoint = void 0, i.stringFromCodePoint = function(o) {
-                                return o > 65535 ? (o -= 65536, String.fromCharCode(55296 + (o >> 10)) + String.fromCharCode(o % 1024 + 56320)) : String.fromCharCode(o)
-                            }, i.utf32ToString = function(o, h = 0, u = o.length) {
+                            }), i.Utf8ToUtf32 = i.StringToUtf32 = i.utf32ToString = i.stringFromCodePoint = void 0, i.stringFromCodePoint = function(h) {
+                                return h > 65535 ? (h -= 65536, String.fromCharCode(55296 + (h >> 10)) + String.fromCharCode(h % 1024 + 56320)) : String.fromCharCode(h)
+                            }, i.utf32ToString = function(h, a = 0, u = h.length) {
                                 let d = "";
-                                for (let _ = h; _ < u; ++_) {
-                                    let g = o[_];
+                                for (let _ = a; _ < u; ++_) {
+                                    let g = h[_];
                                     g > 65535 ? (g -= 65536, d += String.fromCharCode(55296 + (g >> 10)) + String.fromCharCode(g % 1024 + 56320)) : d += String.fromCharCode(g)
                                 }
                                 return d
                             }, i.StringToUtf32 = class {
                                 constructor() {
                                     this._interim = 0
                                 }
                                 clear() {
                                     this._interim = 0
                                 }
-                                decode(o, h) {
-                                    const u = o.length;
+                                decode(h, a) {
+                                    const u = h.length;
                                     if (!u) return 0;
                                     let d = 0,
                                         _ = 0;
                                     if (this._interim) {
-                                        const g = o.charCodeAt(_++);
-                                        56320 <= g && g <= 57343 ? h[d++] = 1024 * (this._interim - 55296) + g - 56320 + 65536 : (h[d++] = this._interim, h[d++] = g), this._interim = 0
+                                        const g = h.charCodeAt(_++);
+                                        56320 <= g && g <= 57343 ? a[d++] = 1024 * (this._interim - 55296) + g - 56320 + 65536 : (a[d++] = this._interim, a[d++] = g), this._interim = 0
                                     }
                                     for (let g = _; g < u; ++g) {
-                                        const v = o.charCodeAt(g);
+                                        const v = h.charCodeAt(g);
                                         if (55296 <= v && v <= 56319) {
                                             if (++g >= u) return this._interim = v, d;
-                                            const c = o.charCodeAt(g);
-                                            56320 <= c && c <= 57343 ? h[d++] = 1024 * (v - 55296) + c - 56320 + 65536 : (h[d++] = v, h[d++] = c)
-                                        } else v !== 65279 && (h[d++] = v)
+                                            const c = h.charCodeAt(g);
+                                            56320 <= c && c <= 57343 ? a[d++] = 1024 * (v - 55296) + c - 56320 + 65536 : (a[d++] = v, a[d++] = c)
+                                        } else v !== 65279 && (a[d++] = v)
                                     }
                                     return d
                                 }
                             }, i.Utf8ToUtf32 = class {
                                 constructor() {
                                     this.interim = new Uint8Array(3)
                                 }
                                 clear() {
                                     this.interim.fill(0)
                                 }
-                                decode(o, h) {
-                                    const u = o.length;
+                                decode(h, a) {
+                                    const u = h.length;
                                     if (!u) return 0;
                                     let d, _, g, v, c = 0,
                                         e = 0,
                                         s = 0;
                                     if (this.interim[0]) {
                                         let r = !1,
                                             l = this.interim[0];
                                         l &= (224 & l) == 192 ? 31 : (240 & l) == 224 ? 15 : 7;
                                         let f, m = 0;
                                         for (;
                                             (f = 63 & this.interim[++m]) && m < 4;) l <<= 6, l |= f;
-                                        const a = (224 & this.interim[0]) == 192 ? 2 : (240 & this.interim[0]) == 224 ? 3 : 4,
-                                            p = a - m;
+                                        const o = (224 & this.interim[0]) == 192 ? 2 : (240 & this.interim[0]) == 224 ? 3 : 4,
+                                            p = o - m;
                                         for (; s < p;) {
                                             if (s >= u) return 0;
-                                            if (f = o[s++], (192 & f) != 128) {
+                                            if (f = h[s++], (192 & f) != 128) {
                                                 s--, r = !0;
                                                 break
                                             }
                                             this.interim[m++] = f, l <<= 6, l |= 63 & f
                                         }
-                                        r || (a === 2 ? l < 128 ? s-- : h[c++] = l : a === 3 ? l < 2048 || l >= 55296 && l <= 57343 || l === 65279 || (h[c++] = l) : l < 65536 || l > 1114111 || (h[c++] = l)), this.interim.fill(0)
+                                        r || (o === 2 ? l < 128 ? s-- : a[c++] = l : o === 3 ? l < 2048 || l >= 55296 && l <= 57343 || l === 65279 || (a[c++] = l) : l < 65536 || l > 1114111 || (a[c++] = l)), this.interim.fill(0)
                                     }
                                     const n = u - 4;
                                     let t = s;
                                     for (; t < u;) {
-                                        for (; !(!(t < n) || 128 & (d = o[t]) || 128 & (_ = o[t + 1]) || 128 & (g = o[t + 2]) || 128 & (v = o[t + 3]));) h[c++] = d, h[c++] = _, h[c++] = g, h[c++] = v, t += 4;
-                                        if (d = o[t++], d < 128) h[c++] = d;
+                                        for (; !(!(t < n) || 128 & (d = h[t]) || 128 & (_ = h[t + 1]) || 128 & (g = h[t + 2]) || 128 & (v = h[t + 3]));) a[c++] = d, a[c++] = _, a[c++] = g, a[c++] = v, t += 4;
+                                        if (d = h[t++], d < 128) a[c++] = d;
                                         else if ((224 & d) == 192) {
                                             if (t >= u) return this.interim[0] = d, c;
-                                            if (_ = o[t++], (192 & _) != 128) {
+                                            if (_ = h[t++], (192 & _) != 128) {
                                                 t--;
                                                 continue
                                             }
                                             if (e = (31 & d) << 6 | 63 & _, e < 128) {
                                                 t--;
                                                 continue
                                             }
-                                            h[c++] = e
+                                            a[c++] = e
                                         } else if ((240 & d) == 224) {
                                             if (t >= u) return this.interim[0] = d, c;
-                                            if (_ = o[t++], (192 & _) != 128) {
+                                            if (_ = h[t++], (192 & _) != 128) {
                                                 t--;
                                                 continue
                                             }
                                             if (t >= u) return this.interim[0] = d, this.interim[1] = _, c;
-                                            if (g = o[t++], (192 & g) != 128) {
+                                            if (g = h[t++], (192 & g) != 128) {
                                                 t--;
                                                 continue
                                             }
                                             if (e = (15 & d) << 12 | (63 & _) << 6 | 63 & g, e < 2048 || e >= 55296 && e <= 57343 || e === 65279) continue;
-                                            h[c++] = e
+                                            a[c++] = e
                                         } else if ((248 & d) == 240) {
                                             if (t >= u) return this.interim[0] = d, c;
-                                            if (_ = o[t++], (192 & _) != 128) {
+                                            if (_ = h[t++], (192 & _) != 128) {
                                                 t--;
                                                 continue
                                             }
                                             if (t >= u) return this.interim[0] = d, this.interim[1] = _, c;
-                                            if (g = o[t++], (192 & g) != 128) {
+                                            if (g = h[t++], (192 & g) != 128) {
                                                 t--;
                                                 continue
                                             }
                                             if (t >= u) return this.interim[0] = d, this.interim[1] = _, this.interim[2] = g, c;
-                                            if (v = o[t++], (192 & v) != 128) {
+                                            if (v = h[t++], (192 & v) != 128) {
                                                 t--;
                                                 continue
                                             }
                                             if (e = (7 & d) << 18 | (63 & _) << 12 | (63 & g) << 6 | 63 & v, e < 65536 || e > 1114111) continue;
-                                            h[c++] = e
+                                            a[c++] = e
                                         }
                                     }
                                     return c
                                 }
                             }
                         },
                         225: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.UnicodeV6 = void 0;
-                            const o = [
+                            const h = [
                                     [768, 879],
                                     [1155, 1158],
                                     [1160, 1161],
                                     [1425, 1469],
                                     [1471, 1471],
                                     [1473, 1474],
                                     [1476, 1477],
@@ -5791,15 +5791,15 @@
                                     [43045, 43046],
                                     [64286, 64286],
                                     [65024, 65039],
                                     [65056, 65059],
                                     [65279, 65279],
                                     [65529, 65531]
                                 ],
-                                h = [
+                                a = [
                                     [68097, 68099],
                                     [68101, 68102],
                                     [68108, 68111],
                                     [68152, 68154],
                                     [68159, 68159],
                                     [119143, 119145],
                                     [119155, 119170],
@@ -5811,41 +5811,41 @@
                                     [917760, 917999]
                                 ];
                             let u;
                             i.UnicodeV6 = class {
                                 constructor() {
                                     if (this.version = "6", !u) {
                                         u = new Uint8Array(65536), u.fill(1), u[0] = 0, u.fill(0, 1, 32), u.fill(0, 127, 160), u.fill(2, 4352, 4448), u[9001] = 2, u[9002] = 2, u.fill(2, 11904, 42192), u[12351] = 1, u.fill(2, 44032, 55204), u.fill(2, 63744, 64256), u.fill(2, 65040, 65050), u.fill(2, 65072, 65136), u.fill(2, 65280, 65377), u.fill(2, 65504, 65511);
-                                        for (let d = 0; d < o.length; ++d) u.fill(0, o[d][0], o[d][1] + 1)
+                                        for (let d = 0; d < h.length; ++d) u.fill(0, h[d][0], h[d][1] + 1)
                                     }
                                 }
                                 wcwidth(d) {
                                     return d < 32 ? 0 : d < 127 ? 1 : d < 65536 ? u[d] : function(_, g) {
                                         let v, c = 0,
                                             e = g.length - 1;
                                         if (_ < g[0][0] || _ > g[e][1]) return !1;
                                         for (; e >= c;)
                                             if (v = c + e >> 1, _ > g[v][1]) c = v + 1;
                                             else {
                                                 if (!(_ < g[v][0])) return !0;
                                                 e = v - 1
                                             } return !1
-                                    }(d, h) ? 0 : d >= 131072 && d <= 196605 || d >= 196608 && d <= 262141 ? 2 : 1
+                                    }(d, a) ? 0 : d >= 131072 && d <= 196605 || d >= 196608 && d <= 262141 ? 2 : 1
                                 }
                             }
                         },
-                        5981: (T, i, o) => {
+                        5981: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.WriteBuffer = void 0;
-                            const h = o(8460),
-                                u = o(844);
+                            const a = h(8460),
+                                u = h(844);
                             class d extends u.Disposable {
                                 constructor(g) {
-                                    super(), this._action = g, this._writeBuffer = [], this._callbacks = [], this._pendingData = 0, this._bufferOffset = 0, this._isSyncWriting = !1, this._syncCalls = 0, this._didUserInput = !1, this._onWriteParsed = this.register(new h.EventEmitter), this.onWriteParsed = this._onWriteParsed.event
+                                    super(), this._action = g, this._writeBuffer = [], this._callbacks = [], this._pendingData = 0, this._bufferOffset = 0, this._isSyncWriting = !1, this._syncCalls = 0, this._didUserInput = !1, this._onWriteParsed = this.register(new a.EventEmitter), this.onWriteParsed = this._onWriteParsed.event
                                 }
                                 handleUserInput() {
                                     this._didUserInput = !0
                                 }
                                 writeSync(g, v) {
                                     if (v !== void 0 && this._syncCalls > v) return void(this._syncCalls = 0);
                                     if (this._pendingData += g.length, this._writeBuffer.push(g), this._callbacks.push(void 0), this._syncCalls++, this._isSyncWriting) return;
@@ -5884,16 +5884,16 @@
                             }
                             i.WriteBuffer = d
                         },
                         5941: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.toRgbString = i.parseColor = void 0;
-                            const o = /^([\da-f])\/([\da-f])\/([\da-f])$|^([\da-f]{2})\/([\da-f]{2})\/([\da-f]{2})$|^([\da-f]{3})\/([\da-f]{3})\/([\da-f]{3})$|^([\da-f]{4})\/([\da-f]{4})\/([\da-f]{4})$/,
-                                h = /^[\da-f]+$/;
+                            const h = /^([\da-f])\/([\da-f])\/([\da-f])$|^([\da-f]{2})\/([\da-f]{2})\/([\da-f]{2})$|^([\da-f]{3})\/([\da-f]{3})\/([\da-f]{3})$|^([\da-f]{4})\/([\da-f]{4})\/([\da-f]{4})$/,
+                                a = /^[\da-f]+$/;
 
                             function u(d, _) {
                                 const g = d.toString(16),
                                     v = g.length < 2 ? "0" + g : g;
                                 switch (_) {
                                     case 4:
                                         return g[0];
@@ -5906,20 +5906,20 @@
                                 }
                             }
                             i.parseColor = function(d) {
                                 if (!d) return;
                                 let _ = d.toLowerCase();
                                 if (_.indexOf("rgb:") === 0) {
                                     _ = _.slice(4);
-                                    const g = o.exec(_);
+                                    const g = h.exec(_);
                                     if (g) {
                                         const v = g[1] ? 15 : g[4] ? 255 : g[7] ? 4095 : 65535;
                                         return [Math.round(parseInt(g[1] || g[4] || g[7] || g[10], 16) / v * 255), Math.round(parseInt(g[2] || g[5] || g[8] || g[11], 16) / v * 255), Math.round(parseInt(g[3] || g[6] || g[9] || g[12], 16) / v * 255)]
                                     }
-                                } else if (_.indexOf("#") === 0 && (_ = _.slice(1), h.exec(_) && [3, 6, 9, 12].includes(_.length))) {
+                                } else if (_.indexOf("#") === 0 && (_ = _.slice(1), a.exec(_) && [3, 6, 9, 12].includes(_.length))) {
                                     const g = _.length / 3,
                                         v = [0, 0, 0];
                                     for (let c = 0; c < 3; ++c) {
                                         const e = parseInt(_.slice(g * c, g * c + g), 16);
                                         v[c] = g === 1 ? e << 4 : g === 2 ? e : g === 3 ? e >> 4 : e >> 8
                                     }
                                     return v
@@ -5930,21 +5930,21 @@
                             }
                         },
                         5770: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.PAYLOAD_LIMIT = void 0, i.PAYLOAD_LIMIT = 1e7
                         },
-                        6351: (T, i, o) => {
+                        6351: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.DcsHandler = i.DcsParser = void 0;
-                            const h = o(482),
-                                u = o(8742),
-                                d = o(5770),
+                            const a = h(482),
+                                u = h(8742),
+                                d = h(5770),
                                 _ = [];
                             i.DcsParser = class {
                                 constructor() {
                                     this._handlers = Object.create(null), this._active = _, this._ident = 0, this._handlerFb = () => {}, this._stack = {
                                         paused: !1,
                                         loopPosition: 0,
                                         fallThrough: !1
@@ -5978,15 +5978,15 @@
                                     if (this.reset(), this._ident = v, this._active = this._handlers[v] || _, this._active.length)
                                         for (let e = this._active.length - 1; e >= 0; e--) this._active[e].hook(c);
                                     else this._handlerFb(this._ident, "HOOK", c)
                                 }
                                 put(v, c, e) {
                                     if (this._active.length)
                                         for (let s = this._active.length - 1; s >= 0; s--) this._active[s].put(v, c, e);
-                                    else this._handlerFb(this._ident, "PUT", (0, h.utf32ToString)(v, c, e))
+                                    else this._handlerFb(this._ident, "PUT", (0, a.utf32ToString)(v, c, e))
                                 }
                                 unhook(v, c = !0) {
                                     if (this._active.length) {
                                         let e = !1,
                                             s = this._active.length - 1,
                                             n = !1;
                                         if (this._stack.paused && (s = this._stack.loopPosition - 1, e = c, n = this._stack.fallThrough, this._stack.paused = !1), !n && e === !1) {
@@ -6005,32 +6005,32 @@
                                 constructor(v) {
                                     this._handler = v, this._data = "", this._params = g, this._hitLimit = !1
                                 }
                                 hook(v) {
                                     this._params = v.length > 1 || v.params[0] ? v.clone() : g, this._data = "", this._hitLimit = !1
                                 }
                                 put(v, c, e) {
-                                    this._hitLimit || (this._data += (0, h.utf32ToString)(v, c, e), this._data.length > d.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0))
+                                    this._hitLimit || (this._data += (0, a.utf32ToString)(v, c, e), this._data.length > d.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0))
                                 }
                                 unhook(v) {
                                     let c = !1;
                                     if (this._hitLimit) c = !1;
                                     else if (v && (c = this._handler(this._data, this._params), c instanceof Promise)) return c.then(e => (this._params = g, this._data = "", this._hitLimit = !1, e));
                                     return this._params = g, this._data = "", this._hitLimit = !1, c
                                 }
                             }
                         },
-                        2015: (T, i, o) => {
+                        2015: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.EscapeSequenceParser = i.VT500_TRANSITION_TABLE = i.TransitionTable = void 0;
-                            const h = o(844),
-                                u = o(8742),
-                                d = o(6242),
-                                _ = o(6351);
+                            const a = h(844),
+                                u = h(8742),
+                                d = h(6242),
+                                _ = h(6351);
                             class g {
                                 constructor(s) {
                                     this.table = new Uint8Array(s)
                                 }
                                 setDefault(s, n) {
                                     this.table.fill(s << 4 | n)
                                 }
@@ -6041,33 +6041,33 @@
                                     for (let l = 0; l < s.length; l++) this.table[n << 8 | s[l]] = t << 4 | r
                                 }
                             }
                             i.TransitionTable = g;
                             const v = 160;
                             i.VT500_TRANSITION_TABLE = function() {
                                 const e = new g(4095),
-                                    s = Array.apply(null, Array(256)).map((m, a) => a),
-                                    n = (m, a) => s.slice(m, a),
+                                    s = Array.apply(null, Array(256)).map((m, o) => o),
+                                    n = (m, o) => s.slice(m, o),
                                     t = n(32, 127),
                                     r = n(0, 24);
                                 r.push(25), r.push.apply(r, n(28, 32));
                                 const l = n(0, 14);
                                 let f;
                                 for (f in e.setDefault(1, 0), e.addMany(t, 0, 2, 0), l) e.addMany([24, 26, 153, 154], f, 3, 0), e.addMany(n(128, 144), f, 3, 0), e.addMany(n(144, 152), f, 3, 0), e.add(156, f, 0, 0), e.add(27, f, 11, 1), e.add(157, f, 4, 8), e.addMany([152, 158, 159], f, 0, 7), e.add(155, f, 11, 3), e.add(144, f, 11, 9);
                                 return e.addMany(r, 0, 3, 0), e.addMany(r, 1, 3, 1), e.add(127, 1, 0, 1), e.addMany(r, 8, 0, 8), e.addMany(r, 3, 3, 3), e.add(127, 3, 0, 3), e.addMany(r, 4, 3, 4), e.add(127, 4, 0, 4), e.addMany(r, 6, 3, 6), e.addMany(r, 5, 3, 5), e.add(127, 5, 0, 5), e.addMany(r, 2, 3, 2), e.add(127, 2, 0, 2), e.add(93, 1, 4, 8), e.addMany(t, 8, 5, 8), e.add(127, 8, 5, 8), e.addMany([156, 27, 24, 26, 7], 8, 6, 0), e.addMany(n(28, 32), 8, 0, 8), e.addMany([88, 94, 95], 1, 0, 7), e.addMany(t, 7, 0, 7), e.addMany(r, 7, 0, 7), e.add(156, 7, 0, 0), e.add(127, 7, 0, 7), e.add(91, 1, 11, 3), e.addMany(n(64, 127), 3, 7, 0), e.addMany(n(48, 60), 3, 8, 4), e.addMany([60, 61, 62, 63], 3, 9, 4), e.addMany(n(48, 60), 4, 8, 4), e.addMany(n(64, 127), 4, 7, 0), e.addMany([60, 61, 62, 63], 4, 0, 6), e.addMany(n(32, 64), 6, 0, 6), e.add(127, 6, 0, 6), e.addMany(n(64, 127), 6, 0, 0), e.addMany(n(32, 48), 3, 9, 5), e.addMany(n(32, 48), 5, 9, 5), e.addMany(n(48, 64), 5, 0, 6), e.addMany(n(64, 127), 5, 7, 0), e.addMany(n(32, 48), 4, 9, 5), e.addMany(n(32, 48), 1, 9, 2), e.addMany(n(32, 48), 2, 9, 2), e.addMany(n(48, 127), 2, 10, 0), e.addMany(n(48, 80), 1, 10, 0), e.addMany(n(81, 88), 1, 10, 0), e.addMany([89, 90, 92], 1, 10, 0), e.addMany(n(96, 127), 1, 10, 0), e.add(80, 1, 11, 9), e.addMany(r, 9, 0, 9), e.add(127, 9, 0, 9), e.addMany(n(28, 32), 9, 0, 9), e.addMany(n(32, 48), 9, 9, 12), e.addMany(n(48, 60), 9, 8, 10), e.addMany([60, 61, 62, 63], 9, 9, 10), e.addMany(r, 11, 0, 11), e.addMany(n(32, 128), 11, 0, 11), e.addMany(n(28, 32), 11, 0, 11), e.addMany(r, 10, 0, 10), e.add(127, 10, 0, 10), e.addMany(n(28, 32), 10, 0, 10), e.addMany(n(48, 60), 10, 8, 10), e.addMany([60, 61, 62, 63], 10, 0, 11), e.addMany(n(32, 48), 10, 9, 12), e.addMany(r, 12, 0, 12), e.add(127, 12, 0, 12), e.addMany(n(28, 32), 12, 0, 12), e.addMany(n(32, 48), 12, 9, 12), e.addMany(n(48, 64), 12, 0, 11), e.addMany(n(64, 127), 12, 12, 13), e.addMany(n(64, 127), 10, 12, 13), e.addMany(n(64, 127), 9, 12, 13), e.addMany(r, 13, 13, 13), e.addMany(t, 13, 13, 13), e.add(127, 13, 0, 13), e.addMany([27, 156, 24, 26], 13, 14, 0), e.add(v, 0, 2, 0), e.add(v, 8, 5, 8), e.add(v, 6, 0, 6), e.add(v, 11, 0, 11), e.add(v, 13, 13, 13), e
                             }();
-                            class c extends h.Disposable {
+                            class c extends a.Disposable {
                                 constructor(s = i.VT500_TRANSITION_TABLE) {
                                     super(), this._transitions = s, this._parseStack = {
                                         state: 0,
                                         handlers: [],
                                         handlerPos: 0,
                                         transition: 0,
                                         chunkPos: 0
-                                    }, this.initialState = 0, this.currentState = this.initialState, this._params = new u.Params, this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0, this._printHandlerFb = (n, t, r) => {}, this._executeHandlerFb = n => {}, this._csiHandlerFb = (n, t) => {}, this._escHandlerFb = n => {}, this._errorHandlerFb = n => n, this._printHandler = this._printHandlerFb, this._executeHandlers = Object.create(null), this._csiHandlers = Object.create(null), this._escHandlers = Object.create(null), this.register((0, h.toDisposable)(() => {
+                                    }, this.initialState = 0, this.currentState = this.initialState, this._params = new u.Params, this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0, this._printHandlerFb = (n, t, r) => {}, this._executeHandlerFb = n => {}, this._csiHandlerFb = (n, t) => {}, this._escHandlerFb = n => {}, this._errorHandlerFb = n => n, this._printHandler = this._printHandlerFb, this._executeHandlers = Object.create(null), this._csiHandlers = Object.create(null), this._escHandlers = Object.create(null), this.register((0, a.toDisposable)(() => {
                                         this._csiHandlers = Object.create(null), this._executeHandlers = Object.create(null), this._escHandlers = Object.create(null)
                                     })), this._oscParser = this.register(new d.OscParser), this._dcsParser = this.register(new _.DcsParser), this._errorHandler = this._errorHandlerFb, this.registerEscHandler({
                                         final: "\\"
                                     }, () => !0)
                                 }
                                 _identifier(s, n = [64, 126]) {
                                     let t = 0;
@@ -6176,149 +6176,149 @@
                                     let r, l = 0,
                                         f = 0,
                                         m = 0;
                                     if (this._parseStack.state)
                                         if (this._parseStack.state === 2) this._parseStack.state = 0, m = this._parseStack.chunkPos + 1;
                                         else {
                                             if (t === void 0 || this._parseStack.state === 1) throw this._parseStack.state = 1, new Error("improper continuation due to previous async handler, giving up parsing");
-                                            const a = this._parseStack.handlers;
+                                            const o = this._parseStack.handlers;
                                             let p = this._parseStack.handlerPos - 1;
                                             switch (this._parseStack.state) {
                                                 case 3:
                                                     if (t === !1 && p > -1) {
-                                                        for (; p >= 0 && (r = a[p](this._params), r !== !0); p--)
+                                                        for (; p >= 0 && (r = o[p](this._params), r !== !0); p--)
                                                             if (r instanceof Promise) return this._parseStack.handlerPos = p, r
                                                     }
                                                     this._parseStack.handlers = [];
                                                     break;
                                                 case 4:
                                                     if (t === !1 && p > -1) {
-                                                        for (; p >= 0 && (r = a[p](), r !== !0); p--)
+                                                        for (; p >= 0 && (r = o[p](), r !== !0); p--)
                                                             if (r instanceof Promise) return this._parseStack.handlerPos = p, r
                                                     }
                                                     this._parseStack.handlers = [];
                                                     break;
                                                 case 6:
                                                     if (l = s[this._parseStack.chunkPos], r = this._dcsParser.unhook(l !== 24 && l !== 26, t), r) return r;
                                                     l === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0;
                                                     break;
                                                 case 5:
                                                     if (l = s[this._parseStack.chunkPos], r = this._oscParser.end(l !== 24 && l !== 26, t), r) return r;
                                                     l === 27 && (this._parseStack.transition |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0
                                             }
                                             this._parseStack.state = 0, m = this._parseStack.chunkPos + 1, this.precedingCodepoint = 0, this.currentState = 15 & this._parseStack.transition
-                                        } for (let a = m; a < n; ++a) {
-                                        switch (l = s[a], f = this._transitions.table[this.currentState << 8 | (l < 160 ? l : v)], f >> 4) {
+                                        } for (let o = m; o < n; ++o) {
+                                        switch (l = s[o], f = this._transitions.table[this.currentState << 8 | (l < 160 ? l : v)], f >> 4) {
                                             case 2:
-                                                for (let D = a + 1;; ++D) {
+                                                for (let D = o + 1;; ++D) {
                                                     if (D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                                                        this._printHandler(s, a, D), a = D - 1;
+                                                        this._printHandler(s, o, D), o = D - 1;
                                                         break
                                                     }
                                                     if (++D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                                                        this._printHandler(s, a, D), a = D - 1;
+                                                        this._printHandler(s, o, D), o = D - 1;
                                                         break
                                                     }
                                                     if (++D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                                                        this._printHandler(s, a, D), a = D - 1;
+                                                        this._printHandler(s, o, D), o = D - 1;
                                                         break
                                                     }
                                                     if (++D >= n || (l = s[D]) < 32 || l > 126 && l < v) {
-                                                        this._printHandler(s, a, D), a = D - 1;
+                                                        this._printHandler(s, o, D), o = D - 1;
                                                         break
                                                     }
                                                 }
                                                 break;
                                             case 3:
                                                 this._executeHandlers[l] ? this._executeHandlers[l]() : this._executeHandlerFb(l), this.precedingCodepoint = 0;
                                                 break;
                                             case 0:
                                                 break;
                                             case 1:
                                                 if (this._errorHandler({
-                                                        position: a,
+                                                        position: o,
                                                         code: l,
                                                         currentState: this.currentState,
                                                         collect: this._collect,
                                                         params: this._params,
                                                         abort: !1
                                                     }).abort) return;
                                                 break;
                                             case 7:
                                                 const p = this._csiHandlers[this._collect << 8 | l];
                                                 let C = p ? p.length - 1 : -1;
                                                 for (; C >= 0 && (r = p[C](this._params), r !== !0); C--)
-                                                    if (r instanceof Promise) return this._preserveStack(3, p, C, f, a), r;
+                                                    if (r instanceof Promise) return this._preserveStack(3, p, C, f, o), r;
                                                 C < 0 && this._csiHandlerFb(this._collect << 8 | l, this._params), this.precedingCodepoint = 0;
                                                 break;
                                             case 8:
                                                 do switch (l) {
                                                     case 59:
                                                         this._params.addParam(0);
                                                         break;
                                                     case 58:
                                                         this._params.addSubParam(-1);
                                                         break;
                                                     default:
                                                         this._params.addDigit(l - 48)
                                                 }
-                                                while (++a < n && (l = s[a]) > 47 && l < 60);
-                                                a--;
+                                                while (++o < n && (l = s[o]) > 47 && l < 60);
+                                                o--;
                                                 break;
                                             case 9:
                                                 this._collect <<= 8, this._collect |= l;
                                                 break;
                                             case 10:
                                                 const y = this._escHandlers[this._collect << 8 | l];
                                                 let w = y ? y.length - 1 : -1;
                                                 for (; w >= 0 && (r = y[w](), r !== !0); w--)
-                                                    if (r instanceof Promise) return this._preserveStack(4, y, w, f, a), r;
+                                                    if (r instanceof Promise) return this._preserveStack(4, y, w, f, o), r;
                                                 w < 0 && this._escHandlerFb(this._collect << 8 | l), this.precedingCodepoint = 0;
                                                 break;
                                             case 11:
                                                 this._params.reset(), this._params.addParam(0), this._collect = 0;
                                                 break;
                                             case 12:
                                                 this._dcsParser.hook(this._collect << 8 | l, this._params);
                                                 break;
                                             case 13:
-                                                for (let D = a + 1;; ++D)
+                                                for (let D = o + 1;; ++D)
                                                     if (D >= n || (l = s[D]) === 24 || l === 26 || l === 27 || l > 127 && l < v) {
-                                                        this._dcsParser.put(s, a, D), a = D - 1;
+                                                        this._dcsParser.put(s, o, D), o = D - 1;
                                                         break
                                                     } break;
                                             case 14:
-                                                if (r = this._dcsParser.unhook(l !== 24 && l !== 26), r) return this._preserveStack(6, [], 0, f, a), r;
+                                                if (r = this._dcsParser.unhook(l !== 24 && l !== 26), r) return this._preserveStack(6, [], 0, f, o), r;
                                                 l === 27 && (f |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0;
                                                 break;
                                             case 4:
                                                 this._oscParser.start();
                                                 break;
                                             case 5:
-                                                for (let D = a + 1;; D++)
+                                                for (let D = o + 1;; D++)
                                                     if (D >= n || (l = s[D]) < 32 || l > 127 && l < v) {
-                                                        this._oscParser.put(s, a, D), a = D - 1;
+                                                        this._oscParser.put(s, o, D), o = D - 1;
                                                         break
                                                     } break;
                                             case 6:
-                                                if (r = this._oscParser.end(l !== 24 && l !== 26), r) return this._preserveStack(5, [], 0, f, a), r;
+                                                if (r = this._oscParser.end(l !== 24 && l !== 26), r) return this._preserveStack(5, [], 0, f, o), r;
                                                 l === 27 && (f |= 1), this._params.reset(), this._params.addParam(0), this._collect = 0, this.precedingCodepoint = 0
                                         }
                                         this.currentState = 15 & f
                                     }
                                 }
                             }
                             i.EscapeSequenceParser = c
                         },
-                        6242: (T, i, o) => {
+                        6242: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.OscHandler = i.OscParser = void 0;
-                            const h = o(5770),
-                                u = o(482),
+                            const a = h(5770),
+                                u = h(482),
                                 d = [];
                             i.OscParser = class {
                                 constructor() {
                                     this._state = 0, this._active = d, this._id = -1, this._handlers = Object.create(null), this._handlerFb = () => {}, this._stack = {
                                         paused: !1,
                                         loopPosition: 0,
                                         fallThrough: !1
@@ -6398,47 +6398,47 @@
                                 constructor(_) {
                                     this._handler = _, this._data = "", this._hitLimit = !1
                                 }
                                 start() {
                                     this._data = "", this._hitLimit = !1
                                 }
                                 put(_, g, v) {
-                                    this._hitLimit || (this._data += (0, u.utf32ToString)(_, g, v), this._data.length > h.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0))
+                                    this._hitLimit || (this._data += (0, u.utf32ToString)(_, g, v), this._data.length > a.PAYLOAD_LIMIT && (this._data = "", this._hitLimit = !0))
                                 }
                                 end(_) {
                                     let g = !1;
                                     if (this._hitLimit) g = !1;
                                     else if (_ && (g = this._handler(this._data), g instanceof Promise)) return g.then(v => (this._data = "", this._hitLimit = !1, v));
                                     return this._data = "", this._hitLimit = !1, g
                                 }
                             }
                         },
                         8742: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.Params = void 0;
-                            const o = 2147483647;
-                            class h {
+                            const h = 2147483647;
+                            class a {
                                 constructor(d = 32, _ = 32) {
                                     if (this.maxLength = d, this.maxSubParamsLength = _, _ > 256) throw new Error("maxSubParamsLength must not be greater than 256");
                                     this.params = new Int32Array(d), this.length = 0, this._subParams = new Int32Array(_), this._subParamsLength = 0, this._subParamsIdx = new Uint16Array(d), this._rejectDigits = !1, this._rejectSubDigits = !1, this._digitIsSub = !1
                                 }
                                 static fromArray(d) {
-                                    const _ = new h;
+                                    const _ = new a;
                                     if (!d.length) return _;
                                     for (let g = Array.isArray(d[0]) ? 1 : 0; g < d.length; ++g) {
                                         const v = d[g];
                                         if (Array.isArray(v))
                                             for (let c = 0; c < v.length; ++c) _.addSubParam(v[c]);
                                         else _.addParam(v)
                                     }
                                     return _
                                 }
                                 clone() {
-                                    const d = new h(this.maxLength, this.maxSubParamsLength);
+                                    const d = new a(this.maxLength, this.maxSubParamsLength);
                                     return d.params.set(this.params), d.length = this.length, d._subParams.set(this._subParams), d._subParamsLength = this._subParamsLength, d._subParamsIdx.set(this._subParamsIdx), d._rejectDigits = this._rejectDigits, d._rejectSubDigits = this._rejectSubDigits, d._digitIsSub = this._digitIsSub, d
                                 }
                                 toArray() {
                                     const d = [];
                                     for (let _ = 0; _ < this.length; ++_) {
                                         d.push(this.params[_]);
                                         const g = this._subParamsIdx[_] >> 8,
@@ -6450,23 +6450,23 @@
                                 reset() {
                                     this.length = 0, this._subParamsLength = 0, this._rejectDigits = !1, this._rejectSubDigits = !1, this._digitIsSub = !1
                                 }
                                 addParam(d) {
                                     if (this._digitIsSub = !1, this.length >= this.maxLength) this._rejectDigits = !0;
                                     else {
                                         if (d < -1) throw new Error("values lesser than -1 are not allowed");
-                                        this._subParamsIdx[this.length] = this._subParamsLength << 8 | this._subParamsLength, this.params[this.length++] = d > o ? o : d
+                                        this._subParamsIdx[this.length] = this._subParamsLength << 8 | this._subParamsLength, this.params[this.length++] = d > h ? h : d
                                     }
                                 }
                                 addSubParam(d) {
                                     if (this._digitIsSub = !0, this.length)
                                         if (this._rejectDigits || this._subParamsLength >= this.maxSubParamsLength) this._rejectSubDigits = !0;
                                         else {
                                             if (d < -1) throw new Error("values lesser than -1 are not allowed");
-                                            this._subParams[this._subParamsLength++] = d > o ? o : d, this._subParamsIdx[this.length - 1]++
+                                            this._subParams[this._subParamsLength++] = d > h ? h : d, this._subParamsIdx[this.length - 1]++
                                         }
                                 }
                                 hasSubParams(d) {
                                     return (255 & this._subParamsIdx[d]) - (this._subParamsIdx[d] >> 8) > 0
                                 }
                                 getSubParams(d) {
                                     const _ = this._subParamsIdx[d] >> 8,
@@ -6483,55 +6483,55 @@
                                     return d
                                 }
                                 addDigit(d) {
                                     let _;
                                     if (this._rejectDigits || !(_ = this._digitIsSub ? this._subParamsLength : this.length) || this._digitIsSub && this._rejectSubDigits) return;
                                     const g = this._digitIsSub ? this._subParams : this.params,
                                         v = g[_ - 1];
-                                    g[_ - 1] = ~v ? Math.min(10 * v + d, o) : d
+                                    g[_ - 1] = ~v ? Math.min(10 * v + d, h) : d
                                 }
                             }
-                            i.Params = h
+                            i.Params = a
                         },
                         5741: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.AddonManager = void 0, i.AddonManager = class {
                                 constructor() {
                                     this._addons = []
                                 }
                                 dispose() {
-                                    for (let o = this._addons.length - 1; o >= 0; o--) this._addons[o].instance.dispose()
+                                    for (let h = this._addons.length - 1; h >= 0; h--) this._addons[h].instance.dispose()
                                 }
-                                loadAddon(o, h) {
+                                loadAddon(h, a) {
                                     const u = {
-                                        instance: h,
-                                        dispose: h.dispose,
+                                        instance: a,
+                                        dispose: a.dispose,
                                         isDisposed: !1
                                     };
-                                    this._addons.push(u), h.dispose = () => this._wrappedAddonDispose(u), h.activate(o)
+                                    this._addons.push(u), a.dispose = () => this._wrappedAddonDispose(u), a.activate(h)
                                 }
-                                _wrappedAddonDispose(o) {
-                                    if (o.isDisposed) return;
-                                    let h = -1;
+                                _wrappedAddonDispose(h) {
+                                    if (h.isDisposed) return;
+                                    let a = -1;
                                     for (let u = 0; u < this._addons.length; u++)
-                                        if (this._addons[u] === o) {
-                                            h = u;
+                                        if (this._addons[u] === h) {
+                                            a = u;
                                             break
-                                        } if (h === -1) throw new Error("Could not dispose an addon that has not been loaded");
-                                    o.isDisposed = !0, o.dispose.apply(o.instance), this._addons.splice(h, 1)
+                                        } if (a === -1) throw new Error("Could not dispose an addon that has not been loaded");
+                                    h.isDisposed = !0, h.dispose.apply(h.instance), this._addons.splice(a, 1)
                                 }
                             }
                         },
-                        8771: (T, i, o) => {
+                        8771: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferApiView = void 0;
-                            const h = o(3785),
-                                u = o(511);
+                            const a = h(3785),
+                                u = h(511);
                             i.BufferApiView = class {
                                 constructor(d, _) {
                                     this._buffer = d, this.type = _
                                 }
                                 init(d) {
                                     return this._buffer = d, this
                                 }
@@ -6548,53 +6548,53 @@
                                     return this._buffer.ybase
                                 }
                                 get length() {
                                     return this._buffer.lines.length
                                 }
                                 getLine(d) {
                                     const _ = this._buffer.lines.get(d);
-                                    if (_) return new h.BufferLineApiView(_)
+                                    if (_) return new a.BufferLineApiView(_)
                                 }
                                 getNullCell() {
                                     return new u.CellData
                                 }
                             }
                         },
-                        3785: (T, i, o) => {
+                        3785: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferLineApiView = void 0;
-                            const h = o(511);
+                            const a = h(511);
                             i.BufferLineApiView = class {
                                 constructor(u) {
                                     this._line = u
                                 }
                                 get isWrapped() {
                                     return this._line.isWrapped
                                 }
                                 get length() {
                                     return this._line.length
                                 }
                                 getCell(u, d) {
-                                    if (!(u < 0 || u >= this._line.length)) return d ? (this._line.loadCell(u, d), d) : this._line.loadCell(u, new h.CellData)
+                                    if (!(u < 0 || u >= this._line.length)) return d ? (this._line.loadCell(u, d), d) : this._line.loadCell(u, new a.CellData)
                                 }
                                 translateToString(u, d, _) {
                                     return this._line.translateToString(u, d, _)
                                 }
                             }
                         },
-                        8285: (T, i, o) => {
+                        8285: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferNamespaceApi = void 0;
-                            const h = o(8771),
-                                u = o(8460);
+                            const a = h(8771),
+                                u = h(8460);
                             i.BufferNamespaceApi = class {
                                 constructor(d) {
-                                    this._core = d, this._onBufferChange = new u.EventEmitter, this.onBufferChange = this._onBufferChange.event, this._normal = new h.BufferApiView(this._core.buffers.normal, "normal"), this._alternate = new h.BufferApiView(this._core.buffers.alt, "alternate"), this._core.buffers.onBufferActivate(() => this._onBufferChange.fire(this.active))
+                                    this._core = d, this._onBufferChange = new u.EventEmitter, this.onBufferChange = this._onBufferChange.event, this._normal = new a.BufferApiView(this._core.buffers.normal, "normal"), this._alternate = new a.BufferApiView(this._core.buffers.alt, "alternate"), this._core.buffers.onBufferActivate(() => this._onBufferChange.fire(this.active))
                                 }
                                 get active() {
                                     if (this._core.buffers.active === this._core.buffers.normal) return this.normal;
                                     if (this._core.buffers.active === this._core.buffers.alt) return this.alternate;
                                     throw new Error("Active buffer is neither normal nor alternate")
                                 }
                                 get normal() {
@@ -6605,66 +6605,66 @@
                                 }
                             }
                         },
                         7975: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.ParserApi = void 0, i.ParserApi = class {
-                                constructor(o) {
-                                    this._core = o
+                                constructor(h) {
+                                    this._core = h
                                 }
-                                registerCsiHandler(o, h) {
-                                    return this._core.registerCsiHandler(o, u => h(u.toArray()))
+                                registerCsiHandler(h, a) {
+                                    return this._core.registerCsiHandler(h, u => a(u.toArray()))
                                 }
-                                addCsiHandler(o, h) {
-                                    return this.registerCsiHandler(o, h)
+                                addCsiHandler(h, a) {
+                                    return this.registerCsiHandler(h, a)
                                 }
-                                registerDcsHandler(o, h) {
-                                    return this._core.registerDcsHandler(o, (u, d) => h(u, d.toArray()))
+                                registerDcsHandler(h, a) {
+                                    return this._core.registerDcsHandler(h, (u, d) => a(u, d.toArray()))
                                 }
-                                addDcsHandler(o, h) {
-                                    return this.registerDcsHandler(o, h)
+                                addDcsHandler(h, a) {
+                                    return this.registerDcsHandler(h, a)
                                 }
-                                registerEscHandler(o, h) {
-                                    return this._core.registerEscHandler(o, h)
+                                registerEscHandler(h, a) {
+                                    return this._core.registerEscHandler(h, a)
                                 }
-                                addEscHandler(o, h) {
-                                    return this.registerEscHandler(o, h)
+                                addEscHandler(h, a) {
+                                    return this.registerEscHandler(h, a)
                                 }
-                                registerOscHandler(o, h) {
-                                    return this._core.registerOscHandler(o, h)
+                                registerOscHandler(h, a) {
+                                    return this._core.registerOscHandler(h, a)
                                 }
-                                addOscHandler(o, h) {
-                                    return this.registerOscHandler(o, h)
+                                addOscHandler(h, a) {
+                                    return this.registerOscHandler(h, a)
                                 }
                             }
                         },
                         7090: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.UnicodeApi = void 0, i.UnicodeApi = class {
-                                constructor(o) {
-                                    this._core = o
+                                constructor(h) {
+                                    this._core = h
                                 }
-                                register(o) {
-                                    this._core.unicodeService.register(o)
+                                register(h) {
+                                    this._core.unicodeService.register(h)
                                 }
                                 get versions() {
                                     return this._core.unicodeService.versions
                                 }
                                 get activeVersion() {
                                     return this._core.unicodeService.activeVersion
                                 }
-                                set activeVersion(o) {
-                                    this._core.unicodeService.activeVersion = o
+                                set activeVersion(h) {
+                                    this._core.unicodeService.activeVersion = h
                                 }
                             }
                         },
-                        744: function(T, i, o) {
-                            var h = this && this.__decorate || function(e, s, n, t) {
+                        744: function(T, i, h) {
+                            var a = this && this.__decorate || function(e, s, n, t) {
                                     var r, l = arguments.length,
                                         f = l < 3 ? s : t === null ? t = Object.getOwnPropertyDescriptor(s, n) : t;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") f = Reflect.decorate(e, s, n, t);
                                     else
                                         for (var m = e.length - 1; m >= 0; m--)(r = e[m]) && (f = (l < 3 ? r(f) : l > 3 ? r(s, n, f) : r(s, n)) || f);
                                     return l > 3 && f && Object.defineProperty(s, n, f), f
                                 },
@@ -6672,18 +6672,18 @@
                                     return function(n, t) {
                                         s(n, t, e)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.BufferService = i.MINIMUM_ROWS = i.MINIMUM_COLS = void 0;
-                            const d = o(2585),
-                                _ = o(5295),
-                                g = o(8460),
-                                v = o(844);
+                            const d = h(2585),
+                                _ = h(5295),
+                                g = h(8460),
+                                v = h(844);
                             i.MINIMUM_COLS = 2, i.MINIMUM_ROWS = 1;
                             let c = class extends v.Disposable {
                                 constructor(e) {
                                     super(), this.isUserScrolling = !1, this._onResize = this.register(new g.EventEmitter), this.onResize = this._onResize.event, this._onScroll = this.register(new g.EventEmitter), this.onScroll = this._onScroll.event, this.cols = Math.max(e.rawOptions.cols || 0, i.MINIMUM_COLS), this.rows = Math.max(e.rawOptions.rows || 0, i.MINIMUM_ROWS), this.buffers = this.register(new _.BufferSet(e, this))
                                 }
                                 get buffer() {
                                     return this.buffers.active
@@ -6731,54 +6731,54 @@
                                     this.scrollLines(this.buffer.ybase - this.buffer.ydisp)
                                 }
                                 scrollToLine(e) {
                                     const s = e - this.buffer.ydisp;
                                     s !== 0 && this.scrollLines(s)
                                 }
                             };
-                            c = h([u(0, d.IOptionsService)], c), i.BufferService = c
+                            c = a([u(0, d.IOptionsService)], c), i.BufferService = c
                         },
                         7994: (T, i) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CharsetService = void 0, i.CharsetService = class {
                                 constructor() {
                                     this.glevel = 0, this._charsets = []
                                 }
                                 reset() {
                                     this.charset = void 0, this._charsets = [], this.glevel = 0
                                 }
-                                setgLevel(o) {
-                                    this.glevel = o, this.charset = this._charsets[o]
+                                setgLevel(h) {
+                                    this.glevel = h, this.charset = this._charsets[h]
                                 }
-                                setgCharset(o, h) {
-                                    this._charsets[o] = h, this.glevel === o && (this.charset = h)
+                                setgCharset(h, a) {
+                                    this._charsets[h] = a, this.glevel === h && (this.charset = a)
                                 }
                             }
                         },
-                        1753: function(T, i, o) {
-                            var h = this && this.__decorate || function(t, r, l, f) {
-                                    var m, a = arguments.length,
-                                        p = a < 3 ? r : f === null ? f = Object.getOwnPropertyDescriptor(r, l) : f;
+                        1753: function(T, i, h) {
+                            var a = this && this.__decorate || function(t, r, l, f) {
+                                    var m, o = arguments.length,
+                                        p = o < 3 ? r : f === null ? f = Object.getOwnPropertyDescriptor(r, l) : f;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") p = Reflect.decorate(t, r, l, f);
                                     else
-                                        for (var C = t.length - 1; C >= 0; C--)(m = t[C]) && (p = (a < 3 ? m(p) : a > 3 ? m(r, l, p) : m(r, l)) || p);
-                                    return a > 3 && p && Object.defineProperty(r, l, p), p
+                                        for (var C = t.length - 1; C >= 0; C--)(m = t[C]) && (p = (o < 3 ? m(p) : o > 3 ? m(r, l, p) : m(r, l)) || p);
+                                    return o > 3 && p && Object.defineProperty(r, l, p), p
                                 },
                                 u = this && this.__param || function(t, r) {
                                     return function(l, f) {
                                         r(l, f, t)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CoreMouseService = void 0;
-                            const d = o(2585),
-                                _ = o(8460),
-                                g = o(844),
+                            const d = h(2585),
+                                _ = h(8460),
+                                g = h(844),
                                 v = {
                                     NONE: {
                                         events: 0,
                                         restrict: () => !1
                                     },
                                     X10: {
                                         events: 1,
@@ -6867,37 +6867,37 @@
                                 _equalEvents(t, r, l) {
                                     if (l) {
                                         if (t.x !== r.x || t.y !== r.y) return !1
                                     } else if (t.col !== r.col || t.row !== r.row) return !1;
                                     return t.button === r.button && t.action === r.action && t.ctrl === r.ctrl && t.alt === r.alt && t.shift === r.shift
                                 }
                             };
-                            n = h([u(0, d.IBufferService), u(1, d.ICoreService)], n), i.CoreMouseService = n
+                            n = a([u(0, d.IBufferService), u(1, d.ICoreService)], n), i.CoreMouseService = n
                         },
-                        6975: function(T, i, o) {
-                            var h = this && this.__decorate || function(n, t, r, l) {
+                        6975: function(T, i, h) {
+                            var a = this && this.__decorate || function(n, t, r, l) {
                                     var f, m = arguments.length,
-                                        a = m < 3 ? t : l === null ? l = Object.getOwnPropertyDescriptor(t, r) : l;
-                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") a = Reflect.decorate(n, t, r, l);
+                                        o = m < 3 ? t : l === null ? l = Object.getOwnPropertyDescriptor(t, r) : l;
+                                    if (typeof Reflect == "object" && typeof Reflect.decorate == "function") o = Reflect.decorate(n, t, r, l);
                                     else
-                                        for (var p = n.length - 1; p >= 0; p--)(f = n[p]) && (a = (m < 3 ? f(a) : m > 3 ? f(t, r, a) : f(t, r)) || a);
-                                    return m > 3 && a && Object.defineProperty(t, r, a), a
+                                        for (var p = n.length - 1; p >= 0; p--)(f = n[p]) && (o = (m < 3 ? f(o) : m > 3 ? f(t, r, o) : f(t, r)) || o);
+                                    return m > 3 && o && Object.defineProperty(t, r, o), o
                                 },
                                 u = this && this.__param || function(n, t) {
                                     return function(r, l) {
                                         t(r, l, n)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.CoreService = void 0;
-                            const d = o(2585),
-                                _ = o(8460),
-                                g = o(1439),
-                                v = o(844),
+                            const d = h(2585),
+                                _ = h(8460),
+                                g = h(1439),
+                                v = h(844),
                                 c = Object.freeze({
                                     insertMode: !1
                                 }),
                                 e = Object.freeze({
                                     applicationCursorKeys: !1,
                                     applicationKeypad: !1,
                                     bracketedPasteMode: !1,
@@ -6918,24 +6918,24 @@
                                     const r = this._bufferService.buffer;
                                     t && this._optionsService.rawOptions.scrollOnUserInput && r.ybase !== r.ydisp && this._onRequestScrollToBottom.fire(), t && this._onUserInput.fire(), this._logService.debug(`sending data "${n}"`, () => n.split("").map(l => l.charCodeAt(0))), this._onData.fire(n)
                                 }
                                 triggerBinaryEvent(n) {
                                     this._optionsService.rawOptions.disableStdin || (this._logService.debug(`sending binary "${n}"`, () => n.split("").map(t => t.charCodeAt(0))), this._onBinary.fire(n))
                                 }
                             };
-                            s = h([u(0, d.IBufferService), u(1, d.ILogService), u(2, d.IOptionsService)], s), i.CoreService = s
+                            s = a([u(0, d.IBufferService), u(1, d.ILogService), u(2, d.IOptionsService)], s), i.CoreService = s
                         },
-                        9074: (T, i, o) => {
+                        9074: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.DecorationService = void 0;
-                            const h = o(8055),
-                                u = o(8460),
-                                d = o(844),
-                                _ = o(6106);
+                            const a = h(8055),
+                                u = h(8460),
+                                d = h(844),
+                                _ = h(6106);
                             let g = 0,
                                 v = 0;
                             class c extends d.Disposable {
                                 constructor() {
                                     super(), this._decorations = new _.SortedList(n => n == null ? void 0 : n.marker.line), this._onDecorationRegistered = this.register(new u.EventEmitter), this.onDecorationRegistered = this._onDecorationRegistered.event, this._onDecorationRemoved = this.register(new u.EventEmitter), this.onDecorationRemoved = this._onDecorationRemoved.event, this.register((0, d.toDisposable)(() => {
                                         for (const n of this._decorations.values()) this._onDecorationRemoved.fire(n);
                                         this.reset()
@@ -6956,51 +6956,51 @@
                                     return t
                                 }
                                 reset() {
                                     for (const n of this._decorations.values()) n.dispose();
                                     this._decorations.clear()
                                 }* getDecorationsAtCell(n, t, r) {
                                     var l, f, m;
-                                    let a = 0,
+                                    let o = 0,
                                         p = 0;
-                                    for (const C of this._decorations.getKeyIterator(t)) a = (l = C.options.x) !== null && l !== void 0 ? l : 0, p = a + ((f = C.options.width) !== null && f !== void 0 ? f : 1), n >= a && n < p && (!r || ((m = C.options.layer) !== null && m !== void 0 ? m : "bottom") === r) && (yield C)
+                                    for (const C of this._decorations.getKeyIterator(t)) o = (l = C.options.x) !== null && l !== void 0 ? l : 0, p = o + ((f = C.options.width) !== null && f !== void 0 ? f : 1), n >= o && n < p && (!r || ((m = C.options.layer) !== null && m !== void 0 ? m : "bottom") === r) && (yield C)
                                 }
                                 forEachDecorationAtCell(n, t, r, l) {
                                     this._decorations.forEachByKey(t, f => {
-                                        var m, a, p;
-                                        g = (m = f.options.x) !== null && m !== void 0 ? m : 0, v = g + ((a = f.options.width) !== null && a !== void 0 ? a : 1), n >= g && n < v && (!r || ((p = f.options.layer) !== null && p !== void 0 ? p : "bottom") === r) && l(f)
+                                        var m, o, p;
+                                        g = (m = f.options.x) !== null && m !== void 0 ? m : 0, v = g + ((o = f.options.width) !== null && o !== void 0 ? o : 1), n >= g && n < v && (!r || ((p = f.options.layer) !== null && p !== void 0 ? p : "bottom") === r) && l(f)
                                     })
                                 }
                                 dispose() {
                                     for (const n of this._decorations.values()) this._onDecorationRemoved.fire(n);
                                     this.reset()
                                 }
                             }
                             i.DecorationService = c;
                             class e extends d.Disposable {
                                 constructor(n) {
                                     super(), this.options = n, this.isDisposed = !1, this.onRenderEmitter = this.register(new u.EventEmitter), this.onRender = this.onRenderEmitter.event, this._onDispose = this.register(new u.EventEmitter), this.onDispose = this._onDispose.event, this._cachedBg = null, this._cachedFg = null, this.marker = n.marker, this.options.overviewRulerOptions && !this.options.overviewRulerOptions.position && (this.options.overviewRulerOptions.position = "full")
                                 }
                                 get backgroundColorRGB() {
-                                    return this._cachedBg === null && (this.options.backgroundColor ? this._cachedBg = h.css.toColor(this.options.backgroundColor) : this._cachedBg = void 0), this._cachedBg
+                                    return this._cachedBg === null && (this.options.backgroundColor ? this._cachedBg = a.css.toColor(this.options.backgroundColor) : this._cachedBg = void 0), this._cachedBg
                                 }
                                 get foregroundColorRGB() {
-                                    return this._cachedFg === null && (this.options.foregroundColor ? this._cachedFg = h.css.toColor(this.options.foregroundColor) : this._cachedFg = void 0), this._cachedFg
+                                    return this._cachedFg === null && (this.options.foregroundColor ? this._cachedFg = a.css.toColor(this.options.foregroundColor) : this._cachedFg = void 0), this._cachedFg
                                 }
                                 dispose() {
                                     this._onDispose.fire(), super.dispose()
                                 }
                             }
                         },
-                        4348: (T, i, o) => {
+                        4348: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.InstantiationService = i.ServiceCollection = void 0;
-                            const h = o(2585),
-                                u = o(8343);
+                            const a = h(2585),
+                                u = h(8343);
                             class d {
                                 constructor(...g) {
                                     this._entries = new Map;
                                     for (const [v, c] of g) this.set(v, c)
                                 }
                                 set(g, v) {
                                     const c = this._entries.get(g);
@@ -7014,15 +7014,15 @@
                                 }
                                 get(g) {
                                     return this._entries.get(g)
                                 }
                             }
                             i.ServiceCollection = d, i.InstantiationService = class {
                                 constructor() {
-                                    this._services = new d, this._services.set(h.IInstantiationService, this)
+                                    this._services = new d, this._services.set(a.IInstantiationService, this)
                                 }
                                 setService(_, g) {
                                     this._services.set(_, g)
                                 }
                                 getService(_) {
                                     return this._services.get(_)
                                 }
@@ -7036,16 +7036,16 @@
                                     }
                                     const e = v.length > 0 ? v[0].index : g.length;
                                     if (g.length !== e) throw new Error(`[createInstance] First service dependency of ${_.name} at position ${e+1} conflicts with ${g.length} static arguments`);
                                     return new _(...g, ...c)
                                 }
                             }
                         },
-                        7866: function(T, i, o) {
-                            var h = this && this.__decorate || function(c, e, s, n) {
+                        7866: function(T, i, h) {
+                            var a = this && this.__decorate || function(c, e, s, n) {
                                     var t, r = arguments.length,
                                         l = r < 3 ? e : n === null ? n = Object.getOwnPropertyDescriptor(e, s) : n;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") l = Reflect.decorate(c, e, s, n);
                                     else
                                         for (var f = c.length - 1; f >= 0; f--)(t = c[f]) && (l = (r < 3 ? t(l) : r > 3 ? t(e, s, l) : t(e, s)) || l);
                                     return r > 3 && l && Object.defineProperty(e, s, l), l
                                 },
@@ -7053,16 +7053,16 @@
                                     return function(s, n) {
                                         e(s, n, c)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.LogService = void 0;
-                            const d = o(844),
-                                _ = o(2585),
+                            const d = h(844),
+                                _ = h(2585),
                                 g = {
                                     debug: _.LogLevelEnum.DEBUG,
                                     info: _.LogLevelEnum.INFO,
                                     warn: _.LogLevelEnum.WARN,
                                     error: _.LogLevelEnum.ERROR,
                                     off: _.LogLevelEnum.OFF
                                 };
@@ -7088,23 +7088,23 @@
                                 warn(c, ...e) {
                                     this.logLevel <= _.LogLevelEnum.WARN && this._log(console.warn, c, e)
                                 }
                                 error(c, ...e) {
                                     this.logLevel <= _.LogLevelEnum.ERROR && this._log(console.error, c, e)
                                 }
                             };
-                            v = h([u(0, _.IOptionsService)], v), i.LogService = v
+                            v = a([u(0, _.IOptionsService)], v), i.LogService = v
                         },
-                        7302: (T, i, o) => {
+                        7302: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.OptionsService = i.DEFAULT_OPTIONS = void 0;
-                            const h = o(8460),
-                                u = o(6114),
-                                d = o(844);
+                            const a = h(8460),
+                                u = h(6114),
+                                d = h(844);
                             i.DEFAULT_OPTIONS = {
                                 cols: 80,
                                 rows: 24,
                                 cursorBlink: !1,
                                 cursorStyle: "block",
                                 cursorWidth: 1,
                                 customGlyphs: !0,
@@ -7141,15 +7141,15 @@
                                 termName: "xterm",
                                 cancelEvents: !1,
                                 overviewRulerWidth: 0
                             };
                             const _ = ["normal", "bold", "100", "200", "300", "400", "500", "600", "700", "800", "900"];
                             class g extends d.Disposable {
                                 constructor(c) {
-                                    super(), this._onOptionChange = this.register(new h.EventEmitter), this.onOptionChange = this._onOptionChange.event;
+                                    super(), this._onOptionChange = this.register(new a.EventEmitter), this.onOptionChange = this._onOptionChange.event;
                                     const e = Object.assign({}, i.DEFAULT_OPTIONS);
                                     for (const s in c)
                                         if (s in e) try {
                                             const n = c[s];
                                             e[s] = this._sanitizeAndValidateOption(s, n)
                                         } catch (n) {
                                             console.error(n)
@@ -7218,16 +7218,16 @@
                                             if (!e && e !== 0) throw new Error(`${c} must be numeric, value: ${e}`)
                                     }
                                     return e
                                 }
                             }
                             i.OptionsService = g
                         },
-                        2660: function(T, i, o) {
-                            var h = this && this.__decorate || function(g, v, c, e) {
+                        2660: function(T, i, h) {
+                            var a = this && this.__decorate || function(g, v, c, e) {
                                     var s, n = arguments.length,
                                         t = n < 3 ? v : e === null ? e = Object.getOwnPropertyDescriptor(v, c) : e;
                                     if (typeof Reflect == "object" && typeof Reflect.decorate == "function") t = Reflect.decorate(g, v, c, e);
                                     else
                                         for (var r = g.length - 1; r >= 0; r--)(s = g[r]) && (t = (n < 3 ? s(t) : n > 3 ? s(v, c, t) : s(v, c)) || t);
                                     return n > 3 && t && Object.defineProperty(v, c, t), t
                                 },
@@ -7235,15 +7235,15 @@
                                     return function(c, e) {
                                         v(c, e, g)
                                     }
                                 };
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.OscLinkService = void 0;
-                            const d = o(2585);
+                            const d = h(2585);
                             let _ = class {
                                 constructor(g) {
                                     this._bufferService = g, this._nextId = 1, this._entriesWithId = new Map, this._dataByLinkId = new Map
                                 }
                                 registerLink(g) {
                                     const v = this._bufferService.buffer;
                                     if (g.id === void 0) {
@@ -7283,56 +7283,56 @@
                                     return `${g.id};;${g.uri}`
                                 }
                                 _removeMarkerFromLink(g, v) {
                                     const c = g.lines.indexOf(v);
                                     c !== -1 && (g.lines.splice(c, 1), g.lines.length === 0 && (g.data.id !== void 0 && this._entriesWithId.delete(g.key), this._dataByLinkId.delete(g.id)))
                                 }
                             };
-                            _ = h([u(0, d.IBufferService)], _), i.OscLinkService = _
+                            _ = a([u(0, d.IBufferService)], _), i.OscLinkService = _
                         },
                         8343: (T, i) => {
-                            function o(h, u, d) {
+                            function h(a, u, d) {
                                 u.di$target === u ? u.di$dependencies.push({
-                                    id: h,
+                                    id: a,
                                     index: d
                                 }) : (u.di$dependencies = [{
-                                    id: h,
+                                    id: a,
                                     index: d
                                 }], u.di$target = u)
                             }
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
-                            }), i.createDecorator = i.getServiceDependencies = i.serviceRegistry = void 0, i.serviceRegistry = new Map, i.getServiceDependencies = function(h) {
-                                return h.di$dependencies || []
-                            }, i.createDecorator = function(h) {
-                                if (i.serviceRegistry.has(h)) return i.serviceRegistry.get(h);
+                            }), i.createDecorator = i.getServiceDependencies = i.serviceRegistry = void 0, i.serviceRegistry = new Map, i.getServiceDependencies = function(a) {
+                                return a.di$dependencies || []
+                            }, i.createDecorator = function(a) {
+                                if (i.serviceRegistry.has(a)) return i.serviceRegistry.get(a);
                                 const u = function(d, _, g) {
                                     if (arguments.length !== 3) throw new Error("@IServiceName-decorator can only be used to decorate a parameter");
-                                    o(u, d, g)
+                                    h(u, d, g)
                                 };
-                                return u.toString = () => h, i.serviceRegistry.set(h, u), u
+                                return u.toString = () => a, i.serviceRegistry.set(a, u), u
                             }
                         },
-                        2585: (T, i, o) => {
+                        2585: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.IDecorationService = i.IUnicodeService = i.IOscLinkService = i.IOptionsService = i.ILogService = i.LogLevelEnum = i.IInstantiationService = i.ICharsetService = i.ICoreService = i.ICoreMouseService = i.IBufferService = void 0;
-                            const h = o(8343);
+                            const a = h(8343);
                             var u;
-                            i.IBufferService = (0, h.createDecorator)("BufferService"), i.ICoreMouseService = (0, h.createDecorator)("CoreMouseService"), i.ICoreService = (0, h.createDecorator)("CoreService"), i.ICharsetService = (0, h.createDecorator)("CharsetService"), i.IInstantiationService = (0, h.createDecorator)("InstantiationService"), (u = i.LogLevelEnum || (i.LogLevelEnum = {}))[u.DEBUG = 0] = "DEBUG", u[u.INFO = 1] = "INFO", u[u.WARN = 2] = "WARN", u[u.ERROR = 3] = "ERROR", u[u.OFF = 4] = "OFF", i.ILogService = (0, h.createDecorator)("LogService"), i.IOptionsService = (0, h.createDecorator)("OptionsService"), i.IOscLinkService = (0, h.createDecorator)("OscLinkService"), i.IUnicodeService = (0, h.createDecorator)("UnicodeService"), i.IDecorationService = (0, h.createDecorator)("DecorationService")
+                            i.IBufferService = (0, a.createDecorator)("BufferService"), i.ICoreMouseService = (0, a.createDecorator)("CoreMouseService"), i.ICoreService = (0, a.createDecorator)("CoreService"), i.ICharsetService = (0, a.createDecorator)("CharsetService"), i.IInstantiationService = (0, a.createDecorator)("InstantiationService"), (u = i.LogLevelEnum || (i.LogLevelEnum = {}))[u.DEBUG = 0] = "DEBUG", u[u.INFO = 1] = "INFO", u[u.WARN = 2] = "WARN", u[u.ERROR = 3] = "ERROR", u[u.OFF = 4] = "OFF", i.ILogService = (0, a.createDecorator)("LogService"), i.IOptionsService = (0, a.createDecorator)("OptionsService"), i.IOscLinkService = (0, a.createDecorator)("OscLinkService"), i.IUnicodeService = (0, a.createDecorator)("UnicodeService"), i.IDecorationService = (0, a.createDecorator)("DecorationService")
                         },
-                        1480: (T, i, o) => {
+                        1480: (T, i, h) => {
                             Object.defineProperty(i, "__esModule", {
                                 value: !0
                             }), i.UnicodeService = void 0;
-                            const h = o(8460),
-                                u = o(225);
+                            const a = h(8460),
+                                u = h(225);
                             i.UnicodeService = class {
                                 constructor() {
-                                    this._providers = Object.create(null), this._active = "", this._onChange = new h.EventEmitter, this.onChange = this._onChange.event;
+                                    this._providers = Object.create(null), this._active = "", this._onChange = new a.EventEmitter, this.onChange = this._onChange.event;
                                     const d = new u.UnicodeV6;
                                     this.register(d), this._active = d.version, this._activeProvider = d
                                 }
                                 dispose() {
                                     this._onChange.dispose()
                                 }
                                 get versions() {
@@ -7369,28 +7369,28 @@
                         }
                     },
                     G = {};
 
                 function W(T) {
                     var i = G[T];
                     if (i !== void 0) return i.exports;
-                    var o = G[T] = {
+                    var h = G[T] = {
                         exports: {}
                     };
-                    return Z[T].call(o.exports, o, o.exports, W), o.exports
+                    return Z[T].call(h.exports, h, h.exports, W), h.exports
                 }
                 var Y = {};
                 return (() => {
                     var T = Y;
                     Object.defineProperty(T, "__esModule", {
                         value: !0
                     }), T.Terminal = void 0;
                     const i = W(3236),
-                        o = W(9042),
-                        h = W(7975),
+                        h = W(9042),
+                        a = W(7975),
                         u = W(7090),
                         d = W(5741),
                         _ = W(8285),
                         g = ["cols", "rows"];
                     T.Terminal = class {
                         constructor(v) {
                             this._core = new i.Terminal(v), this._addonManager = new d.AddonManager, this._publicOptions = Object.assign({}, this._core.options);
@@ -7448,15 +7448,15 @@
                         get onWriteParsed() {
                             return this._core.onWriteParsed
                         }
                         get element() {
                             return this._core.element
                         }
                         get parser() {
-                            return this._parser || (this._parser = new h.ParserApi(this._core)), this._parser
+                            return this._parser || (this._parser = new a.ParserApi(this._core)), this._parser
                         }
                         get unicode() {
                             return this._checkProposedApi(), new u.UnicodeApi(this._core)
                         }
                         get textarea() {
                             return this._core.textarea
                         }
@@ -7598,15 +7598,15 @@
                         clearTextureAtlas() {
                             this._core.clearTextureAtlas()
                         }
                         loadAddon(v) {
                             return this._addonManager.loadAddon(this, v)
                         }
                         static get strings() {
-                            return o
+                            return h
                         }
                         _verifyIntegers(...v) {
                             for (const c of v)
                                 if (c === 1 / 0 || isNaN(c) || c % 1 != 0) throw new Error("This API only accepts integers")
                         }
                         _verifyPositiveIntegers(...v) {
                             for (const c of v)
@@ -7651,19 +7651,19 @@
                         proposeDimensions() {
                             if (!this._terminal || !this._terminal.element || !this._terminal.element.parentElement) return;
                             const W = this._terminal._core,
                                 Y = W._renderService.dimensions;
                             if (Y.css.cell.width === 0 || Y.css.cell.height === 0) return;
                             const T = this._terminal.options.scrollback === 0 ? 0 : W.viewport.scrollBarWidth,
                                 i = window.getComputedStyle(this._terminal.element.parentElement),
-                                o = parseInt(i.getPropertyValue("height")),
-                                h = Math.max(0, parseInt(i.getPropertyValue("width"))),
+                                h = parseInt(i.getPropertyValue("height")),
+                                a = Math.max(0, parseInt(i.getPropertyValue("width"))),
                                 u = window.getComputedStyle(this._terminal.element),
-                                d = o - (parseInt(u.getPropertyValue("padding-top")) + parseInt(u.getPropertyValue("padding-bottom"))),
-                                _ = h - (parseInt(u.getPropertyValue("padding-right")) + parseInt(u.getPropertyValue("padding-left"))) - T;
+                                d = h - (parseInt(u.getPropertyValue("padding-top")) + parseInt(u.getPropertyValue("padding-bottom"))),
+                                _ = a - (parseInt(u.getPropertyValue("padding-right")) + parseInt(u.getPropertyValue("padding-left"))) - T;
                             return {
                                 cols: Math.max(2, Math.floor(_ / Y.css.cell.width)),
                                 rows: Math.max(1, Math.floor(d / Y.css.cell.height))
                             }
                         }
                     }
                 })(), Z
@@ -7698,114 +7698,117 @@
                 emits: ["opened", "disposed", "bell", "binary", "cursorMove", "input", "key", "lineFeed", "render", "writeParsed", "resize", "scroll", "selectionChange", "titleChange"],
                 setup(X, {
                     emit: J,
                     expose: Z
                 }) {
                     const G = ee.ref(null),
                         W = new te.Terminal(X.options),
-                        Y = new ie.FitAddon,
-                        T = new ResizeObserver(() => {
-                            Y.fit()
-                        });
+                        Y = new ie.FitAddon;
+
+                    function T() {
+                        Y.fit()
+                    }
+                    const i = new ResizeObserver(T);
                     W.loadAddon(Y);
-                    for (let o = 0; o < X.listen.length; o++) {
-                        const h = X.listen[o],
-                            u = ae[h];
-                        h === "selectionChange" ? W[u](() => J(h, {
+                    for (let a = 0; a < X.listen.length; a++) {
+                        const u = X.listen[a],
+                            d = ae[u];
+                        u === "selectionChange" ? W[d](() => J(u, {
                             hasSelection: W.hasSelection() ? 1 : 0,
                             selection: W.getSelection(),
                             position: W.getSelectionPosition()
-                        })) : u && W[u](d => J(h, d))
+                        })) : d && W[d](_ => J(u, _))
                     }
-                    const i = {
+                    const h = {
+                        fit: T,
                         blur() {
                             return W.blur()
                         },
                         focus() {
                             return W.focus()
                         },
-                        resize(o, h) {
-                            return W.resize(o, h)
+                        resize(a, u) {
+                            return W.resize(a, u)
                         },
-                        attachCustomKeyEventHandler(o) {
-                            return W.attachCustomKeyEventHandler(o)
+                        attachCustomKeyEventHandler(a) {
+                            return W.attachCustomKeyEventHandler(a)
                         },
-                        registerLinkProvider(o) {
-                            return W.registerLinkProvider(o)
+                        registerLinkProvider(a) {
+                            return W.registerLinkProvider(a)
                         },
-                        registerMarker(o) {
-                            return W.registerMarker(o)
+                        registerMarker(a) {
+                            return W.registerMarker(a)
                         },
-                        registerDecoration(o) {
-                            return W.registerDecoration(o)
+                        registerDecoration(a) {
+                            return W.registerDecoration(a)
                         },
                         hasSelection() {
                             return W.hasSelection()
                         },
                         getSelection() {
                             return W.getSelection()
                         },
                         getSelectionPosition() {
                             return W.getSelectionPosition()
                         },
                         clearSelection() {
                             return W.clearSelection()
                         },
-                        select(o, h, u) {
-                            return W.select(o, h, u)
+                        select(a, u, d) {
+                            return W.select(a, u, d)
                         },
                         selectAll() {
                             return W.selectAll()
                         },
-                        selectLines(o, h) {
-                            return W.selectLines(o, h)
+                        selectLines(a, u) {
+                            return W.selectLines(a, u)
                         },
-                        scrollLines(o) {
-                            return W.scrollLines(o)
+                        scrollLines(a) {
+                            return W.scrollLines(a)
                         },
-                        scrollPages(o) {
-                            return W.scrollPages(o)
+                        scrollPages(a) {
+                            return W.scrollPages(a)
                         },
                         scrollToTop() {
                             return W.scrollToTop()
                         },
                         scrollToBottom() {
                             return W.scrollToBottom()
                         },
-                        scrollToLine(o) {
-                            return W.scrollToLine(o)
+                        scrollToLine(a) {
+                            return W.scrollToLine(a)
                         },
                         clear() {
                             return W.clear()
                         },
-                        write(o, h) {
-                            return W.write(o, h)
+                        write(a, u) {
+                            return W.write(a, u)
                         },
-                        writeln(o, h) {
-                            return W.writeln(o, h)
+                        writeln(a, u) {
+                            return W.writeln(a, u)
                         },
-                        paste(o) {
-                            return W.paste(o)
+                        paste(a) {
+                            return W.paste(a)
                         },
-                        refresh(o, h) {
-                            return W.refresh(o, h)
+                        refresh(a, u) {
+                            return W.refresh(a, u)
                         },
                         clearTextureAtlas() {
                             return W.clearTextureAtlas()
                         },
                         reset() {
                             return W.reset()
                         }
                     };
                     return ee.onMounted(() => {
-                        W.open(G.value), T.observe(G.value), J("opened")
+                        W.open(G.value), i.observe(G.value), J("opened")
                     }), ee.onBeforeUnmount(() => {
-                        T.unobserve(G.value), W.dispose(), J("disposed")
-                    }), Z(i), {
-                        ...i,
+                        i.unobserve(G.value), W.dispose(), J("disposed")
+                    }), Z(h), {
+                        ...h,
                         elem: G
                     }
                 },
                 template: `<div style="position: relative; width: 100%; height: 100%;" v-bind="$attrs">
       <div ref="elem" style="position: absolute; width: 100%; height: 100%;"></div>
     </div>
     `
```

### Comparing `trame-xterm-0.1.1/trame_xterm/widgets/xterm.py` & `trame-xterm-0.1.2/trame_xterm/widgets/xterm.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,18 @@
             "writeParsed",
             "resize",
             "scroll",
             "selectionChange",
             "titleChange",
         ]
 
+    def fit(self):
+        """Trigger a fit on the available space"""
+        self.server.js_call(self.__ref, "fit")
+
     def blur(self):
         """Trigger a blur on the xterm.js widget"""
         self.server.js_call(self.__ref, "blur")
 
     def focus(self):
         """Trigger a focus on the xterm.js widget"""
         self.server.js_call(self.__ref, "focus")
```

### Comparing `trame-xterm-0.1.1/trame_xterm.egg-info/PKG-INFO` & `trame-xterm-0.1.2/trame_xterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-xterm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Trame widget to expose xterm.js
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-xterm-0.1.1/trame_xterm.egg-info/SOURCES.txt` & `trame-xterm-0.1.2/trame_xterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

