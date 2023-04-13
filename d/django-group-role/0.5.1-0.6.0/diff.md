# Comparing `tmp/django-group-role-0.5.1.tar.gz` & `tmp/django-group-role-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-group-role-0.5.1.tar", last modified: Tue Apr  4 15:42:17 2023, max compression
+gzip compressed data, was "django-group-role-0.6.0.tar", last modified: Thu Apr 13 07:52:14 2023, max compression
```

## Comparing `django-group-role-0.5.1.tar` & `django-group-role-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-04 15:42:17.906584 django-group-role-0.5.1/
--rw-rw-r--   0 davide    (1000) davide    (1000)    11357 2021-11-22 11:09:44.000000 django-group-role-0.5.1/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-04-04 15:42:17.906584 django-group-role-0.5.1/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)     3888 2022-08-24 08:14:24.000000 django-group-role-0.5.1/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-04 15:42:17.906584 django-group-role-0.5.1/django_group_role/
--rw-rw-r--   0 davide    (1000) davide    (1000)      165 2023-04-04 15:40:56.000000 django-group-role-0.5.1/django_group_role/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      164 2021-11-19 10:35:10.000000 django-group-role-0.5.1/django_group_role/apps.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      151 2021-11-26 11:53:38.000000 django-group-role-0.5.1/django_group_role/exceptions.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-04 15:42:17.906584 django-group-role-0.5.1/django_group_role/management/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:23.000000 django-group-role-0.5.1/django_group_role/management/__init__.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-04 15:42:17.906584 django-group-role-0.5.1/django_group_role/management/commands/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:32.000000 django-group-role-0.5.1/django_group_role/management/commands/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2514 2022-12-27 08:47:22.000000 django-group-role-0.5.1/django_group_role/management/commands/populate_roles.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     6354 2022-12-27 09:45:38.000000 django-group-role-0.5.1/django_group_role/roles.py
--rw-rw-r--   0 davide    (1000) davide    (1000)       89 2022-08-24 08:05:10.000000 django-group-role-0.5.1/django_group_role/signals.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1014 2021-11-25 16:48:01.000000 django-group-role-0.5.1/django_group_role/test.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1594 2021-11-26 11:53:38.000000 django-group-role-0.5.1/django_group_role/utils.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-04 15:42:17.906584 django-group-role-0.5.1/django_group_role.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-04-04 15:42:17.000000 django-group-role-0.5.1/django_group_role.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      731 2023-04-04 15:42:17.000000 django-group-role-0.5.1/django_group_role.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-04-04 15:42:17.000000 django-group-role-0.5.1/django_group_role.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       35 2023-04-04 15:42:17.000000 django-group-role-0.5.1/django_group_role.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       18 2023-04-04 15:42:17.000000 django-group-role-0.5.1/django_group_role.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)     1742 2023-04-04 15:42:17.910584 django-group-role-0.5.1/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)       60 2021-11-19 10:29:59.000000 django-group-role-0.5.1/setup.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-04 15:42:17.906584 django-group-role-0.5.1/tests/
--rw-rw-r--   0 davide    (1000) davide    (1000)     9438 2023-04-04 15:25:30.000000 django-group-role-0.5.1/tests/test_command.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1334 2021-12-01 11:53:23.000000 django-group-role-0.5.1/tests/test_configuration.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1794 2023-04-04 15:25:30.000000 django-group-role-0.5.1/tests/test_database.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2888 2022-12-27 09:45:38.000000 django-group-role-0.5.1/tests/test_definitions.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     3374 2023-04-04 15:25:30.000000 django-group-role-0.5.1/tests/test_testing_utils.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     4218 2021-12-14 10:07:28.000000 django-group-role-0.5.1/tests/test_utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.640677 django-group-role-0.6.0/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11357 2021-11-22 11:09:44.000000 django-group-role-0.6.0/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-04-13 07:52:14.640677 django-group-role-0.6.0/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3888 2022-08-24 08:14:24.000000 django-group-role-0.6.0/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.632677 django-group-role-0.6.0/django_group_role/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      729 2023-04-13 07:36:23.000000 django-group-role-0.6.0/django_group_role/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      164 2023-04-12 15:35:54.000000 django-group-role-0.6.0/django_group_role/apps.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      151 2021-11-26 11:53:38.000000 django-group-role-0.6.0/django_group_role/exceptions.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.636677 django-group-role-0.6.0/django_group_role/management/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:23.000000 django-group-role-0.6.0/django_group_role/management/__init__.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.636677 django-group-role-0.6.0/django_group_role/management/commands/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:32.000000 django-group-role-0.6.0/django_group_role/management/commands/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2381 2023-04-13 07:24:41.000000 django-group-role-0.6.0/django_group_role/management/commands/populate_roles.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     6621 2023-04-13 07:27:32.000000 django-group-role-0.6.0/django_group_role/roles.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)       89 2022-08-24 08:05:10.000000 django-group-role-0.6.0/django_group_role/signals.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1210 2023-04-12 15:41:34.000000 django-group-role-0.6.0/django_group_role/test.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1693 2023-04-13 06:58:22.000000 django-group-role-0.6.0/django_group_role/utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.636677 django-group-role-0.6.0/django_group_role.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      731 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       35 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       18 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1742 2023-04-13 07:52:14.640677 django-group-role-0.6.0/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)       60 2023-04-12 15:21:16.000000 django-group-role-0.6.0/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.640677 django-group-role-0.6.0/tests/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9417 2023-04-13 07:08:45.000000 django-group-role-0.6.0/tests/test_command.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1358 2023-04-13 07:09:32.000000 django-group-role-0.6.0/tests/test_configuration.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1794 2023-04-04 15:25:30.000000 django-group-role-0.6.0/tests/test_database.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2881 2023-04-13 07:04:33.000000 django-group-role-0.6.0/tests/test_definitions.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2996 2023-04-12 15:43:16.000000 django-group-role-0.6.0/tests/test_testing_utils.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4203 2023-04-13 07:04:18.000000 django-group-role-0.6.0/tests/test_utils.py
```

### Comparing `django-group-role-0.5.1/LICENSE` & `django-group-role-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-group-role-0.5.1/PKG-INFO` & `django-group-role-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-group-role
-Version: 0.5.1
+Version: 0.6.0
 Summary: Django Group-based roles
 Home-page: https://github.com/certego/django-group-role
 Author: Davide Setti
 Project-URL: Bug Tracker, https://github.com/certego/django-group-role/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-group-role-0.5.1/README.md` & `django-group-role-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-group-role-0.5.1/django_group_role/management/commands/populate_roles.py` & `django-group-role-0.6.0/django_group_role/management/commands/populate_roles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from django.core.management.base import BaseCommand
-from django.contrib.auth.models import Permission
-from django.conf import settings
 from ...roles import registry, load_roles, BadRoleException
 
 
 def _fuzzy_search(rolenames):
     fuzzy_rolenames = [
         name.lower().replace("-", " ").replace("_", " ") for name in rolenames
     ]
@@ -45,17 +43,16 @@
         )
 
     def handle(self, *rolenames, **options):
         clear = options.get("clear", False)
         fuzzy = options.get("fuzzy", False)
         if clear:
             self.stdout.write(
-                self.style.NOTICE(
-                    "Clear mode enabled, already bound permissions will be removed!"
-                )
+                "Clear mode enabled, already bound permissions will be removed!",
+                self.style.NOTICE,
             )
         if fuzzy:
             check_name = _fuzzy_search(rolenames)
         else:
             check_name = _standard_search(rolenames)
         # assure roles are loaded
         load_roles()
@@ -64,15 +61,14 @@
                 self.stdout.write(f'Setting permissions for role "{name}"...')
                 # istantiate role class
                 role = role()
                 try:
                     role.setup_permissions(clear)
                 except BadRoleException as ex:
                     self.stdout.write(
-                        self.style.ERROR(
-                            f'Unable to bound permission to "{name}" ({ex})'
-                        )
+                        f'Unable to bound permission to "{name}" ({ex})',
+                        self.style.ERROR,
                     )
                 else:
                     self.stdout.write(
-                        self.style.SUCCESS(f'Role "{name}" setup completed!')
+                        f'Role "{name}" setup completed!', self.style.SUCCESS
                     )
```

### Comparing `django-group-role-0.5.1/django_group_role/roles.py` & `django-group-role-0.6.0/django_group_role/roles.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,76 +10,75 @@
 
 class _RoleRegistry(dict):
     def __delitem__(self, v):
         raise NotImplementedError
 
     def __setitem__(self, k, v):
         if k in self:
-            raise ValueError(f"{key} already bound to role registry")
+            raise ValueError(f"{k} already bound to role registry")
         super().__setitem__(k, v)
 
 
 # registry which stores the list of available roles
 registry = _RoleRegistry()
+registry._loaded = False
 
 
 class RegisterRoleMeta(type):
     @classmethod
     def _get_declared_permissions(cls, bases, classdict):
-        permissions = classdict.get("permissions", [])
+        permissions = classdict.get("permissions", ())
         # merge permissions with base classes
         permissions = [permissions]
         if bases:
             permissions = reduce(
-                lambda a, b: a + [getattr(b, "_permissions", None)], bases, permissions
+                lambda a, b: a + [getattr(b, "_permissions", None)],
+                bases,
+                permissions,
             )
         permissions = map_permissions(*permissions)
         assert not bases or permissions, "A Role must specify at least 1 permission"
         return permissions
 
-    @classmethod
-    def _get_declared_group_name(cls, bases, classdict):
-        name = classdict.pop("name", None)
+    def __new__(cls, classname, bases, classdict, **kwargs):
+        name = classdict.get("name", None)
         assert (
             not bases or isinstance(name, str) and name
         ), "Role name must not be empty"
-        return name
-
-    def __new__(cls, classname, bases, classdict, **kwargs):
-        classdict["_group"] = cls._get_declared_group_name(bases, classdict)
         classdict["_permissions"] = cls._get_declared_permissions(bases, classdict)
         # stop inheritance of abstractness
         is_abstract = classdict.setdefault("abstract", False)
         role_class = super().__new__(cls, classname, bases, classdict, **kwargs)
         if not is_abstract:
             # add role to register
-            registry[role_class._group] = role_class
+            registry[role_class.name] = role_class
 
         return role_class
 
 
 class Role(metaclass=RegisterRoleMeta):
     """Base role class. Every role must inherit from this."""
 
     name: str = None
-    permissions = []
+    permissions = ()
     abstract = True
 
     @cached_property
     def group(self):
         from django.contrib.auth.models import Group
 
-        group, _created = Group.objects.get_or_create(name=self._group)
+        group, _created = Group.objects.get_or_create(name=self.name)
         return group
 
     def setup_permissions(self, clear=False):
         """Assignes declared permissions to this role group.
 
         Args:
-            clear (bool, optional): If passed as True also clears existing permissions bound to this role. Defaults to False.
+            clear (bool, optional): If passed as True also clears existing
+                permissions bound to this role. Defaults to False.
         """
         from django.contrib.auth.models import Permission
         from guardian.shortcuts import assign_perm
 
         pre_role_setup.send(self.__class__, role=self, clear=clear)
         if clear:
             self.group.permissions.clear()
@@ -94,26 +93,27 @@
                             assign_perm(perm, self.group)
                         except (
                             ValueError,
                             Permission.DoesNotExist,
                             MultipleObjectsReturned,
                         ):
                             raise BadRoleException(
-                                f"Permission {perm} cannot be bound to role", perm
+                                f"Permission {perm} cannot be bound to role",
+                                perm,
                             )
                 else:
                     # model-grouped perms
                     for perm in perms:
                         try:
                             perm = Permission.objects.get_by_natural_key(
                                 perm, app_label, modelname
                             )
                         except (ValueError, Permission.DoesNotExist):
                             raise BadRoleException(
-                                f"Permission {perm} ({app_label})  cannot be bound to role",
+                                f"Permission {perm} ({app_label}) cannot be bound to role",
                                 f"{app_label}.{perm}",
                             )
                         else:
                             assign_perm(perm, self.group)
 
         post_role_setup.send(self.__class__, role=self)
 
@@ -123,50 +123,60 @@
         return method(*args, **kwargs)
 
     add = partialmethod(_wrap_group_method, method="add")
     remove = partialmethod(_wrap_group_method, method="remove")
     set = partialmethod(_wrap_group_method, method="set")
     clear = partialmethod(_wrap_group_method, method="clear")
 
-    def has_perm(self, perm):
+    def has_perm(self, perm: str) -> bool:
         # split perm in app and codename
-        app_label, codename = perm.split('.', 1)
+        app_label, codename = perm.split(".", 1)
         if app_label in self._permissions:
             # just check if codename is in any model permission for provided app
-            return any(codename in perms for perms in self._permissions[app_label].values())
+            return any(
+                codename in perms for perms in self._permissions[app_label].values()
+            )
         return False
 
-    def has_perms(self, *perms):
+    def has_perms(self, *perms) -> bool:
         return all(self.has_perm(p) for p in perms)
 
-    def has_any_perm(self, *perms):
+    def has_any_perm(self, *perms) -> bool:
         return any(self.has_perm(p) for p in perms)
 
 
-def load_roles():
+def load_roles(*, force=False, clear=False):
     """Force roles to be loaded and returns the updated role registry."""
     from django.conf import settings
 
     role_module = getattr(settings, "ROLES_MODULE", None)
     if not role_module:
         raise ImproperlyConfigured(
             "ROLES_MODULE settings is required to correctly load roles!"
         )
 
-    try:
-        mod = import_module(role_module)
-    except ImportError:
-        raise ImproperlyConfigured(
-            f"No module {role_module} from which import roles found!"
-        )
+    # avoid to reload the registry if not needed
+    if force or not registry._loaded:
+        if clear:
+            registry.clear()
+
+        try:
+            mod = import_module(role_module)
+        except ImportError:
+            raise ImproperlyConfigured(
+                f"No module {role_module} from which import roles found!"
+            )
 
-    # get roles by inspecting module
-    for name, candidate in inspect.getmembers(mod, inspect.isclass):
-        if (
-            issubclass(candidate, Role)
-            and candidate._group not in registry
-            and not candidate.abstract  # do not register abstract roles
-            and not candidate is Role  # avoid base class to be added to registry
-        ):
-            registry[candidate._group] = candidate
+        # get roles by inspecting module
+        for name, candidate in inspect.getmembers(mod, inspect.isclass):
+            if (
+                issubclass(candidate, Role)
+                and candidate.name not in registry
+                # do not register abstract roles
+                and not candidate.abstract
+                # avoid base class to be added to registry
+                and candidate is not Role
+            ):
+                registry[candidate.name] = candidate
 
+        registry._loaded = True
     return registry
```

### Comparing `django-group-role-0.5.1/django_group_role/test.py` & `django-group-role-0.6.0/django_group_role/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from django.test import override_settings
 from .roles import load_roles, registry, BadRoleException
 
 
 class RoleEnabledTestMixin:
+    force_role_reload = False
+    clear_role_registry = False
+
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         rolenames = getattr(cls, "roles", None)
         if isinstance(rolenames, str):
             rolenames = [rolenames]
         roles_from = getattr(cls, "roles_from", None)
         if roles_from:
             # get roles from override
+            # always force reload
             with override_settings(ROLES_MODULE=roles_from):
-                load_roles()
+                load_roles(force=True, clear=cls.clear_role_registry)
         else:
             # load standard roles
-            load_roles()
+            load_roles(force=cls.force_role_reload, clear=cls.clear_role_registry)
 
         # setup roles
         for name, role in registry.items():
             if not rolenames or name in rolenames:
                 # istantiate role class
                 role = role()
                 try:
```

### Comparing `django-group-role-0.5.1/django_group_role/utils.py` & `django-group-role-0.6.0/django_group_role/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,33 @@
         for label, perms in permissions.items():
             try:
                 app_label, modelname = label.split(".", 1)
             except ValueError:
                 app_label = label
                 if not isinstance(perms, dict):
                     raise ValueError(
-                        "App permissions must be provided on per-model bases by providing a dict"
+                        "App permissions must be provided on per-model "
+                        "bases by providing a dict"
                     )
                 for modelname, model_perms in perms.items():
                     perm_map[app_label][modelname] |= set(model_perms)
             else:
                 perm_map[app_label][modelname] |= set(perms)
     else:
         # legacy permission definition
         for perm in permissions:
             try:
                 app_label, codename = perm.split(".", 1)
             except ValueError:
                 raise ValueError(
-                    "Permissions, should be defined in the"
-                    f" format: 'app_label.codename' (is {perm})"
+                    "Permissions, should be defined in the "
+                    f"format: 'app_label.codename' (but is {perm})"
                 )
             perm_map[app_label]["_codenames"].add(codename)
 
     return perm_map
 
 
 def map_permissions(*permissions_list):
     perm_map = defaultdict(lambda: defaultdict(set))
-    return reduce(_map_permissions, permissions_list, perm_map)
+    # turn back defaultdicto into dict to avoid false matches
+    return dict(reduce(_map_permissions, permissions_list, perm_map))
```

### Comparing `django-group-role-0.5.1/django_group_role.egg-info/PKG-INFO` & `django-group-role-0.6.0/django_group_role.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-group-role
-Version: 0.5.1
+Version: 0.6.0
 Summary: Django Group-based roles
 Home-page: https://github.com/certego/django-group-role
 Author: Davide Setti
 Project-URL: Bug Tracker, https://github.com/certego/django-group-role/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-group-role-0.5.1/django_group_role.egg-info/SOURCES.txt` & `django-group-role-0.6.0/django_group_role.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-group-role-0.5.1/setup.cfg` & `django-group-role-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-group-role
-version = 0.5.1
+version = 0.6.0
 author = Davide Setti
 description = Django Group-based roles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/certego/django-group-role
 project_urls = 
 	Bug Tracker = https://github.com/certego/django-group-role/issues
```

### Comparing `django-group-role-0.5.1/tests/test_command.py` & `django-group-role-0.6.0/tests/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import StringIO
 from django.contrib.auth.models import Group
 from django.core.management import call_command
-from django.test import TestCase, override_settings
+from django.test import TestCase
 from guardian.shortcuts import assign_perm
 
 
 class CommandTestCase(TestCase):
     @classmethod
     def setUpTestData(cls):
         group_maps = {
@@ -30,15 +30,15 @@
                 'Setting permissions for role "User-Managers"...',
                 'Role "User-Managers" setup completed!',
                 'Setting permissions for role "Group Managers"...',
                 'Role "Group Managers" setup completed!',
                 'Setting permissions for role "Top-Managers"...',
                 'Role "Top-Managers" setup completed!',
                 'Setting permissions for role "Erasers"...',
-                'Unable to bound permission to "Erasers" (Permission broken (auth)  cannot be bound to role)',
+                'Unable to bound permission to "Erasers" (Permission broken (auth) cannot be bound to role)',
                 'Setting permissions for role "Broken"...',
                 'Unable to bound permission to "Broken" (Permission auth.non_existing_perm cannot be bound to role)',
                 "",
             ],
         )
         self.assertEqual(Group.objects.all().count(), 7)
         group = Group.objects.get_by_natural_key("Users")
@@ -106,15 +106,15 @@
                 'Setting permissions for role "User-Managers"...',
                 'Role "User-Managers" setup completed!',
                 'Setting permissions for role "Group Managers"...',
                 'Role "Group Managers" setup completed!',
                 'Setting permissions for role "Top-Managers"...',
                 'Role "Top-Managers" setup completed!',
                 'Setting permissions for role "Erasers"...',
-                'Unable to bound permission to "Erasers" (Permission broken (auth)  cannot be bound to role)',
+                'Unable to bound permission to "Erasers" (Permission broken (auth) cannot be bound to role)',
                 'Setting permissions for role "Broken"...',
                 'Unable to bound permission to "Broken" (Permission auth.non_existing_perm cannot be bound to role)',
                 "",
             ],
         )
         self.assertEqual(Group.objects.all().count(), 7)
         group = Group.objects.get_by_natural_key("Users")
```

### Comparing `django-group-role-0.5.1/tests/test_configuration.py` & `django-group-role-0.6.0/tests/test_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from django.core.exceptions import ImproperlyConfigured
 from django.test import SimpleTestCase, override_settings
-from django_group_role.roles import Role, registry, load_roles
+from django_group_role.roles import registry, load_roles
 
 
 class ConfigurationTestCase(SimpleTestCase):
     # need to keep registry clear in these tests
     def setUp(self):
         self._registry = deepcopy(registry)
         registry.clear()
@@ -16,27 +16,27 @@
 
     @override_settings(ROLES_MODULE=None)
     def test_configuration_errors(self):
         with self.assertRaisesMessage(
             ImproperlyConfigured,
             "ROLES_MODULE settings is required to correctly load roles!",
         ):
-            load_roles()
+            load_roles(force=True)
 
     @override_settings(ROLES_MODULE="nowhere.nothing")
     def test_configuration_module_not_found(self):
         with self.assertRaisesMessage(
             ImproperlyConfigured,
             "No module nowhere.nothing from which import roles found!",
         ):
-            load_roles()
+            load_roles(force=True)
 
     @override_settings(ROLES_MODULE="example_project.roles_secondary")
     def test_loading(self):
-        load_roles()
+        load_roles(force=True)
         self.assertCountEqual(
             registry.keys(),
             [
                 "Base",
                 "Managers",
                 "Groupers",
             ],
```

### Comparing `django-group-role-0.5.1/tests/test_database.py` & `django-group-role-0.6.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.5.1/tests/test_definitions.py` & `django-group-role-0.6.0/tests/test_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.test import SimpleTestCase
 from django_group_role import Role, registry
-from example_project.roles import AbstractRole, BasicRole, Erasers, GroupManagers, UserManagers
+from example_project.roles import AbstractRole, Erasers, GroupManagers, UserManagers
 
 
 class DefinitionsTestCase(SimpleTestCase):
     def test_role_wrong_group(self):
         with self.assertRaisesMessage(AssertionError, "Role name must not be empty"):
             class NoGroupRole(Role):
                 pass
@@ -26,15 +26,15 @@
         ):
             class NoPermRole(Role):
                 name = "test"
                 permissions = []
 
         with self.assertRaisesMessage(
             ValueError,
-            "Permissions, should be defined in the format: 'app_label.codename' (is perm)",
+            "Permissions, should be defined in the format: 'app_label.codename' (but is perm)",
         ):
             class NoPermRole(Role):
                 name = "test"
                 permissions = ["perm", 1]
 
     def test_role_composition(self):
         self.assertCountEqual(
```

### Comparing `django-group-role-0.5.1/tests/test_testing_utils.py` & `django-group-role-0.6.0/tests/test_testing_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,15 @@
-from copy import deepcopy
 from django.contrib.auth.models import Group
-from django.test import TestCase, override_settings
-from django_group_role.roles import Role, registry, load_roles
+from django.test import TestCase
 from django_group_role.test import RoleEnabledTestMixin
 
 
 class BaseTestingTestCase(RoleEnabledTestMixin, TestCase):
-    # need to keep registry clear in these tests
-    @classmethod
-    def setUpClass(cls):
-        cls._registry = deepcopy(registry)
-        registry.clear()
-        super().setUpClass()
-
-    @classmethod
-    def tearDownClass(cls):
-        super().tearDownClass()
-        registry.clear()
-        registry.update(cls._registry)
+    clear_role_registry = True
+    force_role_reload = True
 
 
 class OnlySelectedTestCase(BaseTestingTestCase):
     roles = ["Users", "User-Managers"]
 
     def test_roles(self):
         self.assertQuerysetEqual(
```

### Comparing `django-group-role-0.5.1/tests/test_utils.py` & `django-group-role-0.6.0/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from django.test import SimpleTestCase, override_settings
+from django.test import SimpleTestCase
 from django_group_role.utils import map_permissions
 
 
 class UtilsSimpleTestCase(SimpleTestCase):
     def test_map_permissions_list_wrong_code(self):
         with self.assertRaisesMessage(
             ValueError,
-            "Permissions, should be defined in the format: 'app_label.codename' (is view_user)",
+            "Permissions, should be defined in the format: 'app_label.codename' (but is view_user)",
         ):
             map_permissions(["view_user"])
 
     def test_map_permissions_list(self):
         perm_map = map_permissions(
             ["auth.view_user", "auth.view_group", "myapp.view_mymodel"]
         )
```

