# Comparing `tmp/mxcurpy-0.1.4.tar.gz` & `tmp/mxcurpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcurpy-0.1.4.tar", max compression
+gzip compressed data, was "mxcurpy-0.2.0.tar", max compression
```

## Comparing `mxcurpy-0.1.4.tar` & `mxcurpy-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-03-31 05:07:49.031007 mxcurpy-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1245 2023-04-01 15:32:48.658289 mxcurpy-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-04-01 15:47:37.320336 mxcurpy-0.1.4/mxcurpy/__init__.py
--rw-r--r--   0        0        0     3969 2023-03-31 19:32:03.902884 mxcurpy-0.1.4/mxcurpy/curp.py
--rw-r--r--   0        0        0     1651 2023-03-26 21:57:58.476650 mxcurpy-0.1.4/mxcurpy/non_convenient_words.py
--rw-r--r--   0        0        0     1684 2023-04-01 15:47:27.371810 mxcurpy-0.1.4/mxcurpy/states.py
--rw-r--r--   0        0        0     1514 2023-03-31 19:31:41.168453 mxcurpy-0.1.4/mxcurpy/utils.py
--rw-r--r--   0        0        0      472 2023-04-01 15:47:40.334967 mxcurpy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1915 2023-04-01 15:47:44.674558 mxcurpy-0.1.4/setup.py
--rw-r--r--   0        0        0     1936 2023-04-01 15:47:44.674732 mxcurpy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-31 05:07:49.031007 mxcurpy-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2484 2023-04-13 04:40:53.781448 mxcurpy-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-01 15:47:37.320336 mxcurpy-0.2.0/mxcurpy/__init__.py
+-rw-r--r--   0        0        0     3928 2023-04-05 05:46:27.033002 mxcurpy-0.2.0/mxcurpy/curp.py
+-rw-r--r--   0        0        0     2464 2023-04-12 05:28:21.336927 mxcurpy-0.2.0/mxcurpy/non_convenient_words.py
+-rw-r--r--   0        0        0     5162 2023-04-13 04:08:37.738603 mxcurpy-0.2.0/mxcurpy/rfc.py
+-rw-r--r--   0        0        0     1684 2023-04-02 20:23:30.022770 mxcurpy-0.2.0/mxcurpy/states.py
+-rw-r--r--   0        0        0     1645 2023-04-13 04:07:38.049352 mxcurpy-0.2.0/mxcurpy/utils.py
+-rw-r--r--   0        0        0      472 2023-04-13 04:17:57.018820 mxcurpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3181 2023-04-13 04:41:40.938459 mxcurpy-0.2.0/setup.py
+-rw-r--r--   0        0        0     3175 2023-04-13 04:41:40.938655 mxcurpy-0.2.0/PKG-INFO
```

### Comparing `mxcurpy-0.1.4/LICENSE.txt` & `mxcurpy-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.1.4/mxcurpy/curp.py` & `mxcurpy-0.2.0/mxcurpy/curp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""MXCURPY
+"""CURP
 
 Esta biblioteca te ayudará a calcular el CURP (Clave Única de Registro de
 Población de México) y el RFC (Registro Federal de Conritbuyente).
 
 Notas
 ----
 Los únicos datos que no podemos calcular son el dígito
@@ -86,26 +86,27 @@
     sex
         Es el sexo de la persona, acepta 'H' o 'h' para hombres y 'M' o 'm' para mujeres.
     Returns
     -------
     bool
         True if successful, False otherwise.
     """
-    print(clean_and_format_string(lastname))
+
     alphabetic_chars = _generate_first_part(names, lastname, second_lastname)
     first_part = f"{_replace_exceptions_curp(alphabetic_chars)}{_generate_numeric_part(birth_date)}"
 
     if sex not in ("h", "H", "m", "M"):
         raise "Sex formatting is incorrect, must be an 'h' form men or a 'm' for women"
 
     # 1. Primera Consonante interna del apellido paterno
     # 2. Primera Consonante interna del apellido materno
     # 3. Primera Consonante interna del nombre
     state_code = States.get_code(birth_state)
     fic_last_name = get_first_internal_consonant(lastname)
     fic_second_last_name = get_first_internal_consonant(second_lastname)
     fic_name = get_first_internal_consonant(names)
 
-    # Los últimos 2 caracteres son el dígito verificador, generados más o menos aleatoriamente al momento de la creación del CURP
+    # Los últimos 2 caracteres son el dígito verificador, generados más o menos aleatoriamente
+    # al momento de la creación del CURP
     # por la entidad encargada de ello. No podemos calcularlos, por lo que devolvemos 00.
 
     return f"{first_part}{sex}{state_code}{fic_last_name}{fic_second_last_name}{fic_name}00".upper()
```

### Comparing `mxcurpy-0.1.4/mxcurpy/states.py` & `mxcurpy-0.2.0/mxcurpy/states.py`

 * *Files identical despite different names*

### Comparing `mxcurpy-0.1.4/mxcurpy/utils.py` & `mxcurpy-0.2.0/mxcurpy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 
 
 def replace_accented_char(letter):
     """Devuelve un carácter acentuado sin el acento"""
     return ACCENTED_VOWELS.get(letter, letter)
 
 
-def clean_and_format_string(text):
+def clean_and_format_string(text, preserve_spaces=False):
     """Elimina símbolos, espacios y devuelve la cadena en minúsculas, todas las demás
     cadenas de este paquete dependen de recibir la función
     """
     text = text.lower()
     text = [replace_accented_char(c) for c in text]
-    text = "".join([c for c in text if c in LETTERS])
+    if preserve_spaces:
+        text = "".join([c for c in text if c in LETTERS or c == " "])
+    else:
+        text = "".join([c for c in text if c in LETTERS])
     return text
 
 
 @cleaned_string
 def get_first_consonant(text):
     """Extrae la primera consonate de un texto"""
     for c in text:
```

