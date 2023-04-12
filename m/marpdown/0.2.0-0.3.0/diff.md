# Comparing `tmp/marpdown-0.2.0.tar.gz` & `tmp/marpdown-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marpdown-0.2.0.tar", last modified: Wed Apr 12 15:35:43 2023, max compression
+gzip compressed data, was "marpdown-0.3.0.tar", last modified: Wed Apr 12 22:08:26 2023, max compression
```

## Comparing `marpdown-0.2.0.tar` & `marpdown-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:43.300639 marpdown-0.2.0/
--rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      404 2023-04-12 15:35:43.299638 marpdown-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:43.289650 marpdown-0.2.0/marpdown/
--rw-rw-rw-   0        0        0       83 2023-04-12 14:41:19.000000 marpdown-0.2.0/marpdown/__init__.py
--rw-rw-rw-   0        0        0     2138 2023-04-12 15:33:58.000000 marpdown-0.2.0/marpdown/css.py
--rw-rw-rw-   0        0        0     2545 2023-04-12 15:26:33.000000 marpdown-0.2.0/marpdown/ppt.py
--rw-rw-rw-   0        0        0     1518 2023-04-12 15:20:25.000000 marpdown-0.2.0/marpdown/slide.py
--rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.2.0/marpdown/writer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:43.297652 marpdown-0.2.0/marpdown.egg-info/
--rw-rw-rw-   0        0        0      404 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 15:35:43.000000 marpdown-0.2.0/marpdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 15:35:43.300639 marpdown-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-04-12 15:35:28.000000 marpdown-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:08:26.405893 marpdown-0.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-04-12 22:08:26.405893 marpdown-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 22:08:26.395701 marpdown-0.3.0/marpdown/
+-rw-rw-rw-   0        0        0      124 2023-04-12 22:07:50.000000 marpdown-0.3.0/marpdown/__init__.py
+-rw-rw-rw-   0        0        0     3095 2023-04-12 22:07:50.000000 marpdown-0.3.0/marpdown/css.py
+-rw-rw-rw-   0        0        0     2545 2023-04-12 15:26:33.000000 marpdown-0.3.0/marpdown/ppt.py
+-rw-rw-rw-   0        0        0     3404 2023-04-12 22:07:50.000000 marpdown-0.3.0/marpdown/slide.py
+-rw-rw-rw-   0        0        0      250 2023-04-12 22:07:50.000000 marpdown-0.3.0/marpdown/utils.py
+-rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.3.0/marpdown/writer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:08:26.403891 marpdown-0.3.0/marpdown.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-04-12 22:08:26.000000 marpdown-0.3.0/marpdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-12 22:08:26.000000 marpdown-0.3.0/marpdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 22:08:26.000000 marpdown-0.3.0/marpdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 22:08:26.000000 marpdown-0.3.0/marpdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 22:08:26.406894 marpdown-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-04-12 22:08:22.000000 marpdown-0.3.0/setup.py
```

### Comparing `marpdown-0.2.0/LICENSE` & `marpdown-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marpdown-0.2.0/marpdown/ppt.py` & `marpdown-0.3.0/marpdown/ppt.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.2.0/marpdown/slide.py` & `marpdown-0.3.0/marpdown/slide.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from .writer import Writer
+from . import  utils
 
 class BaseSlide:
     def __init__(self,*,content:str='',backgroundImage: str = None, ):
         self.content = content
         self.bgimage = backgroundImage
 
+
 class TOCSlide(BaseSlide):
     def __init__(self, title: str, toc: list[str],focus = -1,backgroundImage: str = None):
         self.toc = toc
         content = f'''# {title}\n\n'''
         if focus == -1:
             tmp = [f'''### {i+1}. {t}''' for i,t in enumerate(toc)]
             content += '\n'.join(tmp)
@@ -27,8 +30,44 @@
                         <div class="timeline-marker"></div>
                         <div class="timeline-content">
                           <h4>{name}</h4>
                           {detail}
                         </div></li>'''
         content += '</ul>'
 
-        super().__init__(content=content, backgroundImage=backgroundImage)
+        super().__init__(content=content, backgroundImage=backgroundImage)
+
+class BoxlineSlide(BaseSlide):
+    def __init__(self, *, title: str,boxlines:list[str] ,backgroundImage: str = None):
+        self.__writer__ = Writer()
+        self.__writer__.append(f"# {title}")
+        self.__writer__.append('<ul class="boxline">')
+
+        for i,box in enumerate(boxlines):
+            self.__writer__.append(f'''<li class="boxline-item">
+    <div class="boxline-marker">{i+1}</div>
+    <div class="boxline-content"><h2>{box}</h2></div>
+  </li>''')
+        self.__writer__.append('</ul>')
+        super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
+
+class CardSlide(BaseSlide):
+    def __init__(self, *, title: str,cards: list[tuple[str,list[str]]] ,backgroundImage: str = None):
+        self.__writer__ = Writer()
+        self.__writer__.append(f"# {title}")
+        self.__writer__.append('<div class="card-container">')
+        for card in cards:
+            name,bulletpoints = card
+            self.__writer__.append(f'''<div class="card">
+    <h2>{name}</h2>
+    <p>
+      {utils.list_to_html_ul(bulletpoints)}
+    </p>
+  </div>''')
+        self.__writer__.append('</div>')
+        super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
+
+class ThanksSlide(BaseSlide):
+    def __init__(self, backgroundImage:str = None):
+        super().__init__(content='''<div style="display: flex; justify-content: center; align-items: center; height: 100vh; text-align: center;padding-left=200px">
+  <h1 style="margin: 0 auto;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Thanks for Attention! Any Questions?</h1>
+</div>''', backgroundImage=backgroundImage)
```

### Comparing `marpdown-0.2.0/marpdown/writer.py` & `marpdown-0.3.0/marpdown/writer.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.2.0/setup.py` & `marpdown-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
 
 ]
 
 setup(
     name="marpdown",
-    version="0.2.0",
+    version="0.3.0",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of RL algorithms",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/marpdown",
     packages=find_packages(),
```

