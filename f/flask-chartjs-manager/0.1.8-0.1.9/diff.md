# Comparing `tmp/flask_chartjs_manager-0.1.8.tar.gz` & `tmp/flask_chartjs_manager-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_chartjs_manager-0.1.8.tar", max compression
+gzip compressed data, was "flask_chartjs_manager-0.1.9.tar", max compression
```

## Comparing `flask_chartjs_manager-0.1.8.tar` & `flask_chartjs_manager-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1804 2022-12-26 16:32:56.328787 flask_chartjs_manager-0.1.8/README.md
--rwxr-xr-x   0        0        0     1627 2022-12-26 16:57:05.601106 flask_chartjs_manager-0.1.8/flask_chartjs/__init__.py
--rwxr-xr-x   0        0        0     4289 2022-12-26 16:32:56.348786 flask_chartjs_manager-0.1.8/flask_chartjs/chart.py
--rwxr-xr-x   0        0        0      285 2022-12-26 16:32:56.379788 flask_chartjs_manager-0.1.8/flask_chartjs/templates/html.jinja
--rwxr-xr-x   0        0        0      454 2022-12-26 16:32:56.388787 flask_chartjs_manager-0.1.8/flask_chartjs/templates/js.jinja
--rwxr-xr-x   0        0        0      222 2022-12-26 17:26:03.367081 flask_chartjs_manager-0.1.8/flask_chartjs/templates/load_chartjs.jinja
--rwxr-xr-x   0        0        0      503 2022-12-26 17:26:49.274322 flask_chartjs_manager-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 flask_chartjs_manager-0.1.8/setup.py
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 flask_chartjs_manager-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1804 2022-12-26 16:32:56.328787 flask_chartjs_manager-0.1.9/README.md
+-rwxr-xr-x   0        0        0     1634 2022-12-26 17:27:37.732040 flask_chartjs_manager-0.1.9/flask_chartjs/__init__.py
+-rwxr-xr-x   0        0        0     4289 2022-12-26 16:32:56.348786 flask_chartjs_manager-0.1.9/flask_chartjs/chart.py
+-rwxr-xr-x   0        0        0      285 2022-12-26 16:32:56.379788 flask_chartjs_manager-0.1.9/flask_chartjs/templates/html.jinja
+-rwxr-xr-x   0        0        0      454 2022-12-26 16:32:56.388787 flask_chartjs_manager-0.1.9/flask_chartjs/templates/js.jinja
+-rwxr-xr-x   0        0        0      222 2022-12-26 17:26:03.367081 flask_chartjs_manager-0.1.9/flask_chartjs/templates/load_chartjs.jinja
+-rwxr-xr-x   0        0        0      503 2022-12-26 17:28:27.079672 flask_chartjs_manager-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 flask_chartjs_manager-0.1.9/setup.py
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 flask_chartjs_manager-0.1.9/PKG-INFO
```

### Comparing `flask_chartjs_manager-0.1.8/README.md` & `flask_chartjs_manager-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `flask_chartjs_manager-0.1.8/flask_chartjs/__init__.py` & `flask_chartjs_manager-0.1.9/flask_chartjs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         @app.context_processor
         def inject_context_variables() -> dict:
             return dict(load_chartjs=self._render_load_chartjs, render_chart=self._render_chart)
 
     def _render_load_chartjs(self) -> Markup:
         return Markup(render_template('load_chartjs.jinja'))
 
-    def _render_chart(self, chart: Chart, options: Dict[str, Any], html_only: bool = False,
+    def _render_chart(self, chart: Chart, options: Dict[str, Any] = None, html_only: bool = False,
                       js_only: bool = False, use_htmx: bool = False) -> Markup:
         html_str, js_str = '', ''
         if not js_only:
             html_str = render_template('html.jinja', chart=chart)
 
         if not html_only:
             js_str = render_template(
```

### Comparing `flask_chartjs_manager-0.1.8/flask_chartjs/chart.py` & `flask_chartjs_manager-0.1.9/flask_chartjs/chart.py`

 * *Files identical despite different names*

### Comparing `flask_chartjs_manager-0.1.8/setup.py` & `flask_chartjs_manager-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'flask_chartjs': ['templates/*']}
 
 install_requires = \
 ['flask>=2.2.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'flask-chartjs-manager',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# Flask-ChartJS\n\nFlask-ChartJS provides a simple interface to use ChartJS javascript library with Flask.\n\n## Installation\n\nInstall the extension with pip:\n\n```bash\npip install flask-chartjs-manager\n```\n\n## Usage\n\nOnce installed the Flask-ChartJS-Manager is easy to use.Let\'s walk through setting up a basic application. Also please note that this is a very basic guide: we will be taking shortcuts here that you should never take in a real application.\n\nTo begin we\'ll set up a Flask app:\n\n```python\nimport flask\n\napp = flask.Flask(__name__)\n```\n\nFlask-ChartJS works via a ChartJS object. To kick things off, we\'ll set up the chartjs manager by instantiating it and telling it about our Flask app:\n\n```python\nfrom flask_chartjs import ChartJSManager\n\nchartjs_manager = ChartJSManager()\nchartjs_manager.init_app(app)\n```\n\nThis will make available the `load_chartjs` function into the templates context so you could load the javascript package easily, like this.\n\n```html\n<head>\n  {{ load_chartjs() }}\n</head>\n```\n\nNow we will construct a basic chart.\n\n```python\nfrom flask_chartjs import Chart, DataSet\nfrom flask import render_template\n\n@app.get(\'/chart-example\')\ndef chart_example():\n    \n    chart = Chart(\'income-outcome\', \'bar\') # Requires at least an ID and a chart type.\n    \n    dataset_income = DataSet(\'Income\', [100,200,300])\n    dataset_outcome = DataSet(\'OutCome\', [50,100,150])\n    \n    chart.data.add_labels(\'jan\', \'feb\', \'mar\')\n    chart.data.add_dataset(dataset_income)\n    chart.data.add_dataset(dataset_outcome)\n\n    return render_template(\'path/to/template.html\', my_chart=chart)\n\n```\n\nOnce created you can pass it to a render_template and use it likewise.\n\n```html\n<!-- load_chartjs() must be called before this line -->\n<div class="my-classes">{{ render_chart(my_chart) }}</div>\n```\n',
     'author': 'Sebastian Salinas',
     'author_email': 'seba.salinas.delrio@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `flask_chartjs_manager-0.1.8/PKG-INFO` & `flask_chartjs_manager-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-chartjs-manager
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Sebastian Salinas
 Author-email: seba.salinas.delrio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

