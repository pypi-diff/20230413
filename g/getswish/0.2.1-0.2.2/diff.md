# Comparing `tmp/getswish-0.2.1.tar.gz` & `tmp/getswish-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getswish-0.2.1.tar", last modified: Thu Apr 13 10:30:08 2023, max compression
+gzip compressed data, was "getswish-0.2.2.tar", last modified: Thu Apr 13 14:21:06 2023, max compression
```

## Comparing `getswish-0.2.1.tar` & `getswish-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      482 2023-04-12 11:58:42.537958 getswish-0.2.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0       82 2023-04-12 10:53:14.553712 getswish-0.2.1/.gitignore
--rw-r--r--   0        0        0      681 2023-04-13 10:29:07.997032 getswish-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-12 05:47:29.766259 getswish-0.2.1/LICENSE
--rw-r--r--   0        0        0     4598 2023-04-12 12:21:45.694971 getswish-0.2.1/README.md
--rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
--rw-r--r--   0        0        0     3247 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
--rw-r--r--   0        0        0     7165 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
--rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
--rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
--rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
--rw-r--r--   0        0        0     1338 2023-04-13 10:14:48.087458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
--rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
--rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
--rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
--rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.087458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
--rw-r--r--   0        0        0     1752 2023-04-12 05:47:28.906216 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
--rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.870215 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
--rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.830213 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
--rw-r--r--   0        0        0     6009 2023-04-12 05:47:28.346189 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
--rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/mss.p12
--rw-r--r--   0        0        0   464323 2023-04-12 05:47:28.194182 getswish-0.2.1/mss_test_1.9/MSS_UserGuide_v1.9.pdf
--rw-r--r--   0        0        0     2565 2023-04-12 05:47:27.938169 getswish-0.2.1/mss_test_1.9/readme.md
--rw-r--r--   0        0        0      312 2023-04-13 09:51:33.541983 getswish-0.2.1/noxfile.py
--rw-r--r--   0        0        0     1567 2023-04-12 13:00:29.698021 getswish-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-13 10:28:12.126435 getswish-0.2.1/src/getswish/__init__.py
--rw-r--r--   0        0        0     6560 2023-04-13 10:24:03.416266 getswish-0.2.1/src/getswish/client.py
--rw-r--r--   0        0        0     1108 2023-04-13 10:08:49.875599 getswish-0.2.1/src/getswish/environments.py
--rw-r--r--   0        0        0      249 2023-04-12 05:47:29.574250 getswish-0.2.1/src/getswish/exceptions.py
--rw-r--r--   0        0        0     2914 2023-04-12 05:47:29.274235 getswish-0.2.1/src/getswish/models.py
--rw-r--r--   0        0        0     1109 2023-04-12 05:47:29.686255 getswish-0.2.1/src/getswish/utils.py
--rw-r--r--   0        0        0        0 2023-04-12 05:47:30.218282 getswish-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     5186 2023-04-12 07:18:51.268043 getswish-0.2.1/tests/fixtures.py
--rw-r--r--   0        0        0     4089 2023-04-12 10:54:24.594831 getswish-0.2.1/tests/test_client.py
--rw-r--r--   0        0        0      832 2023-04-12 05:47:29.842263 getswish-0.2.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     1390 2023-04-12 10:53:53.850345 getswish-0.2.1/tests/test_models.py
--rw-r--r--   0        0        0     1695 2023-04-12 05:47:29.878265 getswish-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 getswish-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      482 2023-04-12 11:58:42.537958 getswish-0.2.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0       82 2023-04-12 10:53:14.553712 getswish-0.2.2/.gitignore
+-rw-r--r--   0        0        0      728 2023-04-13 14:19:43.719833 getswish-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-12 05:47:29.766259 getswish-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4598 2023-04-12 12:21:45.694971 getswish-0.2.2/README.md
+-rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3247 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
+-rw-r--r--   0        0        0     7165 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
+-rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1338 2023-04-13 10:14:48.087458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
+-rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
+-rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
+-rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
+-rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.087458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
+-rw-r--r--   0        0        0     1752 2023-04-12 05:47:28.906216 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
+-rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.870215 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
+-rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.830213 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
+-rw-r--r--   0        0        0     6009 2023-04-12 05:47:28.346189 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
+-rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/mss.p12
+-rw-r--r--   0        0        0   464323 2023-04-12 05:47:28.194182 getswish-0.2.2/mss_test_1.9/MSS_UserGuide_v1.9.pdf
+-rw-r--r--   0        0        0     2565 2023-04-12 05:47:27.938169 getswish-0.2.2/mss_test_1.9/readme.md
+-rw-r--r--   0        0        0      312 2023-04-13 09:51:33.541983 getswish-0.2.2/noxfile.py
+-rw-r--r--   0        0        0     1567 2023-04-12 13:00:29.698021 getswish-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-13 14:18:20.695328 getswish-0.2.2/src/getswish/__init__.py
+-rw-r--r--   0        0        0     6560 2023-04-13 10:24:03.416266 getswish-0.2.2/src/getswish/client.py
+-rw-r--r--   0        0        0     1112 2023-04-13 14:18:09.287262 getswish-0.2.2/src/getswish/environments.py
+-rw-r--r--   0        0        0      249 2023-04-12 05:47:29.574250 getswish-0.2.2/src/getswish/exceptions.py
+-rw-r--r--   0        0        0     2914 2023-04-12 05:47:29.274235 getswish-0.2.2/src/getswish/models.py
+-rw-r--r--   0        0        0     1109 2023-04-12 05:47:29.686255 getswish-0.2.2/src/getswish/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:47:30.218282 getswish-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     5186 2023-04-12 07:18:51.268043 getswish-0.2.2/tests/fixtures.py
+-rw-r--r--   0        0        0     4089 2023-04-12 10:54:24.594831 getswish-0.2.2/tests/test_client.py
+-rw-r--r--   0        0        0      832 2023-04-12 05:47:29.842263 getswish-0.2.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1390 2023-04-12 10:53:53.850345 getswish-0.2.2/tests/test_models.py
+-rw-r--r--   0        0        0     1695 2023-04-12 05:47:29.878265 getswish-0.2.2/tests/test_utils.py
+-rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 getswish-0.2.2/PKG-INFO
```

### Comparing `getswish-0.2.1/CHANGELOG.md` & `getswish-0.2.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.2.1] - 2023-04-13
+## [0.2.2] - 2023-04-13
 
 ### Changed
 
+- Updated production environment default url.
 - Updated default test environment parameters.
 - Corrected project source url in pyproject.toml.
 
 ## [0.2.0] - 2023-04-12
 
 ###  Added
 
@@ -32,8 +33,8 @@
 
 - Added test cases.
 
 ## [0.1.1] - 2022-09-14
 
 ### Added
 
-- Initial version
+- Initial version
```

### Comparing `getswish-0.2.1/LICENSE` & `getswish-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/README.md` & `getswish-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/mss.p12` & `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/mss.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/MSS_UserGuide_v1.9.pdf` & `getswish-0.2.2/mss_test_1.9/MSS_UserGuide_v1.9.pdf`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/mss_test_1.9/readme.md` & `getswish-0.2.2/mss_test_1.9/readme.md`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/pyproject.toml` & `getswish-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/src/getswish/client.py` & `getswish-0.2.2/src/getswish/client.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/src/getswish/environments.py` & `getswish-0.2.2/src/getswish/environments.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 @dataclass
 class Environment:
     name: str
     base: str
 
 
 TestEnvironment = Environment(name="test", base="https://mss.cpc.getswish.net/swish-cpcapi/api/")
-ProductionEnvironment = Environment(name="production", base="https://cpc.getswish.net/swish-cpcapi/")
+ProductionEnvironment = Environment(name="production", base="https://cpc.getswish.net/swish-cpcapi/api/")
 
 TestCertificates = Certificates(
     Certificate(
         public=f"{cert_base}/Swish_Merchant_TestCertificate_1234679304.pem",
         private_key=f"{cert_base}/Swish_Merchant_TestCertificate_1234679304.key",
     ),
     Certificate(
```

### Comparing `getswish-0.2.1/src/getswish/models.py` & `getswish-0.2.2/src/getswish/models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/src/getswish/utils.py` & `getswish-0.2.2/src/getswish/utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/tests/fixtures.py` & `getswish-0.2.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/tests/test_client.py` & `getswish-0.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/tests/test_exceptions.py` & `getswish-0.2.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/tests/test_models.py` & `getswish-0.2.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/tests/test_utils.py` & `getswish-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.1/PKG-INFO` & `getswish-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getswish
-Version: 0.2.1
+Version: 0.2.2
 Summary: Getswish python client library
 Keywords: swish,getswish,payment,payout
 Author-email: Daniel Nibon <daniel@nibon.se>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

