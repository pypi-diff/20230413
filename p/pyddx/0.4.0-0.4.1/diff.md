# Comparing `tmp/pyddx-0.4.0.tar.gz` & `tmp/pyddx-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyddx-0.4.0.tar", last modified: Thu Apr 13 15:40:00 2023, max compression
+gzip compressed data, was "pyddx-0.4.1.tar", last modified: Thu Apr 13 15:40:02 2023, max compression
```

## Comparing `pyddx-0.4.0.tar` & `pyddx-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:00.116902 pyddx-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-13 15:37:28.000000 pyddx-0.4.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-13 15:37:28.000000 pyddx-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 15:37:28.000000 pyddx-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 15:40:00.116902 pyddx-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 15:37:28.000000 pyddx-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:00.108902 pyddx-0.4.0/pyddx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 15:40:00.000000 pyddx-0.4.0/pyddx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 15:40:00.000000 pyddx-0.4.0/pyddx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:40:00.000000 pyddx-0.4.0/pyddx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:37:41.000000 pyddx-0.4.0/pyddx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 15:40:00.000000 pyddx-0.4.0/pyddx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 15:40:00.000000 pyddx-0.4.0/pyddx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 15:37:28.000000 pyddx-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 15:40:00.116902 pyddx-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-04-13 15:37:28.000000 pyddx-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:00.116902 pyddx-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/cbessel.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx.f90
--rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx.h
--rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_cinterface.f90
--rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_constants.f90
--rw-r--r--   0 runner    (1001) docker     (123)   120346 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_cosmo.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_definitions.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_driver.f90
--rw-r--r--   0 runner    (1001) docker     (123)    82968 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_gradients.f90
--rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_harmonics.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_lpb.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_lpb_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_mkrhs.f90
--rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_multipolar_solutes.f90
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_operators.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_parameters.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_pcm.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_solvers.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/ddx_workspace.f90
--rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/llgnew.f
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/matrix_debug.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/pyddx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/pyddx_classes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-04-13 15:37:28.000000 pyddx-0.4.0/src/pyddx_data.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:02.739338 pyddx-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-13 15:37:32.000000 pyddx-0.4.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-13 15:37:32.000000 pyddx-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 15:37:32.000000 pyddx-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 15:40:02.739338 pyddx-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 15:37:32.000000 pyddx-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:02.731337 pyddx-0.4.1/pyddx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:37:44.000000 pyddx-0.4.1/pyddx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 15:40:02.000000 pyddx-0.4.1/pyddx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 15:37:32.000000 pyddx-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 15:40:02.739338 pyddx-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-04-13 15:37:32.000000 pyddx-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:40:02.739338 pyddx-0.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/cbessel.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_cinterface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_constants.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   120346 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_cosmo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_definitions.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_driver.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    82968 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_gradients.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_harmonics.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_lpb.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_lpb_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_mkrhs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_multipolar_solutes.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_operators.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_pcm.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_solvers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/ddx_workspace.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/llgnew.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/matrix_debug.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/pyddx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/pyddx_classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-04-13 15:37:32.000000 pyddx-0.4.1/src/pyddx_data.cpp
```

### Comparing `pyddx-0.4.0/CMakeLists.txt` & `pyddx-0.4.1/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Restrict building in top-level directory
 if("${CMAKE_CURRENT_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_BINARY_DIR}")
     message(FATAL_ERROR "In-source builds are not allowed.\nPlease create a "
         "build directory first and execute cmake configuration from this "
         "directory. Example: mkdir build && cd build && cmake ..")
 endif()
 
-project(ddX VERSION 0.4.0 LANGUAGES Fortran CXX)
+project(ddX VERSION 0.4.1 LANGUAGES Fortran CXX)
 # If ddX is a subproject, append ddx_ prefix to all targets.
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
     set(ddx_is_subproject false)
     set(ddx_ "")
 else()
     set(ddx_is_subproject true)
     set(ddx_ "ddx_")
```

### Comparing `pyddx-0.4.0/LICENSE.txt` & `pyddx-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/PKG-INFO` & `pyddx-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.0
+Version: 0.4.1
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.0/README.md` & `pyddx-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/pyddx.egg-info/PKG-INFO` & `pyddx-0.4.1/pyddx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.0
+Version: 0.4.1
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.0/pyddx.egg-info/SOURCES.txt` & `pyddx-0.4.1/pyddx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/setup.py` & `pyddx-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyddx",
     description="ddx continuum solvation library",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
-    version="0.4.0",
+    version="0.4.1",
     #
     author="ddx developers",
     author_email="best@ians.uni-stuttgart.de",
     license="LGPL v3",
     url="https://ddsolvation.github.io/ddX",
     project_urls={
         "Source": "https://github.com/ddsolvation/ddX",
```

### Comparing `pyddx-0.4.0/src/CMakeLists.txt` & `pyddx-0.4.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/cbessel.f90` & `pyddx-0.4.1/src/cbessel.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx.f90` & `pyddx-0.4.1/src/ddx.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx.h` & `pyddx-0.4.1/src/ddx.h`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_cinterface.f90` & `pyddx-0.4.1/src/ddx_cinterface.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_constants.f90` & `pyddx-0.4.1/src/ddx_constants.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_core.f90` & `pyddx-0.4.1/src/ddx_core.f90`

 * *Files 0% similar despite different names*

```diff
@@ -2957,15 +2957,15 @@
 !!
 !! @param[out] string: container for the logo
 !!
 subroutine get_banner(string)
     implicit none
     character (len=2047), intent(out) :: string
     character (len=10) :: vstr
-    write(vstr, *) "0.4.0"
+    write(vstr, *) "0.4.1"
     write(string, *) &
         & " +----------------------------------------------------------------+", &
         & NEW_LINE('a'), &
         & "  |                                                                |", &
         & NEW_LINE('a'), &
         & "  |                        888      888 Y8b    d8Y                 |", &
         & NEW_LINE('a'), &
```

### Comparing `pyddx-0.4.0/src/ddx_cosmo.f90` & `pyddx-0.4.1/src/ddx_cosmo.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_definitions.f90` & `pyddx-0.4.1/src/ddx_definitions.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_driver.f90` & `pyddx-0.4.1/src/ddx_driver.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_gradients.f90` & `pyddx-0.4.1/src/ddx_gradients.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_harmonics.f90` & `pyddx-0.4.1/src/ddx_harmonics.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_lpb.f90` & `pyddx-0.4.1/src/ddx_lpb.f90`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,20 @@
     type(ddx_state_type), intent(inout) :: state
     real(dp), intent(in) :: phi_cav(constants % ncav)
     real(dp), intent(in) :: e_cav(3, constants % ncav)
     real(dp), intent(in) :: psi(constants % nbasis, params % nsph)
 
     state % psi = psi
     state % rhs_adj_lpb(:, :, 1) = psi
+    ! in ddLPB the polarization density X is expanded according to a
+    ! slightly different definition which lacks the 4pi/(2l + 1) factors
+    ! which are present in ddCOSMO and ddPCM. This affect the adjoint
+    ! density as well. To have a consistent adjoint density with ddCOSMO
+    ! and ddPCM, we have to scale the RHS.
+    call convert_ddcosmo(params, constants, -1, state % rhs_adj_lpb(:,:,1))
     state % rhs_adj_lpb(:, :, 2) = 0.0d0
 
     !! Setting initial values to zero
     state % g_lpb = zero
     state % f_lpb = zero
     state % phi_grid = zero
 
@@ -147,15 +153,14 @@
 !!
 subroutine ddlpb_energy(constants, state, esolv)
     implicit none
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_state_type), intent(in) :: state
     real(dp), intent(out) :: esolv
     real(dp), external :: ddot
-    ! TODO: sort once and for all the fourpi issue
     esolv = pt5*ddot(constants % n, state % x_lpb(:,:,1), 1, state % psi, 1)
 end subroutine ddlpb_energy
 
 !> Do a guess for the primal ddLPB linear system
 !!
 !> @ingroup Fortran_interface_ddlpb
 !! @param[in] params: User specified parameters
@@ -175,15 +180,14 @@
     ! set the inner tolerance
     constants % inner_tol =  sqrt(tol)
 
     ! guess
     workspace % ddcosmo_guess = zero
     workspace % hsp_guess = zero
     call prec_tx(params, constants, workspace, state % rhs_lpb, state % x_lpb)
-    state % x_lpb = state % x_lpb / fourpi
 
 end subroutine ddlpb_guess
 
 !> Do a guess for the adjoint ddLPB linear system
 !!
 !> @ingroup Fortran_interface_ddlpb
 !! @param[in] params: User specified parameters
@@ -205,15 +209,14 @@
 
     ! guess
     workspace % ddcosmo_guess = zero
     workspace % hsp_guess = zero
     call prec_tstarx(params, constants, workspace, state % rhs_adj_lpb, &
         & state % x_adj_lpb)
 
-    state % x_adj_lpb = state % x_adj_lpb / fourpi
 end subroutine ddlpb_guess_adjoint
 
 !> Solve the ddLPB primal linear system
 !!
 !> @ingroup Fortran_interface_ddlpb
 !! @param[in] params       : General options
 !! @param[in] constants    : Precomputed constants
@@ -227,30 +230,32 @@
     type(ddx_constants_type), intent(inout) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     type(ddx_state_type), intent(inout) :: state
     real(dp), intent(in) :: tol
     real(dp) :: start_time
 
     state % x_lpb_niter = params % maxiter
-    state % x_lpb = state % x_lpb * fourpi
 
     ! solve LS using Jacobi/DIIS
     start_time = omp_get_wtime()
     call jacobi_diis_external(params, constants, workspace, &
         & 2*constants % n, tol, state % rhs_lpb, state % x_lpb, &
         & state % x_lpb_niter, state % x_lpb_rel_diff, cx, prec_tx, rmsnorm)
     if (workspace % error_flag .ne. 0) then
         workspace % error_message = 'Jacobi solver failed to converge " // &
             & "in ddlpb_solve'
         return
     end if
     state % x_lpb_time = omp_get_wtime() - start_time
-    ! the integral operators of ddLPB are defined according to a
-    ! different convention, so we need to scale the density by 1/fourpi
-    state % x_lpb = state % x_lpb / fourpi
+    ! in ddLPB the polarization density X is expanded according to a
+    ! slightly different definition which lacks the 4pi/(2l + 1) factors
+    ! which are present in ddCOSMO and ddPCM. Before exiting, we scale
+    ! the density so that it is consistent with the ddCOSMO and ddPCM
+    ! ones.
+    call convert_ddcosmo(params, constants, -1, state % x_lpb(:,:,1))
 end subroutine ddlpb_solve
 
 
 !> Solve the adjoint ddLPB linear system
 !!
 !> @ingroup Fortran_interface_ddlpb
 !! @param[in] params       : General options
@@ -268,32 +273,27 @@
     real(dp), intent(in) :: tol
 
     real(dp) :: start_time
 
     state % x_adj_lpb_niter = params % maxiter
     constants % inner_tol = sqrt(tol)
 
-    state % x_adj_lpb = state % x_adj_lpb * fourpi
-
     ! solve adjoint LS using Jacobi/DIIS
     start_time = omp_get_wtime()
     call jacobi_diis_external(params, constants, workspace, &
         & 2*constants % n, tol, state % rhs_adj_lpb, state % x_adj_lpb, &
         & state % x_adj_lpb_niter, state % x_adj_lpb_rel_diff, &
         & cstarx, prec_tstarx, rmsnorm)
     if (workspace % error_flag .ne. 0) then
         workspace % error_message = 'Jacobi solver failed to ' // &
             & 'converge in ddlpb_solve_adjoint'
         return
     end if
     state % x_adj_lpb_time = omp_get_wtime() - start_time
-    ! the integral operators of ddLPB are defined according to a
-    ! different convention, so we need to scale the adjoint density
-    ! by 1/fourpi
-    state % x_adj_lpb = state % x_adj_lpb / fourpi
+
 end subroutine ddlpb_solve_adjoint
 
 !!
 !! Wrapper routine for the computation of ddPCM forces. It makes the
 !! interface easier to implement. If a fine control is needed, the
 !! worker routine should be directly called.
 !!
@@ -336,15 +336,16 @@
         & scaled_xr(constants % nbasis, params % nsph), stat=istat)
     if (istat.ne.0) then
         workspace % error_message = 'Allocation failed in ddlpb_force_worker'
         workspace % error_flag = 1
         return
     end if
 
-    state % x_lpb = state % x_lpb * fourpi
+    ! we have to insert again the factor that we removed in ddlpb_solve
+    call convert_ddcosmo(params, constants, 1, state % x_lpb(:, :, 1))
 
     diff_re = zero
     vsin = zero
     vcos = zero
     vplm = zero
     basloc = zero
     dbasloc = zero
@@ -436,13 +437,14 @@
         workspace % error_message = 'Deallocation failed in ddlpb_force_worker'
         workspace % error_flag = 1
         return
     end if
     finish_time = omp_get_wtime()
     state % force_time = finish_time - start_time
 
-    ! restore x_lpb
-    state % x_lpb = state % x_lpb / fourpi
+    ! and now we remove again the factor, so that the density is
+    ! restored.
+    call convert_ddcosmo(params, constants, -1, state % x_lpb(:, :, 1))
 
 end subroutine ddlpb_solvation_force_terms
 
 end module ddx_lpb
```

### Comparing `pyddx-0.4.0/src/ddx_lpb_core.f90` & `pyddx-0.4.1/src/ddx_lpb_core.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_mkrhs.f90` & `pyddx-0.4.1/src/ddx_mkrhs.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_multipolar_solutes.f90` & `pyddx-0.4.1/src/ddx_multipolar_solutes.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_operators.f90` & `pyddx-0.4.1/src/ddx_operators.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_parameters.f90` & `pyddx-0.4.1/src/ddx_parameters.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_pcm.f90` & `pyddx-0.4.1/src/ddx_pcm.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_solvers.f90` & `pyddx-0.4.1/src/ddx_solvers.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/ddx_workspace.f90` & `pyddx-0.4.1/src/ddx_workspace.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/llgnew.f` & `pyddx-0.4.1/src/llgnew.f`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/matrix_debug.f90` & `pyddx-0.4.1/src/matrix_debug.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/pyddx.cpp` & `pyddx-0.4.1/src/pyddx.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/pyddx_classes.cpp` & `pyddx-0.4.1/src/pyddx_classes.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.0/src/pyddx_data.cpp` & `pyddx-0.4.1/src/pyddx_data.cpp`

 * *Files identical despite different names*

