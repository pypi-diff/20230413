# Comparing `tmp/getswish-0.2.0.tar.gz` & `tmp/getswish-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getswish-0.2.0.tar", last modified: Wed Apr 12 12:50:46 2023, max compression
+gzip compressed data, was "getswish-0.2.1.tar", last modified: Thu Apr 13 10:30:08 2023, max compression
```

## Comparing `getswish-0.2.0.tar` & `getswish-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      482 2023-04-12 11:58:42.537958 getswish-0.2.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0       82 2023-04-12 10:53:14.553712 getswish-0.2.0/.gitignore
--rw-r--r--   0        0        0      545 2023-04-12 10:52:28.828960 getswish-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-12 05:47:29.766259 getswish-0.2.0/LICENSE
--rw-r--r--   0        0        0     4598 2023-04-12 12:21:45.694971 getswish-0.2.0/README.md
--rw-r--r--   0        0        0     1700 2023-04-12 05:47:28.634203 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
--rw-r--r--   0        0        0     3247 2023-04-12 05:47:28.382191 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
--rw-r--r--   0        0        0     7165 2023-04-12 05:47:28.594201 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-04-12 05:47:28.550199 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
--rw-r--r--   0        0        0     1700 2023-04-12 05:47:28.942218 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
--rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.674205 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
--rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.462195 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-04-12 05:47:28.750209 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
--rw-r--r--   0        0        0     1338 2023-04-12 05:47:28.714207 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
--rw-r--r--   0        0        0     1700 2023-04-12 05:47:28.306187 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
--rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.418193 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
--rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.506197 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
--rw-r--r--   0        0        0     6006 2023-04-12 05:47:28.790211 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
--rw-r--r--   0        0        0     1752 2023-04-12 05:47:28.906216 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
--rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.870215 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
--rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.830213 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
--rw-r--r--   0        0        0     6009 2023-04-12 05:47:28.346189 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
--rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.270186 getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/mss.p12
--rw-r--r--   0        0        0   464323 2023-04-12 05:47:28.194182 getswish-0.2.0/mss_test_1.9/MSS_UserGuide_v1.9.pdf
--rw-r--r--   0        0        0     2565 2023-04-12 05:47:27.938169 getswish-0.2.0/mss_test_1.9/readme.md
--rw-r--r--   0        0        0      312 2023-04-12 12:01:16.027864 getswish-0.2.0/noxfile.py
--rw-r--r--   0        0        0     1559 2023-04-12 12:31:41.642105 getswish-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-12 12:38:28.701423 getswish-0.2.0/src/getswish/__init__.py
--rw-r--r--   0        0        0     6451 2023-04-12 10:31:57.423123 getswish-0.2.0/src/getswish/client.py
--rw-r--r--   0        0        0      668 2023-04-12 07:16:33.425724 getswish-0.2.0/src/getswish/environments.py
--rw-r--r--   0        0        0      249 2023-04-12 05:47:29.574250 getswish-0.2.0/src/getswish/exceptions.py
--rw-r--r--   0        0        0     2914 2023-04-12 05:47:29.274235 getswish-0.2.0/src/getswish/models.py
--rw-r--r--   0        0        0     1109 2023-04-12 05:47:29.686255 getswish-0.2.0/src/getswish/utils.py
--rw-r--r--   0        0        0        0 2023-04-12 05:47:30.218282 getswish-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5186 2023-04-12 07:18:51.268043 getswish-0.2.0/tests/fixtures.py
--rw-r--r--   0        0        0     4089 2023-04-12 10:54:24.594831 getswish-0.2.0/tests/test_client.py
--rw-r--r--   0        0        0      832 2023-04-12 05:47:29.842263 getswish-0.2.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     1390 2023-04-12 10:53:53.850345 getswish-0.2.0/tests/test_models.py
--rw-r--r--   0        0        0     1695 2023-04-12 05:47:29.878265 getswish-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 getswish-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      482 2023-04-12 11:58:42.537958 getswish-0.2.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0       82 2023-04-12 10:53:14.553712 getswish-0.2.1/.gitignore
+-rw-r--r--   0        0        0      681 2023-04-13 10:29:07.997032 getswish-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-12 05:47:29.766259 getswish-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4598 2023-04-12 12:21:45.694971 getswish-0.2.1/README.md
+-rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3247 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
+-rw-r--r--   0        0        0     7165 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
+-rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1338 2023-04-13 10:14:48.087458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
+-rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
+-rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
+-rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
+-rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.087458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
+-rw-r--r--   0        0        0     1752 2023-04-12 05:47:28.906216 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
+-rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.870215 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
+-rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.830213 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
+-rw-r--r--   0        0        0     6009 2023-04-12 05:47:28.346189 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
+-rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/mss.p12
+-rw-r--r--   0        0        0   464323 2023-04-12 05:47:28.194182 getswish-0.2.1/mss_test_1.9/MSS_UserGuide_v1.9.pdf
+-rw-r--r--   0        0        0     2565 2023-04-12 05:47:27.938169 getswish-0.2.1/mss_test_1.9/readme.md
+-rw-r--r--   0        0        0      312 2023-04-13 09:51:33.541983 getswish-0.2.1/noxfile.py
+-rw-r--r--   0        0        0     1567 2023-04-12 13:00:29.698021 getswish-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-04-13 10:28:12.126435 getswish-0.2.1/src/getswish/__init__.py
+-rw-r--r--   0        0        0     6560 2023-04-13 10:24:03.416266 getswish-0.2.1/src/getswish/client.py
+-rw-r--r--   0        0        0     1108 2023-04-13 10:08:49.875599 getswish-0.2.1/src/getswish/environments.py
+-rw-r--r--   0        0        0      249 2023-04-12 05:47:29.574250 getswish-0.2.1/src/getswish/exceptions.py
+-rw-r--r--   0        0        0     2914 2023-04-12 05:47:29.274235 getswish-0.2.1/src/getswish/models.py
+-rw-r--r--   0        0        0     1109 2023-04-12 05:47:29.686255 getswish-0.2.1/src/getswish/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:47:30.218282 getswish-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     5186 2023-04-12 07:18:51.268043 getswish-0.2.1/tests/fixtures.py
+-rw-r--r--   0        0        0     4089 2023-04-12 10:54:24.594831 getswish-0.2.1/tests/test_client.py
+-rw-r--r--   0        0        0      832 2023-04-12 05:47:29.842263 getswish-0.2.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1390 2023-04-12 10:53:53.850345 getswish-0.2.1/tests/test_models.py
+-rw-r--r--   0        0        0     1695 2023-04-12 05:47:29.878265 getswish-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 getswish-0.2.1/PKG-INFO
```

### Comparing `getswish-0.2.0/CHANGELOG.md` & `getswish-0.2.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.1] - 2023-04-13
+
+### Changed
+
+- Updated default test environment parameters.
+- Corrected project source url in pyproject.toml.
+
 ## [0.2.0] - 2023-04-12
 
 ###  Added
 
 - Added nox.
 
 ### Changed
```

### Comparing `getswish-0.2.0/LICENSE` & `getswish-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/README.md` & `getswish-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/Getswish_Test_Certificates/mss.p12` & `getswish-0.2.1/mss_test_1.9/Getswish_Test_Certificates/mss.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/MSS_UserGuide_v1.9.pdf` & `getswish-0.2.1/mss_test_1.9/MSS_UserGuide_v1.9.pdf`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/mss_test_1.9/readme.md` & `getswish-0.2.1/mss_test_1.9/readme.md`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/pyproject.toml` & `getswish-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
-Source = "https://github.com/nibon/getswish"
+Source = "https://github.com/nibon/getswish-python"
 
 [project.optional-dependencies]
 tests = [
     "pytest >= 7",
     "pytest-mock",
     "pytest-cov >= 4",
     "ruff",
@@ -60,8 +60,8 @@
     "node_modules",
 ]
 line-length = 120
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 target-version = "py311"
 
 [tool.ruff.mccabe]
-max-complexity = 10
+max-complexity = 10
```

### Comparing `getswish-0.2.0/src/getswish/client.py` & `getswish-0.2.1/src/getswish/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import base64
 import hashlib
 import json
 from dataclasses import dataclass
 from datetime import datetime
-from pathlib import Path
 
 import requests
 import rsa
 from requests import Response
 
-from .environments import Certificates, Environment
+from .environments import Certificates, Environment, TestEnvironment, TestCertificates
 from .exceptions import SwishError
 from .models import Payment, Payout, Refund
 from .utils import generate_transaction_id
 
-cert_base = Path(__file__).parent.parent.parent.resolve() / "mss_test_1.9" / "Getswish_Test_Certificates"
-
 
 @dataclass
 class SwishClient:
-    environment: Environment
-    certificates: Certificates
-    merchant_swish_number: str = "12345679304"
+    environment: Environment = None
+    certificates: Certificates = None
+    merchant_swish_number: str = "1234679304"
+
+    def __post_init__(self):
+        if self.environment is None and self.certificates is None:
+            self.environment = TestEnvironment
+            self.certificates = TestCertificates
 
     def _url(self, version: str, path: str) -> str:
         return f"{self.environment.base}{version}{path}"
 
     def _requests(self, method: str, url: str, /, **kwargs) -> Response:
         """Requests wrapper that add client certificates and handles api errors and raise http status errors."""
```

### Comparing `getswish-0.2.0/src/getswish/environments.py` & `getswish-0.2.1/src/getswish/environments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 from dataclasses import dataclass, field
+from pathlib import Path
+
+cert_base = Path(__file__).parent.parent.parent.resolve() / "mss_test_1.9" / "Getswish_Test_Certificates"
 
 
 @dataclass
 class Certificate:
     public: str = None
     private_key: str = None
     public_serial: str = None
 
 
 @dataclass
 class Certificates:
     communication: Certificate | None = field(repr=False)  # cert, private key
     verify: Certificate | None = field(repr=False)  # cert
-    signing: Certificate | None = field(repr=False)  # cert, private key, serial
+    signing: Certificate | None = field(repr=False, default=None)  # cert, private key, serial
 
 
 @dataclass
 class Environment:
     name: str
     base: str
 
 
 TestEnvironment = Environment(name="test", base="https://mss.cpc.getswish.net/swish-cpcapi/api/")
 ProductionEnvironment = Environment(name="production", base="https://cpc.getswish.net/swish-cpcapi/")
+
+TestCertificates = Certificates(
+    Certificate(
+        public=f"{cert_base}/Swish_Merchant_TestCertificate_1234679304.pem",
+        private_key=f"{cert_base}/Swish_Merchant_TestCertificate_1234679304.key",
+    ),
+    Certificate(
+        public=f"{cert_base}/Swish_TLS_RootCA.pem"
+    ),
+)
```

### Comparing `getswish-0.2.0/src/getswish/models.py` & `getswish-0.2.1/src/getswish/models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/src/getswish/utils.py` & `getswish-0.2.1/src/getswish/utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/tests/fixtures.py` & `getswish-0.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/tests/test_client.py` & `getswish-0.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/tests/test_exceptions.py` & `getswish-0.2.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/tests/test_models.py` & `getswish-0.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/tests/test_utils.py` & `getswish-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.0/PKG-INFO` & `getswish-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getswish
-Version: 0.2.0
+Version: 0.2.1
 Summary: Getswish python client library
 Keywords: swish,getswish,payment,payout
 Author-email: Daniel Nibon <daniel@nibon.se>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Requires-Dist: requests >= 2.27
 Requires-Dist: rsa >= 4.7.2
 Requires-Dist: flit >= 3.8 ; extra == "deploy"
 Requires-Dist: pytest >= 7 ; extra == "tests"
 Requires-Dist: pytest-mock ; extra == "tests"
 Requires-Dist: pytest-cov >= 4 ; extra == "tests"
 Requires-Dist: ruff ; extra == "tests"
-Project-URL: Source, https://github.com/nibon/getswish
+Project-URL: Source, https://github.com/nibon/getswish-python
 Provides-Extra: deploy
 Provides-Extra: tests
 
 # Swish - Python client
 
 Client library to integrate with the swish commerce and payout api.
```

