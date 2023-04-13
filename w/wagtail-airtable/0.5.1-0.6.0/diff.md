# Comparing `tmp/wagtail_airtable-0.5.1-py3-none-any.whl.zip` & `tmp/wagtail_airtable-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 26699 bytes, number of entries: 19
+Zip file size: 26819 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 wagtail_airtable/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 wagtail_airtable/apps.py
 -rw-r--r--  2.0 unx      719 b- defN 80-Jan-01 00:00 wagtail_airtable/forms.py
 -rw-r--r--  2.0 unx    32713 b- defN 80-Jan-01 00:00 wagtail_airtable/management/commands/import_airtable.py
 -rw-r--r--  2.0 unx      856 b- defN 80-Jan-01 00:00 wagtail_airtable/management/commands/reset_local_airtable_records.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 wagtail_airtable/migrations/__init__.py
--rw-r--r--  2.0 unx    14568 b- defN 80-Jan-01 00:00 wagtail_airtable/mixins.py
+-rw-r--r--  2.0 unx    14911 b- defN 80-Jan-01 00:00 wagtail_airtable/mixins.py
 -rw-r--r--  2.0 unx      738 b- defN 80-Jan-01 00:00 wagtail_airtable/serializers.py
 -rw-r--r--  2.0 unx     1395 b- defN 80-Jan-01 00:00 wagtail_airtable/templates/wagtail_airtable/airtable_import_listing.html
 -rw-r--r--  2.0 unx     3395 b- defN 80-Jan-01 00:00 wagtail_airtable/templates/wagtailsnippets/snippets/type_index.html
 -rw-r--r--  2.0 unx     1298 b- defN 80-Jan-01 00:00 wagtail_airtable/templatetags/wagtail_airtable_tags.py
 -rw-r--r--  2.0 unx     5916 b- defN 80-Jan-01 00:00 wagtail_airtable/tests.py
--rw-r--r--  2.0 unx     5320 b- defN 80-Jan-01 00:00 wagtail_airtable/utils.py
+-rw-r--r--  2.0 unx     5454 b- defN 80-Jan-01 00:00 wagtail_airtable/utils.py
 -rw-r--r--  2.0 unx     5277 b- defN 80-Jan-01 00:00 wagtail_airtable/views.py
 -rw-r--r--  2.0 unx     1692 b- defN 80-Jan-01 00:00 wagtail_airtable/wagtail_hooks.py
--rw-r--r--  2.0 unx     6327 b- defN 80-Jan-01 00:00 wagtail_airtable-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wagtail_airtable-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx     1508 b- defN 80-Jan-01 00:00 wagtail_airtable-0.5.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx     1774 b- defN 16-Jan-01 00:00 wagtail_airtable-0.5.1.dist-info/RECORD
-19 files, 83690 bytes uncompressed, 23723 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx     6327 b- defN 80-Jan-01 00:00 wagtail_airtable-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wagtail_airtable-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1508 b- defN 80-Jan-01 00:00 wagtail_airtable-0.6.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx     1774 b- defN 16-Jan-01 00:00 wagtail_airtable-0.6.0.dist-info/RECORD
+19 files, 84167 bytes uncompressed, 23843 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: wagtail_airtable/views.py
 Comment: 
 
 Filename: wagtail_airtable/wagtail_hooks.py
 Comment: 
 
-Filename: wagtail_airtable-0.5.1.dist-info/METADATA
+Filename: wagtail_airtable-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: wagtail_airtable-0.5.1.dist-info/WHEEL
+Filename: wagtail_airtable-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: wagtail_airtable-0.5.1.dist-info/LICENSE
+Filename: wagtail_airtable-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: wagtail_airtable-0.5.1.dist-info/RECORD
+Filename: wagtail_airtable-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wagtail_airtable/mixins.py

```diff
@@ -1,8 +1,9 @@
 import sys
+from importlib import import_module
 from ast import literal_eval
 from logging import getLogger
 
 from airtable import Airtable
 from django.conf import settings
 from django.db import models
 from django.utils.functional import cached_property
@@ -299,15 +300,15 @@
             error_info = literal_eval(error_json)
             return {
                 "status_code": code,
                 "type": error_info["type"],
                 "message": error_info["message"],
             }
 
-    def save(self, *args, **kwargs):
+    def save_to_airtable(self, *args, **kwargs):
         """
         If there's an existing airtable record id, update the row.
         Otherwise attempt to create a new record.
         """
 
         # Save to database first so we get pk, in case it's used for uniqueness
         saved_model = super().save(*args, **kwargs)
@@ -339,17 +340,23 @@
                     error = self.parse_request_error(e.args[0])
                     message = (
                         f"Could not create Airtable record. Reason: {error['message']}"
                     )
                     logger.warning(message)
                     # Used in the `after_edit_page` hook. If it exists, an error message will be displayed.
                     self._airtable_update_error = message
-
         return saved_model
 
+    def save(self, *args, **kwargs):
+        if getattr(settings, "WAGTAIL_AIRTABLE_SAVE_SYNC", True):
+            # If WAGTAIL_AIRTABLE_SAVE_SYNC is set to True we do it the synchronous way
+            return self.save_to_airtable(*args, **kwargs)
+
+        return super().save(*args, **kwargs)
+
     def delete(self, *args, **kwargs):
         self.setup_airtable()
         if self.push_to_airtable and self._push_to_airtable and self.airtable_record_id:
             # Try to delete the record from the Airtable.
             self.delete_record()
         return super().delete(*args, **kwargs)
```

## wagtail_airtable/utils.py

```diff
@@ -135,14 +135,19 @@
 
 def airtable_message(request, instance, message="Airtable record updated", button_text="View record in Airtable", buttons_enabled=True) -> None:
     """
     Common message handler for Wagtail hooks.
 
     Supports a custom message, custom button text, and the ability to disable buttons entirely (use case: deleting a record)
     """
+    custom_message = getattr(settings, "WAGTAIL_AIRTABLE_PUSH_MESSAGE", '')
+
+    if custom_message:
+        message = custom_message
+
     if hasattr(instance, "_airtable_update_error"):
         messages.error(request, message=instance._airtable_update_error)
     else:
         buttons = None
         if buttons_enabled and instance.get_record_usage_url():
             buttons = [
                 messages.button(instance.get_record_usage_url(), button_text, True)
```

## Comparing `wagtail_airtable-0.5.1.dist-info/METADATA` & `wagtail_airtable-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-airtable
-Version: 0.5.1
+Version: 0.6.0
 Summary: Sync data between Wagtail and Airtable
 Home-page: https://github.com/wagtail/wagtail-airtable
 Keywords: wagtail,airtable
 Author: Kalob Taulien
 Author-email: kalob.taulien@torchbox.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
```

## Comparing `wagtail_airtable-0.5.1.dist-info/LICENSE` & `wagtail_airtable-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wagtail_airtable-0.5.1.dist-info/RECORD` & `wagtail_airtable-0.6.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 wagtail_airtable/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wagtail_airtable/apps.py,sha256=UJ9BT5MzT8FPVXH-kvsA7wxHp2sPkQoTCe085oIyy4k,106
 wagtail_airtable/forms.py,sha256=i0ZSIPhSlzNQCGNn4rpn4RTbVU7fI2Ciymsy81xMqFI,719
 wagtail_airtable/management/commands/import_airtable.py,sha256=d7CszU6DNi7HCE4jP3x-_m3uSkvvlxSMXuyujJl2eSg,32713
 wagtail_airtable/management/commands/reset_local_airtable_records.py,sha256=hEjbVQVVe_gPbLrprfvJYXxGzbEoM2b-ZKJVv7kHBXk,856
 wagtail_airtable/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-wagtail_airtable/mixins.py,sha256=RjFK2dAzKZ8W5ABFrJJFtUWeju608zTiGGCq_e1UKPs,14568
+wagtail_airtable/mixins.py,sha256=Wnolml5H_djA34juXjW8cpc2T7SJTNbJcXdfZWHNNo0,14911
 wagtail_airtable/serializers.py,sha256=TE7hqegG7l6AOO0CYvDIingvvJm82rxv_D3n3mm2H1Q,738
 wagtail_airtable/templates/wagtail_airtable/airtable_import_listing.html,sha256=pygYa0mOo4j-l8tjsBqC6jTRv1ndRe-ap33MjFV9Fu0,1395
 wagtail_airtable/templates/wagtailsnippets/snippets/type_index.html,sha256=Ok8cXWvFEjTtYGMN1x4NZAa8ioEYyejYz-oiErAMv9E,3395
 wagtail_airtable/templatetags/wagtail_airtable_tags.py,sha256=rYuSgeAnOxL1SiIjDiEoDIheSQo_3DQyQMDbiT3kD7c,1298
 wagtail_airtable/tests.py,sha256=xJV7o40-fmFAkuZHz4UZ6Ih9LPY4Igyy-XDjLKxZfSM,5916
-wagtail_airtable/utils.py,sha256=_4OQH7kD_Za7u-ar1OwegWkZkLBum8YBgZ80NcoWsEc,5320
+wagtail_airtable/utils.py,sha256=ym2PkrqwjO2szCak5_CUFGiH7COS1Y-QBIQv4yJHd5Q,5454
 wagtail_airtable/views.py,sha256=4w6MTk_5kqlxIyIi1SFjufyDHsHWJbig5FUsy4u59Zg,5277
 wagtail_airtable/wagtail_hooks.py,sha256=HRJOYn0RaG-NRTYsKViDZ01NMX3gtMw8cRnTZthDnIk,1692
-wagtail_airtable-0.5.1.dist-info/METADATA,sha256=dS9vrdNb3seD9iaaLP431wkHfFAvuEk4xNycBoZYgJo,6327
-wagtail_airtable-0.5.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-wagtail_airtable-0.5.1.dist-info/LICENSE,sha256=DmoAH0hWDG_F6Pa2pvpg3xdL2ur-iKDzIAe96vhfzWs,1508
-wagtail_airtable-0.5.1.dist-info/RECORD,,
+wagtail_airtable-0.6.0.dist-info/METADATA,sha256=FuwHGmUYmLH5ksT7KLreckvzczB5vj1DA0AxKgpNHto,6327
+wagtail_airtable-0.6.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+wagtail_airtable-0.6.0.dist-info/LICENSE,sha256=DmoAH0hWDG_F6Pa2pvpg3xdL2ur-iKDzIAe96vhfzWs,1508
+wagtail_airtable-0.6.0.dist-info/RECORD,,
```

