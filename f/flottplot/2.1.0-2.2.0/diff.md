# Comparing `tmp/flottplot-2.1.0-py3-none-any.whl.zip` & `tmp/flottplot-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 26227 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       97 b- defN 23-Mar-28 10:11 flottplot/__init__.py
--rw-rw-r--  2.0 unx     4270 b- defN 23-Mar-28 10:11 flottplot/__main__.py
--rw-rw-r--  2.0 unx     1712 b- defN 23-Mar-28 10:11 flottplot/assets.py
--rw-rw-r--  2.0 unx     3093 b- defN 23-Mar-28 10:11 flottplot/convert.py
--rw-rw-r--  2.0 unx     1302 b- defN 23-Mar-28 10:11 flottplot/ipython.py
--rw-rw-r--  2.0 unx    37068 b- defN 23-Mar-28 10:13 flottplot/assets/flottplot-min.js
--rw-rw-r--  2.0 unx    37188 b- defN 23-Mar-28 10:13 flottplot/assets/flottplot-scan-min.js
--rw-rw-r--  2.0 unx      702 b- defN 23-Mar-28 10:13 flottplot/assets/flottplot.css
--rw-rw-r--  2.0 unx      251 b- defN 23-Mar-28 10:17 flottplot-2.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-28 10:17 flottplot-2.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Mar-28 10:17 flottplot-2.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      962 b- defN 23-Mar-28 10:17 flottplot-2.1.0.dist-info/RECORD
-12 files, 86747 bytes uncompressed, 24617 bytes compressed:  71.6%
+Zip file size: 27914 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       97 b- defN 23-Apr-10 10:36 flottplot/__init__.py
+-rw-rw-r--  2.0 unx     3809 b- defN 23-Apr-10 10:34 flottplot/__main__.py
+-rw-rw-r--  2.0 unx     1712 b- defN 23-Apr-09 20:51 flottplot/assets.py
+-rw-rw-r--  2.0 unx     3093 b- defN 23-Apr-10 10:34 flottplot/convert.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Apr-05 18:41 flottplot/ipython.py
+-rw-rw-r--  2.0 unx    41582 b- defN 23-Apr-10 11:01 flottplot/assets/flottplot-min.js
+-rw-rw-r--  2.0 unx    41708 b- defN 23-Apr-10 11:01 flottplot/assets/flottplot-scan-min.js
+-rw-rw-r--  2.0 unx      702 b- defN 23-Apr-10 11:01 flottplot/assets/flottplot.css
+-rw-rw-r--  2.0 unx      251 b- defN 23-Apr-10 11:02 flottplot-2.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 11:02 flottplot-2.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-10 11:02 flottplot-2.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      962 b- defN 23-Apr-10 11:02 flottplot-2.2.0.dist-info/RECORD
+12 files, 95320 bytes uncompressed, 26304 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: flottplot/assets/flottplot-scan-min.js
 Comment: 
 
 Filename: flottplot/assets/flottplot.css
 Comment: 
 
-Filename: flottplot-2.1.0.dist-info/METADATA
+Filename: flottplot-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: flottplot-2.1.0.dist-info/WHEEL
+Filename: flottplot-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: flottplot-2.1.0.dist-info/top_level.txt
+Filename: flottplot-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: flottplot-2.1.0.dist-info/RECORD
+Filename: flottplot-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flottplot/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .ipython import load_ipython_extension
 from .convert import convert
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

## flottplot/__main__.py

```diff
@@ -30,21 +30,16 @@
     # Write flottplot[-scan]-min.js
     _js_file = "flottplot-scan-min.js" if args.scan else "flottplot-min.js"
     asset_js = write_asset(_js_file, assetdir, args.overwrite)
     # Write flottplot.css if requested
     asset_css = None
     if args.style:
         asset_css = write_asset("flottplot.css", assetdir, args.overwrite)
-    # Write page with appropriate references to assets and all requested tags included
-    tags = []
-    if args.add_overlay:
-        tags.append("fp-overlay")
-    if args.add_state:
-        tags.append("fp-state")
-    filename.write_text(create_page(filename, js=asset_js, css=asset_css, tags=tags))
+    # Write page with appropriate references to assets
+    filename.write_text(create_page(filename, js=asset_js, css=asset_css))
 
 parser_init = subparsers.add_parser("init", description="""
     Create a new Flottplot page.
 """, help="""
     Create a new Flottplot page.
 """)
 parser_init.add_argument("-e", "--extension", metavar="EXT", default="html", help="""
@@ -63,21 +58,14 @@
 """)
 parser_init.add_argument("--no-style", action="store_false", dest="style", help="""
     Do not include the Flottplot styling (CSS file) in the output page.
 """)
 parser_init.add_argument("--no-scan", action="store_false", dest="scan", help="""
     Do not include the automatic element scan in the output page.
 """)
-parser_init.add_argument("--add-overlay", action="store_true", help="""
-    Include an <fp-overlay> tag. The overlay element will not work properly if
-    --no-style is also set.
-""")
-parser_init.add_argument("--add-state", action="store_true", help="""
-    Include an <fp-state> tag.
-""")
 parser_init.add_argument("file", metavar="FILE", help="""
     File name for the new Flottplot page. The file extension ".html" is added
     automatically unless otherwise specfied with -e.
 """)
 parser_init.set_defaults(cmd=init)
```

## flottplot/assets/flottplot-min.js

### js-beautify {}

```diff
@@ -119,24 +119,24 @@
         }
         _eval(substitutions) {
             return this
         }
         static from(value) {
             if (value == null) {
                 return null
-            }
-            if (false) {
-                return new TextValue(value)
-            }
-            for (let Cls of [NumberValue, DateDeltaValue, DateValue, TextValue]) {
-                try {
-                    return new Cls(value)
-                } catch (error) {
-                    if (!(error instanceof ParseError)) {
-                        throw error
+            } else if (value instanceof Value) {
+                return value
+            } else {
+                for (let Cls of [NumberValue, DateDeltaValue, DateValue, TextValue]) {
+                    try {
+                        return new Cls(value)
+                    } catch (error) {
+                        if (!(error instanceof ParseError)) {
+                            throw error
+                        }
                     }
                 }
             }
             throw new ParseError
         }
     }
     class TextValue extends Value {
@@ -823,45 +823,58 @@
             if (index < this.indexMin || this.indexMax < index) throw new ItemsError("invalid index " + index + " (out of range)");
             this._selected = index
         }
         get value() {
             return this._options[this._selected]
         }
         set value(value) {
+            value = Value.from(value);
             let index = this._options.findIndex(_ => _._eq(value));
             if (index < 0) throw new ItemsError("value " + value.toString() + " not found in options");
             this._selected = this.indexMin + index
         }
         map(...args) {
             return Array.from(this._options).map(...args)
         }
     }
     class RangeItems extends Items {
         constructor(init, step, min, max, wrap) {
             super();
             this.wrap = wrap;
+            init = Value.from(init);
+            step = Value.from(step);
+            min = Value.from(min);
+            max = Value.from(max);
             if (init != null) {
                 this._offset = init
             } else if (min != null) {
                 this._offset = min
             } else if (max != null) {
                 this._offset = max
             } else throw new ItemsError("range requires specification of at least one of init, min or max");
+            if (!(min == null || min instanceof this.valueType)) throw new ItemsError("min is a " + min.constructor.name + " but range expects " + this.valueType.name);
+            if (!(max == null || max instanceof this.valueType)) throw new ItemsError("max is a " + max.constructor.name + " but range expects " + this.valueType.name);
             if (step == null) throw new ItemsError("no step specified");
-            this._factor = step;
+            this._factor = Value.from(step);
             this.indexMin = min == null ? Number.NEGATIVE_INFINITY : Math.ceil(min._sub(this._offset)._div(step)._value);
             this.indexMax = max == null ? Number.POSITIVE_INFINITY : Math.floor(max._sub(this._offset)._div(step)._value);
             if (this.wrap && !this.isFinite) throw new ItemsError("open-ended range cannot wrap");
             this.value = this._offset
         }
+        get valueType() {
+            return this._offset.constructor
+        }
         _genValue(index) {
             return this._offset._add(this._factor._mul(new NumberValue(index)))
         }
         _genIndex(value) {
-            return Math.round(value._sub(this._offset)._div(this._factor)._value)
+            value = Value.from(value);
+            if (value instanceof this.valueType) {
+                return Math.round(value._sub(this._offset)._div(this._factor)._value)
+            } else throw new ItemsError("range expects " + this.valueType.name + " but received " + value.constructor.name)
         }
         get index() {
             return this._selected
         }
         set index(index) {
             if (index < this.indexMin || this.indexMax < index) throw new ItemsError("cannot set to index " + index);
             this._selected = index
@@ -878,20 +891,32 @@
             for (let index = this.indexMin; index <= this.indexMax; index++) {
                 out.push(this._genValue(index))
             }
             return out.map(...args)
         }
     }
     let dom = {
+        getPageRect: function(node) {
+            const rect = node.getBoundingClientRect();
+            return {
+                x: window.pageXOffset + rect.left,
+                y: window.pageYOffset + rect.top,
+                w: rect.width,
+                h: rect.height
+            }
+        },
         newNode: function(tag, attrs, children) {
             let node = document.createElement(tag);
             dom.setAttrs(node, attrs);
             if (children != null) {
                 for (let child of children) {
-                    node.appendChild(isString(child) ? document.createTextNode(child) : child)
+                    if (typeof child == "string" || child instanceof String) {
+                        child = document.createTextNode(child)
+                    }
+                    node.appendChild(child)
                 }
             }
             return node
         },
         newButton: function(attrs, label, f) {
             if (typeof label === "string") {
                 label = [label]
@@ -923,15 +948,17 @@
                 let value = this._attrs.has(attr) ? this._attrs.get(attr) : fallback;
                 switch (asType) {
                     case "VALUE":
                         return Value.from(value);
                     case "ACTION":
                         return value == null ? [] : value.split(";").map(call => call.split("."));
                     case "TARGET":
-                        return value == null ? [] : value.split(";")
+                        return value == null ? [] : value.split(";");
+                    case "BOOL":
+                        return value === "true"
                 }
                 return value
             }
             pop(attr, fallback, asType) {
                 const value = this.get(attr, fallback, asType);
                 this._attrs.delete(attr);
                 return value
@@ -957,24 +984,49 @@
             static from(node) {
                 const out = new dom.Attributes;
                 for (let attr of node.attributes) {
                     out.set(attr.name, attr.value)
                 }
                 return out
             }
+        },
+        Fullscreen: class {
+            constructor() {
+                this.exitCalls = [];
+                document.addEventListener("fullscreenchange", () => {
+                    if (document.fullscreenElement == null && this.exitCalls.length > 0) {
+                        const call = this.exitCalls.pop();
+                        if (call != null) {
+                            call()
+                        }
+                    }
+                })
+            }
+            show(node, onenter, onexit, onfail) {
+                node.requestFullscreen().then(() => {
+                    this.exitCalls.push(onexit);
+                    if (onenter != null) {
+                        onenter()
+                    }
+                }).catch(() => {
+                    if (onfail != null) {
+                        onfail()
+                    }
+                })
+            }
         }
     };
     class FPItems extends FPElement {
         constructor(id, items, format, calls) {
             super(id);
             this.items = items;
             this.format = format;
+            this.actions.add("reset");
             this.actions.add("prev");
             this.actions.add("next");
-            this.actions.add("reset");
             this._reset_index = this.items.index;
             this.calls = calls != null ? calls : new Map
         }
         get value() {
             return this.items.value
         }
         assertFinite() {
@@ -984,29 +1036,29 @@
         }
         get state() {
             return this.items.index
         }
         set state(state) {
             this.items.index = state
         }
+        reset() {
+            this.items.index = this._reset_index
+        }
         prev() {
             let e = this.items.prev();
             if (e === Items.WRAP) {
                 this.flottplot.invokeAll(this.calls.get("min-wrap"))
             }
         }
         next() {
             let e = this.items.next();
             if (e === Items.WRAP) {
                 this.flottplot.invokeAll(this.calls.get("max-wrap"))
             }
         }
-        reset() {
-            this.items.index = this._reset_index
-        }
         static ofType(etype, eid, items, format, calls) {
             switch (etype) {
                 case "counter":
                     return new FPCounter(eid, items, format, calls);
                 case "slider":
                     return new FPSlider(eid, items, format, calls);
                 case "dropdown":
@@ -1014,20 +1066,27 @@
                 case "radio":
                     return new FPRadio(eid, items, format, calls)
             }
             throw new ElementError("unknown items type '" + etype + "'")
         }
     }
     class FPCounter extends FPItems {
-        constructor(id, range, format, calls) {
-            super(id, range, format, calls);
+        constructor(id, items, format, calls) {
+            super(id, items, format, calls);
             this.box = dom.newNode("input", {
                 type: "text"
             });
-            this.box.disabled = true;
+            this.box.addEventListener("change", () => {
+                try {
+                    this.items.value = this.box.value
+                } catch (err) {
+                    console.error(err)
+                }
+                this.update()
+            });
             this.node = dom.newNode("span", {
                 class: "fp-range fp-range-counter"
             }, [dom.newButton({}, "<", () => this.invoke("prev")), this.box, dom.newButton({}, ">", () => this.invoke("next"))])
         }
         update() {
             this.box.value = this.items.value.toString(this.format)
         }
@@ -1125,14 +1184,28 @@
                 this.flottplot.invoke(target, action)
             }
         }
         trigger() {
             this.invokeAll(this.speed >= 0 ? "next" : "prev");
             this.timeout = setTimeout(() => this.trigger(), 2e3 / Math.abs(this.speed))
         }
+        get state() {
+            return {
+                playing: this.timeout != null,
+                speed: this.speed
+            }
+        }
+        set state(state) {
+            this.speed = state.speed;
+            if (state.playing) {
+                this.start()
+            } else {
+                this.stop()
+            }
+        }
         reset() {
             this.stop();
             this.invokeAll("reset")
         }
         start() {
             if (this.timeout == null) {
                 this.toggle()
@@ -1191,56 +1264,125 @@
             this.flottplot.invokeAll(this.calls)
         }
         static from(node) {
             let attrs = dom.Attributes.from(node);
             return new FPButton(attrs.id, Array.from(node.childNodes), attrs.pop("action", null, "ACTION"), attrs)
         }
     }
-
-    function getPageRect(node) {
-        let rect = node.getBoundingClientRect();
-        return {
-            x: window.pageXOffset + rect.left,
-            y: window.pageYOffset + rect.top,
-            w: rect.width,
-            h: rect.height
+    class FPCalendar extends FPElement {
+        constructor(id, init, attrs) {
+            super(id);
+            if (init == null) {
+                init = (new Date).toISOString().slice(0, 10)
+            } else if (init instanceof DateValue) {
+                init = init.toString("%Y-%m-%d")
+            } else throw new ValueError("cannot initialize calendar with " + init.constructor.name);
+            this._resetValue = init;
+            this.node = dom.newNode("input", attrs);
+            this.node.id = this.id;
+            this.node.type = "date";
+            this.node.value = init;
+            this.node.addEventListener("change", () => this.notify());
+            this.actions.add("reset");
+            this.actions.add("prevYear");
+            this.actions.add("prevMonth");
+            this.actions.add("prev");
+            this.actions.add("next");
+            this.actions.add("nextMonth");
+            this.actions.add("nextYear")
+        }
+        static from(node) {
+            const attrs = dom.Attributes.from(node);
+            return new FPCalendar(attrs.id, attrs.pop("init", null, "VALUE"), attrs)
+        }
+        get value() {
+            return Value.from(this.node.value)
+        }
+        get _date() {
+            return new Date(this.node.valueAsNumber)
+        }
+        reset() {
+            this.node.value = this._resetValue
+        }
+        prev() {
+            this.node.valueAsNumber = this._date.setUTCDate(this._date.getUTCDate() - 1)
+        }
+        next() {
+            this.node.valueAsNumber = this._date.setUTCDate(this._date.getUTCDate() + 1)
+        }
+        prevMonth() {
+            this.node.valueAsNumber = this._date.setUTCMonth(this._date.getUTCMonth() - 1)
+        }
+        nextMonth() {
+            this.node.valueAsNumber = this._date.setUTCMonth(this._date.getUTCMonth() + 1)
+        }
+        prevYear() {
+            this.node.valueAsNumber = this._date.setUTCFullYear(this._date.getUTCFullYear() - 1)
+        }
+        nextYear() {
+            this.node.valueAsNumber = this._date.setUTCFullYear(this._date.getUTCFullYear() + 1)
+        }
+    }
+    class FPControls extends FPElement {
+        constructor(id, target, attrs) {
+            super(id);
+            this.node = dom.newNode("span", attrs);
+            this.node.id = this.id;
+            this.node.classList.add("fp-controls");
+            this.target = target
+        }
+        initialize() {
+            const element = this.flottplot.getElement(this.target);
+            for (const action of element.actions) {
+                let label = action.replace(/([A-Z])/g, " $1").toLowerCase();
+                this.node.appendChild(dom.newButton({}, label, () => {
+                    this.flottplot.invoke(element.id, action)
+                }))
+            }
+        }
+        static from(node) {
+            const attrs = dom.Attributes.from(node);
+            const targets = attrs.pop("target", null, "TARGET");
+            if (targets.length > 1) {
+                throw new ElementError("only one target allowed")
+            }
+            return new FPControls(attrs.id, targets[0], attrs)
         }
     }
     class FPCursors extends FPElement {
         constructor(id, cursors, attrs) {
             super(id);
             this.cursors = cursors;
             for (let cc of this.cursors) {
-                if (cc["cursor"] === "hidden") continue;
-                cc.node = dom.newNode("div");
-                if (cc["class"] != null) cc.node.setAttribute("class", cc["class"]);
-                if (cc["style"] != null) cc.node.setAttribute("style", cc["style"]);
+                if (cc.cursor === "hidden") continue;
+                cc.node = dom.newNode("div", cc.attrs);
+                cc.node.classList.add("fp-cursor", "fp-" + cc.cursor);
                 cc.node.style.position = "absolute"
             }
-            this.node = dom.newNode("div", attrs, this.cursors.map(_ => _.node).filter(_ => _ != null));
+            this.node = dom.newNode("div", attrs, this.cursors.map(_ => _.node));
             this.node.id = this.id;
-            this.node.className = "fp-cursors"
+            this.node.classList.add("fp-cursors")
         }
         initialize() {
             for (let cursor of this.cursors) {
                 let origin = this.flottplot.getElement(cursor.target);
                 origin.node.addEventListener("mouseover", event => this.cursors.forEach(cc => {
                     if (cc.target !== cursor.target && cc.node != null) {
                         cc.node.style.display = "block"
                     }
                 }));
                 origin.node.addEventListener("mousemove", event => {
-                    let etr = getPageRect(event.target);
+                    let etr = dom.getPageRect(event.target);
                     let x = (event.pageX - etr.x) / etr.w;
                     let y = (event.pageY - etr.y) / etr.h;
                     for (let cc of this.cursors) {
                         let target = this.flottplot.getElement(cc.target);
                         if (origin.id === target.id || cc.node == null) continue;
                         let style = cc.node.style;
-                        let ctr = getPageRect(target.node);
+                        let ctr = dom.getPageRect(target.node);
                         if (cc.cursor === "hline") {
                             style.top = ctr.y + y * ctr.h + "px";
                             style.left = ctr.x + "px";
                             style.width = ctr.w + "px"
                         } else if (cc.cursor === "vline") {
                             style.top = ctr.y + "px";
                             style.left = ctr.x + x * ctr.w + "px";
@@ -1258,35 +1400,51 @@
                 }))
             }
         }
         static from(node) {
             let cursors = [];
             for (let child of node.childNodes) {
                 if (child.nodeType !== Node.ELEMENT_NODE) continue;
-                let attrs = dom.Attributes.from(child);
-                let cur = attrs.pop("cursor", "pointer");
+                const attrs = dom.Attributes.from(child);
                 cursors.push({
                     target: attrs.pop("target"),
-                    cursor: cur,
-                    style: attrs.pop("style"),
-                    class: attrs.pop("class", "fp-cursor fp-" + cur)
+                    cursor: attrs.pop("cursor", "pointer"),
+                    attrs: attrs
                 })
             }
             return new FPCursors(node.id, cursors, dom.Attributes.from(node))
         }
     }
+    class FPFrame extends FPElement {
+        constructor(id, attrs, children, calls) {
+            super(id);
+            this.node = dom.newNode("div", attrs, Array.from(children));
+            this.node.id = this.id;
+            this.node.classList.add("fp-frame");
+            this.calls = calls != null ? calls : new Map;
+            this.actions.add("fullscreen")
+        }
+        fullscreen() {
+            this.flottplot.fullscreen.show(this.node, () => this.flottplot.invokeAll(this.calls.get("enter")), () => this.flottplot.invokeAll(this.calls.get("exit")), () => this.fail("browser refused fullscreen request, see console for more information"))
+        }
+        static from(node) {
+            const attrs = dom.Attributes.from(node);
+            const calls = attrs.popActions(["enter", "exit"]);
+            return new FPFrame(attrs.id, attrs, node.children, calls)
+        }
+    }
     class FPOverlay extends FPElement {
         constructor(id, attrs) {
             super(id);
             this.inner = dom.newNode("div", {
                 class: "fp-overlay-inner"
             });
             this.node = dom.newNode("div", attrs, [this.inner]);
             this.node.id = this.id;
-            this.node.className = "fp-overlay";
+            this.node.classList.add("fp-overlay");
             this.node.style.display = "none";
             this.node.addEventListener("click", event => this.hide());
             this.actions.add("show");
             this.actions.add("hide");
             this.actions.add("toggle")
         }
         initialize() {
@@ -1325,19 +1483,25 @@
             this.node.addEventListener("click", () => {
                 if (this.flottplot.overlay != null) this.flottplot.overlay.put(this.overlay)
             });
             if (src == null) {
                 return this.fail("must provide source (src) of plot")
             }
             this.src = src;
-            this.setDependenciesFrom(src)
+            this.setDependenciesFrom(src);
+            this.actions.add("fullscreen")
         }
         get value() {
             return Value.from(this.node.src)
         }
+        fullscreen() {
+            this.flottplot.fullscreen.show(this.node, null, null, () => {
+                this.fail("browser refused fullscreen request, see console for more information")
+            })
+        }
         update(substitution) {
             let src = this.substitute(this.src, substitution);
             this.node.src = src;
             this.overlay.src = src
         }
         static from(node) {
             let attrs = dom.Attributes.from(node);
@@ -1369,15 +1533,15 @@
     }
     class FPStack extends FPElement {
         constructor(id, plots, attrs) {
             super(id);
             this.plots = plots;
             this.node = dom.newNode("div", attrs, this.plots);
             this.node.id = this.id;
-            this.node.className = "fp-stack";
+            this.node.classList.add("fp-stack");
             this.overlay = dom.newNode("div", {
                 class: "fp-stack"
             });
             this.node.addEventListener("click", event => {
                 if (this.flottplot.overlay != null) {
                     this.flottplot.overlay.put(this.overlay);
                     event.stopPropagation()
@@ -1402,19 +1566,37 @@
                 if (child.nodeName !== "IMG") throw new flottplot.ElementError("invalid element '" + child.nodeName + "' in stack");
                 plots.push(child)
             }
             return new FPStack(node.id, plots, dom.Attributes.from(node))
         }
     }
     class FPState extends FPElement {
+        constructor(id, useURL) {
+            super(id);
+            this.useURL = useURL;
+            this.savedState = null;
+            this.actions.add("save");
+            this.actions.add("restore")
+        }
         initialize() {
-            this.flottplot.urlstate = true
+            if (this.useURL === true) {
+                this.flottplot.urlstate = true
+            }
+        }
+        save() {
+            this.savedState = this.flottplot.state
+        }
+        restore() {
+            if (this.savedState != null) {
+                this.flottplot.state = this.savedState
+            }
         }
         static from(node) {
-            return new FPState(node.id)
+            const attrs = dom.Attributes.from(node);
+            return new FPState(attrs.id, attrs.pop("url", false, "BOOL"))
         }
     }
     class FPText extends FPElement {
         constructor(id, text) {
             super(id);
             this.node = dom.newNode("span", {
                 id: id
@@ -1464,68 +1646,66 @@
             return new FPVideo(attrs.id, [attrs.pop("src")], attrs)
         }
     }
     class Flottplot {
         constructor() {
             this._elements = new Map;
             this._graph = new UpdateGraph;
+            this.fullscreen = new dom.Fullscreen;
             this.overlay = null;
             this.bindings = new Map;
             this.urlstate = false
         }
         getElement(target) {
             let element = this._elements.get(target);
             if (element == null) throw new ElementError("element with id '" + target + "' does not exist");
             return element
         }
-        convert(original) {
-            let tag = Flottplot.tags.get(original.nodeName);
-            if (tag == null) throw new ElementError("unable to convert '" + original.nodeName + "': no corresponding flottplot element found");
-            let element;
-            try {
-                element = tag.Class.from(original)
-            } catch (error) {
-                if (!(error instanceof FlottplotError)) {
-                    throw error
-                }
-                original.replaceWith(dom.newNode("div", {
-                    style: "border:3px solid #F00;background-color:#FCC;padding:3px;"
-                }, [dom.newNode("b", {}, [error.constructor.name, ": "]), error.message]));
-                console.error(error);
-                return
-            }
-            if (element.node == null) {
-                original.remove()
-            } else {
-                original.replaceWith(element.node)
-            }
+        add(element) {
             if (this._elements.has(element.id)) {
                 element.fail("duplicate id");
                 this._elements.get(element.id).fail("duplicate id")
             }
             this._elements.set(element.id, element);
             this._graph.getNode(element.id);
             for (let dep of element.dependencies) {
                 this._graph.addEdge(element.id, dep)
             }
-            element.flottplot = this;
-            return this
+            element.flottplot = this
         }
-        scan(root) {
-            let tag = Flottplot.tags.get(root.nodeName);
+        convert(node) {
+            const tag = Flottplot.tags.get(node.nodeName);
             if (tag == null || tag.isRecursive) {
-                let children = Array.from(root.childNodes);
-                for (let child of children) {
-                    this.scan(child)
+                const children = Array.from(node.childNodes);
+                for (const child of children) {
+                    this.convert(child)
                 }
             }
-            if (tag != null) {
-                this.convert(root)
+            if (tag == null || tag.Class == null) {
+                return
             }
-            return this
+            let element;
+            try {
+                element = tag.Class.from(node)
+            } catch (error) {
+                if (!(error instanceof FlottplotError)) {
+                    throw error
+                }
+                node.replaceWith(dom.newNode("div", {
+                    style: "border:3px solid #F00;background-color:#FCC;padding:3px;"
+                }, [dom.newNode("b", {}, [error.constructor.name, ": "]), error.message]));
+                console.error(error);
+                return
+            }
+            if (element.node == null) {
+                node.remove()
+            } else {
+                node.replaceWith(element.node)
+            }
+            this.add(element)
         }
         initialize() {
             for (let id of this._graph.orderedNodes) {
                 let element = this._elements.get(id);
                 if (element == null) {
                     console.warn("flottplot element with id '" + id + "' does not exist");
                     continue
@@ -1536,25 +1716,25 @@
                     element.failWith(error);
                     console.error(error)
                 }
             }
             if (this.urlstate) {
                 let hash = window.location.hash.substring(1);
                 if (hash.length !== 0) {
-                    this._state = JSON.parse(window.atob(hash))
+                    this.state = JSON.parse(window.atob(hash))
                 }
             }
         }
         notify(source) {
             for (let target of this._graph.updateOrderedNodesOf(source)) {
                 let element = this._elements.get(target);
                 element.update(this._substitutionFor(element))
             }
             if (this.urlstate) {
-                window.location.hash = window.btoa(JSON.stringify(this._state))
+                window.location.hash = window.btoa(JSON.stringify(this.state))
             }
         }
         _substitutionFor(element) {
             let values = new Map;
             for (let dep of element.dependencies) {
                 let dep_element = this._elements.get(dep);
                 if (dep_element == null) {
@@ -1591,25 +1771,25 @@
                 return
             }
             let callable = this.bindings.get(event.key);
             if (callable != null) {
                 callable()
             }
         }
-        get _state() {
+        get state() {
             let out = {};
             for (let [id, element] of this._elements) {
                 if (id.startsWith("_")) continue;
                 let state = element.state;
                 if (state === undefined) continue;
                 out[id] = state
             }
             return out
         }
-        set _state(state) {
+        set state(state) {
             for (let id of this._graph.orderedNodes) {
                 if (!state.hasOwnProperty(id)) continue;
                 let element = this._elements.get(id);
                 element.state = state[id];
                 element.update(this._substitutionFor(element));
                 element.notify()
             }
@@ -1619,27 +1799,30 @@
                 Class: element,
                 isRecursive: recursive
             })
         }
     }
     Flottplot.tags = new Map;
     Flottplot.registerTag("fp-animation", FPAnimation, false);
+    Flottplot.registerTag("fp-controls", FPControls, false);
     Flottplot.registerTag("fp-bind", FPBind, false);
     Flottplot.registerTag("fp-button", FPButton, false);
     Flottplot.registerTag("fp-cursors", FPCursors, false);
+    Flottplot.registerTag("fp-calendar", FPCalendar, false);
+    Flottplot.registerTag("fp-frame", FPFrame, true);
     Flottplot.registerTag("fp-overlay", FPOverlay, false);
     Flottplot.registerTag("fp-plot", FPPlot, false);
     Flottplot.registerTag("fp-range", FPRange, false);
     Flottplot.registerTag("fp-select", FPSelect, false);
     Flottplot.registerTag("fp-stack", FPStack, true);
     Flottplot.registerTag("fp-state", FPState, false);
     Flottplot.registerTag("fp-text", FPText, true);
     Flottplot.registerTag("fp-video", FPVideo, false);
     return {
-        __version__: "2.1.0",
+        VERSION: "2.2.0",
         Flottplot: Flottplot,
         FPElement: FPElement,
         Value: Value,
         OptionsItems: OptionsItems,
         RangeItems: RangeItems,
         FlottplotError: FlottplotError,
         ElementError: ElementError,
```

## flottplot/assets/flottplot-scan-min.js

### js-beautify {}

```diff
@@ -119,24 +119,24 @@
         }
         _eval(substitutions) {
             return this
         }
         static from(value) {
             if (value == null) {
                 return null
-            }
-            if (false) {
-                return new TextValue(value)
-            }
-            for (let Cls of [NumberValue, DateDeltaValue, DateValue, TextValue]) {
-                try {
-                    return new Cls(value)
-                } catch (error) {
-                    if (!(error instanceof ParseError)) {
-                        throw error
+            } else if (value instanceof Value) {
+                return value
+            } else {
+                for (let Cls of [NumberValue, DateDeltaValue, DateValue, TextValue]) {
+                    try {
+                        return new Cls(value)
+                    } catch (error) {
+                        if (!(error instanceof ParseError)) {
+                            throw error
+                        }
                     }
                 }
             }
             throw new ParseError
         }
     }
     class TextValue extends Value {
@@ -823,45 +823,58 @@
             if (index < this.indexMin || this.indexMax < index) throw new ItemsError("invalid index " + index + " (out of range)");
             this._selected = index
         }
         get value() {
             return this._options[this._selected]
         }
         set value(value) {
+            value = Value.from(value);
             let index = this._options.findIndex(_ => _._eq(value));
             if (index < 0) throw new ItemsError("value " + value.toString() + " not found in options");
             this._selected = this.indexMin + index
         }
         map(...args) {
             return Array.from(this._options).map(...args)
         }
     }
     class RangeItems extends Items {
         constructor(init, step, min, max, wrap) {
             super();
             this.wrap = wrap;
+            init = Value.from(init);
+            step = Value.from(step);
+            min = Value.from(min);
+            max = Value.from(max);
             if (init != null) {
                 this._offset = init
             } else if (min != null) {
                 this._offset = min
             } else if (max != null) {
                 this._offset = max
             } else throw new ItemsError("range requires specification of at least one of init, min or max");
+            if (!(min == null || min instanceof this.valueType)) throw new ItemsError("min is a " + min.constructor.name + " but range expects " + this.valueType.name);
+            if (!(max == null || max instanceof this.valueType)) throw new ItemsError("max is a " + max.constructor.name + " but range expects " + this.valueType.name);
             if (step == null) throw new ItemsError("no step specified");
-            this._factor = step;
+            this._factor = Value.from(step);
             this.indexMin = min == null ? Number.NEGATIVE_INFINITY : Math.ceil(min._sub(this._offset)._div(step)._value);
             this.indexMax = max == null ? Number.POSITIVE_INFINITY : Math.floor(max._sub(this._offset)._div(step)._value);
             if (this.wrap && !this.isFinite) throw new ItemsError("open-ended range cannot wrap");
             this.value = this._offset
         }
+        get valueType() {
+            return this._offset.constructor
+        }
         _genValue(index) {
             return this._offset._add(this._factor._mul(new NumberValue(index)))
         }
         _genIndex(value) {
-            return Math.round(value._sub(this._offset)._div(this._factor)._value)
+            value = Value.from(value);
+            if (value instanceof this.valueType) {
+                return Math.round(value._sub(this._offset)._div(this._factor)._value)
+            } else throw new ItemsError("range expects " + this.valueType.name + " but received " + value.constructor.name)
         }
         get index() {
             return this._selected
         }
         set index(index) {
             if (index < this.indexMin || this.indexMax < index) throw new ItemsError("cannot set to index " + index);
             this._selected = index
@@ -878,20 +891,32 @@
             for (let index = this.indexMin; index <= this.indexMax; index++) {
                 out.push(this._genValue(index))
             }
             return out.map(...args)
         }
     }
     let dom = {
+        getPageRect: function(node) {
+            const rect = node.getBoundingClientRect();
+            return {
+                x: window.pageXOffset + rect.left,
+                y: window.pageYOffset + rect.top,
+                w: rect.width,
+                h: rect.height
+            }
+        },
         newNode: function(tag, attrs, children) {
             let node = document.createElement(tag);
             dom.setAttrs(node, attrs);
             if (children != null) {
                 for (let child of children) {
-                    node.appendChild(isString(child) ? document.createTextNode(child) : child)
+                    if (typeof child == "string" || child instanceof String) {
+                        child = document.createTextNode(child)
+                    }
+                    node.appendChild(child)
                 }
             }
             return node
         },
         newButton: function(attrs, label, f) {
             if (typeof label === "string") {
                 label = [label]
@@ -923,15 +948,17 @@
                 let value = this._attrs.has(attr) ? this._attrs.get(attr) : fallback;
                 switch (asType) {
                     case "VALUE":
                         return Value.from(value);
                     case "ACTION":
                         return value == null ? [] : value.split(";").map(call => call.split("."));
                     case "TARGET":
-                        return value == null ? [] : value.split(";")
+                        return value == null ? [] : value.split(";");
+                    case "BOOL":
+                        return value === "true"
                 }
                 return value
             }
             pop(attr, fallback, asType) {
                 const value = this.get(attr, fallback, asType);
                 this._attrs.delete(attr);
                 return value
@@ -957,24 +984,49 @@
             static from(node) {
                 const out = new dom.Attributes;
                 for (let attr of node.attributes) {
                     out.set(attr.name, attr.value)
                 }
                 return out
             }
+        },
+        Fullscreen: class {
+            constructor() {
+                this.exitCalls = [];
+                document.addEventListener("fullscreenchange", () => {
+                    if (document.fullscreenElement == null && this.exitCalls.length > 0) {
+                        const call = this.exitCalls.pop();
+                        if (call != null) {
+                            call()
+                        }
+                    }
+                })
+            }
+            show(node, onenter, onexit, onfail) {
+                node.requestFullscreen().then(() => {
+                    this.exitCalls.push(onexit);
+                    if (onenter != null) {
+                        onenter()
+                    }
+                }).catch(() => {
+                    if (onfail != null) {
+                        onfail()
+                    }
+                })
+            }
         }
     };
     class FPItems extends FPElement {
         constructor(id, items, format, calls) {
             super(id);
             this.items = items;
             this.format = format;
+            this.actions.add("reset");
             this.actions.add("prev");
             this.actions.add("next");
-            this.actions.add("reset");
             this._reset_index = this.items.index;
             this.calls = calls != null ? calls : new Map
         }
         get value() {
             return this.items.value
         }
         assertFinite() {
@@ -984,29 +1036,29 @@
         }
         get state() {
             return this.items.index
         }
         set state(state) {
             this.items.index = state
         }
+        reset() {
+            this.items.index = this._reset_index
+        }
         prev() {
             let e = this.items.prev();
             if (e === Items.WRAP) {
                 this.flottplot.invokeAll(this.calls.get("min-wrap"))
             }
         }
         next() {
             let e = this.items.next();
             if (e === Items.WRAP) {
                 this.flottplot.invokeAll(this.calls.get("max-wrap"))
             }
         }
-        reset() {
-            this.items.index = this._reset_index
-        }
         static ofType(etype, eid, items, format, calls) {
             switch (etype) {
                 case "counter":
                     return new FPCounter(eid, items, format, calls);
                 case "slider":
                     return new FPSlider(eid, items, format, calls);
                 case "dropdown":
@@ -1014,20 +1066,27 @@
                 case "radio":
                     return new FPRadio(eid, items, format, calls)
             }
             throw new ElementError("unknown items type '" + etype + "'")
         }
     }
     class FPCounter extends FPItems {
-        constructor(id, range, format, calls) {
-            super(id, range, format, calls);
+        constructor(id, items, format, calls) {
+            super(id, items, format, calls);
             this.box = dom.newNode("input", {
                 type: "text"
             });
-            this.box.disabled = true;
+            this.box.addEventListener("change", () => {
+                try {
+                    this.items.value = this.box.value
+                } catch (err) {
+                    console.error(err)
+                }
+                this.update()
+            });
             this.node = dom.newNode("span", {
                 class: "fp-range fp-range-counter"
             }, [dom.newButton({}, "<", () => this.invoke("prev")), this.box, dom.newButton({}, ">", () => this.invoke("next"))])
         }
         update() {
             this.box.value = this.items.value.toString(this.format)
         }
@@ -1125,14 +1184,28 @@
                 this.flottplot.invoke(target, action)
             }
         }
         trigger() {
             this.invokeAll(this.speed >= 0 ? "next" : "prev");
             this.timeout = setTimeout(() => this.trigger(), 2e3 / Math.abs(this.speed))
         }
+        get state() {
+            return {
+                playing: this.timeout != null,
+                speed: this.speed
+            }
+        }
+        set state(state) {
+            this.speed = state.speed;
+            if (state.playing) {
+                this.start()
+            } else {
+                this.stop()
+            }
+        }
         reset() {
             this.stop();
             this.invokeAll("reset")
         }
         start() {
             if (this.timeout == null) {
                 this.toggle()
@@ -1191,56 +1264,125 @@
             this.flottplot.invokeAll(this.calls)
         }
         static from(node) {
             let attrs = dom.Attributes.from(node);
             return new FPButton(attrs.id, Array.from(node.childNodes), attrs.pop("action", null, "ACTION"), attrs)
         }
     }
-
-    function getPageRect(node) {
-        let rect = node.getBoundingClientRect();
-        return {
-            x: window.pageXOffset + rect.left,
-            y: window.pageYOffset + rect.top,
-            w: rect.width,
-            h: rect.height
+    class FPCalendar extends FPElement {
+        constructor(id, init, attrs) {
+            super(id);
+            if (init == null) {
+                init = (new Date).toISOString().slice(0, 10)
+            } else if (init instanceof DateValue) {
+                init = init.toString("%Y-%m-%d")
+            } else throw new ValueError("cannot initialize calendar with " + init.constructor.name);
+            this._resetValue = init;
+            this.node = dom.newNode("input", attrs);
+            this.node.id = this.id;
+            this.node.type = "date";
+            this.node.value = init;
+            this.node.addEventListener("change", () => this.notify());
+            this.actions.add("reset");
+            this.actions.add("prevYear");
+            this.actions.add("prevMonth");
+            this.actions.add("prev");
+            this.actions.add("next");
+            this.actions.add("nextMonth");
+            this.actions.add("nextYear")
+        }
+        static from(node) {
+            const attrs = dom.Attributes.from(node);
+            return new FPCalendar(attrs.id, attrs.pop("init", null, "VALUE"), attrs)
+        }
+        get value() {
+            return Value.from(this.node.value)
+        }
+        get _date() {
+            return new Date(this.node.valueAsNumber)
+        }
+        reset() {
+            this.node.value = this._resetValue
+        }
+        prev() {
+            this.node.valueAsNumber = this._date.setUTCDate(this._date.getUTCDate() - 1)
+        }
+        next() {
+            this.node.valueAsNumber = this._date.setUTCDate(this._date.getUTCDate() + 1)
+        }
+        prevMonth() {
+            this.node.valueAsNumber = this._date.setUTCMonth(this._date.getUTCMonth() - 1)
+        }
+        nextMonth() {
+            this.node.valueAsNumber = this._date.setUTCMonth(this._date.getUTCMonth() + 1)
+        }
+        prevYear() {
+            this.node.valueAsNumber = this._date.setUTCFullYear(this._date.getUTCFullYear() - 1)
+        }
+        nextYear() {
+            this.node.valueAsNumber = this._date.setUTCFullYear(this._date.getUTCFullYear() + 1)
+        }
+    }
+    class FPControls extends FPElement {
+        constructor(id, target, attrs) {
+            super(id);
+            this.node = dom.newNode("span", attrs);
+            this.node.id = this.id;
+            this.node.classList.add("fp-controls");
+            this.target = target
+        }
+        initialize() {
+            const element = this.flottplot.getElement(this.target);
+            for (const action of element.actions) {
+                let label = action.replace(/([A-Z])/g, " $1").toLowerCase();
+                this.node.appendChild(dom.newButton({}, label, () => {
+                    this.flottplot.invoke(element.id, action)
+                }))
+            }
+        }
+        static from(node) {
+            const attrs = dom.Attributes.from(node);
+            const targets = attrs.pop("target", null, "TARGET");
+            if (targets.length > 1) {
+                throw new ElementError("only one target allowed")
+            }
+            return new FPControls(attrs.id, targets[0], attrs)
         }
     }
     class FPCursors extends FPElement {
         constructor(id, cursors, attrs) {
             super(id);
             this.cursors = cursors;
             for (let cc of this.cursors) {
-                if (cc["cursor"] === "hidden") continue;
-                cc.node = dom.newNode("div");
-                if (cc["class"] != null) cc.node.setAttribute("class", cc["class"]);
-                if (cc["style"] != null) cc.node.setAttribute("style", cc["style"]);
+                if (cc.cursor === "hidden") continue;
+                cc.node = dom.newNode("div", cc.attrs);
+                cc.node.classList.add("fp-cursor", "fp-" + cc.cursor);
                 cc.node.style.position = "absolute"
             }
-            this.node = dom.newNode("div", attrs, this.cursors.map(_ => _.node).filter(_ => _ != null));
+            this.node = dom.newNode("div", attrs, this.cursors.map(_ => _.node));
             this.node.id = this.id;
-            this.node.className = "fp-cursors"
+            this.node.classList.add("fp-cursors")
         }
         initialize() {
             for (let cursor of this.cursors) {
                 let origin = this.flottplot.getElement(cursor.target);
                 origin.node.addEventListener("mouseover", event => this.cursors.forEach(cc => {
                     if (cc.target !== cursor.target && cc.node != null) {
                         cc.node.style.display = "block"
                     }
                 }));
                 origin.node.addEventListener("mousemove", event => {
-                    let etr = getPageRect(event.target);
+                    let etr = dom.getPageRect(event.target);
                     let x = (event.pageX - etr.x) / etr.w;
                     let y = (event.pageY - etr.y) / etr.h;
                     for (let cc of this.cursors) {
                         let target = this.flottplot.getElement(cc.target);
                         if (origin.id === target.id || cc.node == null) continue;
                         let style = cc.node.style;
-                        let ctr = getPageRect(target.node);
+                        let ctr = dom.getPageRect(target.node);
                         if (cc.cursor === "hline") {
                             style.top = ctr.y + y * ctr.h + "px";
                             style.left = ctr.x + "px";
                             style.width = ctr.w + "px"
                         } else if (cc.cursor === "vline") {
                             style.top = ctr.y + "px";
                             style.left = ctr.x + x * ctr.w + "px";
@@ -1258,35 +1400,51 @@
                 }))
             }
         }
         static from(node) {
             let cursors = [];
             for (let child of node.childNodes) {
                 if (child.nodeType !== Node.ELEMENT_NODE) continue;
-                let attrs = dom.Attributes.from(child);
-                let cur = attrs.pop("cursor", "pointer");
+                const attrs = dom.Attributes.from(child);
                 cursors.push({
                     target: attrs.pop("target"),
-                    cursor: cur,
-                    style: attrs.pop("style"),
-                    class: attrs.pop("class", "fp-cursor fp-" + cur)
+                    cursor: attrs.pop("cursor", "pointer"),
+                    attrs: attrs
                 })
             }
             return new FPCursors(node.id, cursors, dom.Attributes.from(node))
         }
     }
+    class FPFrame extends FPElement {
+        constructor(id, attrs, children, calls) {
+            super(id);
+            this.node = dom.newNode("div", attrs, Array.from(children));
+            this.node.id = this.id;
+            this.node.classList.add("fp-frame");
+            this.calls = calls != null ? calls : new Map;
+            this.actions.add("fullscreen")
+        }
+        fullscreen() {
+            this.flottplot.fullscreen.show(this.node, () => this.flottplot.invokeAll(this.calls.get("enter")), () => this.flottplot.invokeAll(this.calls.get("exit")), () => this.fail("browser refused fullscreen request, see console for more information"))
+        }
+        static from(node) {
+            const attrs = dom.Attributes.from(node);
+            const calls = attrs.popActions(["enter", "exit"]);
+            return new FPFrame(attrs.id, attrs, node.children, calls)
+        }
+    }
     class FPOverlay extends FPElement {
         constructor(id, attrs) {
             super(id);
             this.inner = dom.newNode("div", {
                 class: "fp-overlay-inner"
             });
             this.node = dom.newNode("div", attrs, [this.inner]);
             this.node.id = this.id;
-            this.node.className = "fp-overlay";
+            this.node.classList.add("fp-overlay");
             this.node.style.display = "none";
             this.node.addEventListener("click", event => this.hide());
             this.actions.add("show");
             this.actions.add("hide");
             this.actions.add("toggle")
         }
         initialize() {
@@ -1325,19 +1483,25 @@
             this.node.addEventListener("click", () => {
                 if (this.flottplot.overlay != null) this.flottplot.overlay.put(this.overlay)
             });
             if (src == null) {
                 return this.fail("must provide source (src) of plot")
             }
             this.src = src;
-            this.setDependenciesFrom(src)
+            this.setDependenciesFrom(src);
+            this.actions.add("fullscreen")
         }
         get value() {
             return Value.from(this.node.src)
         }
+        fullscreen() {
+            this.flottplot.fullscreen.show(this.node, null, null, () => {
+                this.fail("browser refused fullscreen request, see console for more information")
+            })
+        }
         update(substitution) {
             let src = this.substitute(this.src, substitution);
             this.node.src = src;
             this.overlay.src = src
         }
         static from(node) {
             let attrs = dom.Attributes.from(node);
@@ -1369,15 +1533,15 @@
     }
     class FPStack extends FPElement {
         constructor(id, plots, attrs) {
             super(id);
             this.plots = plots;
             this.node = dom.newNode("div", attrs, this.plots);
             this.node.id = this.id;
-            this.node.className = "fp-stack";
+            this.node.classList.add("fp-stack");
             this.overlay = dom.newNode("div", {
                 class: "fp-stack"
             });
             this.node.addEventListener("click", event => {
                 if (this.flottplot.overlay != null) {
                     this.flottplot.overlay.put(this.overlay);
                     event.stopPropagation()
@@ -1402,19 +1566,37 @@
                 if (child.nodeName !== "IMG") throw new flottplot.ElementError("invalid element '" + child.nodeName + "' in stack");
                 plots.push(child)
             }
             return new FPStack(node.id, plots, dom.Attributes.from(node))
         }
     }
     class FPState extends FPElement {
+        constructor(id, useURL) {
+            super(id);
+            this.useURL = useURL;
+            this.savedState = null;
+            this.actions.add("save");
+            this.actions.add("restore")
+        }
         initialize() {
-            this.flottplot.urlstate = true
+            if (this.useURL === true) {
+                this.flottplot.urlstate = true
+            }
+        }
+        save() {
+            this.savedState = this.flottplot.state
+        }
+        restore() {
+            if (this.savedState != null) {
+                this.flottplot.state = this.savedState
+            }
         }
         static from(node) {
-            return new FPState(node.id)
+            const attrs = dom.Attributes.from(node);
+            return new FPState(attrs.id, attrs.pop("url", false, "BOOL"))
         }
     }
     class FPText extends FPElement {
         constructor(id, text) {
             super(id);
             this.node = dom.newNode("span", {
                 id: id
@@ -1464,68 +1646,66 @@
             return new FPVideo(attrs.id, [attrs.pop("src")], attrs)
         }
     }
     class Flottplot {
         constructor() {
             this._elements = new Map;
             this._graph = new UpdateGraph;
+            this.fullscreen = new dom.Fullscreen;
             this.overlay = null;
             this.bindings = new Map;
             this.urlstate = false
         }
         getElement(target) {
             let element = this._elements.get(target);
             if (element == null) throw new ElementError("element with id '" + target + "' does not exist");
             return element
         }
-        convert(original) {
-            let tag = Flottplot.tags.get(original.nodeName);
-            if (tag == null) throw new ElementError("unable to convert '" + original.nodeName + "': no corresponding flottplot element found");
-            let element;
-            try {
-                element = tag.Class.from(original)
-            } catch (error) {
-                if (!(error instanceof FlottplotError)) {
-                    throw error
-                }
-                original.replaceWith(dom.newNode("div", {
-                    style: "border:3px solid #F00;background-color:#FCC;padding:3px;"
-                }, [dom.newNode("b", {}, [error.constructor.name, ": "]), error.message]));
-                console.error(error);
-                return
-            }
-            if (element.node == null) {
-                original.remove()
-            } else {
-                original.replaceWith(element.node)
-            }
+        add(element) {
             if (this._elements.has(element.id)) {
                 element.fail("duplicate id");
                 this._elements.get(element.id).fail("duplicate id")
             }
             this._elements.set(element.id, element);
             this._graph.getNode(element.id);
             for (let dep of element.dependencies) {
                 this._graph.addEdge(element.id, dep)
             }
-            element.flottplot = this;
-            return this
+            element.flottplot = this
         }
-        scan(root) {
-            let tag = Flottplot.tags.get(root.nodeName);
+        convert(node) {
+            const tag = Flottplot.tags.get(node.nodeName);
             if (tag == null || tag.isRecursive) {
-                let children = Array.from(root.childNodes);
-                for (let child of children) {
-                    this.scan(child)
+                const children = Array.from(node.childNodes);
+                for (const child of children) {
+                    this.convert(child)
                 }
             }
-            if (tag != null) {
-                this.convert(root)
+            if (tag == null || tag.Class == null) {
+                return
             }
-            return this
+            let element;
+            try {
+                element = tag.Class.from(node)
+            } catch (error) {
+                if (!(error instanceof FlottplotError)) {
+                    throw error
+                }
+                node.replaceWith(dom.newNode("div", {
+                    style: "border:3px solid #F00;background-color:#FCC;padding:3px;"
+                }, [dom.newNode("b", {}, [error.constructor.name, ": "]), error.message]));
+                console.error(error);
+                return
+            }
+            if (element.node == null) {
+                node.remove()
+            } else {
+                node.replaceWith(element.node)
+            }
+            this.add(element)
         }
         initialize() {
             for (let id of this._graph.orderedNodes) {
                 let element = this._elements.get(id);
                 if (element == null) {
                     console.warn("flottplot element with id '" + id + "' does not exist");
                     continue
@@ -1536,25 +1716,25 @@
                     element.failWith(error);
                     console.error(error)
                 }
             }
             if (this.urlstate) {
                 let hash = window.location.hash.substring(1);
                 if (hash.length !== 0) {
-                    this._state = JSON.parse(window.atob(hash))
+                    this.state = JSON.parse(window.atob(hash))
                 }
             }
         }
         notify(source) {
             for (let target of this._graph.updateOrderedNodesOf(source)) {
                 let element = this._elements.get(target);
                 element.update(this._substitutionFor(element))
             }
             if (this.urlstate) {
-                window.location.hash = window.btoa(JSON.stringify(this._state))
+                window.location.hash = window.btoa(JSON.stringify(this.state))
             }
         }
         _substitutionFor(element) {
             let values = new Map;
             for (let dep of element.dependencies) {
                 let dep_element = this._elements.get(dep);
                 if (dep_element == null) {
@@ -1591,25 +1771,25 @@
                 return
             }
             let callable = this.bindings.get(event.key);
             if (callable != null) {
                 callable()
             }
         }
-        get _state() {
+        get state() {
             let out = {};
             for (let [id, element] of this._elements) {
                 if (id.startsWith("_")) continue;
                 let state = element.state;
                 if (state === undefined) continue;
                 out[id] = state
             }
             return out
         }
-        set _state(state) {
+        set state(state) {
             for (let id of this._graph.orderedNodes) {
                 if (!state.hasOwnProperty(id)) continue;
                 let element = this._elements.get(id);
                 element.state = state[id];
                 element.update(this._substitutionFor(element));
                 element.notify()
             }
@@ -1619,34 +1799,38 @@
                 Class: element,
                 isRecursive: recursive
             })
         }
     }
     Flottplot.tags = new Map;
     Flottplot.registerTag("fp-animation", FPAnimation, false);
+    Flottplot.registerTag("fp-controls", FPControls, false);
     Flottplot.registerTag("fp-bind", FPBind, false);
     Flottplot.registerTag("fp-button", FPButton, false);
     Flottplot.registerTag("fp-cursors", FPCursors, false);
+    Flottplot.registerTag("fp-calendar", FPCalendar, false);
+    Flottplot.registerTag("fp-frame", FPFrame, true);
     Flottplot.registerTag("fp-overlay", FPOverlay, false);
     Flottplot.registerTag("fp-plot", FPPlot, false);
     Flottplot.registerTag("fp-range", FPRange, false);
     Flottplot.registerTag("fp-select", FPSelect, false);
     Flottplot.registerTag("fp-stack", FPStack, true);
     Flottplot.registerTag("fp-state", FPState, false);
     Flottplot.registerTag("fp-text", FPText, true);
     Flottplot.registerTag("fp-video", FPVideo, false);
     return {
-        __version__: "2.1.0",
+        VERSION: "2.2.0",
         Flottplot: Flottplot,
         FPElement: FPElement,
         Value: Value,
         OptionsItems: OptionsItems,
         RangeItems: RangeItems,
         FlottplotError: FlottplotError,
         ElementError: ElementError,
         dom: dom
     }
 }();
 let fp = new flottplot.Flottplot;
 document.addEventListener("DOMContentLoaded", function() {
-    fp.scan(document).initialize()
+    fp.convert(document);
+    fp.initialize()
 });
```

## Comparing `flottplot-2.1.0.dist-info/RECORD` & `flottplot-2.2.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-flottplot/__init__.py,sha256=yJCykF9I8PQQlUQ9vsrdb_RzPSh0F-mZdo5t63dJOGY,97
-flottplot/__main__.py,sha256=Hj5VOfyT-GpZrU7oKjnWNXN8i-C5VvlrAHV14mkMKcE,4270
+flottplot/__init__.py,sha256=QJsgqzF86HFEljN3Is2nWaCBSuQzEOqjGKVMlnhMufA,97
+flottplot/__main__.py,sha256=cOgUzinWbcb43gClpK2-tJwQpw5CtYxsWFlbZ-c43yc,3809
 flottplot/assets.py,sha256=uWVjYN2nc-wHpbytGOVWyViMHvvgKgKdYh2HK6H4jzs,1712
 flottplot/convert.py,sha256=5_SCxmbMKnIwixQEzS2kC4B0Re30ScG89y9mpjp1zF4,3093
 flottplot/ipython.py,sha256=0dLkhc9kY1GapqfRIPj7U3Dkt1Q-XpT1QG0u3lUMPHE,1302
-flottplot/assets/flottplot-min.js,sha256=Fg2j-TUs3NgtHClQrtrR_3owrIz-rwZM3TpzqwAXijA,37068
-flottplot/assets/flottplot-scan-min.js,sha256=fx-0dfBh1znRwLxi-4oxa737UvJTV6S-DCmuThUZaOY,37188
+flottplot/assets/flottplot-min.js,sha256=jgtwHciEhMyWC5rr6lH6kSg8Vs73NyyIAtxNmru-aFI,41582
+flottplot/assets/flottplot-scan-min.js,sha256=e4KdmcvmtcPIDH2Fb1MPFQ9aLeXhLF7BOWAliZWdzN0,41708
 flottplot/assets/flottplot.css,sha256=TXCt1NftHLnO8qWegcgosxidbv6UnP38tbCIN7E9fj4,702
-flottplot-2.1.0.dist-info/METADATA,sha256=2J3DSBghox7ZYcEvhrCPz00oiR1QyrFrmbzf-5fQLDM,251
-flottplot-2.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-flottplot-2.1.0.dist-info/top_level.txt,sha256=8tpuK3Jt-CAxrw-ceg1AhvTvkqOVbs07hxm8F3QGSKk,10
-flottplot-2.1.0.dist-info/RECORD,,
+flottplot-2.2.0.dist-info/METADATA,sha256=9vPVKPHajT4s0p96MQTnZmnragPhw9JaBSdkJAVshtc,251
+flottplot-2.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+flottplot-2.2.0.dist-info/top_level.txt,sha256=8tpuK3Jt-CAxrw-ceg1AhvTvkqOVbs07hxm8F3QGSKk,10
+flottplot-2.2.0.dist-info/RECORD,,
```

