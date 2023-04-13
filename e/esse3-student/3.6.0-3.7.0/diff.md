# Comparing `tmp/esse3_student-3.6.0.tar.gz` & `tmp/esse3_student-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esse3_student-3.6.0.tar", max compression
+gzip compressed data, was "esse3_student-3.7.0.tar", max compression
```

## Comparing `esse3_student-3.6.0.tar` & `esse3_student-3.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-12-19 10:49:50.550756 esse3_student-3.6.0/LICENSE
--rw-r--r--   0        0        0        0 2022-12-19 10:49:50.546754 esse3_student-3.6.0/esse3_student/__init__.py
--rw-r--r--   0        0        0      103 2023-04-06 14:27:12.244058 esse3_student-3.6.0/esse3_student/__main__.py
--rw-r--r--   0        0        0    16169 2023-04-08 13:44:03.091663 esse3_student-3.6.0/esse3_student/cli.py
--rw-r--r--   0        0        0    15453 2023-04-08 13:45:53.721355 esse3_student-3.6.0/esse3_student/esse3_wrapper.py
--rw-r--r--   0        0        0     1774 2023-04-08 13:31:38.102107 esse3_student-3.6.0/esse3_student/primitives.py
--rw-r--r--   0        0        0        0 2023-01-17 09:15:01.604898 esse3_student-3.6.0/esse3_student/tui/__init__.py
--rw-r--r--   0        0        0    10284 2023-04-09 13:42:37.495211 esse3_student-3.6.0/esse3_student/tui/booklet.py
--rw-r--r--   0        0        0     5016 2023-04-09 13:41:54.009478 esse3_student-3.6.0/esse3_student/tui/exams.py
--rw-r--r--   0        0        0     4442 2023-03-30 11:18:57.871585 esse3_student-3.6.0/esse3_student/tui/main.py
--rw-r--r--   0        0        0     6518 2023-04-09 13:41:53.949448 esse3_student-3.6.0/esse3_student/tui/reservations.py
--rw-r--r--   0        0        0     6652 2023-04-09 13:48:39.804275 esse3_student-3.6.0/esse3_student/tui/style.css
--rw-r--r--   0        0        0     2991 2023-04-09 13:44:45.875369 esse3_student-3.6.0/esse3_student/tui/taxes.py
--rw-r--r--   0        0        0        0 2022-12-19 10:49:50.542752 esse3_student-3.6.0/esse3_student/utils/__init__.py
--rw-r--r--   0        0        0      162 2022-12-19 10:49:50.542752 esse3_student-3.6.0/esse3_student/utils/console.py
--rw-r--r--   0        0        0     4668 2023-03-30 11:20:34.848047 esse3_student-3.6.0/esse3_student/utils/primitives.py
--rw-r--r--   0        0        0      991 2022-12-19 10:49:50.542752 esse3_student-3.6.0/esse3_student/utils/validators.py
--rw-r--r--   0        0        0      814 2023-04-09 14:31:43.073821 esse3_student-3.6.0/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 esse3_student-3.6.0/setup.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 esse3_student-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-19 10:49:50.550756 esse3_student-3.7.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-19 10:49:50.546754 esse3_student-3.7.0/esse3_student/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-06 14:27:12.244058 esse3_student-3.7.0/esse3_student/__main__.py
+-rw-r--r--   0        0        0    16187 2023-04-12 12:01:55.086064 esse3_student-3.7.0/esse3_student/cli.py
+-rw-r--r--   0        0        0    15453 2023-04-12 14:34:05.382235 esse3_student-3.7.0/esse3_student/esse3_wrapper.py
+-rw-r--r--   0        0        0     1774 2023-04-08 13:31:38.102107 esse3_student-3.7.0/esse3_student/primitives.py
+-rw-r--r--   0        0        0        0 2023-01-17 09:15:01.604898 esse3_student-3.7.0/esse3_student/tui/__init__.py
+-rw-r--r--   0        0        0    10284 2023-04-09 13:42:37.495211 esse3_student-3.7.0/esse3_student/tui/booklet.py
+-rw-r--r--   0        0        0     5016 2023-04-09 13:41:54.009478 esse3_student-3.7.0/esse3_student/tui/exams.py
+-rw-r--r--   0        0        0     4442 2023-03-30 11:18:57.871585 esse3_student-3.7.0/esse3_student/tui/main.py
+-rw-r--r--   0        0        0     6518 2023-04-12 14:32:09.278233 esse3_student-3.7.0/esse3_student/tui/reservations.py
+-rw-r--r--   0        0        0     6652 2023-04-09 13:48:39.804275 esse3_student-3.7.0/esse3_student/tui/style.css
+-rw-r--r--   0        0        0     2991 2023-04-09 13:44:45.875369 esse3_student-3.7.0/esse3_student/tui/taxes.py
+-rw-r--r--   0        0        0        0 2022-12-19 10:49:50.542752 esse3_student-3.7.0/esse3_student/utils/__init__.py
+-rw-r--r--   0        0        0      162 2022-12-19 10:49:50.542752 esse3_student-3.7.0/esse3_student/utils/console.py
+-rw-r--r--   0        0        0     4668 2023-03-30 11:20:34.848047 esse3_student-3.7.0/esse3_student/utils/primitives.py
+-rw-r--r--   0        0        0      991 2022-12-19 10:49:50.542752 esse3_student-3.7.0/esse3_student/utils/validators.py
+-rw-r--r--   0        0        0      814 2023-04-12 14:32:44.850233 esse3_student-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 esse3_student-3.7.0/setup.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 esse3_student-3.7.0/PKG-INFO
```

### Comparing `esse3_student-3.6.0/LICENSE` & `esse3_student-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/cli.py` & `esse3_student-3.7.0/esse3_student/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             metavar="Reservations name",
             help="[bold]One or more strings of the form. Example: remove 'name_1' 'name_2'"
         ),
 
 ):
 
     """
-    [bold][#E1C699]Operation that allows the [red]deletion[/red] of booked examinations[/][/bold] :wastebasket:
+    [bold][#E1C699]Operation to [red]cancel[/red] exam reservations[/][/bold] :wastebasket:
     """
 
     def parse(names: list) -> list[ExamName]:
         try:
             exams_list = [ExamName(v) for v in names]
         except ValueError:
             console.print("[bold yellow]Invalid strings[/]")
@@ -245,15 +245,15 @@
         exam_status: str = typer.Option(str, help="[bold][green]'passed'[/green] or [yellow]'to be done'[/yellow]"),
         exam_grade: int = typer.Option(int, help="[bold]Grade of the exam (from 18 to 30)"),
         new_average: Tuple[int, str] = typer.Option((None, None), help="[bold]Plan a new average: '25 12' (grade cfu)"),
         statistics: Optional[bool] = typer.Option(False, "--statistics", "-s", help="[bold]Show statistics on the actual averages"),
 ) -> None:
 
     """
-    [bold][#E1C699]shows all the student's activities[/][/bold] :bookmark_tabs:
+    [bold][#E1C699]Shows all the student's activities[/][/bold] :bookmark_tabs:
     """
 
     if academic_year:
         try:
             academic_year = AcademicYear(academic_year)
         except ValueError:
             console.print("[bold yellow]Invalid year[/]")
@@ -364,15 +364,15 @@
 @app.command(name="taxes")
 def command_taxes(
         payment: str = typer.Option(str, help="[bold]Shows taxes by status type: ('to pay'|'confirmed'|'refund')"),
         year: int = typer.Option(int, "--year", "-y", help="[bold]Filter taxes by year; es: 2021"),
 ) -> None:
 
     """
-    [bold][#E1C699]Show all taxes[/][/bold] :bookmark_tabs:
+    [bold][#E1C699]Show taxes list[/][/bold] :bookmark_tabs:
     """
 
     if year:
         try:
             year = Year(year).value
         except ValueError:
             console.print("Invalid year value")
@@ -394,16 +394,17 @@
         names = {" pagato confermato": "payment confirmed", " non pagato": "to pay", " pagato": "refund"}
         return names[payment_status], colors[payment_status]
 
     for index, (id, date, amount, status) in enumerate(track(taxes, description="[bold]Processing....[/]", transient=True), start=1):
         id, date, amount, status = map(lambda x: x.value, (id, date, amount, status))
         payment_status, c = payment_changes(status)
 
-        if payment in payment_status and str(year) in date:
-            table.add_row(str(index), id, date, f'[{c}]{amount}[/{c}]', payment_status)
+        if payment and year:
+            if payment in payment_status and str(year) in date:
+                table.add_row(str(index), id, date, f'[{c}]{amount}[/{c}]', payment_status)
 
         elif payment:
             if payment in payment_status:
                 table.add_row(str(index), id, date, f'[{c}]{amount}[/{c}]', payment_status)
 
         elif year:
             if str(year) in date:
```

### Comparing `esse3_student-3.6.0/esse3_student/esse3_wrapper.py` & `esse3_student-3.7.0/esse3_student/esse3_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,21 +185,21 @@
 
         index = 2
         for reservation in reservations:
             name = reservation.find_element(By.XPATH,
                                             f"/html/body/div[2]/div/div/main/div[3]/div/div/div/div[{index}]/h2").text
             start = name.find(" [")
             name = name[:start]
-            dict = {"Name": name}
+            dict = {"Nome": name}
             elements = reservation.find_elements(By.XPATH, "./dl/dt")
             for position, element in enumerate(elements, start=1):
                 key = element.text
                 value = element.find_element(By.XPATH, f"../dd[{position}]").text
                 if position == 1:
-                    dict["Date"] = key
+                    dict["Data"] = key
                 elif key != "Riservato per" and key != "Data Prenotazione" and key != '':
                     dict[key] = value
             rows.append(dict)
             index += 2
 
         return rows
```

### Comparing `esse3_student-3.6.0/esse3_student/primitives.py` & `esse3_student-3.7.0/esse3_student/primitives.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/tui/booklet.py` & `esse3_student-3.7.0/esse3_student/tui/booklet.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/tui/exams.py` & `esse3_student-3.7.0/esse3_student/tui/exams.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/tui/main.py` & `esse3_student-3.7.0/esse3_student/tui/main.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/tui/reservations.py` & `esse3_student-3.7.0/esse3_student/tui/reservations.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/tui/style.css` & `esse3_student-3.7.0/esse3_student/tui/style.css`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/tui/taxes.py` & `esse3_student-3.7.0/esse3_student/tui/taxes.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/utils/primitives.py` & `esse3_student-3.7.0/esse3_student/utils/primitives.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/esse3_student/utils/validators.py` & `esse3_student-3.7.0/esse3_student/utils/validators.py`

 * *Files identical despite different names*

### Comparing `esse3_student-3.6.0/pyproject.toml` & `esse3_student-3.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esse3-student"
-version = "3.6.0"
+version = "3.7.0"
 description = "Esse3 command line utility"
 authors = ["Antonio Pallaria <pallaria98@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 xdotool = { version = "^0.4.0", python = ">=3.10,<4.0" }
 typer = "^0.6.1"
```

### Comparing `esse3_student-3.6.0/setup.py` & `esse3_student-3.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'webdriver-manager>=3.8.3,<4.0.0']
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "4.0"': ['xdotool>=0.4.0,<0.5.0']}
 
 setup_kwargs = {
     'name': 'esse3-student',
-    'version': '3.6.0',
+    'version': '3.7.0',
     'description': 'Esse3 command line utility',
     'long_description': 'None',
     'author': 'Antonio Pallaria',
     'author_email': 'pallaria98@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `esse3_student-3.6.0/PKG-INFO` & `esse3_student-3.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esse3-student
-Version: 3.6.0
+Version: 3.7.0
 Summary: Esse3 command line utility
 Author: Antonio Pallaria
 Author-email: pallaria98@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

