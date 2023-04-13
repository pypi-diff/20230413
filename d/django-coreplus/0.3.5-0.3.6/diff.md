# Comparing `tmp/django-coreplus-0.3.5.tar.gz` & `tmp/django-coreplus-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-coreplus-0.3.5.tar", last modified: Thu Apr 13 03:34:13 2023, max compression
+gzip compressed data, was "django-coreplus-0.3.6.tar", last modified: Thu Apr 13 04:22:31 2023, max compression
```

## Comparing `django-coreplus-0.3.5.tar` & `django-coreplus-0.3.6.tar`

### file list

```diff
@@ -1,491 +1,491 @@
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3828 2023-04-13 03:31:11.000000 django-coreplus-0.3.5/CHANGELOG.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/LICENSE
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      141 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/MANIFEST.in
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3670 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/PKG-INFO
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2429 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/README.md
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      110 2023-04-13 03:31:26.000000 django-coreplus-0.3.5/coreplus/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       77 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      440 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    10774 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/base.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      890 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/filters.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1402 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2602 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2379 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/mixins.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    10056 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/sites.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/static/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    37296 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/alpine.min.js
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    34881 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/htmx.min.js
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    89501 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/jquery.min.js
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2881 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/base.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/confirmation.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3051 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/form_view.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      942 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/inspect.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1590 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/inspect_object_tools.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      130 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/object_buttons.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      338 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/print.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/print_cover.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/print_footer.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/admin/templates/admin/print_header.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/ads/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/ads/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/ads/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/ads/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/ads/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/ads/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/ads/api/v1/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       55 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/ads/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/ads/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1882 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      182 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/consts.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/endpoints/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/endpoints/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      237 2022-12-28 08:58:55.000000 django-coreplus-0.3.5/coreplus/api/endpoints/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      585 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/endpoints/v1.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      599 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/endpoints/v2.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2377 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/helpers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      562 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      910 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      275 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/schemas.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/api/templates/drf_spectacular/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1069 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/templates/drf_spectacular/redoc.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      231 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      418 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/api/views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6886 2022-12-28 08:58:55.000000 django-coreplus-0.3.5/coreplus/configs.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    13235 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/contacts/abstracts.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      298 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      193 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      452 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      496 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/gis.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2934 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/inlines.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3484 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6069 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/management/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/management/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/management/commands/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/management/commands/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2280 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/management/commands/populate_countries.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/contacts/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    24385 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6351 2022-12-13 04:40:56.000000 django-coreplus-0.3.5/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1106 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3644 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/contacts/models.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      245 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      243 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1288 2022-12-28 08:58:55.000000 django-coreplus-0.3.5/coreplus/discuss/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      194 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4367 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      448 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1034 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1623 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/discuss/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4163 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      591 2023-01-30 02:56:44.000000 django-coreplus-0.3.5/coreplus/discuss/migrations/0002_alter_discuss_flag.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3597 2023-03-14 07:44:17.000000 django-coreplus-0.3.5/coreplus/discuss/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/discuss/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       57 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      269 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/management/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/management/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/management/commands/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/management/commands/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      467 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/management/commands/build_docs.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/templates/docs/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      468 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/templates/docs/_base_one.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      581 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/templates/docs/_base_two.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      505 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/templates/docs/index.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/tests/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/tests/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2022 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/tests/runtests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/tests/test_docs/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        2 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/tests/test_docs/index.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/docs/tests/test_docs/sub_dir/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        2 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/tests/test_docs/sub_dir/index.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3898 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/tests/test_views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      345 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/tests/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      419 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3537 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/docs/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       78 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      521 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2150 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/heralds/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      214 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     8624 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/heralds/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      444 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1142 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1851 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      323 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/managers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/heralds/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5041 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      441 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/heralds/migrations/0002_alter_directmessage_content.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/heralds/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2406 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/heralds/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1216 2022-12-13 05:03:37.000000 django-coreplus-0.3.5/coreplus/heralds/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      753 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       28 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1069 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/admin.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      438 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2249 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/core.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      395 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      658 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/templates/admin/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/hooks/templates/admin/coreplus_hooks/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      677 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      240 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/hooks/urls.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      683 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/markdown/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      106 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3313 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      280 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1529 2023-04-13 03:30:17.000000 django-coreplus-0.3.5/coreplus/markdown/bleaching.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/markdown/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/markdown/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/markdown/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      562 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      910 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/markdown/plugins/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/plugins/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      951 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/plugins/gist.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      614 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/plugins/linkify.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1837 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/plugins/twitter.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1430 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/plugins/youtube.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      112 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/renderer.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      953 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/markdown/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       68 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3960 2023-01-09 06:47:42.000000 django-coreplus-0.3.5/coreplus/media/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      333 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4386 2023-01-09 06:47:42.000000 django-coreplus-0.3.5/coreplus/media/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      439 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      766 2023-01-09 06:47:42.000000 django-coreplus-0.3.5/coreplus/media/helpers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2051 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2976 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/media/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5350 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4011 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      434 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/media/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/navigators/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2099 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      361 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/admin.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      606 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/navigators/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/navigators/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/navigators/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1377 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2174 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/navigators/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4224 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5698 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/models.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/navigators/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      567 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/templatetags/navigators_tags.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/navigators/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       61 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1030 2023-01-26 04:08:06.000000 django-coreplus-0.3.5/coreplus/notices/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1217 2023-01-24 06:23:58.000000 django-coreplus-0.3.5/coreplus/notices/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      622 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2037 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      276 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1290 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2077 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3941 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2805 2023-01-26 04:08:06.000000 django-coreplus-0.3.5/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     9233 2023-01-26 04:08:06.000000 django-coreplus-0.3.5/coreplus/notices/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      211 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/signals.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      325 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/tasks.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/notices/templates/notices/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       79 2023-01-26 04:08:06.000000 django-coreplus-0.3.5/coreplus/notices/templates/notices/email_broadcast.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      392 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/notices/urls.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/numerators/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       87 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      290 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/numerators/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/api/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/api/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/api/views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/api/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      452 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/numerators/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/numerators/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/numerators/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      746 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1346 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/numerators/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2052 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5998 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/numerators/models.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/profanity/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       81 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      166 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3380 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/extras.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/profanity/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/migrations/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/profanity/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      264 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/templatetags/profanity.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      402 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      257 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/validators.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3583 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/profanity/wordlist.txt
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/qrcodes/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       79 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/qrcodes/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/qrcodes/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       41 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/qrcodes/admin.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      155 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/qrcodes/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4184 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/qrcodes/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/qrcodes/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      115 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      628 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1332 2023-03-07 09:24:58.000000 django-coreplus-0.3.5/coreplus/reactions/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      517 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3073 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/reactions/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     8838 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    15907 2023-03-17 05:46:47.000000 django-coreplus-0.3.5/coreplus/reactions/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/reactions/tests.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       73 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      444 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      637 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1005 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/templates/search/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       94 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/templates/search/algolia_search.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1724 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/templates/search/search.html
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      413 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/templates/search/search_form.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/search/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      674 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/templatetags/search_tags.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      131 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2350 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/search/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       94 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1273 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/api/v1/views.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      477 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2395 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/contexts.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      918 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1985 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1716 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3441 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1283 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/permissions.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2254 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/registries.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/templates/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/templates/admin/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      173 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/templates/admin/base.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/templates/admin/settings/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/templates/admin/settings/.gitinclude
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2461 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/templates/admin/settings/edit.html
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/templates/simpel_settings/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/templates/simpel_settings/.gitinclude
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/settings/templatetags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/templatetags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1629 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/templatetags/settings_tags.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       68 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      438 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3650 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/settings/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       63 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       63 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/api/__init__.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      412 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      197 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1491 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      505 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/apps.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/locale/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/locale/id/
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/locale/id/LC_MESSAGES/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      399 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      663 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      136 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/managers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/shorts/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2354 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1362 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      125 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      692 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/utils.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      625 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/shorts/views.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/spams/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       83 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      150 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1018 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/extras.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      101 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/spams.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/spams/static/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)   311221 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)   253954 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      951 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      223 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/spams/validators.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/tags/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       72 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/README.md
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      706 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/admin.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/tags/api/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       34 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/api/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      420 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/api/extensions.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/tags/api/v1/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/api/v1/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      524 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/api/v1/serializers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      300 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/api/v1/urls.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      881 2023-04-13 03:22:37.000000 django-coreplus-0.3.5/coreplus/tags/api/v1/viewsets.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      146 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/apps.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      131 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/managers.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/tags/migrations/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4657 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/migrations/0001_initial.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      450 2023-03-28 02:54:06.000000 django-coreplus-0.3.5/coreplus/tags/migrations/0002_category_category_id.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/migrations/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3597 2023-03-28 02:53:55.000000 django-coreplus-0.3.5/coreplus/tags/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      683 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/resources.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/tags/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      117 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/urls.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/utils/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      997 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/avatars.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      823 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/contenttypes.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3995 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/currencies.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3901 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/decorators.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/utils/forms/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/forms/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      996 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/forms/fields.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3122 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/loading.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/coreplus/utils/models/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/__init__.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    11822 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/actions.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5723 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/choices.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    17271 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/fields.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    14099 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/managers.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     7742 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/models.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2308 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/paranoid.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1117 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/signals.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    14851 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/models/tracker.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2593 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/slugs.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/tests.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4505 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/utils/validators.py
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1471 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/coreplus/version.py
-drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/django_coreplus.egg-info/
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3670 2023-04-13 03:34:12.000000 django-coreplus-0.3.5/django_coreplus.egg-info/PKG-INFO
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    12011 2023-04-13 03:34:12.000000 django-coreplus-0.3.5/django_coreplus.egg-info/SOURCES.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        1 2023-04-13 03:34:12.000000 django-coreplus-0.3.5/django_coreplus.egg-info/dependency_links.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        1 2022-12-13 05:23:51.000000 django-coreplus-0.3.5/django_coreplus.egg-info/not-zip-safe
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      433 2023-04-13 03:34:12.000000 django-coreplus-0.3.5/django_coreplus.egg-info/requires.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        9 2023-04-13 03:34:12.000000 django-coreplus-0.3.5/django_coreplus.egg-info/top_level.txt
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2123 2023-04-13 03:34:13.000000 django-coreplus-0.3.5/setup.cfg
--rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       61 2022-12-05 03:07:46.000000 django-coreplus-0.3.5/setup.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.091709 django-coreplus-0.3.6/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4025 2023-04-13 04:18:53.000000 django-coreplus-0.3.6/CHANGELOG.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/LICENSE
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      141 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/MANIFEST.in
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3670 2023-04-13 04:22:31.091709 django-coreplus-0.3.6/PKG-INFO
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2429 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/README.md
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.591725 django-coreplus-0.3.6/coreplus/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      110 2023-04-13 04:18:08.000000 django-coreplus-0.3.6/coreplus/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.595725 django-coreplus-0.3.6/coreplus/admin/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       77 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      440 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    10774 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/base.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      890 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/filters.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.515728 django-coreplus-0.3.6/coreplus/admin/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.519728 django-coreplus-0.3.6/coreplus/admin/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.599725 django-coreplus-0.3.6/coreplus/admin/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1402 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2602 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2379 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/mixins.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    10056 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/sites.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.519728 django-coreplus-0.3.6/coreplus/admin/static/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.519728 django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.603725 django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    37296 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/alpine.min.js
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    34881 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/htmx.min.js
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    89501 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/jquery.min.js
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.519728 django-coreplus-0.3.6/coreplus/admin/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.611725 django-coreplus-0.3.6/coreplus/admin/templates/admin/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2881 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/base.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/confirmation.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3051 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/form_view.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      942 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/inspect.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1590 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/inspect_object_tools.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      130 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/object_buttons.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      338 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/print.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/print_cover.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/print_footer.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/admin/templates/admin/print_header.html
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.615724 django-coreplus-0.3.6/coreplus/ads/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/ads/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.615724 django-coreplus-0.3.6/coreplus/ads/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/ads/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.619724 django-coreplus-0.3.6/coreplus/ads/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/ads/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/ads/api/v1/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       55 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/ads/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/ads/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.631724 django-coreplus-0.3.6/coreplus/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1882 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      182 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/consts.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.635724 django-coreplus-0.3.6/coreplus/api/endpoints/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/endpoints/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      237 2022-12-28 08:58:55.000000 django-coreplus-0.3.6/coreplus/api/endpoints/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      585 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/endpoints/v1.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      599 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/endpoints/v2.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2377 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/helpers.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.523728 django-coreplus-0.3.6/coreplus/api/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.523728 django-coreplus-0.3.6/coreplus/api/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.635724 django-coreplus-0.3.6/coreplus/api/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      562 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      910 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      275 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/schemas.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.523728 django-coreplus-0.3.6/coreplus/api/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.639724 django-coreplus-0.3.6/coreplus/api/templates/drf_spectacular/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1069 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/templates/drf_spectacular/redoc.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      231 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      418 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/api/views.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6886 2022-12-28 08:58:55.000000 django-coreplus-0.3.6/coreplus/configs.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.647724 django-coreplus-0.3.6/coreplus/contacts/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    13235 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/contacts/abstracts.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      298 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.647724 django-coreplus-0.3.6/coreplus/contacts/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.647724 django-coreplus-0.3.6/coreplus/contacts/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      193 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      452 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      496 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/gis.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2934 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/inlines.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.523728 django-coreplus-0.3.6/coreplus/contacts/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.523728 django-coreplus-0.3.6/coreplus/contacts/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.651723 django-coreplus-0.3.6/coreplus/contacts/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3484 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6069 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.651723 django-coreplus-0.3.6/coreplus/contacts/management/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/management/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.655723 django-coreplus-0.3.6/coreplus/contacts/management/commands/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/management/commands/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2280 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/management/commands/populate_countries.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.655723 django-coreplus-0.3.6/coreplus/contacts/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    24385 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     6351 2022-12-13 04:40:56.000000 django-coreplus-0.3.6/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1106 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3644 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/contacts/models.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.659723 django-coreplus-0.3.6/coreplus/discuss/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      245 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      243 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.659723 django-coreplus-0.3.6/coreplus/discuss/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.663723 django-coreplus-0.3.6/coreplus/discuss/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1288 2022-12-28 08:58:55.000000 django-coreplus-0.3.6/coreplus/discuss/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      194 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4367 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      448 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.527727 django-coreplus-0.3.6/coreplus/discuss/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.527727 django-coreplus-0.3.6/coreplus/discuss/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.663723 django-coreplus-0.3.6/coreplus/discuss/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1034 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1623 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.663723 django-coreplus-0.3.6/coreplus/discuss/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4163 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      591 2023-01-30 02:56:44.000000 django-coreplus-0.3.6/coreplus/discuss/migrations/0002_alter_discuss_flag.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3597 2023-03-14 07:44:17.000000 django-coreplus-0.3.6/coreplus/discuss/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/discuss/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.667723 django-coreplus-0.3.6/coreplus/docs/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       57 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      269 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.667723 django-coreplus-0.3.6/coreplus/docs/management/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/management/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.671723 django-coreplus-0.3.6/coreplus/docs/management/commands/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/management/commands/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      467 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/management/commands/build_docs.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.527727 django-coreplus-0.3.6/coreplus/docs/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.675722 django-coreplus-0.3.6/coreplus/docs/templates/docs/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      468 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/templates/docs/_base_one.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      581 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/templates/docs/_base_two.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      505 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/templates/docs/index.html
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.675722 django-coreplus-0.3.6/coreplus/docs/tests/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/tests/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2022 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/tests/runtests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.679722 django-coreplus-0.3.6/coreplus/docs/tests/test_docs/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        2 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/tests/test_docs/index.html
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.679722 django-coreplus-0.3.6/coreplus/docs/tests/test_docs/sub_dir/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        2 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/tests/test_docs/sub_dir/index.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3898 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/tests/test_views.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      345 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/tests/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      419 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3537 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/docs/views.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.691722 django-coreplus-0.3.6/coreplus/heralds/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       78 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      521 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.691722 django-coreplus-0.3.6/coreplus/heralds/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.695722 django-coreplus-0.3.6/coreplus/heralds/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2150 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/heralds/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      214 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     8624 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/heralds/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      444 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.531727 django-coreplus-0.3.6/coreplus/heralds/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.531727 django-coreplus-0.3.6/coreplus/heralds/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.695722 django-coreplus-0.3.6/coreplus/heralds/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1142 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1851 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      323 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/managers.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.699722 django-coreplus-0.3.6/coreplus/heralds/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5041 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      441 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/heralds/migrations/0002_alter_directmessage_content.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/heralds/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2406 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/heralds/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1216 2022-12-13 05:03:37.000000 django-coreplus-0.3.6/coreplus/heralds/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.707722 django-coreplus-0.3.6/coreplus/hooks/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      753 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       28 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1069 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/admin.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      438 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2249 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/core.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.531727 django-coreplus-0.3.6/coreplus/hooks/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.531727 django-coreplus-0.3.6/coreplus/hooks/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.707722 django-coreplus-0.3.6/coreplus/hooks/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      395 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      658 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.535727 django-coreplus-0.3.6/coreplus/hooks/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.535727 django-coreplus-0.3.6/coreplus/hooks/templates/admin/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.707722 django-coreplus-0.3.6/coreplus/hooks/templates/admin/coreplus_hooks/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      677 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      240 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/hooks/urls.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.535727 django-coreplus-0.3.6/coreplus/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.535727 django-coreplus-0.3.6/coreplus/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.711721 django-coreplus-0.3.6/coreplus/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      683 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.715721 django-coreplus-0.3.6/coreplus/markdown/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      106 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3313 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      280 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1529 2023-04-13 03:30:17.000000 django-coreplus-0.3.6/coreplus/markdown/bleaching.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.535727 django-coreplus-0.3.6/coreplus/markdown/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.535727 django-coreplus-0.3.6/coreplus/markdown/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.719721 django-coreplus-0.3.6/coreplus/markdown/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      562 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      910 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.727721 django-coreplus-0.3.6/coreplus/markdown/plugins/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/plugins/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      951 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/plugins/gist.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      614 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/plugins/linkify.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1837 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/plugins/twitter.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1430 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/plugins/youtube.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      112 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/renderer.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      953 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/markdown/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.739720 django-coreplus-0.3.6/coreplus/media/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       68 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.743720 django-coreplus-0.3.6/coreplus/media/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.759720 django-coreplus-0.3.6/coreplus/media/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3960 2023-01-09 06:47:42.000000 django-coreplus-0.3.6/coreplus/media/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      333 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4386 2023-01-09 06:47:42.000000 django-coreplus-0.3.6/coreplus/media/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      439 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      766 2023-01-09 06:47:42.000000 django-coreplus-0.3.6/coreplus/media/helpers.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.539727 django-coreplus-0.3.6/coreplus/media/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.539727 django-coreplus-0.3.6/coreplus/media/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.759720 django-coreplus-0.3.6/coreplus/media/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2051 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2976 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.763720 django-coreplus-0.3.6/coreplus/media/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5350 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4011 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      434 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/media/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.775719 django-coreplus-0.3.6/coreplus/navigators/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2099 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      361 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/admin.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      606 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.543727 django-coreplus-0.3.6/coreplus/navigators/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.543727 django-coreplus-0.3.6/coreplus/navigators/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.779719 django-coreplus-0.3.6/coreplus/navigators/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1377 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2174 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.779719 django-coreplus-0.3.6/coreplus/navigators/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4224 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5698 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/models.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.783719 django-coreplus-0.3.6/coreplus/navigators/templatetags/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/templatetags/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      567 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/templatetags/navigators_tags.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/navigators/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.811718 django-coreplus-0.3.6/coreplus/notices/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       61 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1030 2023-01-26 04:08:06.000000 django-coreplus-0.3.6/coreplus/notices/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.815718 django-coreplus-0.3.6/coreplus/notices/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.823718 django-coreplus-0.3.6/coreplus/notices/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1217 2023-01-24 06:23:58.000000 django-coreplus-0.3.6/coreplus/notices/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      622 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2037 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      276 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.547727 django-coreplus-0.3.6/coreplus/notices/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.547727 django-coreplus-0.3.6/coreplus/notices/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.827718 django-coreplus-0.3.6/coreplus/notices/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1290 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2077 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.831717 django-coreplus-0.3.6/coreplus/notices/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3941 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2805 2023-01-26 04:08:06.000000 django-coreplus-0.3.6/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     9233 2023-01-26 04:08:06.000000 django-coreplus-0.3.6/coreplus/notices/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      211 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/signals.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      325 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/tasks.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.547727 django-coreplus-0.3.6/coreplus/notices/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.831717 django-coreplus-0.3.6/coreplus/notices/templates/notices/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       79 2023-01-26 04:08:06.000000 django-coreplus-0.3.6/coreplus/notices/templates/notices/email_broadcast.txt
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      392 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/notices/urls.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.839717 django-coreplus-0.3.6/coreplus/numerators/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       87 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      290 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.847717 django-coreplus-0.3.6/coreplus/numerators/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/api/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/api/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/api/views.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/api/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      452 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.551727 django-coreplus-0.3.6/coreplus/numerators/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.551727 django-coreplus-0.3.6/coreplus/numerators/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.847717 django-coreplus-0.3.6/coreplus/numerators/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      746 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1346 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.851717 django-coreplus-0.3.6/coreplus/numerators/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2052 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5998 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/numerators/models.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.859717 django-coreplus-0.3.6/coreplus/profanity/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       81 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      166 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3380 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/extras.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.863716 django-coreplus-0.3.6/coreplus/profanity/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/migrations/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.871716 django-coreplus-0.3.6/coreplus/profanity/templatetags/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/templatetags/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      264 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/templatetags/profanity.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      402 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      257 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/validators.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3583 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/profanity/wordlist.txt
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.879716 django-coreplus-0.3.6/coreplus/qrcodes/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       79 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/qrcodes/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/qrcodes/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       41 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/qrcodes/admin.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      155 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/qrcodes/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4184 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/qrcodes/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/qrcodes/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.899715 django-coreplus-0.3.6/coreplus/reactions/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      115 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      628 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.899715 django-coreplus-0.3.6/coreplus/reactions/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.903715 django-coreplus-0.3.6/coreplus/reactions/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1332 2023-03-07 09:24:58.000000 django-coreplus-0.3.6/coreplus/reactions/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      517 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.555726 django-coreplus-0.3.6/coreplus/reactions/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.555726 django-coreplus-0.3.6/coreplus/reactions/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.903715 django-coreplus-0.3.6/coreplus/reactions/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3073 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.907715 django-coreplus-0.3.6/coreplus/reactions/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     8838 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    15907 2023-03-17 05:46:47.000000 django-coreplus-0.3.6/coreplus/reactions/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/reactions/tests.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.919715 django-coreplus-0.3.6/coreplus/search/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       73 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.923714 django-coreplus-0.3.6/coreplus/search/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.923714 django-coreplus-0.3.6/coreplus/search/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      444 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.555726 django-coreplus-0.3.6/coreplus/search/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.555726 django-coreplus-0.3.6/coreplus/search/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.927714 django-coreplus-0.3.6/coreplus/search/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      637 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1005 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.555726 django-coreplus-0.3.6/coreplus/search/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.935714 django-coreplus-0.3.6/coreplus/search/templates/search/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       94 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/templates/search/algolia_search.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1724 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/templates/search/search.html
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      413 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/templates/search/search_form.html
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.939714 django-coreplus-0.3.6/coreplus/search/templatetags/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/templatetags/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      674 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/templatetags/search_tags.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      131 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2350 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/search/views.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.951713 django-coreplus-0.3.6/coreplus/settings/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       94 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1273 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.951713 django-coreplus-0.3.6/coreplus/settings/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.955713 django-coreplus-0.3.6/coreplus/settings/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/api/v1/views.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      477 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2395 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/contexts.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.559726 django-coreplus-0.3.6/coreplus/settings/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.559726 django-coreplus-0.3.6/coreplus/settings/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.959713 django-coreplus-0.3.6/coreplus/settings/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      918 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1985 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.963713 django-coreplus-0.3.6/coreplus/settings/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1716 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3441 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1283 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/permissions.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2254 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/registries.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.567726 django-coreplus-0.3.6/coreplus/settings/templates/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.963713 django-coreplus-0.3.6/coreplus/settings/templates/admin/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      173 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/templates/admin/base.html
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.963713 django-coreplus-0.3.6/coreplus/settings/templates/admin/settings/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/templates/admin/settings/.gitinclude
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2461 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/templates/admin/settings/edit.html
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.967713 django-coreplus-0.3.6/coreplus/settings/templates/simpel_settings/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/templates/simpel_settings/.gitinclude
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.967713 django-coreplus-0.3.6/coreplus/settings/templatetags/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/templatetags/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1629 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/templatetags/settings_tags.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       68 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      438 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3650 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/settings/views.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.987712 django-coreplus-0.3.6/coreplus/shorts/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       63 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       63 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.987712 django-coreplus-0.3.6/coreplus/shorts/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/api/__init__.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.995712 django-coreplus-0.3.6/coreplus/shorts/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      412 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      197 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1491 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      505 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/apps.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.567726 django-coreplus-0.3.6/coreplus/shorts/locale/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.567726 django-coreplus-0.3.6/coreplus/shorts/locale/id/
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:30.999712 django-coreplus-0.3.6/coreplus/shorts/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      399 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/locale/id/LC_MESSAGES/django.mo
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      663 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      136 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/managers.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.003712 django-coreplus-0.3.6/coreplus/shorts/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2354 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1362 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      125 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      692 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/utils.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      625 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/shorts/views.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.015711 django-coreplus-0.3.6/coreplus/spams/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       83 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      150 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1018 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/extras.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      101 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/spams.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.023711 django-coreplus-0.3.6/coreplus/spams/static/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)   311221 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)   253954 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      951 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      223 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/spams/validators.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.039711 django-coreplus-0.3.6/coreplus/tags/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       72 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/README.md
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      706 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/admin.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.039711 django-coreplus-0.3.6/coreplus/tags/api/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       34 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/api/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      420 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/api/extensions.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.047710 django-coreplus-0.3.6/coreplus/tags/api/v1/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/api/v1/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      524 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/api/v1/serializers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      300 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/api/v1/urls.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      907 2023-04-13 04:22:09.000000 django-coreplus-0.3.6/coreplus/tags/api/v1/viewsets.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      146 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/apps.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      131 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/managers.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.063710 django-coreplus-0.3.6/coreplus/tags/migrations/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4657 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/migrations/0001_initial.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      450 2023-03-28 02:54:06.000000 django-coreplus-0.3.6/coreplus/tags/migrations/0002_category_category_id.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/migrations/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3597 2023-03-28 02:53:55.000000 django-coreplus-0.3.6/coreplus/tags/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      826 2023-04-13 03:50:58.000000 django-coreplus-0.3.6/coreplus/tags/resources.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/tags/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      117 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/urls.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.071709 django-coreplus-0.3.6/coreplus/utils/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      997 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/avatars.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      823 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/contenttypes.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3995 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/currencies.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3901 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/decorators.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.075709 django-coreplus-0.3.6/coreplus/utils/forms/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/forms/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      996 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/forms/fields.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3122 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/loading.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.083709 django-coreplus-0.3.6/coreplus/utils/models/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/__init__.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    11822 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/actions.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     5723 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/choices.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    17271 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/fields.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    14099 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/managers.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     7742 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/models.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2308 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/paranoid.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1117 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/signals.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    14851 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/models/tracker.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2593 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/slugs.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        0 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/tests.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     4505 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/utils/validators.py
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     1471 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/coreplus/version.py
+drwxrwxr-x   0 wilsen    (1000) wilsen    (1000)        0 2023-04-13 04:22:31.087709 django-coreplus-0.3.6/django_coreplus.egg-info/
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     3670 2023-04-13 04:22:29.000000 django-coreplus-0.3.6/django_coreplus.egg-info/PKG-INFO
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)    12011 2023-04-13 04:22:29.000000 django-coreplus-0.3.6/django_coreplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        1 2023-04-13 04:22:29.000000 django-coreplus-0.3.6/django_coreplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        1 2022-12-13 05:23:51.000000 django-coreplus-0.3.6/django_coreplus.egg-info/not-zip-safe
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)      433 2023-04-13 04:22:29.000000 django-coreplus-0.3.6/django_coreplus.egg-info/requires.txt
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)        9 2023-04-13 04:22:29.000000 django-coreplus-0.3.6/django_coreplus.egg-info/top_level.txt
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)     2123 2023-04-13 04:22:31.091709 django-coreplus-0.3.6/setup.cfg
+-rw-rw-r--   0 wilsen    (1000) wilsen    (1000)       61 2022-12-05 03:07:46.000000 django-coreplus-0.3.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-coreplus-0.3.5/CHANGELOG.md` & `django-coreplus-0.3.6/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # coreplus/main
 
+## 0.3.6
+
+### Patch
+
+- update ordering filter for category viewset [wilsen](https://gitlab.com/wilsen.widjaja1)
+- update resources for export category [wilsen](https://gitlab.com/wilsen.widjaja1)
+
 ## 0.3.5
 
 ### Patch
 
 - update ordering filter for category viewset [wilsen](https://gitlab.com/wilsen.widjaja1)
```

### Comparing `django-coreplus-0.3.5/PKG-INFO` & `django-coreplus-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-coreplus
-Version: 0.3.5
+Version: 0.3.6
 Summary: Django functional modules
 Home-page: https://gitlab.com/zeroplus/django/django-coreplus
 Author: Zero Plus
 Author-email: sasri.works@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/zeroplus/django/django-coreplus/-/wikis/
 Project-URL: Source, https://gitlab.com/zeroplus/django/django-coreplus
```

### Comparing `django-coreplus-0.3.5/README.md` & `django-coreplus-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/base.py` & `django-coreplus-0.3.6/coreplus/admin/base.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/filters.py` & `django-coreplus-0.3.6/coreplus/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/admin/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/admin/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/mixins.py` & `django-coreplus-0.3.6/coreplus/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/sites.py` & `django-coreplus-0.3.6/coreplus/admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/alpine.min.js` & `django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/alpine.min.js`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/htmx.min.js` & `django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/static/coreplus_admin/js/jquery.min.js` & `django-coreplus-0.3.6/coreplus/admin/static/coreplus_admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/templates/admin/base.html` & `django-coreplus-0.3.6/coreplus/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/templates/admin/form_view.html` & `django-coreplus-0.3.6/coreplus/admin/templates/admin/form_view.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/templates/admin/inspect.html` & `django-coreplus-0.3.6/coreplus/admin/templates/admin/inspect.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/admin/templates/admin/inspect_object_tools.html` & `django-coreplus-0.3.6/coreplus/admin/templates/admin/inspect_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/README.md` & `django-coreplus-0.3.6/coreplus/api/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/endpoints/v1.py` & `django-coreplus-0.3.6/coreplus/api/endpoints/v1.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/endpoints/v2.py` & `django-coreplus-0.3.6/coreplus/api/endpoints/v2.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/helpers.py` & `django-coreplus-0.3.6/coreplus/api/helpers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/api/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/api/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/api/templates/drf_spectacular/redoc.html` & `django-coreplus-0.3.6/coreplus/api/templates/drf_spectacular/redoc.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/configs.py` & `django-coreplus-0.3.6/coreplus/configs.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/abstracts.py` & `django-coreplus-0.3.6/coreplus/contacts/abstracts.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/inlines.py` & `django-coreplus-0.3.6/coreplus/contacts/inlines.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/contacts/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/contacts/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/management/commands/populate_countries.py` & `django-coreplus-0.3.6/coreplus/contacts/management/commands/populate_countries.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/contacts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py` & `django-coreplus-0.3.6/coreplus/contacts/migrations/0002_alter_billingaddress_address_and_more.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py` & `django-coreplus-0.3.6/coreplus/contacts/migrations/0003_billingaddress_district_deliverableaddress_district_and_more.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/contacts/models.py` & `django-coreplus-0.3.6/coreplus/contacts/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/api/v1/serializers.py` & `django-coreplus-0.3.6/coreplus/discuss/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/api/v1/viewsets.py` & `django-coreplus-0.3.6/coreplus/discuss/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/discuss/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/discuss/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/discuss/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/migrations/0002_alter_discuss_flag.py` & `django-coreplus-0.3.6/coreplus/discuss/migrations/0002_alter_discuss_flag.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/discuss/models.py` & `django-coreplus-0.3.6/coreplus/discuss/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/docs/templates/docs/_base_two.html` & `django-coreplus-0.3.6/coreplus/docs/templates/docs/_base_two.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/docs/tests/runtests.py` & `django-coreplus-0.3.6/coreplus/docs/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/docs/tests/test_views.py` & `django-coreplus-0.3.6/coreplus/docs/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/docs/views.py` & `django-coreplus-0.3.6/coreplus/docs/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/admin.py` & `django-coreplus-0.3.6/coreplus/heralds/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/api/v1/serializers.py` & `django-coreplus-0.3.6/coreplus/heralds/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/api/v1/viewsets.py` & `django-coreplus-0.3.6/coreplus/heralds/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/heralds/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/heralds/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/heralds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/models.py` & `django-coreplus-0.3.6/coreplus/heralds/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/heralds/tests.py` & `django-coreplus-0.3.6/coreplus/heralds/tests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/hooks/README.md` & `django-coreplus-0.3.6/coreplus/hooks/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/hooks/admin.py` & `django-coreplus-0.3.6/coreplus/hooks/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/hooks/core.py` & `django-coreplus-0.3.6/coreplus/hooks/core.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/hooks/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/hooks/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html` & `django-coreplus-0.3.6/coreplus/hooks/templates/admin/coreplus_hooks/hooks_registry.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/__init__.py` & `django-coreplus-0.3.6/coreplus/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/bleaching.py` & `django-coreplus-0.3.6/coreplus/markdown/bleaching.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/markdown/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/markdown/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/plugins/gist.py` & `django-coreplus-0.3.6/coreplus/markdown/plugins/gist.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/plugins/linkify.py` & `django-coreplus-0.3.6/coreplus/markdown/plugins/linkify.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/plugins/twitter.py` & `django-coreplus-0.3.6/coreplus/markdown/plugins/twitter.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/plugins/youtube.py` & `django-coreplus-0.3.6/coreplus/markdown/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/markdown/tests.py` & `django-coreplus-0.3.6/coreplus/markdown/tests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/api/v1/serializers.py` & `django-coreplus-0.3.6/coreplus/media/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/api/v1/viewsets.py` & `django-coreplus-0.3.6/coreplus/media/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/helpers.py` & `django-coreplus-0.3.6/coreplus/media/helpers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/media/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/media/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/media/models.py` & `django-coreplus-0.3.6/coreplus/media/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/README.md` & `django-coreplus-0.3.6/coreplus/navigators/README.md`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/apps.py` & `django-coreplus-0.3.6/coreplus/navigators/apps.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/navigators/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/navigators/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/navigators/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/models.py` & `django-coreplus-0.3.6/coreplus/navigators/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/navigators/templatetags/navigators_tags.py` & `django-coreplus-0.3.6/coreplus/navigators/templatetags/navigators_tags.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/admin.py` & `django-coreplus-0.3.6/coreplus/notices/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/api/v1/serializers.py` & `django-coreplus-0.3.6/coreplus/notices/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/api/v1/urls.py` & `django-coreplus-0.3.6/coreplus/notices/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/api/v1/viewsets.py` & `django-coreplus-0.3.6/coreplus/notices/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/notices/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/notices/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/notices/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py` & `django-coreplus-0.3.6/coreplus/notices/migrations/0002_remove_broadcast_recipient_broadcast_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/notices/models.py` & `django-coreplus-0.3.6/coreplus/notices/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/numerators/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/numerators/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/numerators/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/numerators/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/numerators/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/numerators/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/numerators/models.py` & `django-coreplus-0.3.6/coreplus/numerators/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/profanity/extras.py` & `django-coreplus-0.3.6/coreplus/profanity/extras.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/profanity/wordlist.txt` & `django-coreplus-0.3.6/coreplus/profanity/wordlist.txt`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/qrcodes/models.py` & `django-coreplus-0.3.6/coreplus/qrcodes/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/reactions/admin.py` & `django-coreplus-0.3.6/coreplus/reactions/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/reactions/api/v1/serializers.py` & `django-coreplus-0.3.6/coreplus/reactions/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/reactions/apps.py` & `django-coreplus-0.3.6/coreplus/reactions/apps.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/reactions/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/reactions/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/reactions/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/reactions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/reactions/models.py` & `django-coreplus-0.3.6/coreplus/reactions/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/search/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/search/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/search/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/search/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/search/templates/search/search.html` & `django-coreplus-0.3.6/coreplus/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/search/templatetags/search_tags.py` & `django-coreplus-0.3.6/coreplus/search/templatetags/search_tags.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/search/views.py` & `django-coreplus-0.3.6/coreplus/search/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/admin.py` & `django-coreplus-0.3.6/coreplus/settings/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/contexts.py` & `django-coreplus-0.3.6/coreplus/settings/contexts.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/locale/id/LC_MESSAGES/django.mo` & `django-coreplus-0.3.6/coreplus/settings/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/settings/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/models.py` & `django-coreplus-0.3.6/coreplus/settings/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/permissions.py` & `django-coreplus-0.3.6/coreplus/settings/permissions.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/registries.py` & `django-coreplus-0.3.6/coreplus/settings/registries.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/templates/admin/settings/edit.html` & `django-coreplus-0.3.6/coreplus/settings/templates/admin/settings/edit.html`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/templatetags/settings_tags.py` & `django-coreplus-0.3.6/coreplus/settings/templatetags/settings_tags.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/settings/views.py` & `django-coreplus-0.3.6/coreplus/settings/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/shorts/api/v1/viewsets.py` & `django-coreplus-0.3.6/coreplus/shorts/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/shorts/locale/id/LC_MESSAGES/django.po` & `django-coreplus-0.3.6/coreplus/shorts/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/shorts/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/shorts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/shorts/models.py` & `django-coreplus-0.3.6/coreplus/shorts/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/shorts/utils.py` & `django-coreplus-0.3.6/coreplus/shorts/utils.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/shorts/views.py` & `django-coreplus-0.3.6/coreplus/shorts/views.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/spams/extras.py` & `django-coreplus-0.3.6/coreplus/spams/extras.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl` & `django-coreplus-0.3.6/coreplus/spams/static/model_and_vectorizer_with_pickle(en).pkl`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl` & `django-coreplus-0.3.6/coreplus/spams/static/model_and_vectorizer_with_pickle(id).pkl`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/spams/tests.py` & `django-coreplus-0.3.6/coreplus/spams/tests.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/tags/admin.py` & `django-coreplus-0.3.6/coreplus/tags/admin.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/tags/api/v1/serializers.py` & `django-coreplus-0.3.6/coreplus/tags/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/tags/api/v1/viewsets.py` & `django-coreplus-0.3.6/coreplus/tags/api/v1/viewsets.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,12 +21,12 @@
     filter_backends = [SearchFilter]
     search_fields = ["@name"]
 
 
 class CategoryViewSet(ReadOnlyModelViewSet):
     authentication_classes = []
     permission_classes = []
-    queryset = Category.objects.all()
+    queryset = Category.objects.all().order_by("name")
     serializer_class = serializers.CategorySerializer
     filter_backends = [SearchFilter, OrderingFilter]
     search_fields = ["@name"]
-    ordering_fields = ["pk", "name"]
+    ordering_fields = ["pk", "name", "order"]
```

### Comparing `django-coreplus-0.3.5/coreplus/tags/migrations/0001_initial.py` & `django-coreplus-0.3.6/coreplus/tags/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/tags/models.py` & `django-coreplus-0.3.6/coreplus/tags/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/tags/resources.py` & `django-coreplus-0.3.6/coreplus/tags/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,13 +13,18 @@
         widget=CharWidget(),
     )
     parent = Field(
         attribute="parent",
         column_name="parent",
         widget=ForeignKeyWidget(Category, field="slug"),
     )
+    category_id = Field(
+        attribute="category_id",
+        column_name="category_id",
+        widget=CharWidget(),
+    )
 
     class Meta:
         model = Category
         exclude = ("lft", "rght", "tree_id", "level")
-        export_order = ("id", "name", "slug", "parent")
+        export_order = ("id", "name", "slug", "parent", "category_id")
         import_id_fields = ("slug",)
```

### Comparing `django-coreplus-0.3.5/coreplus/utils/avatars.py` & `django-coreplus-0.3.6/coreplus/utils/avatars.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/contenttypes.py` & `django-coreplus-0.3.6/coreplus/utils/contenttypes.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/currencies.py` & `django-coreplus-0.3.6/coreplus/utils/currencies.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/decorators.py` & `django-coreplus-0.3.6/coreplus/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/forms/fields.py` & `django-coreplus-0.3.6/coreplus/utils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/loading.py` & `django-coreplus-0.3.6/coreplus/utils/loading.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/actions.py` & `django-coreplus-0.3.6/coreplus/utils/models/actions.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/choices.py` & `django-coreplus-0.3.6/coreplus/utils/models/choices.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/fields.py` & `django-coreplus-0.3.6/coreplus/utils/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/managers.py` & `django-coreplus-0.3.6/coreplus/utils/models/managers.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/models.py` & `django-coreplus-0.3.6/coreplus/utils/models/models.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/paranoid.py` & `django-coreplus-0.3.6/coreplus/utils/models/paranoid.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/signals.py` & `django-coreplus-0.3.6/coreplus/utils/models/signals.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/models/tracker.py` & `django-coreplus-0.3.6/coreplus/utils/models/tracker.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/slugs.py` & `django-coreplus-0.3.6/coreplus/utils/slugs.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/utils/validators.py` & `django-coreplus-0.3.6/coreplus/utils/validators.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/coreplus/version.py` & `django-coreplus-0.3.6/coreplus/version.py`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/django_coreplus.egg-info/PKG-INFO` & `django-coreplus-0.3.6/django_coreplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-coreplus
-Version: 0.3.5
+Version: 0.3.6
 Summary: Django functional modules
 Home-page: https://gitlab.com/zeroplus/django/django-coreplus
 Author: Zero Plus
 Author-email: sasri.works@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/zeroplus/django/django-coreplus/-/wikis/
 Project-URL: Source, https://gitlab.com/zeroplus/django/django-coreplus
```

### Comparing `django-coreplus-0.3.5/django_coreplus.egg-info/SOURCES.txt` & `django-coreplus-0.3.6/django_coreplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-coreplus-0.3.5/setup.cfg` & `django-coreplus-0.3.6/setup.cfg`

 * *Files identical despite different names*

