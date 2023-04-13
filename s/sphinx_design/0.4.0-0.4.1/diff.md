# Comparing `tmp/sphinx_design-0.4.0.tar.gz` & `tmp/sphinx_design-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_design-0.4.0.tar", last modified: Thu Apr 13 09:20:02 2023, max compression
+gzip compressed data, was "sphinx_design-0.4.1.tar", last modified: Thu Apr 13 09:30:53 2023, max compression
```

## Comparing `sphinx_design-0.4.0.tar` & `sphinx_design-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2889 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2081 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/.gitignore
--rw-r--r--   0        0        0     1224 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/.readthedocs.yml
--rw-r--r--   0        0        0     7841 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1099 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/LICENSE
--rw-r--r--   0        0        0     3114 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/README.md
--rw-r--r--   0        0        0      162 2023-04-13 09:19:58.169975 sphinx_design-0.4.0/codecov.yml
--rwxr-xr-x   0        0        0      214 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/git_rebase_theme_branches.sh
--rw-r--r--   0        0        0    11363 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/package-lock.json
--rw-r--r--   0        0        0      302 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/package.json
--rw-r--r--   0        0        0     2145 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      433 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/__init__.py
--rw-r--r--   0        0        0      722 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/_compat.py
--rw-r--r--   0        0        0     6410 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/article_info.py
--rw-r--r--   0        0        0     8252 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/badges_buttons.py
--rw-r--r--   0        0        0    10316 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/cards.py
--rw-r--r--   0        0        0        0 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/compiled/__init__.py
--rw-r--r--   0        0        0      577 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/compiled/material-icons_LICENSE
--rw-r--r--   0        0        0      106 2023-04-13 09:19:58.173976 sphinx_design-0.4.0/sphinx_design/compiled/material-icons_VERSION.txt
--rw-r--r--   0        0        0  1613646 2023-04-13 09:19:58.193976 sphinx_design-0.4.0/sphinx_design/compiled/material_outlined.json
--rw-r--r--   0        0        0  1504323 2023-04-13 09:19:58.197976 sphinx_design-0.4.0/sphinx_design/compiled/material_regular.json
--rw-r--r--   0        0        0  2003117 2023-04-13 09:19:58.205976 sphinx_design-0.4.0/sphinx_design/compiled/material_round.json
--rw-r--r--   0        0        0  1370513 2023-04-13 09:19:58.205976 sphinx_design-0.4.0/sphinx_design/compiled/material_sharp.json
--rw-r--r--   0        0        0  1995382 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/compiled/material_twotone.json
--rw-r--r--   0        0        0     1068 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/compiled/octicon_LICENSE
--rw-r--r--   0        0        0   277166 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/compiled/octicons.json
--rw-r--r--   0        0        0      770 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/compiled/sd_tabs.js
--rw-r--r--   0        0        0    48417 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/compiled/style.min.css
--rw-r--r--   0        0        0     7822 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/dropdown.py
--rw-r--r--   0        0        0     5614 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/extension.py
--rw-r--r--   0        0        0     9771 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/grids.py
--rw-r--r--   0        0        0    10620 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/icons.py
--rw-r--r--   0        0        0       26 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/py.typed
--rw-r--r--   0        0        0     3117 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/shared.py
--rw-r--r--   0        0        0     9681 2023-04-13 09:19:58.209976 sphinx_design-0.4.0/sphinx_design/tabs.py
--rw-r--r--   0        0        0     2103 2023-04-13 09:19:58.213976 sphinx_design-0.4.0/tox.ini
--rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 sphinx_design-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2889 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2081 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1224 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.readthedocs.yml
+-rw-r--r--   0        0        0     7841 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1099 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3114 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/README.md
+-rw-r--r--   0        0        0      162 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/codecov.yml
+-rwxr-xr-x   0        0        0      214 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/git_rebase_theme_branches.sh
+-rw-r--r--   0        0        0    11363 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/package-lock.json
+-rw-r--r--   0        0        0      302 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/package.json
+-rw-r--r--   0        0        0     2145 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/__init__.py
+-rw-r--r--   0        0        0      722 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/_compat.py
+-rw-r--r--   0        0        0     6410 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/article_info.py
+-rw-r--r--   0        0        0     8252 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/badges_buttons.py
+-rw-r--r--   0        0        0    10377 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/cards.py
+-rw-r--r--   0        0        0        0 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/compiled/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/compiled/material-icons_LICENSE
+-rw-r--r--   0        0        0      106 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/compiled/material-icons_VERSION.txt
+-rw-r--r--   0        0        0  1613646 2023-04-13 09:30:50.538980 sphinx_design-0.4.1/sphinx_design/compiled/material_outlined.json
+-rw-r--r--   0        0        0  1504323 2023-04-13 09:30:50.538980 sphinx_design-0.4.1/sphinx_design/compiled/material_regular.json
+-rw-r--r--   0        0        0  2003117 2023-04-13 09:30:50.546980 sphinx_design-0.4.1/sphinx_design/compiled/material_round.json
+-rw-r--r--   0        0        0  1370513 2023-04-13 09:30:50.546980 sphinx_design-0.4.1/sphinx_design/compiled/material_sharp.json
+-rw-r--r--   0        0        0  1995382 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/material_twotone.json
+-rw-r--r--   0        0        0     1068 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/octicon_LICENSE
+-rw-r--r--   0        0        0   277166 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/octicons.json
+-rw-r--r--   0        0        0      770 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/sd_tabs.js
+-rw-r--r--   0        0        0    48417 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/style.min.css
+-rw-r--r--   0        0        0     7822 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/dropdown.py
+-rw-r--r--   0        0        0     5614 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/extension.py
+-rw-r--r--   0        0        0     9839 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/grids.py
+-rw-r--r--   0        0        0    10620 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/icons.py
+-rw-r--r--   0        0        0       26 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/py.typed
+-rw-r--r--   0        0        0     3117 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/shared.py
+-rw-r--r--   0        0        0     9681 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/tabs.py
+-rw-r--r--   0        0        0     2103 2023-04-13 09:30:50.554980 sphinx_design-0.4.1/tox.ini
+-rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 sphinx_design-0.4.1/PKG-INFO
```

### Comparing `sphinx_design-0.4.0/.github/workflows/ci.yml` & `sphinx_design-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/.gitignore` & `sphinx_design-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/.pre-commit-config.yaml` & `sphinx_design-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/CHANGELOG.md` & `sphinx_design-0.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/LICENSE` & `sphinx_design-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/README.md` & `sphinx_design-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/package-lock.json` & `sphinx_design-0.4.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/pyproject.toml` & `sphinx_design-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/_compat.py` & `sphinx_design-0.4.1/sphinx_design/_compat.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/article_info.py` & `sphinx_design-0.4.1/sphinx_design/article_info.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/badges_buttons.py` & `sphinx_design-0.4.1/sphinx_design/badges_buttons.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/cards.py` & `sphinx_design-0.4.1/sphinx_design/cards.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     option_spec = {
         "width": make_choice(["auto", "25%", "50%", "75%", "100%"]),
         "margin": margin_option,
         "text-align": text_align,
         "img-top": directives.uri,
         "img-bottom": directives.uri,
         "img-background": directives.uri,
+        "img-alt": directives.unchanged,
         "link": directives.uri,
         "link-type": make_choice(["url", "any", "ref", "doc"]),
         "link-alt": directives.unchanged,
         "shadow": make_choice(["none", "sm", "md", "lg"]),
         "class-card": directives.class_option,
         "class-header": directives.class_option,
         "class-body": directives.class_option,
@@ -92,33 +93,35 @@
             "card",
             card_classes
             + options.get("text-align", [])
             + options.get("class-card", []),
         )
         inst.set_source_info(card)
 
+        img_alt = options.get("img-alt") or ""
+
         container = card
         if "img-background" in options:
             card.append(
                 nodes.image(
                     uri=options["img-background"],
                     classes=["sd-card-img"],
-                    alt="background image",
+                    alt=img_alt,
                 )
             )
             overlay = create_component("card-overlay", ["sd-card-img-overlay"])
             inst.set_source_info(overlay)
             card += overlay
             container = overlay
 
         if "img-top" in options:
             image_top = nodes.image(
                 "",
                 uri=options["img-top"],
-                alt="card-img-top",
+                alt=img_alt,
                 classes=["sd-card-img-top"] + options.get("class-img-top", []),
             )
             container.append(image_top)
 
         components = cls.split_content(inst.content, inst.content_offset)
 
         if components.header:
@@ -152,15 +155,15 @@
                 )
             )
 
         if "img-bottom" in options:
             image_bottom = nodes.image(
                 "",
                 uri=options["img-bottom"],
-                alt="card-img-bottom",
+                alt=img_alt,
                 classes=["sd-card-img-bottom"] + options.get("class-img-bottom", []),
             )
             container.append(image_bottom)
 
         if "link" in options:
             link_container = PassthroughTextElement()
             _classes = ["sd-stretched-link"]
```

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/material-icons_LICENSE` & `sphinx_design-0.4.1/sphinx_design/compiled/material-icons_LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/material_outlined.json` & `sphinx_design-0.4.1/sphinx_design/compiled/material_outlined.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/material_regular.json` & `sphinx_design-0.4.1/sphinx_design/compiled/material_regular.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/material_round.json` & `sphinx_design-0.4.1/sphinx_design/compiled/material_round.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/material_sharp.json` & `sphinx_design-0.4.1/sphinx_design/compiled/material_sharp.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/material_twotone.json` & `sphinx_design-0.4.1/sphinx_design/compiled/material_twotone.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/octicon_LICENSE` & `sphinx_design-0.4.1/sphinx_design/compiled/octicon_LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/octicons.json` & `sphinx_design-0.4.1/sphinx_design/compiled/octicons.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/sd_tabs.js` & `sphinx_design-0.4.1/sphinx_design/compiled/sd_tabs.js`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/compiled/style.min.css` & `sphinx_design-0.4.1/sphinx_design/compiled/style.min.css`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/dropdown.py` & `sphinx_design-0.4.1/sphinx_design/dropdown.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/extension.py` & `sphinx_design-0.4.1/sphinx_design/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/grids.py` & `sphinx_design-0.4.1/sphinx_design/grids.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,15 @@
         "class-item": directives.class_option,
         # The options below must be sync'ed with CardDirective.option_spec (minus margin).
         "width": make_choice(["auto", "25%", "50%", "75%", "100%"]),
         "text-align": text_align,
         "img-background": directives.uri,
         "img-top": directives.uri,
         "img-bottom": directives.uri,
+        "img-alt": directives.unchanged,
         "link": directives.uri,
         "link-type": make_choice(["url", "any", "ref", "doc"]),
         "link-alt": directives.unchanged,
         "shadow": make_choice(["none", "sm", "md", "lg"]),
         "class-card": directives.class_option,
         "class-body": directives.class_option,
         "class-title": directives.class_option,
@@ -262,14 +263,15 @@
             if key
             in [
                 "width",
                 "text-align",
                 "img-background",
                 "img-top",
                 "img-bottom",
+                "img-alt",
                 "link",
                 "link-type",
                 "link-alt",
                 "shadow",
                 "class-card",
                 "class-body",
                 "class-title",
```

### Comparing `sphinx_design-0.4.0/sphinx_design/icons.py` & `sphinx_design-0.4.1/sphinx_design/icons.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/shared.py` & `sphinx_design-0.4.1/sphinx_design/shared.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/sphinx_design/tabs.py` & `sphinx_design-0.4.1/sphinx_design/tabs.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/tox.ini` & `sphinx_design-0.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.0/PKG-INFO` & `sphinx_design-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_design
-Version: 0.4.0
+Version: 0.4.1
 Summary: A sphinx extension for designing beautiful, view size responsive web components.
 Keywords: sphinx,extension,material design,web components
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
```

