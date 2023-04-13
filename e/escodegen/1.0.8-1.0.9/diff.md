# Comparing `tmp/escodegen-1.0.8-py3-none-any.whl.zip` & `tmp/escodegen-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 20277 bytes, number of entries: 6
+Zip file size: 20251 bytes, number of entries: 6
 -rw-r--r--  2.0 fat       83 b- defN 20-Feb-02 00:00 escodegen/__init__.py
--rw-r--r--  2.0 fat    92046 b- defN 20-Feb-02 00:00 escodegen/escodegen.py
-?rw-r--r--  2.0 fat     1848 b- defN 20-Feb-02 00:00 escodegen-1.0.8.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 escodegen-1.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1340 b- defN 20-Feb-02 00:00 escodegen-1.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      467 b- defN 20-Feb-02 00:00 escodegen-1.0.8.dist-info/RECORD
-6 files, 95871 bytes uncompressed, 19435 bytes compressed:  79.7%
+-rw-r--r--  2.0 fat    91865 b- defN 20-Feb-02 00:00 escodegen/escodegen.py
+?rw-r--r--  2.0 fat     1848 b- defN 20-Feb-02 00:00 escodegen-1.0.9.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 escodegen-1.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1340 b- defN 20-Feb-02 00:00 escodegen-1.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      467 b- defN 20-Feb-02 00:00 escodegen-1.0.9.dist-info/RECORD
+6 files, 95690 bytes uncompressed, 19409 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: escodegen/__init__.py
 Comment: 
 
 Filename: escodegen/escodegen.py
 Comment: 
 
-Filename: escodegen-1.0.8.dist-info/METADATA
+Filename: escodegen-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: escodegen-1.0.8.dist-info/WHEEL
+Filename: escodegen-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: escodegen-1.0.8.dist-info/licenses/LICENSE
+Filename: escodegen-1.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: escodegen-1.0.8.dist-info/RECORD
+Filename: escodegen-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## escodegen/escodegen.py

```diff
@@ -1211,16 +1211,14 @@
             return join(result, self.generateStatement(stmt.declaration, bodyFlags))
         
         # export ExportClause[NoReference] FromClause 
         # export ExportClause 
         if stmt.specifiers:
             if len(stmt.specifiers) == 0:
                 result = join(result, '{' + space + '}')
-            elif stmt.specifiers[0].type == Syntax.ExportSpecifier:
-                result = join(result, self.generateExpression(stmt.specifiers[0], Precedence.Sequence, E_TTT))
             else:
                 result = join(result, '{')
                 
                 def fn(indent, *args, **kwargs):
                     nonlocal result
                     result.append(newline)
                     iz = len(stmt.specifiers)
```

## Comparing `escodegen-1.0.8.dist-info/METADATA` & `escodegen-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escodegen
-Version: 1.0.8
+Version: 1.0.9
 Summary: ECMAScript code generator
 Project-URL: Homepage, https://github.com/0o120/escodegen-python
 Author-email: 0x78 <contact@0x78.com>
 License-File: LICENSE
 Keywords: ast,ecmascript,escodegen,generate,generator,javascript
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `escodegen-1.0.8.dist-info/licenses/LICENSE` & `escodegen-1.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

