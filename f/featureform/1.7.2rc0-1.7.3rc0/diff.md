# Comparing `tmp/featureform-1.7.2rc0.tar.gz` & `tmp/featureform-1.7.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform-1.7.2rc0.tar", last modified: Thu Apr  6 02:45:17 2023, max compression
+gzip compressed data, was "featureform-1.7.3rc0.tar", last modified: Thu Apr 13 01:17:12 2023, max compression
```

## Comparing `featureform-1.7.2rc0.tar` & `featureform-1.7.3rc0.tar`

### file list

```diff
@@ -1,364 +1,358 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.820930 featureform-1.7.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-06 02:45:17.820930 featureform-1.7.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-06 02:45:17.820930 featureform-1.7.2rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.712930 featureform-1.7.2rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.736930 featureform-1.7.2rc0/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.712930 featureform-1.7.2rc0/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.740930 featureform-1.7.2rc0/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.740930 featureform-1.7.2rc0/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.716930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.720930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.740930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.740930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/ZeSp5jbiz_whztxZm-YJw/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.788930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
--rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
--rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
--rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
--rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.804930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.804930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
--rw-r--r--   0 runner    (1001) docker     (123)  3582374 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-131cf942d8b62ea7.js
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.804930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
--rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.804930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.804930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.804930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.808930 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)    35774 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.812930 featureform-1.7.2rc0/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-06 02:45:10.000000 featureform-1.7.2rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/dashboard_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/get_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/get_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/list_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    89078 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/local_dash_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/local_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.816930 featureform-1.7.2rc0/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-06 02:44:20.000000 featureform-1.7.2rc0/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-04-06 02:44:22.000000 featureform-1.7.2rc0/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-04-06 02:44:22.000000 featureform-1.7.2rc0/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-06 02:44:20.000000 featureform-1.7.2rc0/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-06 02:44:21.000000 featureform-1.7.2rc0/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-06 02:44:21.000000 featureform-1.7.2rc0/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   166307 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/register_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    56454 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/search_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/serving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/sqlite_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.736930 featureform-1.7.2rc0/src/featureform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-06 02:45:17.000000 featureform-1.7.2rc0/src/featureform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32884 2023-04-06 02:45:17.000000 featureform-1.7.2rc0/src/featureform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:45:17.000000 featureform-1.7.2rc0/src/featureform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 02:45:17.000000 featureform-1.7.2rc0/src/featureform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-06 02:45:17.000000 featureform-1.7.2rc0/src/featureform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 02:45:17.000000 featureform-1.7.2rc0/src/featureform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:45:17.820930 featureform-1.7.2rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_localmode_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_localmode_include_label_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_localmode_lag_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-06 02:43:31.000000 featureform-1.7.2rc0/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.437099 featureform-1.7.3rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-13 01:17:12.437099 featureform-1.7.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-13 01:17:12.437099 featureform-1.7.3rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.393099 featureform-1.7.3rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.397099 featureform-1.7.3rc0/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.393099 featureform-1.7.3rc0/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.401099 featureform-1.7.3rc0/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.401099 featureform-1.7.3rc0/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.393099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.393099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.401099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.401099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/MIAYyZbApb_poPrdNhxsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.425099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3582042 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-01b1894ee40506d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.429099 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35774 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.433099 featureform-1.7.3rc0/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-13 01:17:06.000000 featureform-1.7.3rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/dashboard_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/get_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/get_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/list_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89078 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/local_dash_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.437099 featureform-1.7.3rc0/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-13 01:16:30.000000 featureform-1.7.3rc0/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-04-13 01:16:31.000000 featureform-1.7.3rc0/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-04-13 01:16:31.000000 featureform-1.7.3rc0/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 01:16:30.000000 featureform-1.7.3rc0/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-13 01:16:31.000000 featureform-1.7.3rc0/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-13 01:16:31.000000 featureform-1.7.3rc0/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162242 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/register_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48774 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/search_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/serving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24494 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/sqlite_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.397099 featureform-1.7.3rc0/src/featureform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-13 01:17:12.000000 featureform-1.7.3rc0/src/featureform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32703 2023-04-13 01:17:12.000000 featureform-1.7.3rc0/src/featureform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:17:12.000000 featureform-1.7.3rc0/src/featureform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 01:17:12.000000 featureform-1.7.3rc0/src/featureform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 01:17:12.000000 featureform-1.7.3rc0/src/featureform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 01:17:12.000000 featureform-1.7.3rc0/src/featureform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:17:12.437099 featureform-1.7.3rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_localmode_include_label_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_localmode_lag_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-13 01:15:48.000000 featureform-1.7.3rc0/tests/test_updating_provider.py
```

### Comparing `featureform-1.7.2rc0/LICENSE` & `featureform-1.7.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/PKG-INFO` & `featureform-1.7.3rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.7.2rc0
+Version: 1.7.3rc0
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.7.2rc0/README.md` & `featureform-1.7.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/setup.cfg` & `featureform-1.7.3rc0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform
-version = 1.7.2rc0
+version = 1.7.3rc0
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls = 
@@ -33,15 +33,14 @@
 	flask==2.2.1
 	Flask-Cors==3.0.10
 	validators>=0.20.0
 	dill==0.3.5.1
 	pandasql==0.7.3
 	sqlalchemy<2.0.0
 	requests
-	rich
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	featureform = featureform.cli:cli
```

### Comparing `featureform-1.7.2rc0/src/featureform/__init__.py` & `featureform-1.7.3rc0/src/featureform/__init__.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/cli.py` & `featureform-1.7.3rc0/src/featureform/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,31 +169,26 @@
               help="Disables TLS verification")
 @click.option("--local",
               is_flag=True,
               help="Enable local mode")
 @click.option("--dry-run",
               is_flag=True,
               help="Checks the definitions without applying them")
-@click.option("--no-wait",
-              is_flag=True,
-              help="Applies the resources asynchronously")
-def apply(host, cert, insecure, local, files, dry_run, no_wait):
+def apply(host, cert, insecure, local, files, dry_run):
     for file in files:
         if os.path.isfile(file):
             read_file(file)
         elif validators.url(file):
             read_url(file)
         else:
             raise ValueError(
                 f"Argument must be a path to a file or URL with a valid schema (http:// or https://): {file}")
 
     rc = ResourceClient(host=host, local=local, insecure=insecure, cert_path=cert, dry_run=dry_run)
-    asynchronous = no_wait
-    rc.apply(asynchronous=asynchronous)
-
+    rc.apply()
 
 @cli.command()
 @click.option("--query",
               "-q",
               "query",
               required=True,
               help="The phrase to search resources (e.g. 'quick').")
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/404.html` & `featureform-1.7.3rc0/src/featureform/dashboard/out/404.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-131cf942d8b62ea7.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"ZeSp5jbiz_whztxZm-YJw","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"MIAYyZbApb_poPrdNhxsm","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/[type]/[entity].html` & `featureform-1.7.3rc0/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-131cf942d8b62ea7.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div class="MuiContainer-root MuiContainer-maxWidthXl"><div class="MuiPaper-root MuiPaper-elevation3 MuiPaper-rounded"><div class="MuiContainer-root MuiContainer-maxWidthSm"><div aria-busy="true" class=""><svg width="40" height="40" viewBox="0 0 120 30" xmlns="http://www.w3.org/2000/svg" fill="grey" aria-label="audio-loading"><circle cx="15" cy="15" r="15"><animate attributeName="r" from="15" to="15" begin="0s" dur="0.8s" values="15;9;15" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="1" to="1" begin="0s" dur="0.8s" values="1;.5;1" calcMode="linear" repeatCount="indefinite"></animate></circle><circle cx="60" cy="15" r="9" attributeName="fillOpacity" from="1" to="0.3"><animate attributeName="r" from="9" to="9" begin="0s" dur="0.8s" values="9;15;9" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="0.5" to="0.5" begin="0s" dur="0.8s" values=".5;1;.5" calcMode="linear" repeatCount="indefinite"></animate></circle><circle cx="105" cy="15" r="15"><animate attributeName="r" from="15" to="15" begin="0s" dur="0.8s" values="15;9;15" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="1" to="1" begin="0s" dur="0.8s" values="1;.5;1" calcMode="linear" repeatCount="indefinite"></animate></circle></svg></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"ZeSp5jbiz_whztxZm-YJw","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div class="MuiContainer-root MuiContainer-maxWidthXl"><div class="MuiPaper-root MuiPaper-elevation3 MuiPaper-rounded"><div class="MuiContainer-root MuiContainer-maxWidthSm"><div aria-busy="true" class=""><svg width="40" height="40" viewBox="0 0 120 30" xmlns="http://www.w3.org/2000/svg" fill="grey" aria-label="audio-loading"><circle cx="15" cy="15" r="15"><animate attributeName="r" from="15" to="15" begin="0s" dur="0.8s" values="15;9;15" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="1" to="1" begin="0s" dur="0.8s" values="1;.5;1" calcMode="linear" repeatCount="indefinite"></animate></circle><circle cx="60" cy="15" r="9" attributeName="fillOpacity" from="1" to="0.3"><animate attributeName="r" from="9" to="9" begin="0s" dur="0.8s" values="9;15;9" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="0.5" to="0.5" begin="0s" dur="0.8s" values=".5;1;.5" calcMode="linear" repeatCount="indefinite"></animate></circle><circle cx="105" cy="15" r="15"><animate attributeName="r" from="15" to="15" begin="0s" dur="0.8s" values="15;9;15" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="1" to="1" begin="0s" dur="0.8s" values="1;.5;1" calcMode="linear" repeatCount="indefinite"></animate></circle></svg></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"MIAYyZbApb_poPrdNhxsm","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/[type].html` & `featureform-1.7.3rc0/src/featureform/dashboard/out/[type].html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-131cf942d8b62ea7.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"ZeSp5jbiz_whztxZm-YJw","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"MIAYyZbApb_poPrdNhxsm","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-131cf942d8b62ea7.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-01b1894ee40506d5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -89421,15 +89421,15 @@
                                                 }), (0, e.jsx)(y.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
                                                     onClick: X,
                                                     label: I.entity
                                                 })]
-                                            }), I.location && !I["is-on-demand"] && (0, e.jsxs)("div", {
+                                            }), I.location && (0, e.jsxs)("div", {
                                                 className: Q.linkBox,
                                                 children: [(0, e.jsxs)(r.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
                                                     children: [(0, e.jsx)("b", {
                                                         children: "Columns:"
                                                     }), " "]
@@ -89439,29 +89439,14 @@
                                                         children: "Entity:"
                                                     }), " ", I.location.Entity, "\xa0", (0, e.jsx)("b", {
                                                         children: "Value:"
                                                     }), " ", I.location.Value, "\xa0", (0, e.jsx)("b", {
                                                         children: "Timestamp:"
                                                     }), " ", I.location.TS]
                                                 })]
-                                            }), I.location && I["is-on-demand"] && (0, e.jsxs)("div", {
-                                                className: Q.linkBox,
-                                                children: [(0, e.jsxs)(r.Z, {
-                                                    variant: "body1",
-                                                    className: Q.typeTitle,
-                                                    children: [(0, e.jsx)("b", {
-                                                        children: "Feature Variant Type:"
-                                                    }), " "]
-                                                }), (0, e.jsx)(y.Z, {
-                                                    variant: "outlined",
-                                                    className: Q.linkChip,
-                                                    size: "small",
-                                                    onClick: function() {},
-                                                    label: "On-Demand"
-                                                })]
                                             })]
                                         }), (null === (b = I.tags) || void 0 === b ? void 0 : b.length) > 0 && (0, e.jsx)(v.Z, {
                                             item: !0,
                                             xs: !0,
                                             children: (0, e.jsx)(O, {
                                                 attributes: I.tags,
                                                 title: "Tags"
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform-1.7.3rc0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/connections.html` & `featureform-1.7.3rc0/src/featureform/dashboard/out/connections.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-131cf942d8b62ea7.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -1058,8 +1058,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"ZeSp5jbiz_whztxZm-YJw","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"MIAYyZbApb_poPrdNhxsm","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/index.html` & `featureform-1.7.3rc0/src/featureform/dashboard/out/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-131cf942d8b62ea7.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -1456,8 +1456,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search " class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"ZeSp5jbiz_whztxZm-YJw","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search " class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"MIAYyZbApb_poPrdNhxsm","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/search.html` & `featureform-1.7.3rc0/src/featureform/dashboard/out/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-131cf942d8b62ea7.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js" defer=""></script><script src="/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js" defer=""></script><script src="/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div>No Results</div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"ZeSp5jbiz_whztxZm-YJw","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div>No Results</div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"MIAYyZbApb_poPrdNhxsm","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/favicon.ico` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/logo192.png` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/logo512.png` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform-1.7.3rc0/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/dashboard_metadata.py` & `featureform-1.7.3rc0/src/featureform/dashboard_metadata.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/get.py` & `featureform-1.7.3rc0/src/featureform/get.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/get_local.py` & `featureform-1.7.3rc0/src/featureform/get_local.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/get_test.py` & `featureform-1.7.3rc0/src/featureform/get_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/list.py` & `featureform-1.7.3rc0/src/featureform/list.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/list_local.py` & `featureform-1.7.3rc0/src/featureform/list_local.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/list_test.py` & `featureform-1.7.3rc0/src/featureform/list_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/local_dash_test.py` & `featureform-1.7.3rc0/src/featureform/local_dash_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/proto/metadata.proto` & `featureform-1.7.3rc0/src/featureform/proto/metadata.proto`

 * *Files 4% similar despite different names*

```diff
@@ -139,44 +139,33 @@
 
 message Columns {
     string entity = 1;
     string value = 2;
     string ts = 3;
 }
 
-message PythonFunction {
-    bytes query = 1;
-}
-
-enum ComputationMode {
-    PRECOMPUTED = 0;
-    CLIENT_COMPUTED = 1;
-}
-
 message FeatureVariant {
     string name = 1;
     string variant = 2;
     NameVariant source = 3;
     string type = 4;
     string entity = 5;
     google.protobuf.Timestamp created = 6;
     string owner = 7;
     string description = 8;
     string provider = 9;
     ResourceStatus status = 10;
     repeated NameVariant trainingsets = 11;
     oneof location {
         Columns columns = 12;
-        PythonFunction function = 17;
     }
     google.protobuf.Timestamp last_updated = 13;
     string schedule = 14;
     Tags tags = 15;
     Properties properties = 16;
-    ComputationMode mode = 18;
 }
 
 message FeatureLag {
     string feature = 1;
     string variant = 2;
     string name = 3;
     google.protobuf.Duration lag = 4;
```

### Comparing `featureform-1.7.2rc0/src/featureform/proto/metadata_pb2.py` & `featureform-1.7.3rc0/src/featureform/proto/metadata_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n featureform/proto/metadata.proto\x12\"featureform.serving.metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"\x14\n\x04Name\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xbc\x01\n\x0eResourceStatus\x12I\n\x06status\x18\x01 \x01(\x0e\x32\x39.featureform.serving.metadata.proto.ResourceStatus.Status\x12\x15\n\rerror_message\x18\x02 \x01(\t\"H\n\x06Status\x12\r\n\tNO_STATUS\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\t\n\x05READY\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04\"\x98\x01\n\nResourceID\x12\x41\n\x08resource\x18\x01 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12G\n\rresource_type\x18\x02 \x01(\x0e\x32\x30.featureform.serving.metadata.proto.ResourceType\"\x9b\x01\n\x10SetStatusRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\"n\n\x15ScheduleChangeRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x10\n\x08schedule\x18\x02 \x01(\t\",\n\x0bNameVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\"\x07\n\x05\x45mpty\"\x86\x01\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"4\n\x07\x43olumns\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\n\n\x02ts\x18\x03 \x01(\t\"\x1f\n\x0ePythonFunction\x12\r\n\x05query\x18\x01 \x01(\x0c\"\x93\x06\n\x0e\x46\x65\x61tureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12?\n\x06source\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x05 \x01(\t\x12+\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x46\n\x08\x66unction\x18\x11 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.PythonFunctionH\x00\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x36\n\x04tags\x18\x0f \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x10 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x41\n\x04mode\x18\x12 \x01(\x0e\x32\x33.featureform.serving.metadata.proto.ComputationModeB\n\n\x08location\"d\n\nFeatureLag\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\x03lag\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x84\x01\n\x05Label\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xc2\x04\n\x0cLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12?\n\x06source\x18\x05 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x36\n\x04tags\x18\r \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x0e \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\n\n\x08location\"\xc3\x04\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08software\x18\x04 \x01(\t\x12\x0c\n\x04team\x18\x05 \x01(\t\x12\x19\n\x11serialized_config\x18\x06 \x01(\x0c\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12@\n\x07sources\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x0c \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\r \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x8a\x01\n\x0bTrainingSet\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xe3\x04\n\x12TrainingSetVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12+\n\x07\x63reated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08provider\x18\x06 \x01(\t\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x05label\x18\t \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x44\n\x0c\x66\x65\x61ture_lags\x18\x0f \x03(\x0b\x32..featureform.serving.metadata.proto.FeatureLag\x12\x36\n\x04tags\x18\x10 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x11 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xb6\x03\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x42\n\x06status\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x07 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x08 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xf1\x02\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x06 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x07 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xe1\x03\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12@\n\x07sources\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x08 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\t \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x85\x01\n\x06Source\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\x93\x06\n\rSourceVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12L\n\x0etransformation\x18\x0e \x01(\x0b\x32\x32.featureform.serving.metadata.proto.TransformationH\x00\x12\x46\n\x0bprimaryData\x18\x0f \x01(\x0b\x32/.featureform.serving.metadata.proto.PrimaryDataH\x00\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x10\n\x08provider\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06status\x18\x08 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\r\n\x05table\x18\t \x01(\t\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0c \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x10 \x01(\t\x12\x36\n\x04tags\x18\x11 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x12 \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\x0c\n\ndefinition\"\x95\x02\n\x0eTransformation\x12R\n\x11SQLTransformation\x18\x01 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.SQLTransformationH\x00\x12P\n\x10\x44\x46Transformation\x18\x02 \x01(\x0b\x32\x34.featureform.serving.metadata.proto.DFTransformationH\x00\x12M\n\x0fkubernetes_args\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.KubernetesArgsH\x01\x42\x06\n\x04typeB\x06\n\x04\x61rgs\"o\n\x17KubernetesResourceSpecs\x12\x13\n\x0b\x63pu_request\x18\x01 \x01(\t\x12\x11\n\tcpu_limit\x18\x02 \x01(\t\x12\x16\n\x0ememory_request\x18\x03 \x01(\t\x12\x14\n\x0cmemory_limit\x18\x04 \x01(\t\"r\n\x0eKubernetesArgs\x12\x14\n\x0c\x64ocker_image\x18\x01 \x01(\t\x12J\n\x05specs\x18\x02 \x01(\x0b\x32;.featureform.serving.metadata.proto.KubernetesResourceSpecs\"c\n\x11SQLTransformation\x12\r\n\x05query\x18\x01 \x01(\t\x12?\n\x06source\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"b\n\x10\x44\x46Transformation\x12\r\n\x05query\x18\x01 \x01(\x0c\x12?\n\x06inputs\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"_\n\x0bPrimaryData\x12\x44\n\x05table\x18\x01 \x01(\x0b\x32\x33.featureform.serving.metadata.proto.PrimarySQLTableH\x00\x42\n\n\x08location\"\x1f\n\x0fPrimarySQLTable\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x13\n\x04Tags\x12\x0b\n\x03tag\x18\x01 \x03(\t\"+\n\x08Property\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x42\x07\n\x05value\"\xbb\x01\n\nProperties\x12N\n\x08property\x18\x01 \x03(\x0b\x32<.featureform.serving.metadata.proto.Properties.PropertyEntry\x1a]\n\rPropertyEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.featureform.serving.metadata.proto.Property:\x02\x38\x01*\xc9\x01\n\x0cResourceType\x12\x0b\n\x07\x46\x45\x41TURE\x10\x00\x12\t\n\x05LABEL\x10\x01\x12\x10\n\x0cTRAINING_SET\x10\x02\x12\n\n\x06SOURCE\x10\x03\x12\x13\n\x0f\x46\x45\x41TURE_VARIANT\x10\x04\x12\x11\n\rLABEL_VARIANT\x10\x05\x12\x18\n\x14TRAINING_SET_VARIANT\x10\x06\x12\x12\n\x0eSOURCE_VARIANT\x10\x07\x12\x0c\n\x08PROVIDER\x10\x08\x12\n\n\x06\x45NTITY\x10\t\x12\t\n\x05MODEL\x10\n\x12\x08\n\x04USER\x10\x0b*7\n\x0f\x43omputationMode\x12\x0f\n\x0bPRECOMPUTED\x10\x00\x12\x13\n\x0f\x43LIENT_COMPUTED\x10\x01\x32\x88\x1a\n\x08Metadata\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12t\n\x11SetResourceStatus\x12\x34.featureform.serving.metadata.proto.SetStatusRequest\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty2\x8d\x19\n\x03\x41pi\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x42\'Z%github.com/featureform/metadata/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n featureform/proto/metadata.proto\x12\"featureform.serving.metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"\x14\n\x04Name\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xbc\x01\n\x0eResourceStatus\x12I\n\x06status\x18\x01 \x01(\x0e\x32\x39.featureform.serving.metadata.proto.ResourceStatus.Status\x12\x15\n\rerror_message\x18\x02 \x01(\t\"H\n\x06Status\x12\r\n\tNO_STATUS\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\t\n\x05READY\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04\"\x98\x01\n\nResourceID\x12\x41\n\x08resource\x18\x01 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12G\n\rresource_type\x18\x02 \x01(\x0e\x32\x30.featureform.serving.metadata.proto.ResourceType\"\x9b\x01\n\x10SetStatusRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\"n\n\x15ScheduleChangeRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x10\n\x08schedule\x18\x02 \x01(\t\",\n\x0bNameVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\"\x07\n\x05\x45mpty\"\x86\x01\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"4\n\x07\x43olumns\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\n\n\x02ts\x18\x03 \x01(\t\"\x88\x05\n\x0e\x46\x65\x61tureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12?\n\x06source\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x05 \x01(\t\x12+\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x36\n\x04tags\x18\x0f \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x10 \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\n\n\x08location\"d\n\nFeatureLag\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\x03lag\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x84\x01\n\x05Label\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xc2\x04\n\x0cLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12?\n\x06source\x18\x05 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x36\n\x04tags\x18\r \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x0e \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\n\n\x08location\"\xc3\x04\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08software\x18\x04 \x01(\t\x12\x0c\n\x04team\x18\x05 \x01(\t\x12\x19\n\x11serialized_config\x18\x06 \x01(\x0c\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12@\n\x07sources\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x0c \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\r \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x8a\x01\n\x0bTrainingSet\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xe3\x04\n\x12TrainingSetVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12+\n\x07\x63reated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08provider\x18\x06 \x01(\t\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x05label\x18\t \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x44\n\x0c\x66\x65\x61ture_lags\x18\x0f \x03(\x0b\x32..featureform.serving.metadata.proto.FeatureLag\x12\x36\n\x04tags\x18\x10 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x11 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xb6\x03\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x42\n\x06status\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x07 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x08 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xf1\x02\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x06 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x07 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xe1\x03\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12@\n\x07sources\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x08 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\t \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x85\x01\n\x06Source\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\x93\x06\n\rSourceVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12L\n\x0etransformation\x18\x0e \x01(\x0b\x32\x32.featureform.serving.metadata.proto.TransformationH\x00\x12\x46\n\x0bprimaryData\x18\x0f \x01(\x0b\x32/.featureform.serving.metadata.proto.PrimaryDataH\x00\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x10\n\x08provider\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06status\x18\x08 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\r\n\x05table\x18\t \x01(\t\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0c \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x10 \x01(\t\x12\x36\n\x04tags\x18\x11 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x12 \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\x0c\n\ndefinition\"\x95\x02\n\x0eTransformation\x12R\n\x11SQLTransformation\x18\x01 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.SQLTransformationH\x00\x12P\n\x10\x44\x46Transformation\x18\x02 \x01(\x0b\x32\x34.featureform.serving.metadata.proto.DFTransformationH\x00\x12M\n\x0fkubernetes_args\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.KubernetesArgsH\x01\x42\x06\n\x04typeB\x06\n\x04\x61rgs\"o\n\x17KubernetesResourceSpecs\x12\x13\n\x0b\x63pu_request\x18\x01 \x01(\t\x12\x11\n\tcpu_limit\x18\x02 \x01(\t\x12\x16\n\x0ememory_request\x18\x03 \x01(\t\x12\x14\n\x0cmemory_limit\x18\x04 \x01(\t\"r\n\x0eKubernetesArgs\x12\x14\n\x0c\x64ocker_image\x18\x01 \x01(\t\x12J\n\x05specs\x18\x02 \x01(\x0b\x32;.featureform.serving.metadata.proto.KubernetesResourceSpecs\"c\n\x11SQLTransformation\x12\r\n\x05query\x18\x01 \x01(\t\x12?\n\x06source\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"b\n\x10\x44\x46Transformation\x12\r\n\x05query\x18\x01 \x01(\x0c\x12?\n\x06inputs\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"_\n\x0bPrimaryData\x12\x44\n\x05table\x18\x01 \x01(\x0b\x32\x33.featureform.serving.metadata.proto.PrimarySQLTableH\x00\x42\n\n\x08location\"\x1f\n\x0fPrimarySQLTable\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x13\n\x04Tags\x12\x0b\n\x03tag\x18\x01 \x03(\t\"+\n\x08Property\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x42\x07\n\x05value\"\xbb\x01\n\nProperties\x12N\n\x08property\x18\x01 \x03(\x0b\x32<.featureform.serving.metadata.proto.Properties.PropertyEntry\x1a]\n\rPropertyEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.featureform.serving.metadata.proto.Property:\x02\x38\x01*\xc9\x01\n\x0cResourceType\x12\x0b\n\x07\x46\x45\x41TURE\x10\x00\x12\t\n\x05LABEL\x10\x01\x12\x10\n\x0cTRAINING_SET\x10\x02\x12\n\n\x06SOURCE\x10\x03\x12\x13\n\x0f\x46\x45\x41TURE_VARIANT\x10\x04\x12\x11\n\rLABEL_VARIANT\x10\x05\x12\x18\n\x14TRAINING_SET_VARIANT\x10\x06\x12\x12\n\x0eSOURCE_VARIANT\x10\x07\x12\x0c\n\x08PROVIDER\x10\x08\x12\n\n\x06\x45NTITY\x10\t\x12\t\n\x05MODEL\x10\n\x12\x08\n\x04USER\x10\x0b\x32\x88\x1a\n\x08Metadata\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12t\n\x11SetResourceStatus\x12\x34.featureform.serving.metadata.proto.SetStatusRequest\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty2\x8d\x19\n\x03\x41pi\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x42\'Z%github.com/featureform/metadata/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.metadata_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z%github.com/featureform/metadata/proto'
   _PROPERTIES_PROPERTYENTRY._options = None
   _PROPERTIES_PROPERTYENTRY._serialized_options = b'8\001'
-  _RESOURCETYPE._serialized_start=7319
-  _RESOURCETYPE._serialized_end=7520
-  _COMPUTATIONMODE._serialized_start=7522
-  _COMPUTATIONMODE._serialized_end=7577
+  _RESOURCETYPE._serialized_start=7147
+  _RESOURCETYPE._serialized_end=7348
   _NAME._serialized_start=137
   _NAME._serialized_end=157
   _RESOURCESTATUS._serialized_start=160
   _RESOURCESTATUS._serialized_end=348
   _RESOURCESTATUS_STATUS._serialized_start=276
   _RESOURCESTATUS_STATUS._serialized_end=348
   _RESOURCEID._serialized_start=351
@@ -45,60 +43,58 @@
   _NAMEVARIANT._serialized_end=819
   _EMPTY._serialized_start=821
   _EMPTY._serialized_end=828
   _FEATURE._serialized_start=831
   _FEATURE._serialized_end=965
   _COLUMNS._serialized_start=967
   _COLUMNS._serialized_end=1019
-  _PYTHONFUNCTION._serialized_start=1021
-  _PYTHONFUNCTION._serialized_end=1052
-  _FEATUREVARIANT._serialized_start=1055
-  _FEATUREVARIANT._serialized_end=1842
-  _FEATURELAG._serialized_start=1844
-  _FEATURELAG._serialized_end=1944
-  _LABEL._serialized_start=1947
-  _LABEL._serialized_end=2079
-  _LABELVARIANT._serialized_start=2082
-  _LABELVARIANT._serialized_end=2660
-  _PROVIDER._serialized_start=2663
-  _PROVIDER._serialized_end=3242
-  _TRAININGSET._serialized_start=3245
-  _TRAININGSET._serialized_end=3383
-  _TRAININGSETVARIANT._serialized_start=3386
-  _TRAININGSETVARIANT._serialized_end=3997
-  _ENTITY._serialized_start=4000
-  _ENTITY._serialized_end=4438
-  _MODEL._serialized_start=4441
-  _MODEL._serialized_end=4810
-  _USER._serialized_start=4813
-  _USER._serialized_end=5294
-  _SOURCE._serialized_start=5297
-  _SOURCE._serialized_end=5430
-  _SOURCEVARIANT._serialized_start=5433
-  _SOURCEVARIANT._serialized_end=6220
-  _TRANSFORMATION._serialized_start=6223
-  _TRANSFORMATION._serialized_end=6500
-  _KUBERNETESRESOURCESPECS._serialized_start=6502
-  _KUBERNETESRESOURCESPECS._serialized_end=6613
-  _KUBERNETESARGS._serialized_start=6615
-  _KUBERNETESARGS._serialized_end=6729
-  _SQLTRANSFORMATION._serialized_start=6731
-  _SQLTRANSFORMATION._serialized_end=6830
-  _DFTRANSFORMATION._serialized_start=6832
-  _DFTRANSFORMATION._serialized_end=6930
-  _PRIMARYDATA._serialized_start=6932
-  _PRIMARYDATA._serialized_end=7027
-  _PRIMARYSQLTABLE._serialized_start=7029
-  _PRIMARYSQLTABLE._serialized_end=7060
-  _TAGS._serialized_start=7062
-  _TAGS._serialized_end=7081
-  _PROPERTY._serialized_start=7083
-  _PROPERTY._serialized_end=7126
-  _PROPERTIES._serialized_start=7129
-  _PROPERTIES._serialized_end=7316
-  _PROPERTIES_PROPERTYENTRY._serialized_start=7223
-  _PROPERTIES_PROPERTYENTRY._serialized_end=7316
-  _METADATA._serialized_start=7580
-  _METADATA._serialized_end=10916
-  _API._serialized_start=10919
-  _API._serialized_end=14132
+  _FEATUREVARIANT._serialized_start=1022
+  _FEATUREVARIANT._serialized_end=1670
+  _FEATURELAG._serialized_start=1672
+  _FEATURELAG._serialized_end=1772
+  _LABEL._serialized_start=1775
+  _LABEL._serialized_end=1907
+  _LABELVARIANT._serialized_start=1910
+  _LABELVARIANT._serialized_end=2488
+  _PROVIDER._serialized_start=2491
+  _PROVIDER._serialized_end=3070
+  _TRAININGSET._serialized_start=3073
+  _TRAININGSET._serialized_end=3211
+  _TRAININGSETVARIANT._serialized_start=3214
+  _TRAININGSETVARIANT._serialized_end=3825
+  _ENTITY._serialized_start=3828
+  _ENTITY._serialized_end=4266
+  _MODEL._serialized_start=4269
+  _MODEL._serialized_end=4638
+  _USER._serialized_start=4641
+  _USER._serialized_end=5122
+  _SOURCE._serialized_start=5125
+  _SOURCE._serialized_end=5258
+  _SOURCEVARIANT._serialized_start=5261
+  _SOURCEVARIANT._serialized_end=6048
+  _TRANSFORMATION._serialized_start=6051
+  _TRANSFORMATION._serialized_end=6328
+  _KUBERNETESRESOURCESPECS._serialized_start=6330
+  _KUBERNETESRESOURCESPECS._serialized_end=6441
+  _KUBERNETESARGS._serialized_start=6443
+  _KUBERNETESARGS._serialized_end=6557
+  _SQLTRANSFORMATION._serialized_start=6559
+  _SQLTRANSFORMATION._serialized_end=6658
+  _DFTRANSFORMATION._serialized_start=6660
+  _DFTRANSFORMATION._serialized_end=6758
+  _PRIMARYDATA._serialized_start=6760
+  _PRIMARYDATA._serialized_end=6855
+  _PRIMARYSQLTABLE._serialized_start=6857
+  _PRIMARYSQLTABLE._serialized_end=6888
+  _TAGS._serialized_start=6890
+  _TAGS._serialized_end=6909
+  _PROPERTY._serialized_start=6911
+  _PROPERTY._serialized_end=6954
+  _PROPERTIES._serialized_start=6957
+  _PROPERTIES._serialized_end=7144
+  _PROPERTIES_PROPERTYENTRY._serialized_start=7051
+  _PROPERTIES_PROPERTYENTRY._serialized_end=7144
+  _METADATA._serialized_start=7351
+  _METADATA._serialized_end=10687
+  _API._serialized_start=10690
+  _API._serialized_end=13903
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform-1.7.2rc0/src/featureform/proto/metadata_pb2_grpc.py` & `featureform-1.7.3rc0/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/proto/serving.proto` & `featureform-1.7.3rc0/src/featureform/proto/serving.proto`

 * *Files 6% similar despite different names*

```diff
@@ -57,10 +57,9 @@
         string str_value = 1;
         int32 int_value = 2;
         float float_value = 3;
         double double_value = 4;
         int64  int64_value = 5;
         int32  int32_value = 6;
         bool   bool_value = 7;
-        bytes on_demand_function = 8;
     }
 }
```

### Comparing `featureform-1.7.2rc0/src/featureform/proto/serving_pb2.py` & `featureform-1.7.3rc0/src/featureform/proto/serving_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\">\n\nFeatureRow\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcb\x01\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12on_demand_function\x18\x08 \x01(\x0cH\x00\x42\x07\n\x05value2\xe2\x01\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\">\n\nFeatureRow\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xad\x01\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x42\x07\n\x05value2\xe2\x01\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.serving_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\034github.com/featureform/proto'
@@ -34,11 +34,11 @@
   _FEATUREROW._serialized_start=563
   _FEATUREROW._serialized_end=625
   _FEATUREID._serialized_start=627
   _FEATUREID._serialized_end=669
   _ENTITY._serialized_start=671
   _ENTITY._serialized_end=708
   _VALUE._serialized_start=711
-  _VALUE._serialized_end=914
-  _FEATURE._serialized_start=917
-  _FEATURE._serialized_end=1143
+  _VALUE._serialized_end=884
+  _FEATURE._serialized_start=887
+  _FEATURE._serialized_end=1113
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform-1.7.2rc0/src/featureform/proto/serving_pb2_grpc.py` & `featureform-1.7.3rc0/src/featureform/proto/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/register.py` & `featureform-1.7.3rc0/src/featureform/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
-from os.path import exists
+
+from os.path import exists 
 from datetime import timedelta
 from typeguard import typechecked
 from typing import Dict, Tuple, Callable, List, Union
 
 import dill
 import pandas as pd
 
@@ -16,15 +17,15 @@
 from .sqlite_metadata import SQLiteMetadata
 from .tls import insecure_channel, secure_channel
 from .resources import ColumnTypes, Model, ResourceState, Provider, RedisConfig, FirestoreConfig, CassandraConfig, DynamodbConfig, \
     MongoDBConfig, PostgresConfig, SnowflakeConfig, LocalConfig, RedshiftConfig, BigQueryConfig, SparkConfig, \
     AzureFileStoreConfig, OnlineBlobConfig, K8sConfig, S3StoreConfig, GCSFileStoreConfig, User, Location, Source, PrimaryData, SQLTable, \
     SQLTransformation, DFTransformation, Entity, Feature, Label, ResourceColumnMapping, TrainingSet, ProviderReference, \
     EntityReference, SourceReference, ExecutorCredentials, ResourceRedefinedError, ResourceStatus, Transformation, \
-    K8sArgs, AWSCredentials, GCPCredentials, HDFSConfig, K8sResourceSpecs, FilePrefix, OnDemandFeature
+    K8sArgs, AWSCredentials, GCPCredentials, HDFSConfig, K8sResourceSpecs, FilePrefix
 
 from .proto import metadata_pb2_grpc as ff_grpc
 from .search_local import search_local
 from .search import search
 
 NameVariant = Tuple[str, str]
 
@@ -622,16 +623,14 @@
         fn.register_resources = self.register_resources
         return fn
 
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
             raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
-        elif col_len > 3:
-            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
         return (self.registrar, self.name_variant(), columns)
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def pandas(self):
         """
@@ -720,20 +719,18 @@
         # the methods to the subscriptable_fn instance; however, the descriptor protocol
         # produces the same result while also being compatible with `classmethod`
         # and `staticmethod`.
         self.register_resources = decorator_register_resources_method.__get__(self)
         self.name_variant = decorator_name_variant_method.__get__(self)
         pass
 
-    def __getitem__(self, columns: List[str]):
+    def __getitem__(self, columns):
         col_len = len(columns)
         if col_len < 2:
             raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
-        elif col_len > 3:
-            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
         return (self.registrar, self.name_variant(), columns)
 
     def __call__(self, *args, **kwds):
         return self.fn(*args, **kwds)
 
 
 class SQLTransformationDecorator:
@@ -905,16 +902,14 @@
 
 class ColumnSourceRegistrar(SourceRegistrar):
 
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
             raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
-        elif col_len > 3:
-            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
         return (self.registrar(), self.id(), columns)
 
     def register_resources(
             self,
             entity: Union[str, EntityRegistrar],
             entity_column: str,
             owner: Union[str, UserRegistrar] = "",
@@ -1275,41 +1270,15 @@
             name (str): Name of Snowflake provider to be retrieved
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="snowflake", obj=None)
         self.__resources.append(get)
-        fakeConfig = SnowflakeConfig(account="ff_fake", database="ff_fake", organization="ff_fake", username="ff_fake", password="ff_fake", schema="ff_fake")
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
-        return OfflineSQLProvider(self, fakeProvider)
-    
-    def get_snowflake_legacy(self, name: str):
-        """Get a Snowflake provider. The returned object can be used to register additional resources.
-
-        **Examples**:
-        ``` py
-        snowflake = ff.get_snowflake_legacy("snowflake-quickstart")
-        transactions = snowflake.register_table(
-            name="transactions",
-            variant="kaggle",
-            description="Fraud Dataset From Kaggle",
-            table="Transactions",  # This is the table's name in Postgres
-        )
-        ```
-        Args:
-            name (str): Name of Snowflake provider to be retrieved
-
-        Returns:
-            snowflake_legacy (OfflineSQLProvider): Provider
-        """
-        get = ProviderReference(name=name, provider_type="snowflake", obj=None)
-        self.__resources.append(get)
-
-        fakeConfig = SnowflakeConfig(account_locator="ff_fake", database="ff_fake", username="ff_fake", password="ff_fake", schema="ff_fake", warehouse="ff_fake", role="ff_fake")
+        fakeConfig = SnowflakeConfig(account="", database="", organization="", username="", password="", schema="")
         fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_redshift(self, name):
         """Get a Redshift provider. The returned object can be used to register additional resources.
 
         **Examples**:
@@ -2063,16 +2032,16 @@
                           description: str = "",
                           team: str = "",
                           host: str = "0.0.0.0",
                           port: str = "5432",
                           user: str = "postgres",
                           password: str = "password",
                           database: str = "postgres",
-                          tags: List[str] = None,
-                          properties: dict = None):
+                          tags: List[str] = [],
+                          properties: dict = {}):
         """Register a Postgres provider.
 
         **Examples**:
         ```
         postgres = ff.register_postgres(
             name="postgres-quickstart",
             description="A Postgres deployment we created for the Featureform quickstart",
@@ -2104,16 +2073,16 @@
                                 user=user,
                                 password=password)
         provider = Provider(name=name,
                             function="OFFLINE",
                             description=description,
                             team=team,
                             config=config,
-                            tags=tags or [],
-                            properties=properties or {})
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
     def register_redshift(self,
                           name: str,
                           description: str = "",
                           team: str = "",
@@ -2567,64 +2536,14 @@
             args=args,
             tags=tags,
             properties=properties
         )
         self.__resources.append(decorator)
         return decorator
 
-    def ondemand_feature(self, 
-                          fn=None, *,
-                          tags: List[str] = None,
-                          properties: dict = None,
-                          variant: str = "default",
-                          name: str = "",
-                          owner: Union[str, UserRegistrar] = "",
-                          description: str = "",
-                          ):
-        """On Demand Feature decorator.
-
-        Args:
-            variant (str): Name of variant
-            name (str): Name of source
-            owner (Union[str, UserRegistrar]): Owner
-            description (str): Description of on demand feature
-            tags (List[str]): Optional grouping mechanism for resources
-            properties (dict): Optional grouping mechanism for resources
-
-        Returns:
-            decorator (OnDemandFeature): decorator
-
-        **Examples**
-        ```python
-        @ff.ondemand_feature()
-        def avg_user_transactions():
-            pass
-        ```
-        """
-
-        if not isinstance(owner, str):
-            owner = owner.name()
-        if owner == "":
-            owner = self.must_get_default_owner()
-    
-        decorator = OnDemandFeature(
-            name=name,
-            variant=variant,
-            owner=owner,
-            description=description,
-            tags=tags or [],
-            properties=properties or {},
-        )
-        self.__resources.append(decorator)
-        
-        if fn is None:
-            return decorator
-        else:
-            return decorator(fn)
-
     def state(self):
         for resource in self.__resources:
             try:
                 if isinstance(resource, SQLTransformationDecorator) or isinstance(resource, DFTransformationDecorator):
                     resource = resource.to_source()
                 self.__state.add(resource)
             except ResourceRedefinedError:
@@ -2942,36 +2861,26 @@
             if insecure:
                 channel = insecure_channel(host)
             else:
                 channel = secure_channel(host, cert_path)
             self._stub = ff_grpc.ApiStub(channel)
             self._host = host
 
-    def apply(self, asynchronous=True):
+    def apply(self):
+        """Apply all definitions, creating and retrieving all specified resources.
         """
-        Apply all definitions, creating and retrieving all specified resources.
 
-        @param asynchronous: Wait for all resources to be ready before returning.
-        """
-        resource_state = state()
         if self._dry_run:
-            print(resource_state.sorted_list())
+            print(state().sorted_list())
             return
 
         if self.local:
-            resource_state.create_all_local()
+            state().create_all_local()
         else:
-            resource_state.create_all(self._stub)
-
-        if not asynchronous and self._stub:
-            resources = resource_state.sorted_list()
-            display_statuses(self._stub, resources)
-
-        self.clear_state()
-
+            state().create_all(self._stub)
 
     def get_user(self, name, local=False):
         """Get a user. Prints out name of user, and all resources associated with the user.
 
         **Examples:**
 
         ``` py title="Input"
@@ -3558,16 +3467,14 @@
             name=source.name,
             definition=definition,
             owner=source.owner,
             provider=source.provider,
             description=source.description,
             variant=source.variant,
             status=source.status.Status._enum_type.values[source.status.status].name,
-            tags=[],
-            properties={}
         )
 
     def _get_source_definition(self, source):
         if source.primaryData.table.name:
             return PrimaryData(
                 Location(source.primaryData.table.name)
             )
@@ -4132,20 +4039,15 @@
         self.entity_column = columns[0]
         self.source_column = columns[1]
         self.resource_type = resource_type
         self.entity = entity
         self.variant = variant
         self.owner = owner
         self.inference_store = inference_store
-        if not timestamp_column and len(columns) == 3:
-            self.timestamp_column = columns[2]
-        elif timestamp_column and len(columns) == 3:
-            raise Exception("Timestamp column specified twice.")
-        else:
-            self.timestamp_column = timestamp_column
+        self.timestamp_column = timestamp_column
         self.description = description
         self.schedule = schedule
         self.tags = tags
         self.properties = properties
 
     def register(self):
         features, labels = self.features_and_labels()
@@ -4186,15 +4088,15 @@
 class Variants:
     def __init__(self, resources: Dict[str, ColumnResource]):
         self.resources = resources
         self.validate_variant_names()
 
     def validate_variant_names(self):
         for variant_key, resource in self.resources.items():
-            if resource.variant == "default":
+            if resource.variant is "default":
                 resource.variant = variant_key
             if resource.variant != variant_key:
                 raise ValueError(
                     f"Variant name {variant_key} does not match resource variant name {resource.variant}"
                 )
 
     def register(self):
@@ -4324,23 +4226,21 @@
 get_entity = global_registrar.get_entity
 get_source = global_registrar.get_source
 get_local_provider = global_registrar.get_local_provider
 get_redis = global_registrar.get_redis
 get_postgres = global_registrar.get_postgres
 get_mongodb = global_registrar.get_mongodb
 get_snowflake = global_registrar.get_snowflake
-get_snowflake_legacy = global_registrar.get_snowflake_legacy
 get_redshift = global_registrar.get_redshift
 get_bigquery = global_registrar.get_bigquery
 get_spark = global_registrar.get_spark
 get_kubernetes = global_registrar.get_kubernetes
 get_blob_store = global_registrar.get_blob_store
 get_s3 = global_registrar.get_s3
 get_gcs = global_registrar.get_gcs
-ondemand_feature = global_registrar.ondemand_feature
 ResourceStatus = ResourceStatus
 
 
 Nil = ColumnTypes.NIL
 String = ColumnTypes.STRING
 Int = ColumnTypes.INT
 Int32 = ColumnTypes.INT32
```

### Comparing `featureform-1.7.2rc0/src/featureform/register_test.py` & `featureform-1.7.3rc0/src/featureform/register_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/resources.py` & `featureform-1.7.3rc0/src/featureform/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,77 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import sys
 import json
 import time
-import base64
+import datetime
 from enum import Enum
 from typeguard import typechecked
-from typing import List, Tuple, Union, Optional
+from typing import List, Tuple, Union
 
-import dill
 import grpc
 from .sqlite_metadata import SQLiteMetadata
 from google.protobuf.duration_pb2 import Duration
 
 from featureform.proto import metadata_pb2 as pb
 from dataclasses import dataclass, field
 from .version import check_up_to_date
-from .exceptions import *
-from .enums import *
 
 NameVariant = Tuple[str, str]
 
 
 # Constants for Pyspark Versions
 MAJOR_VERSION = "3"
 MINOR_VERSIONS = ["7", "8", "9", "10"]
 
 
+class ColumnTypes(Enum):
+    NIL = ""
+    INT = "int"
+    INT32 = "int32"
+    INT64 = "int64"
+    FLOAT32 = "float32"
+    FLOAT64 = "float64"
+    STRING = "string"
+    BOOL = "bool"
+    DATETIME = "datetime"
+
+
+class ResourceStatus(Enum):
+    NO_STATUS = "NO_STATUS"
+    CREATED = "CREATED"
+    PENDING = "PENDING"
+    READY = "READY"
+    FAILED = "FAILED"
+
+
+@typechecked
+@dataclass
+class OperationType(Enum):
+    GET = 0
+    CREATE = 1
+
+
+@typechecked
+@dataclass
+class SourceType(Enum):
+    PRIMARY_SOURCE = "PRIMARY"
+    DF_TRANSFORMATION = "DF"
+    SQL_TRANSFORMATION = "SQL"
+
+
+@typechecked
+@dataclass
+class FilePrefix(Enum):
+    S3 = "s3://"
+    S3A = "s3a://"
+
+
 @typechecked
 def valid_name_variant(nvar: NameVariant) -> bool:
     return nvar[0] != "" and nvar[1] != ""
 
 
 @typechecked
 @dataclass
@@ -47,16 +86,20 @@
         return OperationType.CREATE
 
     def type(self) -> str:
         return "schedule"
 
     def _create(self, stub) -> None:
         serialized = pb.SetScheduleChangeRequest(
-            resource=pb.ResourceId(pb.NameVariant(name=self.name, variant=self.variant),
-                                   resource_type=self.resource_type), schedule=self.schedule_string)
+            resource=pb.ResourceId(
+                pb.NameVariant(name=self.name, variant=self.variant),
+                resource_type=self.resource_type,
+            ),
+            schedule=self.schedule_string,
+        )
         stub.RequestScheduleChange(serialized)
 
 
 @typechecked
 @dataclass
 class RedisConfig:
     host: str
@@ -78,20 +121,24 @@
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class AWSCredentials:
-    def __init__(self,
-                 aws_access_key_id: str = "",
-                 aws_secret_access_key: str = "",):
+    def __init__(
+        self,
+        aws_access_key_id: str = "",
+        aws_secret_access_key: str = "",
+    ):
         empty_strings = aws_access_key_id == "" or aws_secret_access_key == ""
         if empty_strings:
-            raise Exception("'AWSCredentials' requires all parameters: 'aws_access_key_id', 'aws_secret_access_key'")
+            raise Exception(
+                "'AWSCredentials' requires all parameters: 'aws_access_key_id', 'aws_secret_access_key'"
+            )
 
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
 
     def type(self):
         return "AWS_CREDENTIALS"
 
@@ -101,18 +148,19 @@
             "AWSSecretKey": self.aws_secret_access_key,
         }
 
 
 @typechecked
 @dataclass
 class GCPCredentials:
-    def __init__(self,
-                 project_id: str,
-                 credentials_path: str,):
-
+    def __init__(
+        self,
+        project_id: str,
+        credentials_path: str,
+    ):
         self.project_id = project_id
         self.credentials = json.load(open(credentials_path))
 
     def type(self):
         return "GCPCredentials"
 
     def config(self):
@@ -188,23 +236,22 @@
     def store_type(self):
         return self.type()
 
 
 @typechecked
 @dataclass
 class S3StoreConfig:
-    def __init__(self, 
-                 bucket_path: str,
-                 bucket_region: str,
-                 credentials: AWSCredentials):
+    def __init__(
+        self, bucket_path: str, bucket_region: str, credentials: AWSCredentials
+    ):
         bucket_path_ends_with_slash = len(bucket_path) != 0 and bucket_path[-1] == "/"
 
         if bucket_path_ends_with_slash:
             raise Exception("The 'bucket_path' cannot end with '/'.")
-                 
+
         self.bucket_path = bucket_path
         self.bucket_region = bucket_region
         self.credentials = credentials
 
     def software(self) -> str:
         return "S3"
 
@@ -221,26 +268,23 @@
 
     def config(self):
         return {
             "Credentials": self.credentials.config(),
             "BucketRegion": self.bucket_region,
             "BucketPath": self.bucket_path,
         }
-    
+
     def store_type(self):
         return self.type()
 
+
 @typechecked
 @dataclass
 class HDFSConfig:
-    def __init__(self,
-                 host: str,
-                 port: str,
-                 path: str,
-                 username: str):
+    def __init__(self, host: str, port: str, path: str, username: str):
         bucket_path_ends_with_slash = len(path) != 0 and path[-1] == "/"
 
         if bucket_path_ends_with_slash:
             raise Exception("The 'bucket_path' cannot end with '/'.")
 
         self.path = path
         self.host = host
@@ -254,24 +298,24 @@
         return "HDFS"
 
     def serialize(self) -> bytes:
         config = {
             "Host": self.host,
             "Port": self.port,
             "Path": self.path,
-            "Username": self.username
+            "Username": self.username,
         }
         return bytes(json.dumps(config), "utf-8")
 
     def config(self):
         return {
             "Host": self.host,
             "Port": self.port,
             "Path": self.path,
-            "Username": self.username
+            "Username": self.username,
         }
 
     def store_type(self):
         return self.type()
 
 
 @typechecked
@@ -339,15 +383,15 @@
     def serialize(self) -> bytes:
         config = {
             "Keyspace": self.keyspace,
             "Addr": f"{self.host}:{self.port}",
             "Username": self.username,
             "Password": self.password,
             "Consistency": self.consistency,
-            "Replication": self.replication
+            "Replication": self.replication,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class DynamodbConfig:
@@ -361,15 +405,15 @@
     def type(self) -> str:
         return "DYNAMODB_ONLINE"
 
     def serialize(self) -> bytes:
         config = {
             "Region": self.region,
             "AccessKey": self.access_key,
-            "SecretKey": self.secret_key
+            "SecretKey": self.secret_key,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class MongoDBConfig:
@@ -389,32 +433,30 @@
     def serialize(self) -> bytes:
         config = {
             "Username": self.username,
             "Password": self.password,
             "Host": self.host,
             "Port": self.port,
             "Database": self.database,
-            "Throughput": self.throughput
+            "Throughput": self.throughput,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class LocalConfig:
-
     def software(self) -> str:
         return "localmode"
 
     def type(self) -> str:
         return "LOCAL_ONLINE"
 
     def serialize(self) -> bytes:
-        config = {
-        }
+        config = {}
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class SnowflakeConfig:
     username: str
@@ -425,24 +467,28 @@
     database: str = ""
     account_locator: str = ""
     warehouse: str = ""
     role: str = ""
 
     def __post_init__(self):
         if self.__has_legacy_credentials() and self.__has_current_credentials():
-            raise ValueError("Cannot create configure Snowflake with both current and legacy credentials")
+            raise ValueError(
+                "Cannot create configure Snowflake with both current and legacy credentials"
+            )
 
         if not self.__has_legacy_credentials() and not self.__has_current_credentials():
             raise ValueError("Cannot create configure Snowflake without credentials")
 
     def __has_legacy_credentials(self) -> bool:
         return self.account_locator != ""
 
     def __has_current_credentials(self) -> bool:
-        if (self.account != "" and self.organization == "") or (self.account == "" and self.organization != ""):
+        if (self.account != "" and self.organization == "") or (
+            self.account == "" and self.organization != ""
+        ):
             raise ValueError("Both Snowflake organization and account must be included")
         elif self.account != "" and self.organization != "":
             return True
         else:
             return False
 
     def software(self) -> str:
@@ -457,15 +503,15 @@
             "Password": self.password,
             "Organization": self.organization,
             "AccountLocator": self.account_locator,
             "Account": self.account,
             "Schema": self.schema,
             "Database": self.database,
             "Warehouse": self.warehouse,
-            "Role": self.role
+            "Role": self.role,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class PostgresConfig:
@@ -559,34 +605,38 @@
             "ExecutorType": self.executor_type,
             "StoreType": self.store_type,
             "ExecutorConfig": self.executor_config,
             "StoreConfig": self.store_config,
         }
         return bytes(json.dumps(config), "utf-8")
 
+
 @typechecked
 @dataclass
 class K8sResourceSpecs:
     cpu_request: str = ""
     cpu_limit: str = ""
     memory_request: str = ""
     memory_limit: str = ""
 
+
 @typechecked
 @dataclass
 class K8sArgs:
     docker_image: str
     specs: Union[K8sResourceSpecs, None] = None
 
     def apply(self, transformation: pb.Transformation):
         transformation.kubernetes_args.docker_image = self.docker_image
         if self.specs is not None:
             transformation.kubernetes_args.specs.cpu_request = self.specs.cpu_request
             transformation.kubernetes_args.specs.cpu_limit = self.specs.cpu_limit
-            transformation.kubernetes_args.specs.memory_request = self.specs.memory_request
+            transformation.kubernetes_args.specs.memory_request = (
+                self.specs.memory_request
+            )
             transformation.kubernetes_args.specs.memory_limit = self.specs.memory_limit
         return transformation
 
 
 @typechecked
 @dataclass
 class K8sConfig:
@@ -599,42 +649,39 @@
 
     def type(self) -> str:
         return "K8S_OFFLINE"
 
     def serialize(self) -> bytes:
         config = {
             "ExecutorType": "K8S",
-            "ExecutorConfig": {
-                "docker_image": self.docker_image
-            },
+            "ExecutorConfig": {"docker_image": self.docker_image},
             "StoreType": self.store_type,
             "StoreConfig": self.store_config,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
-@typechecked
-@dataclass
-class EmptyConfig:
-    def software(self) -> str:
-        return ""
-
-    def type(self) -> str:
-        return ""
-
-    def serialize(self) -> bytes:
-        return bytes("", "utf-8")
-
-
 Config = Union[
-    RedisConfig, SnowflakeConfig, PostgresConfig, RedshiftConfig, LocalConfig, BigQueryConfig,
-    FirestoreConfig, SparkConfig, OnlineBlobConfig, AzureFileStoreConfig, S3StoreConfig, K8sConfig,
-    MongoDBConfig, GCSFileStoreConfig, EmptyConfig
+    RedisConfig,
+    SnowflakeConfig,
+    PostgresConfig,
+    RedshiftConfig,
+    LocalConfig,
+    BigQueryConfig,
+    FirestoreConfig,
+    SparkConfig,
+    OnlineBlobConfig,
+    AzureFileStoreConfig,
+    S3StoreConfig,
+    K8sConfig,
+    MongoDBConfig,
+    GCSFileStoreConfig,
 ]
 
+
 @typechecked
 @dataclass
 class Properties:
     properties: dict
 
     def __post_init__(self):
         self.serialized = pb.Properties()
@@ -642,79 +689,64 @@
             self.serialized.property[key].string_value = val
 
 
 @typechecked
 @dataclass
 class Provider:
     name: str
+    function: str
+    config: Config
     description: str
     team: str
-    config: Config
-    function: str
-    status: str = "NO_STATUS"
-    tags: list = None
-    properties: dict = None
-    error: Optional[str] = None
+    tags: list
+    properties: dict
 
     def __post_init__(self):
-        self.software = self.config.software() if self.config is not None else None
+        self.software = self.config.software()
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "provider"
 
-    def get(self, stub) -> 'Provider':
-        name = pb.Name(name=self.name)
-        provider = next(stub.GetProviders(iter([name])))
-
-        return Provider(
-            name=provider.name,
-            description=provider.description,
-            function=provider.type,
-            team=provider.team,
-            config=EmptyConfig(),  # TODO add deserializer to configs
-            tags=list(provider.tags.tag),
-            properties={k: v for k, v in provider.properties.property.items()},
-            status=provider.status.Status._enum_type.values[provider.status.status].name,
-            error=provider.status.error_message
-        )
-
     def _create(self, stub) -> None:
         serialized = pb.Provider(
             name=self.name,
             description=self.description,
             type=self.config.type(),
             software=self.config.software(),
             team=self.team,
             serialized_config=self.config.serialize(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateProvider(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("providers",
-                  self.name,
-                  "Provider",
-                  self.description,
-                  self.config.type(),
-                  self.config.software(),
-                  self.team,
-                  "sources",
-                  "ready",
-                  str(self.config.serialize(), 'utf-8')
-                  )
+        db.insert(
+            "providers",
+            self.name,
+            "Provider",
+            self.description,
+            self.config.type(),
+            self.config.software(),
+            self.team,
+            "sources",
+            "ready",
+            str(self.config.serialize(), "utf-8"),
+        )
         if len(self.tags):
             db.upsert("tags", self.name, "", "providers", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert("properties", self.name, "", "providers", json.dumps(self.properties))
+            db.upsert(
+                "properties", self.name, "", "providers", json.dumps(self.properties)
+            )
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
@@ -738,19 +770,15 @@
             name=self.name,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateUser(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("users",
-                  self.name,
-                  "User",
-                  "ready"
-                  )
+        db.insert("users", self.name, "User", "ready")
         if len(self.tags):
             db.upsert("tags", self.name, "", "users", json.dumps(self.tags))
         if len(self.properties):
             db.upsert("properties", self.name, "", "users", json.dumps(self.properties))
 
     def __eq__(self, other):
         for attribute in vars(self):
@@ -771,17 +799,19 @@
 @typechecked
 @dataclass
 class PrimaryData:
     location: Location
 
     def kwargs(self):
         return {
-            "primaryData":
-                pb.PrimaryData(table=pb.PrimarySQLTable(
-                    name=self.location.name, ), ),
+            "primaryData": pb.PrimaryData(
+                table=pb.PrimarySQLTable(
+                    name=self.location.name,
+                ),
+            ),
         }
 
     def name(self):
         return self.location.name
 
 
 class Transformation:
@@ -803,17 +833,15 @@
                 query=self.query,
             )
         )
 
         if self.args is not None:
             transformation = self.args.apply(transformation)
 
-        return {
-            "transformation": transformation
-        }
+        return {"transformation": transformation}
 
 
 @typechecked
 @dataclass
 class DFTransformation(Transformation):
     query: bytes
     inputs: list
@@ -822,24 +850,22 @@
     def type(self):
         return SourceType.DF_TRANSFORMATION.value
 
     def kwargs(self):
         transformation = pb.Transformation(
             DFTransformation=pb.DFTransformation(
                 query=self.query,
-                inputs=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.inputs]
+                inputs=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.inputs],
             )
         )
-        
+
         if self.args is not None:
             transformation = self.args.apply(transformation)
 
-        return {
-            "transformation": transformation
-        }
+        return {"transformation": transformation}
 
 
 SourceDefinition = Union[PrimaryData, Transformation]
 
 
 @typechecked
 @dataclass
@@ -847,76 +873,38 @@
     name: str
     definition: SourceDefinition
     owner: str
     provider: str
     description: str
     tags: list
     properties: dict
-    status: str = "NO_STATUS"
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     is_transformation = SourceType.PRIMARY_SOURCE.value
-    inputs = [],
-    error: Optional[str] = None
+    inputs = ([],)
+    status: str = "NO_STATUS"
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=7, schedule_string=schedule)
+        self.schedule_obj = Schedule(
+            name=self.name,
+            variant=self.variant,
+            resource_type=7,
+            schedule_string=schedule,
+        )
         self.schedule = schedule
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "source"
 
-    def get(self, stub):
-        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
-        source = next(stub.GetSourceVariants(iter([name_variant])))
-        definition = self._get_source_definition(source)
-
-        return Source(
-            name=source.name,
-            definition=definition,
-            owner=source.owner,
-            provider=source.provider,
-            description=source.description,
-            variant=source.variant,
-            tags=list(source.tags.tag),
-            properties={k: v for k, v in source.properties.property.items()},
-            status=source.status.Status._enum_type.values[source.status.status].name,
-            error=source.status.error_message,
-        )
-
-    def _get_source_definition(self, source):
-        if source.primaryData.table.name:
-            return PrimaryData(
-                Location(source.primaryData.table.name)
-            )
-        elif source.transformation:
-            return self._get_transformation_definition(source)
-        else:
-            raise Exception(f"Invalid source type {source}")
-
-    def _get_transformation_definition(self, source):
-        if source.transformation.DFTransformation.query != bytes():
-            transformation = source.transformation.DFTransformation
-            return DFTransformation(
-                query=transformation.query,
-                inputs=[(input.name, input.variant) for input in transformation.inputs]
-            )
-        elif source.transformation.SQLTransformation.query != "":
-            return SQLTransformation(
-                source.transformation.SQLTransformation.query
-            )
-        else:
-            raise Exception(f"Invalid transformation type {source}")
-
     def _create(self, stub) -> None:
         defArgs = self.definition.kwargs()
         serialized = pb.SourceVariant(
             name=self.name,
             variant=self.variant,
             owner=self.owner,
             description=self.description,
@@ -935,40 +923,44 @@
             self.definition = self.definition.query
         elif type(self.definition) == SQLTransformation:
             self.is_transformation = SourceType.SQL_TRANSFORMATION.value
             self.definition = self.definition.query
         elif type(self.definition) == PrimaryData:
             self.definition = self.definition.name()
             self.is_transformation = SourceType.PRIMARY_SOURCE.value
-        db.insert_source("source_variant",
-                         str(time.time()),
-                         self.description,
-                         self.name,
-                         "Source",
-                         self.owner,
-                         self.provider,
-                         self.variant,
-                         "ready",
-                         self.is_transformation,
-                         json.dumps(self.inputs),
-                         self.definition
-                         )
+        db.insert_source(
+            "source_variant",
+            str(time.time()),
+            self.description,
+            self.name,
+            "Source",
+            self.owner,
+            self.provider,
+            self.variant,
+            "ready",
+            self.is_transformation,
+            json.dumps(self.inputs),
+            self.definition,
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "source_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags", self.name, self.variant, "source_variant", json.dumps(self.tags)
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "source_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "source_variant",
+                json.dumps(self.properties),
+            )
         self._create_source_resource(db)
 
     def _create_source_resource(self, db) -> None:
-        db.insert(
-            "sources",
-            "Source",
-            self.variant,
-            self.name
-        )
+        db.insert("sources", "Source", self.variant, self.name)
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1001,24 +993,21 @@
             description=self.description,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateEntity(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("entities",
-                  self.name,
-                  "Entity",
-                  self.description,
-                  "ready"
-                  )
+        db.insert("entities", self.name, "Entity", self.description, "ready")
         if len(self.tags):
             db.upsert("tags", self.name, "", "entities", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert("properties", self.name, "", "entities", json.dumps(self.properties))
+            db.upsert(
+                "properties", self.name, "", "entities", json.dumps(self.properties)
+            )
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
@@ -1048,59 +1037,45 @@
     source: NameVariant
     value_type: str
     entity: str
     owner: str
     provider: str
     location: ResourceLocation
     description: str
-    tags: list = None
-    properties: dict = None
+    tags: list
+    properties: dict
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     status: str = "NO_STATUS"
-    error: Optional[str] = None
 
     def __post_init__(self):
         col_types = [member.value for member in ColumnTypes]
         if self.value_type not in col_types:
-            raise ValueError(f"Invalid feature type ({self.value_type}) must be one of: {col_types}")
+            raise ValueError(
+                f"Invalid feature type ({self.value_type}) must be one of: {col_types}"
+            )
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=4, schedule_string=schedule)
+        self.schedule_obj = Schedule(
+            name=self.name,
+            variant=self.variant,
+            resource_type=4,
+            schedule_string=schedule,
+        )
         self.schedule = schedule
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "feature"
 
-    def get(self, stub) -> "Feature":
-        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
-        feature = next(stub.GetFeatureVariants(iter([name_variant])))
-
-        return Feature(
-            name=feature.name,
-            variant=feature.variant,
-            source=(feature.source.name, feature.source.variant),
-            value_type=feature.type,
-            entity=feature.entity,
-            owner=feature.owner,
-            provider=feature.provider,
-            location=ResourceColumnMapping("", "", ""),
-            description=feature.description,
-            tags=list(feature.tags.tag),
-            properties={k: v for k, v in feature.properties.property.items()},
-            status=feature.status.Status._enum_type.values[feature.status.status].name,
-            error=feature.status.error_message,
-        )
-
     def _create(self, stub) -> None:
         serialized = pb.FeatureVariant(
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
                 name=self.source[0],
                 variant=self.source[1],
@@ -1108,170 +1083,57 @@
             type=self.value_type,
             entity=self.entity,
             owner=self.owner,
             description=self.description,
             schedule=self.schedule,
             provider=self.provider,
             columns=self.location.proto(),
-            mode=ComputationMode.PRECOMPUTED.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateFeatureVariant(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("feature_variant",
-                  str(time.time()),
-                  self.description,
-                  self.entity,
-                  self.name,
-                  self.owner,
-                  self.provider,
-                  self.value_type,
-                  self.variant,
-                  "ready",
-                  self.location.entity,
-                  self.location.timestamp,
-                  self.location.value,
-                  self.source[0],
-                  self.source[1]
-                  )
-        if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "feature_variant", json.dumps(self.tags))
-        if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "feature_variant", json.dumps(self.properties))
-
-        self._write_feature_variant_and_mode(db)
-
-    def _write_feature_variant_and_mode(self, db) -> None:
         db.insert(
-            "features",
+            "feature_variant",
+            str(time.time()),
+            self.description,
+            self.entity,
             self.name,
-            self.variant,
+            self.owner,
+            self.provider,
             self.value_type,
-        )
-        is_on_demand = 0
-        db.insert(
-            "feature_computation_mode",
-            self.name,
             self.variant,
-            ComputationMode.PRECOMPUTED.value,
-            is_on_demand,
+            "ready",
+            self.location.entity,
+            self.location.timestamp,
+            self.location.value,
+            self.source[0],
+            self.source[1],
         )
-
-    def get_status(self):
-        return ResourceStatus(self.status)
-
-    def is_ready(self):
-        return self.status == ResourceStatus.READY.value
-
-    def __eq__(self, other):
-        for attribute in vars(self):
-            if getattr(self, attribute) != getattr(other, attribute):
-                return False
-        return True
-
-@typechecked
-@dataclass
-class OnDemandFeature:
-    owner: str
-    tags: List[str] = field(default_factory=list)
-    properties: dict = field(default_factory=dict)
-    variant: str = "default"
-    name: str = ""
-    description: str = ""
-    status: str = "READY"
-    error: Optional[str] = None
-
-    def __call__(self, fn):
-        if self.description == "" and fn.__doc__ is not None:
-            self.description = fn.__doc__
-        if self.name == "":
-            self.name = fn.__name__
-
-        self.query = dill.dumps(fn.__code__)
-        fn.name_variant = self.name_variant
-        fn.query = self.query
-        return fn
-
-    def name_variant(self):
-        return (self.name, self.variant)
-
-    @staticmethod
-    def operation_type() -> OperationType:
-        return OperationType.CREATE
-
-    @staticmethod
-    def type() -> str:
-        return "ondemand_feature"
-
-    def _create(self, stub) -> None:
-        serialized = pb.FeatureVariant(
-            name=self.name,
-            variant=self.variant,
-            owner=self.owner,
-            description=self.description,
-            function=pb.PythonFunction(query=self.query),
-            mode=ComputationMode.CLIENT_COMPUTED.proto(),
-            tags=pb.Tags(tag=self.tags),
-            properties=Properties(self.properties).serialized,
-            status=pb.ResourceStatus(status=pb.ResourceStatus.READY),
-        )
-        stub.CreateFeatureVariant(serialized)
-
-    def _create_local(self, db) -> None:
-        decode_query = base64.b64encode(self.query).decode("ascii")
-
-        db.insert("ondemand_feature_variant",
-                  str(time.time()),
-                  self.description,
-                  self.name,
-                  self.owner,
-                  self.variant,
-                  "ready",
-                  decode_query,
-                  )
-        if self.tags and len(self.tags):
-            db.upsert("tags", self.name, self.variant, "feature_variant", json.dumps(self.tags))
+        if len(self.tags):
+            db.upsert(
+                "tags",
+                self.name,
+                self.variant,
+                "feature_variant",
+                json.dumps(self.tags),
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "feature_variant", json.dumps(self.properties))
-
-        self._write_feature_variant_and_mode(db)
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "feature_variant",
+                json.dumps(self.properties),
+            )
+        self._create_feature_resource(db)
 
-    def _write_feature_variant_and_mode(self, db) -> None:
-        db.insert(
-            "features",
-            self.name,
-            self.variant,
-            "tbd",
-        )
-        is_on_demand = 1
-
-        db.insert(
-            "feature_computation_mode",
-            self.name,
-            self.variant,
-            ComputationMode.CLIENT_COMPUTED.value,
-            is_on_demand,
-        )
-    
-    def get(self, stub) -> "OnDemandFeature":
-        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
-        ondemand_feature = next(stub.GetFeatureVariants(iter([name_variant])))
-
-        return OnDemandFeature(
-            name=ondemand_feature.name,
-            variant=ondemand_feature.variant,
-            owner=ondemand_feature.owner,
-            description=ondemand_feature.description,
-            tags=list(ondemand_feature.tags.tag),
-            properties={k: v for k, v in ondemand_feature.properties.property.items()},
-            status=ondemand_feature.status.Status._enum_type.values[ondemand_feature.status.status].name,
-            error=ondemand_feature.status.error_message,
-        )
+    def _create_feature_resource(self, db) -> None:
+        db.insert("features", self.name, self.variant, self.value_type)
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1291,51 +1153,32 @@
     entity: str
     owner: str
     provider: str
     description: str
     tags: list
     properties: dict
     location: ResourceLocation
-    status: str = "NO_STATUS"
     variant: str = "default"
-    error: Optional[str] = None
+    status: str = "NO_STATUS"
 
     def __post_init__(self):
         col_types = [member.value for member in ColumnTypes]
         if self.value_type not in col_types:
-            raise ValueError(f"Invalid label type ({self.value_type}) must be one of: {col_types}")
+            raise ValueError(
+                f"Invalid label type ({self.value_type}) must be one of: {col_types}"
+            )
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "label"
 
-    def get(self, stub) -> "Label":
-        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
-        label = next(stub.GetLabelVariants(iter([name_variant])))
-
-        return Label(
-            name=label.name,
-            variant=label.variant,
-            source=(label.source.name, label.source.variant),
-            value_type=label.type,
-            entity=label.entity,
-            owner=label.owner,
-            provider=label.provider,
-            location=ResourceColumnMapping("", "", ""),
-            description=label.description,
-            tags=list(label.tags.tag),
-            properties={k: v for k, v in label.properties.property.items()},
-            status=label.status.Status._enum_type.values[label.status.status].name,
-            error=label.status.error_message
-        )
-
     def _create(self, stub) -> None:
         serialized = pb.LabelVariant(
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
                 name=self.source[0],
                 variant=self.source[1],
@@ -1347,43 +1190,47 @@
             columns=self.location.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateLabelVariant(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("label_variant",
-                  str(time.time()),
-                  self.description,
-                  self.entity,
-                  self.name,
-                  self.owner,
-                  self.provider,
-                  self.value_type,
-                  self.variant,
-                  self.location.entity,
-                  self.location.timestamp,
-                  self.location.value,
-                  "ready",
-                  self.source[0],
-                  self.source[1]
-                  )
+        db.insert(
+            "label_variant",
+            str(time.time()),
+            self.description,
+            self.entity,
+            self.name,
+            self.owner,
+            self.provider,
+            self.value_type,
+            self.variant,
+            self.location.entity,
+            self.location.timestamp,
+            self.location.value,
+            "ready",
+            self.source[0],
+            self.source[1],
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "label_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags", self.name, self.variant, "label_variant", json.dumps(self.tags)
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "label_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "label_variant",
+                json.dumps(self.properties),
+            )
         self._create_label_resource(db)
 
     def _create_label_resource(self, db) -> None:
-        db.insert(
-            "labels",
-            self.value_type,
-            self.variant,
-            self.name
-        )
+        db.insert("labels", self.value_type, self.variant, self.name)
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1440,15 +1287,17 @@
 
     def _get(self, stub):
         providerList = stub.GetProviders(iter([pb.Name(name=self.name)]))
         try:
             for provider in providerList:
                 self.obj = provider
         except grpc._channel._MultiThreadedRendezvous:
-            raise ValueError(f"Provider {self.name} of type {self.provider_type} not found.")
+            raise ValueError(
+                f"Provider {self.name} of type {self.provider_type} not found."
+            )
 
     def _get_local(self, db):
         local_provider = db.query_resource("providers", "name", self.name)
         if local_provider == []:
             raise ValueError("Local mode provider not found.")
         self.obj = local_provider
 
@@ -1465,15 +1314,17 @@
         return OperationType.GET
 
     @staticmethod
     def type() -> str:
         return "source"
 
     def _get(self, stub):
-        sourceList = stub.GetSourceVariants(iter([pb.NameVariant(name=self.name, variant=self.variant)]))
+        sourceList = stub.GetSourceVariants(
+            iter([pb.NameVariant(name=self.name, variant=self.variant)])
+        )
         try:
             for source in sourceList:
                 self.obj = source
         except grpc._channel._MultiThreadedRendezvous:
             raise ValueError(f"Source {self.name}, variant {self.variant} not found.")
 
     def _get_local(self, db):
@@ -1487,26 +1338,30 @@
 @dataclass
 class TrainingSet:
     name: str
     owner: str
     label: NameVariant
     features: List[NameVariant]
     description: str
+    tags: list
+    properties: dict
     feature_lags: list = field(default_factory=list)
-    tags: list = None
-    properties: dict = None
+    status: str = "NO_STATUS"
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     provider: str = ""
-    status: str = "NO_STATUS"
-    error: Optional[str] = None
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=6, schedule_string=schedule)
+        self.schedule_obj = Schedule(
+            name=self.name,
+            variant=self.variant,
+            resource_type=6,
+            schedule_string=schedule,
+        )
         self.schedule = schedule
 
     def __post_init__(self):
         if not valid_name_variant(self.label):
             raise ValueError("Label must be set")
         if len(self.features) == 0:
             raise ValueError("A training-set must have atleast one feature")
@@ -1518,33 +1373,14 @@
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "training-set"
 
-    def get(self, stub):
-        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
-        ts = next(stub.GetTrainingSetVariants(iter([name_variant])))
-
-        return TrainingSet(
-            name=ts.name,
-            variant=ts.variant,
-            owner=ts.owner,
-            description=ts.description,
-            status=ts.status.Status._enum_type.values[ts.status.status].name,
-            label=(ts.label.name, ts.label.variant),
-            features=[(f.name, f.variant) for f in ts.features],
-            feature_lags=[],
-            provider=ts.provider,
-            tags=list(ts.tags.tag),
-            properties={k: v for k, v in ts.properties.property.items()},
-            error=ts.status.error_message,
-        )
-
     def _create(self, stub) -> None:
         feature_lags = []
         for lag in self.feature_lags:
             lag_duration = Duration()
             _ = lag_duration.FromTimedelta(lag["lag"])
             feature_lag = pb.FeatureLag(
                 feature=lag["feature"],
@@ -1556,65 +1392,71 @@
 
         serialized = pb.TrainingSetVariant(
             name=self.name,
             variant=self.variant,
             description=self.description,
             schedule=self.schedule,
             owner=self.owner,
-            features=[
-                pb.NameVariant(name=v[0], variant=v[1]) for v in self.features
-            ],
+            features=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.features],
             label=pb.NameVariant(name=self.label[0], variant=self.label[1]),
             feature_lags=feature_lags,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateTrainingSetVariant(serialized)
 
     def _create_local(self, db) -> None:
         self._check_insert_training_set_resources(db)
-        db.insert("training_set_variant",
-                  str(time.time()),
-                  self.description,
-                  self.name,
-                  self.owner,
-                  self.variant,
-                  self.label[0],
-                  self.label[1],
-                  "ready"
-                  )
+        db.insert(
+            "training_set_variant",
+            str(time.time()),
+            self.description,
+            self.name,
+            self.owner,
+            self.variant,
+            self.label[0],
+            self.label[1],
+            "ready",
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "training_set_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags",
+                self.name,
+                self.variant,
+                "training_set_variant",
+                json.dumps(self.tags),
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "training_set_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "training_set_variant",
+                json.dumps(self.properties),
+            )
         self._create_training_set_resource(db)
 
     def _create_training_set_resource(self, db) -> None:
-        db.insert(
-            "training_sets",
-            "TrainingSet",
-            self.variant,
-            self.name
-        )
+        db.insert("training_sets", "TrainingSet", self.variant, self.name)
 
     def _check_insert_training_set_resources(self, db) -> None:
         try:
             db.get_label_variant(self.label[0], self.label[1])
         except ValueError:
-            raise ValueError(f"{self.label[0]} does not exist. Failed to register training set")
+            raise ValueError(
+                f"{self.label[0]} does not exist. Failed to register training set"
+            )
 
         for feature_name, feature_variant in self.features:
             try:
-                is_on_demand = db.get_feature_variant_on_demand(feature_name, feature_variant)
-                if is_on_demand:
-                    raise InvalidTrainingSetFeatureComputationMode(feature_name, feature_variant)
-            except InvalidTrainingSetFeatureComputationMode as e:
-                raise e
+                db.get_feature_variant(feature_name, feature_variant)
             except Exception as e:
-                raise Exception(f"{feature_name}:{feature_variant} does not exist. Failed to register training set. Error: {e}")
+                raise Exception(
+                    f"{feature_name} does not exist. Failed to register training set. Error: {e}"
+                )
 
             db.insert(
                 "training_set_features",
                 self.name,
                 self.variant,
                 feature_name,  # feature name
                 feature_variant,  # feature variant
@@ -1625,24 +1467,26 @@
             feature_variant = feature["variant"]
             feature_new_name = feature["name"]
             feature_lag = feature["lag"].total_seconds()
 
             try:
                 db.get_feature_variant(feature_name, feature_variant)
             except Exception as e:
-                raise Exception(f"{feature_name} does not exist. Failed to register training set. Error: {e}")
+                raise Exception(
+                    f"{feature_name} does not exist. Failed to register training set. Error: {e}"
+                )
 
             db.insert(
                 "training_set_lag_features",
                 self.name,
                 self.variant,
                 feature_name,  # feature name
                 feature_variant,  # feature variant
                 feature_new_name,  # feature new name
-                feature_lag  # feature_lag
+                feature_lag,  # feature_lag
             )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
@@ -1665,122 +1509,142 @@
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     def type(self) -> str:
         return "model"
 
     def _create(self, stub) -> None:
-        properties = pb.Properties(
-            property=self.properties
-        )
+        properties = pb.Properties(property=self.properties)
         serialized = pb.Model(
             name=self.name,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateModel(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("models",
-                  self.name,
-                  "Model",
-                  )
+        db.insert(
+            "models",
+            self.name,
+            "Model",
+        )
         if len(self.tags):
             db.upsert("tags", self.name, "", "models", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert("properties", self.name, "", "models", json.dumps(self.properties))
+            db.upsert(
+                "properties", self.name, "", "models", json.dumps(self.properties)
+            )
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
 
-Resource = Union[PrimaryData, Provider, Entity, User, Feature, Label,
-                 TrainingSet, Source, Schedule, ProviderReference, SourceReference, EntityReference, Model, OnDemandFeature]
+Resource = Union[
+    PrimaryData,
+    Provider,
+    Entity,
+    User,
+    Feature,
+    Label,
+    TrainingSet,
+    Source,
+    Schedule,
+    ProviderReference,
+    SourceReference,
+    EntityReference,
+    Model,
+]
 
 
 class ResourceRedefinedError(Exception):
     @typechecked
     def __init__(self, resource: Resource):
-        variantStr = f" variant {resource.variant}" if hasattr(
-            resource, 'variant') else ""
+        variantStr = (
+            f" variant {resource.variant}" if hasattr(resource, "variant") else ""
+        )
         resourceId = f"{resource.name}{variantStr}"
         super().__init__(
             f"{resource.type()} resource {resourceId} defined in multiple places"
         )
 
 
 class ResourceState:
-
     def __init__(self):
         self.__state = {}
+        self.__create_list = []
 
     @typechecked
     def add(self, resource: Resource) -> None:
-        if hasattr(resource, 'variant'):
-            key = (resource.operation_type().name, resource.type(), resource.name, resource.variant)
+        if hasattr(resource, "variant"):
+            key = (
+                resource.operation_type().name,
+                resource.type(),
+                resource.name,
+                resource.variant,
+            )
         else:
             key = (resource.operation_type().name, resource.type(), resource.name)
         if key in self.__state:
             if resource == self.__state[key]:
                 print(f"Resource {resource.type()} already registered.")
                 return
             raise ResourceRedefinedError(resource)
         self.__state[key] = resource
-        if hasattr(resource, 'schedule_obj') and resource.schedule_obj != None:
+        self.__create_list.append(resource)
+        if hasattr(resource, "schedule_obj") and resource.schedule_obj != None:
             my_schedule = resource.schedule_obj
             key = (my_schedule.type(), my_schedule.name)
             self.__state[key] = my_schedule
+            self.__create_list.append(my_schedule)
 
     def sorted_list(self) -> List[Resource]:
         resource_order = {
             "user": 0,
             "provider": 1,
             "source": 2,
             "entity": 3,
             "feature": 4,
-            "ondemand_feature": 5,
-            "label": 6,
-            "training-set": 7,
-            "schedule": 8,
-            "model": 9
+            "label": 5,
+            "training-set": 6,
+            "schedule": 7,
         }
 
         def to_sort_key(res):
             resource_num = resource_order[res.type()]
             variant = res.variant if hasattr(res, "variant") else ""
             return (resource_num, res.name, variant)
 
         return sorted(self.__state.values(), key=to_sort_key)
 
     def create_all_dryrun(self) -> None:
-        for resource in self.__state.values():
+        for resource in self.__create_list:
             if resource.operation_type() is OperationType.GET:
                 print("Getting", resource.type(), resource.name)
             if resource.operation_type() is OperationType.CREATE:
                 print("Creating", resource.type(), resource.name)
 
     def create_all_local(self) -> None:
         db = SQLiteMetadata()
         check_up_to_date(True, "register")
-        for resource in self.__state.values():
+        for resource in self.__create_list:
             if resource.operation_type() is OperationType.GET:
                 print("Getting", resource.type(), resource.name)
                 resource._get_local(db)
             if resource.operation_type() is OperationType.CREATE:
                 print("Creating", resource.type(), resource.name)
                 resource._create_local(db)
         db.close()
         return
 
     def create_all(self, stub) -> None:
         check_up_to_date(False, "register")
-        for resource in self.__state.values():
+        for resource in self.__create_list:
             if resource.type() == "provider" and resource.name == "local-mode":
                 continue
             try:
                 if resource.operation_type() is OperationType.GET:
                     print("Getting", resource.type(), resource.name)
                     resource._get(stub)
                 if resource.operation_type() is OperationType.CREATE:
@@ -1793,89 +1657,107 @@
 
                 raise e
 
 
 ## Executor Providers
 @typechecked
 class DatabricksCredentials:
-    def __init__(self,
-                 username: str = "",
-                 password: str = "",
-                 host: str = "",
-                 token: str = "",
-                 cluster_id: str = ""):
+    def __init__(
+        self,
+        username: str = "",
+        password: str = "",
+        host: str = "",
+        token: str = "",
+        cluster_id: str = "",
+    ):
         self.username = username
         self.password = password
         self.host = host
         self.token = token
         self.cluster_id = cluster_id
 
-        host_token_provided = username == "" and password == "" and host != "" and token != ""
-        username_password_provided = username != "" and password != "" and host == "" and token == ""
+        host_token_provided = (
+            username == "" and password == "" and host != "" and token != ""
+        )
+        username_password_provided = (
+            username != "" and password != "" and host == "" and token == ""
+        )
 
-        if not host_token_provided and not username_password_provided or host_token_provided and username_password_provided:
+        if (
+            not host_token_provided
+            and not username_password_provided
+            or host_token_provided
+            and username_password_provided
+        ):
             raise Exception(
-                "The DatabricksCredentials requires only one credentials set ('username' and 'password' or 'host' and 'token' set.)")
+                "The DatabricksCredentials requires only one credentials set ('username' and 'password' or 'host' and 'token' set.)"
+            )
 
         if not cluster_id:
             raise Exception("Cluster_id of existing cluster must be provided")
 
     def type(self):
         return "DATABRICKS"
 
     def config(self):
         return {
             "Username": self.username,
             "Password": self.password,
             "Host": self.host,
             "Token": self.token,
-            "Cluster": self.cluster_id
+            "Cluster": self.cluster_id,
         }
 
 
-
 @typechecked
 @dataclass
 class EMRCredentials:
-    def __init__(self,
-                 emr_cluster_id: str,
-                 emr_cluster_region: str,
-                 credentials: AWSCredentials):
-        
+    def __init__(
+        self, emr_cluster_id: str, emr_cluster_region: str, credentials: AWSCredentials
+    ):
         self.emr_cluster_id = emr_cluster_id
         self.emr_cluster_region = emr_cluster_region
         self.credentials = credentials
 
     def type(self):
         return "EMR"
 
     def config(self):
         return {
             "ClusterName": self.emr_cluster_id,
             "ClusterRegion": self.emr_cluster_region,
             "Credentials": self.credentials.config(),
         }
 
+
 @typechecked
 @dataclass
 class SparkCredentials:
-    def __init__(self,
-                 master: str,
-                 deploy_mode: str,
-                 python_version: str = "",
-                ):
-        
+    def __init__(
+        self,
+        master: str,
+        deploy_mode: str,
+        python_version: str = "",
+        core_site_path: str = "",
+        yarn_site_path: str = "",
+    ):
         self.master = master.lower()
         self.deploy_mode = deploy_mode.lower()
 
         if self.deploy_mode != "cluster" and self.deploy_mode != "client":
-            raise Exception(f"Spark does not support '{self.deploy_mode}' deploy mode. It only supports 'cluster' and 'client'.")
+            raise Exception(
+                f"Spark does not support '{self.deploy_mode}' deploy mode. It only supports 'cluster' and 'client'."
+            )
+
+        self.python_version = self._verify_python_version(
+            self.deploy_mode, python_version
+        )
+
+        self._verify_yarn_config()
 
-        self.python_version = self._verify_python_version(self.deploy_mode, python_version)
-    
     def _verify_python_version(self, deploy_mode, version):
         if deploy_mode == "cluster" and version == "":
             client_python_version = sys.version_info
             client_major = str(client_python_version.major)
             client_minor = str(client_python_version.minor)
 
             if client_major != MAJOR_VERSION:
@@ -1884,36 +1766,53 @@
                 client_minor = "7"
 
             version = f"{client_major}.{client_minor}"
 
         if version.count(".") == 2:
             major, minor, _ = version.split(".")
         elif version.count(".") == 1:
-            major, minor = version.split(".")    
+            major, minor = version.split(".")
         else:
-            raise Exception("Please specify your Python version on the Spark cluster. Accepted formats: Major.Minor or Major.Minor.Patch; ex. '3.7' or '3.7.16")
+            raise Exception(
+                "Please specify your Python version on the Spark cluster. Accepted formats: Major.Minor or Major.Minor.Patch; ex. '3.7' or '3.7.16"
+            )
 
         if major != MAJOR_VERSION or minor not in MINOR_VERSIONS:
-            raise Exception(f"The Python version {version} is not supported. Currently, supported versions are 3.7-3.10.")
-        
+            raise Exception(
+                f"The Python version {version} is not supported. Currently, supported versions are 3.7-3.10."
+            )
+
         """
         The Python versions on the Docker image are 3.7.16, 3.8.16, 3.9.16, and 3.10.10. 
         This conditional statement sets the patch number based on the minor version. 
         """
         if minor == "10":
             patch = "10"
         else:
             patch = "16"
-        
+
         return f"{major}.{minor}.{patch}"
 
+    def _verify_yarn_config(self):
+        if self.master == "yarn" and (
+            self.core_site_path == "" or self.yarn_site_path == ""
+        ):
+            raise Exception(
+                "Yarn requires core-site.xml and yarn-site.xml files."
+                "Please copy these files from your Spark instance to local, then provide the local path in "
+                "core_site_path and yarn_site_path. "
+            )
+
     def type(self):
         return "SPARK"
 
     def config(self):
         return {
             "Master": self.master,
             "DeployMode": self.deploy_mode,
-            "PythonVersion": self.python_version
+            "PythonVersion": self.python_version,
+            "CoreSite": open(self.core_site_path, "rb").read(),
+            "YarnSite": open(self.yarn_site_path, "rb").read(),
         }
 
+
 ExecutorCredentials = Union[EMRCredentials, DatabricksCredentials, SparkCredentials]
```

### Comparing `featureform-1.7.2rc0/src/featureform/search.py` & `featureform-1.7.3rc0/src/featureform/search.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/serving.py` & `featureform-1.7.3rc0/src/featureform/serving.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,30 +5,24 @@
 import os
 import re
 from typing import Union
 import dill
 import json
 import math
 import types
-import base64
 import random
 
 import numpy as np
 import pandas as pd
-from pandas.core.generic import NDFrame
 from pandasql import sqldf
 from featureform.proto import serving_pb2
-
-from .local_cache import LocalCache
-from .local_utils import get_sql_transformation_sources, feature_df_with_entity, list_to_combined_df, \
-    get_features_for_entity, feature_df_from_csv, label_df_from_csv, merge_feature_into_ts
 from .sqlite_metadata import SQLiteMetadata
 from featureform.proto import serving_pb2_grpc
 
-from .resources import Model, SourceType, ComputationMode
+from .resources import Model, SourceType
 from .tls import insecure_channel, secure_channel
 from .version import check_up_to_date
 
 
 def check_feature_type(features):
     checked_features = []
     for feature in features:
@@ -131,130 +125,74 @@
             return insecure_channel(host)
         else:
             return secure_channel(host, cert_path)
 
     def training_set(self, name, variation, include_label_timestamp, model: Union[str, Model] = None):
         return Dataset(self._stub).from_stub(name, variation, model)
 
-    def features(self, features, entities, model: Union[str, Model] = None, params: list = None):
+    def features(self, features, entities, model: Union[str, Model] = None):
         req = serving_pb2.FeatureServeRequest()
         for name, value in entities.items():
             entity_proto = req.entities.add()
             entity_proto.name = name
             entity_proto.value = value
         for (name, variation) in features:
             feature_id = req.features.add()
             feature_id.name = name
             feature_id.version = variation
         if model is not None:
             req.model.name = model if isinstance(model, str) else model.name
         resp = self._stub.FeatureServe(req)
-
-        feature_values = []
-        for val in resp.values:
-            parsed_value = parse_proto_value(val)
-
-            is_ondemand_feature = type(parsed_value) == bytes
-            if is_ondemand_feature:
-                code = dill.loads(bytearray(parsed_value))
-                func = types.FunctionType(code, globals(), "transformation")
-                parsed_value = func(self, params, entities)
-
-            feature_values.append(parsed_value)
-
-        return feature_values
+        return [parse_proto_value(val) for val in resp.values]
 
 
 class LocalClientImpl:
     def __init__(self):
         self.db = SQLiteMetadata()
-        self.local_cache = LocalCache(self.db)
         check_up_to_date(True, "serving")
 
-    def get_training_set_dataframe(
-        self, label, label_df, training_set_name, training_set_variant
-    ) -> NDFrame:
-        def get() -> pd.DataFrame:
-            feature_columns = []
-
-            # We will build the training set DF by merging each feature one by one into it.
-            training_set_df = label_df
-            features = self.db.get_training_set_features(
-                training_set_name, training_set_variant
-            )
-            for feature in features:
-                feature_variant = self.db.get_feature_variant(
-                    feature["feature_name"], feature["feature_variant"]
-                )
-                feature_df = self.get_feature_dataframe(feature_variant)
-                training_set_df = merge_feature_into_ts(
-                    feature_variant, label, feature_df, training_set_df
-                )
-                feature_columns.append(
-                    f"{feature['feature_name']}.{feature['feature_variant']}"
-                )
-
-            lag_features = self.db.get_training_set_lag_features(
-                training_set_name, training_set_variant
-            )
-            if len(lag_features) > 0:
-                timestamp_column = label["source_timestamp"]
-                entity_column = label["source_entity"]
-                label_column = "label"
-                lag_sql_query = self.get_lag_features_sql_query(
-                    lag_features,
-                    feature_columns,
-                    entity_column,
-                    label_column,
-                    timestamp_column,
-                )
-
-                globals()["source_0"] = training_set_df
-                mysql = lambda q: sqldf(q, globals())
-                training_set_df = mysql(lag_sql_query)
-
-            return training_set_df
-
-        return self.local_cache.get_or_put_training_set(
-            training_set_name=training_set_name,
-            training_set_variant=training_set_variant,
-            func=get
-        )
-
-    def training_set(
-        self,
-        training_set_name,
-        training_set_variant,
-        include_label_timestamp,
-        model: Union[str, Model] = None,
-    ):
-        training_set = self.db.get_training_set_variant(
-            training_set_name, training_set_variant
-        )
-
-        label = self.db.get_label_variant(
-            training_set["label_name"], training_set["label_variant"]
-        )
-        label_df = self.get_label_dataframe(label)
+    def training_set(self, training_set_name, training_set_variant, include_label_timestamp, model: Union[str, Model] = None):
+        training_set = self.db.get_training_set_variant(training_set_name, training_set_variant)
 
         if model is not None:
             self._register_model(
                 model,
                 look_up_table="model_training_sets",
                 association_name=training_set_name,
-                association_variant=training_set_variant,
+                association_variant=training_set_variant
             )
 
-        training_set_df = self.get_training_set_dataframe(
-            label, label_df, training_set_name, training_set_variant
-        )
-
-        return self.convert_ts_df_to_dataset(
-            label, training_set_df, include_label_timestamp
-        )
+        label = self.db.get_label_variant(training_set['label_name'], training_set['label_variant'])
+        label_df = self.get_label_dataframe(label)
+
+        feature_columns = []
+
+        # We will build the training set DF by merging each feature one by one into it.
+        trainingset_df = label_df
+        features = self.db.get_training_set_features(training_set_name, training_set_variant)
+        for feature_variant in features:
+            feature = self.db.get_feature_variant(feature_variant['feature_name'], feature_variant['feature_variant'])
+            feature_df = self.get_feature_dataframe(feature)
+            trainingset_df = self.merge_feature_into_ts(feature, label, feature_df, trainingset_df)
+
+            feature_columns.append(f"{feature_variant['feature_name']}.{feature_variant['feature_variant']}")
+
+        lag_features = self.db.get_training_set_lag_features(training_set_name, training_set_variant)
+        if len(lag_features) > 0:
+            timestamp_column = label["source_timestamp"]
+            entity_column = label["source_entity"]
+            label_column = "label"
+            lag_sql_query = self.get_lag_features_sql_query(lag_features, feature_columns, entity_column, label_column, timestamp_column)
+
+            globals()["source_0"] = trainingset_df
+            mysql = lambda q: sqldf(q, globals())
+            trainingset_df = mysql(lag_sql_query)
+        
+        return self.convert_ts_df_to_dataset(label, trainingset_df, include_label_timestamp)
+
 
     def get_lag_features_sql_query(self, lag_features, feature_columns, entity, label, ts):
         """
         Returns the SQL query to compute the lag features. 
         Input:
         - lag_features: dict
         
@@ -302,237 +240,254 @@
         lag_timestamps = " DESC, ".join(lag_timestamps)
 
         INNER_SELECT = f"SELECT {entity}, {ts}, {label}, {features}, {lag_columns}, ROW_NUMBER() over (PARTITION BY {entity}, {label}, {ts} ORDER BY {ts} DESC, {lag_timestamps} DESC) as row_number"
         FULL_QUERY = f"{MAIN_SELECT}, {label} {SUBQUERY} {INNER_SELECT} {INNER_QUERY} {LAG_QUERIES} {CLOSING_QUERY}"
 
         return FULL_QUERY
 
+
     def get_input_df(self, source_name, source_variant):
         if self.db.is_transformation(source_name, source_variant) == SourceType.PRIMARY_SOURCE.value:
             source = self.db.get_source_variant(source_name, source_variant)
             df = pd.read_csv(str(source['definition']))
         else:
             df = self.process_transformation(source_name, source_variant)
         return df
 
     def sql_transformation(self, query):
-        transformation_sources = get_sql_transformation_sources(query)
-        for i, (source_name, source_variant) in enumerate(transformation_sources):
+        # Use regex to parse query inputs in double curly braces {{ }} and store in a list
+        inputs = re.findall("(?={{).*?(?<=}})", query)
+        for i, input in enumerate(inputs):
+            # Trim curly braces before and after to get name.variant from {{name.variant}}
+            name_variant = input[2:-2].split(".")
+            source_name, source_variant = name_variant[0], name_variant[1]
             # Creates a variable called dataframes_i which stores the corresponding df for each input
             df_variable = f"dataframes_{i}"
             # globals()[df_variable]:
             # 1. Converts a string "dataframes_i" to a variable name
             # 2. Assigns a global scope to the variable, to access it outside the loop
             globals()[df_variable] = self.get_input_df(source_name, source_variant)
-
-            # using '+' signs for readability
-            query_source_to_replace = '{{' + f'{source_name}.{source_variant}' + '}}'
-            query = query.replace(query_source_to_replace, df_variable)
+            query = query.replace(input, df_variable)
 
         return sqldf(query, globals())
 
     def process_transformation(self, name, variant):
-
-        def get():
-            source = self.db.get_source_variant(name, variant)
-            if self.db.is_transformation(name, variant) == SourceType.SQL_TRANSFORMATION.value:
-                query = source['definition']
-                new_data = self.sql_transformation(query)
-            else:
-                code = dill.loads(bytearray(source['definition']))
-                inputs = json.loads(source['inputs'])
-                dataframes = []
-                for input in inputs:
-                    source_name, source_variant = input[0], input[1],
-                    dataframes.append(self.get_input_df(source_name, source_variant))
-                func = types.FunctionType(code, globals(), "transformation")
-                new_data = func(*dataframes)
-            return new_data
-
-        return self.local_cache.get_or_put(
-            resource_type='transformation',
-            resource_name=name,
-            resource_variant=variant,
-            source_name=name,
-            source_variant=variant,
-            func=get
-        )
-
-    def get_label_dataframe(self, label) -> NDFrame:
-
-        def get() -> pd.DataFrame:
-            transform_type = self.db.is_transformation(
-                label["source_name"], label["source_variant"]
-            )
-            if (
-                transform_type == SourceType.SQL_TRANSFORMATION.value
-                or transform_type == SourceType.DF_TRANSFORMATION.value
-            ):
-                label_df = self.label_df_from_transformation(label)
-            else:
-                label_source = self.db.get_source_variant(
-                    label["source_name"], label["source_variant"]
-                )
-                label_df = label_df_from_csv(label, label_source["definition"])
-            label_df.rename(columns={label["source_value"]: "label"}, inplace=True)
-            return label_df
-
-        return self.local_cache.get_or_put(
-            resource_type='label',
-            resource_name=label['name'],
-            resource_variant=label['variant'],
-            source_name=label['source_name'],
-            source_variant=label['source_variant'],
-            func=get
-        )
+        source = self.db.get_source_variant(name, variant)
+        if self.db.is_transformation(name, variant) == SourceType.SQL_TRANSFORMATION.value:
+            query = source['definition']
+            new_data = self.sql_transformation(query)
+        else:
+            code = dill.loads(bytearray(source['definition']))
+            inputs = json.loads(source['inputs'])
+            dataframes = []
+            for input in inputs:
+                source_name, source_variant = input[0], input[1],
+                dataframes.append(self.get_input_df(source_name, source_variant))
+            func = types.FunctionType(code, globals(), "transformation")
+            new_data = func(*dataframes)
+
+        return new_data
+
+    def get_label_dataframe(self, label):
+        transform_type = self.db.is_transformation(label['source_name'], label['source_variant'])
+        if transform_type == SourceType.SQL_TRANSFORMATION.value or transform_type == SourceType.DF_TRANSFORMATION.value:
+            label_df = self.label_df_from_transformation(label)
+        else:
+            label_source = self.db.get_source_variant(label['source_name'], label['source_variant'])
+            label_df = self.label_df_from_csv(label, label_source['definition'])
+        label_df.rename(columns={label['source_value']: 'label'}, inplace=True)
+        return label_df
 
     def label_df_from_transformation(self, label):
         df = self.process_transformation(label['source_name'], label['source_variant'])
         if label['source_timestamp'] != "":
             df = df[[label['source_entity'], label['source_value'], label['source_timestamp']]]
             df[label['source_timestamp']] = pd.to_datetime(df[label['source_timestamp']])
         else:
             df = df[[label['source_entity'], label['source_value']]]
         df.set_index(label['source_entity'])
         return df
 
-    def get_feature_dataframe(self, feature) -> NDFrame:
+    def label_df_from_csv(self, label, file_name):
+        df = pd.read_csv(file_name)
+        self.check_missing_values(label, df)
+        if label['source_timestamp'] != "":
+            df = df[[label['source_entity'], label['source_value'], label['source_timestamp']]]
+            df[label['source_timestamp']] = pd.to_datetime(df[label['source_timestamp']])
+            df.sort_values(by=label['source_timestamp'], inplace=True)
+            df.drop_duplicates(subset=[label['source_entity'], label['source_timestamp']], keep="last", inplace=True)
+        else:
+            df = df[[label['source_entity'], label['source_value']]]
+        df.set_index(label['source_entity'], inplace=True)
+        return df
 
-        def get() -> pd.DataFrame:
-            name_variant = feature['name'] + "." + feature['variant']
-            transform_type = self.db.is_transformation(feature['source_name'], feature['source_variant'])
-            if transform_type == SourceType.SQL_TRANSFORMATION.value or transform_type == SourceType.DF_TRANSFORMATION.value:
-                feature_df = self.feature_df_from_transformation(feature)
-            else:
-                source = self.db.get_source_variant(feature['source_name'], feature['source_variant'])
-                feature_df = feature_df_from_csv(feature, source['definition'])
-            feature_df.set_index(feature['source_entity'])
-            feature_df.rename(columns={feature['source_value']: name_variant}, inplace=True)
-            return feature_df
-
-        return self.local_cache.get_or_put(
-            resource_type='feature',
-            resource_name=feature['name'],
-            resource_variant=feature['variant'],
-            source_name=feature['source_name'],
-            source_variant=feature['source_variant'],
-            func=get
-        )
+    def get_feature_dataframe(self, feature):
+        name_variant = feature['name'] + "." + feature['variant']
+        transform_type = self.db.is_transformation(feature['source_name'], feature['source_variant'])
+        if transform_type == SourceType.SQL_TRANSFORMATION.value or transform_type == SourceType.DF_TRANSFORMATION.value:
+            feature_df = self.feature_df_from_transformation(feature)
+        else:
+            source = self.db.get_source_variant(feature['source_name'], feature['source_variant'])
+            feature_df = self.feature_df_from_csv(feature, source['definition'])
+        feature_df.set_index(feature['source_entity'])
+        feature_df.rename(columns={feature['source_value']: name_variant}, inplace=True)
+        return feature_df
 
     def feature_df_from_transformation(self, feature):
         df = self.process_transformation(feature['source_name'], feature['source_variant'])
         if isinstance(df, pd.Series):
             df = df.to_frame()
             df.reset_index(inplace=True)
         if feature['source_timestamp'] != "":
             df = df[[feature['source_entity'], feature['source_value'], feature['source_timestamp']]]
             df[feature['source_timestamp']] = pd.to_datetime(df[feature['source_timestamp']])
         else:
             df = df[[feature['source_entity'], feature['source_value']]]
         return df
 
-    def features(self, feature_variant_list, entities, model: Union[str, Model] = None, params: list = None):
-        if len(feature_variant_list) == 0:
-            raise Exception("No features provided")
+    def feature_df_from_csv(self, feature, filename):
+        df = pd.read_csv(str(filename))
+        self.check_missing_values(feature, df)
+        if feature['source_timestamp'] != "":
+            df = df[[feature['source_entity'], feature['source_value'], feature['source_timestamp']]]
+            df[feature['source_timestamp']] = pd.to_datetime(df[feature['source_timestamp']])
+            df = df.sort_values(by=feature['source_timestamp'], ascending=True)
+        else:
+            df = df[[feature['source_entity'], feature['source_value']]]
+        return df
 
-        self.entities = entities
-        self.params = params if params else []
+    def merge_feature_into_ts(self, feature_row, label_row, df, trainingset_df):
+        if feature_row['source_timestamp'] != "":
+            trainingset_df = pd.merge_asof(trainingset_df, df.sort_values(feature_row['source_timestamp']),
+                                           direction='backward',
+                                           left_on=label_row['source_timestamp'],
+                                           right_on=feature_row['source_timestamp'], left_by=label_row['source_entity'],
+                                           right_by=feature_row['source_entity'])
+            if feature_row['source_timestamp'] != label_row['source_timestamp']:
+                trainingset_df.drop(columns=feature_row['source_timestamp'], inplace=True)
+        else:
+            df.drop_duplicates(subset=[feature_row['source_entity']], keep="last", inplace=True)
+            trainingset_df.reset_index(inplace=True)
+            trainingset_df[label_row['source_entity']] = trainingset_df[label_row['source_entity']].astype('string')
+            df[label_row['source_entity']] = df[label_row['source_entity']].astype('string')
+            trainingset_df = trainingset_df.join(df.set_index(label_row['source_entity']), how="left",
+                                                 on=label_row['source_entity'],
+                                                 lsuffix="_left")
+            if "index" in trainingset_df.columns:
+                trainingset_df.drop(columns='index', inplace=True)
+        return trainingset_df
+
+    def convert_ts_df_to_dataset(self, label_row, trainingset_df, include_label_timestamp): 
+        if label_row['source_timestamp'] != "" and include_label_timestamp != True:
+            trainingset_df.drop(columns=label_row['source_timestamp'], inplace=True)
+        elif label_row['source_timestamp'] != "" and include_label_timestamp:
+            source_timestamp_col = trainingset_df.pop(label_row['source_timestamp'])
+            trainingset_df = trainingset_df.assign(label_timestamp=source_timestamp_col)
+        trainingset_df.drop(columns=label_row['source_entity'], inplace=True)
+            
+        label_col = trainingset_df.pop('label')
+        trainingset_df = trainingset_df.assign(label=label_col)
+        return Dataset.from_dataframe(trainingset_df, include_label_timestamp)
 
+    def features(self, feature_variant_list, entities, model: Union[str, Model] = None):
+        if len(feature_variant_list) == 0:
+            raise Exception("No features provided")
         # This code assumes that the entities dictionary only has one entity
         entity_id = list(entities.keys())[0]
         entity_value = entities[entity_id]
         all_features_list = self.add_feature_dfs_to_list(feature_variant_list, entity_id)
-        all_features_df = list_to_combined_df(all_features_list, entity_id)
-        features = get_features_for_entity(entity_id, entity_value, all_features_df)
+        all_features_df = self.list_to_combined_df(all_features_list, entity_id)
+        features = self.get_features_for_entity(entity_id, entity_value, all_features_df)
 
         if model is not None:
             for feature_name, feature_variant in feature_variant_list:
                 self._register_model(
                     model,
                     look_up_table="model_features",
                     association_name=feature_name,
                     association_variant=feature_variant
                 )
 
         return features
 
     def add_feature_dfs_to_list(self, feature_variant_list, entity_id):
         feature_df_list = []
-
         for feature_variant in feature_variant_list:
-            f_name = feature_variant[0]
-            f_variant = feature_variant[1]
-            f_mode = self.db.get_feature_variant_mode(f_name, f_variant)
-
-            if f_mode == ComputationMode.CLIENT_COMPUTED:
-                feature_df = self.calculate_ondemand_feature(f_name, f_variant, entity_id)
+            feature = self.db.get_feature_variant(feature_variant[0], feature_variant[1])
+            name_variant = f"{feature['name']}.{feature['variant']}"
+            source_name, source_variant = feature['source_name'], feature['source_variant']
+            if feature["entity"] != entity_id:
+                raise ValueError(
+                    f"Invalid entity {entity_id} for feature {source_name}-{source_variant}")
+            if self.db.is_transformation(source_name, source_variant) != SourceType.PRIMARY_SOURCE.value:
+                feature_df = self.process_transformation(source_name, source_variant)
+                if isinstance(feature_df, pd.Series):
+                    feature_df = feature_df.to_frame()
+                    feature_df.reset_index(inplace=True)
+                if not feature["source_entity"] in feature_df.columns:
+                    raise ValueError(
+                        f"Could not set entity column. No column name {feature['source_entity']} exists in {source_name}-{source_variant}")
+                if not feature['source_value'] in feature_df.columns:
+                    raise ValueError(
+                        f"Could not access feature value column. No column name {feature['source_value']} exists in {source_name}-{source_variant}")
+                feature_df = feature_df[[feature['source_entity'], feature['source_value']]]
+                feature_df.rename(columns={feature['source_entity']: entity_id, feature['source_value']: name_variant}, inplace=True)
+                feature_df.drop_duplicates(subset=[entity_id], keep="last", inplace=True)
+                feature_df.set_index(entity_id)
             else:
-                feature_df = self.get_precomputed_feature(f_name, f_variant, entity_id)
-
+                source = self.db.get_source_variant(source_name, source_variant)
+                feature_df = self.feature_df_with_entity(source['definition'], entity_id, feature)
             feature_df_list.append(feature_df)
 
         return feature_df_list
 
-    def get_precomputed_feature(self, f_name, f_variant, entity_id):
-        feature = self.db.get_feature_variant(f_name, f_variant)
-        source_name, source_variant = feature['source_name'], feature['source_variant']
-        if feature["entity"] != entity_id:
-            raise ValueError(
-                f"Invalid entity {entity_id} for feature {source_name}-{source_variant}")
-        if self.db.is_transformation(source_name, source_variant) != SourceType.PRIMARY_SOURCE.value:
-            feature_df = self.process_non_primary_df_transformation(feature, source_name, source_variant, entity_id)
+    def list_to_combined_df(self, features_list, entity_id):
+        all_feature_df = None
+        try:
+            for feature in features_list:
+                if all_feature_df is None:
+                    all_feature_df = feature
+                else:
+                    all_feature_df = all_feature_df.join(feature.set_index(entity_id), on=entity_id,
+                                                         lsuffix='_left')
+            return all_feature_df
+        except TypeError:
+            print("Set is empty")
+
+    def get_features_for_entity(self, entity_id, entity_value, all_feature_df):
+        entity = all_feature_df.loc[all_feature_df[entity_id] == entity_value].copy()
+        entity.drop(columns=entity_id, inplace=True)
+        if len(entity.values) > 0:
+            return entity.values[0]
         else:
-            source = self.db.get_source_variant(source_name, source_variant)
-            feature_df = feature_df_with_entity(source['definition'], entity_id, feature)
-
-        return feature_df
+            raise Exception(f"No matching entities for {entity_id}: {entity_value}")
 
-    def process_non_primary_df_transformation(self, feature, source_name, source_variant, entity_id):
+    def feature_df_with_entity(self, source_path, entity_id, feature):
         name_variant = f"{feature['name']}.{feature['variant']}"
-        feature_df = self.process_transformation(source_name, source_variant)
-        if isinstance(feature_df, pd.Series):
-            feature_df = feature_df.to_frame()
-            feature_df.reset_index(inplace=True)
-        if not feature["source_entity"] in feature_df.columns:
-            raise ValueError(
-                f"Could not set entity column. No column name {feature['source_entity']} exists in {source_name}-{source_variant}")
-        if not feature['source_value'] in feature_df.columns:
-            raise ValueError(
-                f"Could not access feature value column. No column name {feature['source_value']} exists in {source_name}-{source_variant}")
-        feature_df = feature_df[[feature['source_entity'], feature['source_value']]]
-        feature_df.rename(columns={feature['source_entity']: entity_id, feature['source_value']: name_variant}, inplace=True)
-        feature_df.drop_duplicates(subset=[entity_id], keep="last", inplace=True)
-        feature_df.set_index(entity_id)
-        return feature_df
-
-    def calculate_ondemand_feature(self, f_name, f_variant, entity_id):
-        query = self.db.get_ondemand_feature_query(f_name, f_variant)
-        base64_bytes = query.encode("ascii")
-        query = base64.b64decode(base64_bytes)
-
-        code = dill.loads(bytearray(query))
-        func = types.FunctionType(code, globals(), "transformation")
-        output_value = func(self, self.params, self.entities)
-
-        feature_col_name = f"{f_name}.{f_variant}"
-        df = pd.DataFrame.from_dict({entity_id: [self.entities.get(entity_id, "")], feature_col_name: [output_value]})
+        df = pd.read_csv(str(source_path))
+        self.check_missing_values(feature, df)
+        if feature['source_timestamp'] != "":
+            df = df[[feature['source_entity'], feature['source_value'], feature['source_timestamp']]]
+            df = df.sort_values(by=feature['source_timestamp'], ascending=True)
+            df = df.drop(columns=feature['source_timestamp'])
+        else:
+            df = df[[feature['source_entity'], feature['source_value']]]
+        df.set_index(feature['source_entity'])
+        df.rename(columns={feature['source_entity']: entity_id, feature['source_value']: name_variant}, inplace=True)
+        df.drop_duplicates(subset=[entity_id], keep="last", inplace=True)
         return df
 
-    @staticmethod
-    def convert_ts_df_to_dataset(label_row, trainingset_df, include_label_timestamp):
-        if label_row["source_timestamp"] != "" and include_label_timestamp != True:
-            trainingset_df.drop(columns=label_row["source_timestamp"], inplace=True)
-        elif label_row["source_timestamp"] != "" and include_label_timestamp:
-            source_timestamp_col = trainingset_df.pop(label_row["source_timestamp"])
-            trainingset_df = trainingset_df.assign(label_timestamp=source_timestamp_col)
-        trainingset_df.drop(columns=label_row["source_entity"], inplace=True)
+    def check_missing_values(self, resource, df):
+        if resource['source_entity'] not in df.columns:
+            raise KeyError(f"Entity column does not exist: {resource['source_entity']}")
+        if resource['source_value'] not in df.columns:
+            raise KeyError(f"Value column does not exist: {resource['source_value']}")
+        if resource['source_timestamp'] not in df.columns and resource['source_timestamp'] != "":
+            raise KeyError(f"Timestamp column does not exist: {resource['source_timestamp']}")
 
-        label_col = trainingset_df.pop("label")
-        trainingset_df = trainingset_df.assign(label=label_col)
-        return Dataset.from_dataframe(trainingset_df, include_label_timestamp)
 
     def _register_model(self, model: Union[str, Model], look_up_table: str, association_name: str, association_variant: str):
         name = model if isinstance(model, str) else model.name
         type = "Model" if isinstance(model, str) else model.type()
 
         self.db.insert("models", name, type)
         self.db.insert(look_up_table, name, association_name, association_variant)
```

### Comparing `featureform-1.7.2rc0/src/featureform/sqlite_metadata.py` & `featureform-1.7.3rc0/src/featureform/sqlite_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,45 +60,22 @@
 
           PRIMARY KEY(name, variant),
 
           FOREIGN KEY(name) REFERENCES features(name),
           FOREIGN KEY(entity) REFERENCES entities(name),
           FOREIGN KEY(provider) REFERENCES providers(name),
           FOREIGN KEY(source_name) REFERENCES sources(name))''')
-      
-        # OnDemand Features variant table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS ondemand_feature_variant(
-          created text,
-          description text,
-          name text NOT NULL,
-          owner text,
-          variant text NOT NULL,
-          status text,
-          query text,
-
-          PRIMARY KEY(name, variant),
-
-          FOREIGN KEY(name) REFERENCES features(name))''')
 
         # Features table
         self.__conn.execute('''CREATE TABLE IF NOT EXISTS features(
           name text NOT NULL,
           default_variant text NOT NULL,
           type text,
           PRIMARY KEY (name));''')
 
-        # features type table
-        # this is used to determine if it is a pre-calculated or client-calculated feature
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS feature_computation_mode (
-          name text NOT NULL,
-          variant text NOT NULL,
-          mode text,
-          is_on_demand integer,
-          PRIMARY KEY (name, variant));''')
-
         # training set variant
         self.__conn.execute('''CREATE TABLE IF NOT EXISTS training_set_variant(
           created text,
           description text,            
           name text NOT NULL,
           owner text,
           variant text,
@@ -221,25 +198,14 @@
           provider_type     text,
           software         text,
           team             text,
           sources          text,
           status           text,
           serialized_config text)''')
 
-        # source files for a resource
-        # tracks the source files that have been used to create a resource and contains the files last_updated
-        # this is used to determined if caches need to be invalidated
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS resource_source_files(
-            resource_type text NOT NULL,
-            name text NOT NULL,
-            variant text NOT NULL,
-            file_path text NOT NULL,
-            updated_at text NOT NULL,
-            PRIMARY KEY(resource_type, name, variant, file_path))''')
-
         # full-text search table
         self.__conn.execute('''CREATE VIRTUAL TABLE IF NOT EXISTS resources_fts USING fts5(
           resource_type, -- an "enum" column to filter with (e.g. feature, training_set, source, provider, entity, label, model, user)
           name,
           variant,
           description,
           status,
@@ -380,27 +346,27 @@
       return self.query_resource("users", "name", name, should_fetch_tags_properties)[0]
 
     def get_entity(self, name, should_fetch_tags_properties):
       return self.query_resource("entities", "name", name, should_fetch_tags_properties)[0]
 
     def get_feature(self, name, should_fetch_tags_properties):
       return self.query_resource("features", "name", name, should_fetch_tags_properties)[0]
-
+    
     def get_label(self, name, should_fetch_tags_properties):
       return self.query_resource("labels", "name", name, should_fetch_tags_properties)[0]
-
+    
     def get_source(self, name, should_fetch_tags_properties):
       return self.query_resource("sources", "name", name, should_fetch_tags_properties)[0]
 
     def get_training_set(self, name, should_fetch_tags_properties):
       return self.query_resource("training_sets", "name", name, should_fetch_tags_properties)[0]
-
+    
     def get_model(self, name, should_fetch_tags_properties):
       return self.query_resource("models", "name", name, should_fetch_tags_properties)[0]
-
+    
     def get_provider(self, name, should_fetch_tags_properties):
       return self.query_resource("providers", "name", name, should_fetch_tags_properties)[0]
 
     def get_feature_variant(self, name, variant):
         query = '''SELECT fv.*, t.tag_list as tags, p.property_list as properties
         FROM feature_variant fv
         LEFT JOIN tags t ON t.name = fv.name AND t.variant = fv.variant
@@ -417,26 +383,14 @@
         LEFT JOIN tags t ON t.name = fv.name AND t.variant = fv.variant
         LEFT JOIN properties p ON p.name = fv.name AND p.variant = fv.variant
         WHERE fv.source_name = '{0}' AND fv.source_variant = '{1}';'''.format(name, variant)
         return self.fetch_data_safe(query, "feature_variant", name, variant)
 
     def get_feature_variants_from_feature(self, name):
       return self.query_resource_variant("feature_variant", "name", name)
-    
-    def get_feature_variant_mode(self, name, variant):
-      query = f"SELECT mode FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
-      return self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0]["mode"]
-    
-    def get_feature_variant_on_demand(self, name, variant):
-      query = f"SELECT is_on_demand FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
-      return bool(self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0]["is_on_demand"])
-
-    def get_ondemand_feature_query(self, name, variant):
-      query = f"SELECT query FROM ondemand_feature_variant WHERE name='{name}' AND variant='{variant}'"
-      return self.fetch_data_safe(query, "ondemand_feature_variant", name, variant)[0]["query"]
 
     def get_training_set_variant(self, name, variant):
         query = f"SELECT * FROM training_set_variant WHERE name = '{name}' AND variant = '{variant}';"
         query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
@@ -542,51 +496,27 @@
         transformation = self.__conn.execute(query)
         self.__conn.commit()
         t = transformation.fetchall()
         if len(t) == 0:
             return 0
         return t[0][0]
 
-    def get_source_files_for_resource(self, resource_type, name, variant):
-        query = f"SELECT * FROM resource_source_files WHERE resource_type='{resource_type}' and name='{name}' and variant='{variant}';"
-        result = self.__conn.execute(query)
-        self.__conn.commit()
-        return result.fetchall()
-
-    def get_source_file_last_updated(self, resource_type, name, variant, file_path):
-        query = f"SELECT * FROM resource_source_files WHERE resource_type='{resource_type}' and name='{name}' and variant='{variant}' and file_path='{file_path}';"
-        result = self.__conn.execute(query)
-        self.__conn.commit()
-        res = result.fetchone()
-        return res[0] if res else None
-
     def insert_source(self, tablename, *args):
         stmt = f"INSERT OR IGNORE INTO {tablename} VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
         self.__conn.execute_stmt(stmt, args)
         self.__conn.commit()
 
     def insert(self, tablename, *args):
         query = f"INSERT OR IGNORE INTO {tablename} VALUES {str(args)}"
         self.__conn.execute(query)
         self.__conn.commit()
 
-    def insert_or_update(self, tablename, keys, cols, *args):
-        """
-        Upserts a row into the table. `keys` indicate columns that are unique
-        and `cols` are the columns that are updated.
-        """
-        query = (
-            f"INSERT INTO {tablename} VALUES {str(args)} "
-            f"ON CONFLICT ({','.join(keys)}) DO UPDATE SET {','.join([f'{col}=excluded.{col}' for col in cols])}"
-        )
-        self.__conn.execute(query)
-        self.__conn.commit()
-
-    # TODO get something generic working, possibly consider using the above insert or update
     def upsert(self, tablename, *args):
+        query = ""
+        is_update = False
         if tablename == "tags" or tablename == "properties":
            query, is_update = self.upsert_tags_properties(tablename, *args)
         else:
            raise NotImplementedError(f"UPSERT not implemented for table {tablename}")
 
         if is_update:
           self.__conn.execute(query)
```

### Comparing `featureform-1.7.2rc0/src/featureform/type_objects.py` & `featureform-1.7.3rc0/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform/version.py` & `featureform-1.7.3rc0/src/featureform/version.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/src/featureform.egg-info/PKG-INFO` & `featureform-1.7.3rc0/src/featureform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.7.2rc0
+Version: 1.7.3rc0
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.7.2rc0/src/featureform.egg-info/SOURCES.txt` & `featureform-1.7.3rc0/src/featureform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,23 @@
 README.md
 pyproject.toml
 setup.cfg
 src/featureform/__init__.py
 src/featureform/__main__.py
 src/featureform/cli.py
 src/featureform/dashboard_metadata.py
-src/featureform/enums.py
-src/featureform/exceptions.py
 src/featureform/format.py
 src/featureform/get.py
 src/featureform/get_local.py
 src/featureform/get_test.py
 src/featureform/list.py
 src/featureform/list_local.py
 src/featureform/list_test.py
 src/featureform/local.py
-src/featureform/local_cache.py
 src/featureform/local_dash_test.py
-src/featureform/local_utils.py
 src/featureform/register.py
 src/featureform/register_test.py
 src/featureform/resources.py
 src/featureform/search.py
 src/featureform/search_local.py
 src/featureform/serving.py
 src/featureform/serving_test.py
@@ -43,16 +39,16 @@
 src/featureform/dashboard/out/index.html
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/[type]/[entity].html
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-src/featureform/dashboard/out/_next/static/ZeSp5jbiz_whztxZm-YJw/_buildManifest.js
-src/featureform/dashboard/out/_next/static/ZeSp5jbiz_whztxZm-YJw/_ssgManifest.js
+src/featureform/dashboard/out/_next/static/MIAYyZbApb_poPrdNhxsm/_buildManifest.js
+src/featureform/dashboard/out/_next/static/MIAYyZbApb_poPrdNhxsm/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
 src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
 src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
 src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
 src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
 src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
@@ -278,15 +274,15 @@
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
 src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
 src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
-src/featureform/dashboard/out/_next/static/chunks/pages/_app-131cf942d8b62ea7.js
+src/featureform/dashboard/out/_next/static/chunks/pages/_app-01b1894ee40506d5.js
 src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
 src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
 src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
 src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
 src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
@@ -326,16 +322,14 @@
 src/featureform/proto/serving.proto
 src/featureform/proto/serving_pb2.py
 src/featureform/proto/serving_pb2_grpc.py
 tests/test_class_api.py
 tests/test_cli.py
 tests/test_executor_resources.py
 tests/test_getting_model.py
-tests/test_localmode_caching.py
 tests/test_localmode_include_label_ts.py
 tests/test_localmode_lag_features.py
-tests/test_ondemand_features.py
 tests/test_search.py
 tests/test_serving_model.py
 tests/test_spark_provider.py
 tests/test_tags_and_properties.py
 tests/test_updating_provider.py
```

### Comparing `featureform-1.7.2rc0/tests/test_cli.py` & `featureform-1.7.3rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/tests/test_executor_resources.py` & `featureform-1.7.3rc0/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/tests/test_getting_model.py` & `featureform-1.7.3rc0/tests/test_getting_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,10 @@
     setup_teardown()
     yield
     setup_teardown()
 
 def arrange_resources(model_name, is_local, is_insecure):
     ff.register_model(model_name)
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
-    resource_client.apply(asynchronous=True)
+    resource_client.apply()
 
     return resource_client
```

### Comparing `featureform-1.7.2rc0/tests/test_localmode_include_label_ts.py` & `featureform-1.7.3rc0/tests/test_localmode_include_label_ts.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,41 @@
 
     @local.df_transformation(variant="quickstart",
                                 inputs=[("transactions", "quickstart")])
     def average_user_transaction(transactions):
         """the average transaction amount for a user """
         return transactions.groupby("CustomerID")["TransactionAmount"].mean()
 
+    @local.sql_transformation(variant="quickstart")
+    def sql_average_user_transaction():
+        """the average transaction amount for a user """
+        return "SELECT CustomerID as user_id, avg(TransactionAmount) " \
+            "as avg_transaction_amt from {{transactions.kaggle}} GROUP BY user_id"
+
     user = ff.register_entity("user")
 
     # Register a column from our transformation as a feature
     average_user_transaction.register_resources(
         entity=user,
         entity_column="CustomerID",
         inference_store=local,
         features=[
             {"name": "avg_transactions", "variant": "quickstart", "column": "TransactionAmount", "type": "float32"},
         ],
     )
 
+    sql_average_user_transaction.register_resources(
+        entity=user,
+        entity_column="CustomerID",
+        inference_store=local,
+        features=[
+            {"name": "avg_transactions", "variant": "sql", "column": "TransactionAmount", "type": "float32"},
+        ],
+    )
+
     # Register label from our base Transactions table
     transactions.register_resources(
         entity=user,
         entity_column="CustomerID",
         timestamp_column="Timestamp",
         labels=[
             {"name": "fraudulent", "variant": "quickstart", "column": "IsFraud", "type": "bool"},
```

### Comparing `featureform-1.7.2rc0/tests/test_localmode_lag_features.py` & `featureform-1.7.3rc0/tests/test_localmode_lag_features.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/tests/test_search.py` & `featureform-1.7.3rc0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/tests/test_serving_model.py` & `featureform-1.7.3rc0/tests/test_serving_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import time
 import featureform as ff
 from featureform.resources import Model
 import pytest
-from featureform.serving import LocalClientImpl
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -23,18 +21,14 @@
 
     fts = serving_client.features([("avg_transactions", "quickstart")], {"user": "C1410926"})
 
     models = resource_client.list_models(is_local)
 
     assert len(models) == 0
 
-    # TODO: Shouldn't have to do this
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -53,17 +47,14 @@
     ts = serving_client.training_set("fraud_training", "quickstart", model=model_name_a)
     next(ts)
 
     model = resource_client.get_model(model_name_a, is_local)
 
     assert isinstance(model, Model) and model.name == model_name_a and model.type() == "model"
 
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -89,17 +80,14 @@
     models_names = [model.name for model in models]
 
     contains_expected_names = all(expected_name in models_names for expected_name in [model_name_b, model_name_c])
     are_models_instances = all([isinstance(model, Model) for model in models])
 
     assert contains_expected_names and are_models_instances
 
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -121,17 +109,14 @@
     next(ts_2)
 
     models = resource_client.list_models(is_local)
     expected = [model.name for model in models if model.name == model_name_d]
 
     assert model_name_d in expected and len(expected) == 1 and all([isinstance(model, Model) for model in models])
 
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -149,17 +134,14 @@
 
     fts = serving_client.features([("avg_transactions", "quickstart")], {"user": "C1410926"}, model=model_name_e)
 
     model = resource_client.get_model(model_name_e, is_local)
 
     assert isinstance(model, Model) and model.name == model_name_e and model.type() == "model"
 
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -183,17 +165,14 @@
     models_names = [model.name for model in models]
 
     contains_expected_names = all(expected_name in models_names for expected_name in [model_name_f, model_name_g])
     are_models_instances = all([isinstance(model, Model) for model in models])
 
     assert contains_expected_names and are_models_instances
 
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -213,17 +192,14 @@
     fts_2 = serving_client.features([("avg_transactions", "quickstart")], {"user": "C1410926"}, model=model_name_h)
 
     models = resource_client.list_models(is_local)
     expected = [model.name for model in models if model.name == model_name_h]
 
     assert model_name_h in expected and len(expected) == 1 and all([isinstance(model, Model) for model in models])
 
-    if is_local:
-        serving_client.impl.db.close()
-
 
 @pytest.fixture(autouse=True)
 def before_and_after_each(setup_teardown):
     setup_teardown()
     yield
     setup_teardown()
 
@@ -266,15 +242,15 @@
     ff.register_training_set(
         training_set_name, training_set_variant,
         label=("fraudulent", "quickstart"),
         features=[("avg_transactions", "quickstart")],
     )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
-    resource_client.apply(asynchronous=True)
+    resource_client.apply()
 
     if not is_local:
         start = time.time()
         while True:
             time.sleep(3)
             ts = resource_client.get_training_set(training_set_name, training_set_variant)
             elapsed_wait = time.time() - start
```

### Comparing `featureform-1.7.2rc0/tests/test_spark_provider.py` & `featureform-1.7.3rc0/tests/test_spark_provider.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/tests/test_tags_and_properties.py` & `featureform-1.7.3rc0/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.2rc0/tests/test_updating_provider.py` & `featureform-1.7.3rc0/tests/test_updating_provider.py`

 * *Files identical despite different names*

