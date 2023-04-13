# Comparing `tmp/committed-1.0.14.tar.gz` & `tmp/committed-1.0.15.tar.gz`

## Comparing `committed-1.0.14.tar` & `committed-1.0.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.14/pyproject.toml
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 committed-1.0.14/rust_src/committed/Cargo.toml
--rw-r--r--   0     1001      123     9680 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/checks.rs
--rw-r--r--   0     1001      123     1388 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/color.rs
--rw-r--r--   0     1001      123     4614 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/config.rs
--rw-r--r--   0     1001      123      461 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/conventional.rs
--rw-r--r--   0     1001      123     1914 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/git.rs
--rw-r--r--   0     1001      123      109 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/lib.rs
--rw-r--r--   0     1001      123    13085 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/main.rs
--rw-r--r--   0     1001      123     1764 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/no_style.rs
--rw-r--r--   0     1001      123     5273 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/report.rs
--rw-r--r--   0     1001      123      198 2023-03-16 15:28:51.000000 committed-1.0.14/rust_src/committed/src/style.rs
--rw-r--r--   0     1001      123    28604 2023-03-16 15:28:51.000000 committed-1.0.14/Cargo.lock
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.14/PKG-INFO
+-rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.15/pyproject.toml
+-rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 committed-1.0.15/rust_src/committed/Cargo.toml
+-rw-r--r--   0     1001      123     9680 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/checks.rs
+-rw-r--r--   0     1001      123     1414 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/color.rs
+-rw-r--r--   0     1001      123     4614 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/config.rs
+-rw-r--r--   0     1001      123      461 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/conventional.rs
+-rw-r--r--   0     1001      123     1914 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/git.rs
+-rw-r--r--   0     1001      123      109 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/lib.rs
+-rw-r--r--   0     1001      123    13085 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/main.rs
+-rw-r--r--   0     1001      123     1764 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/no_style.rs
+-rw-r--r--   0     1001      123     5273 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/report.rs
+-rw-r--r--   0     1001      123      198 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/style.rs
+-rw-r--r--   0     1001      123    30418 2023-04-13 16:04:16.000000 committed-1.0.15/Cargo.lock
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.15/PKG-INFO
```

### Comparing `committed-1.0.14/rust_src/committed/Cargo.toml` & `committed-1.0.15/rust_src/committed/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [package]
 name = "committed"
-version = "1.0.14"
+version = "1.0.15"
 description = "Nitpicking commit history since beabf39"
 documentation = "https://docs.rs/committed"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/committed"
 edition= "2021"
-rust-version= "1.64.0"  # MSRV
+rust-version= "1.65.0"  # MSRV
 include= [
+  "build.rs",
   "src/**/*",
   "Cargo.toml",
   "Cargo.lock",
   "LICENSE*",
   "README.md",
+  "benches/**/*",
   "examples/**/*"
 ]
 
 [package.metadata.release]
 tag-prefix = ""
 pre-release-replacements = [
   {file="../../CHANGELOG.md", search="Unreleased", replace="{{version}}", min=1},
@@ -35,25 +37,25 @@
 [dependencies]
 regex = "1.7"
 once_cell = "1.17.1"
 git-conventional = "0.12"
 unicase = "2.6.0"
 anyhow = "1.0"
 git2 = { version = "0.16", default-features = false }
-clap = { version = "4.1", features = ["derive"] }
+clap = { version = "4.2", features = ["derive"] }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 toml = "0.7"
 unicode-segmentation = "1.10.1"
 log = "0.4"
 env_logger = "0.10"
 clap-verbosity-flag = "2.0"
 concolor = { version = "0.1.1" }
 concolor-clap = { version = "0.1.0", features = ["api"] }
 grep-cli = "0.1"
 imperative = "1.0.4"
 derive_more = "0.99.17"
 itertools = "0.10.5"
 proc-exit = "2.0"
-human-panic = "1.1.1"
-anstream = "0.2.0"
-anstyle = "0.3.0"
+human-panic = "1.1.3"
+anstream = "0.3.0"
+anstyle = "1.0.0"
```

### Comparing `committed-1.0.14/rust_src/committed/src/checks.rs` & `committed-1.0.15/rust_src/committed/src/checks.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.14/rust_src/committed/src/color.rs` & `committed-1.0.15/rust_src/committed/src/color.rs`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     pub(crate) error: anstyle::Style,
     pub(crate) content: anstyle::Style,
 }
 
 impl Palette {
     pub(crate) fn new() -> Self {
         Self {
-            source: anstyle::AnsiColor::Blue | anstyle::Effects::BOLD,
-            error: anstyle::AnsiColor::Red | anstyle::Effects::BOLD,
+            source: anstyle::AnsiColor::Blue.on_default() | anstyle::Effects::BOLD,
+            error: anstyle::AnsiColor::Red.on_default() | anstyle::Effects::BOLD,
             content: anstyle::Style::default(),
         }
     }
 
     pub(crate) fn source<D: std::fmt::Display>(self, display: D) -> Styled<D> {
         Styled::new(display, self.source)
     }
```

### Comparing `committed-1.0.14/rust_src/committed/src/config.rs` & `committed-1.0.15/rust_src/committed/src/config.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.14/rust_src/committed/src/git.rs` & `committed-1.0.15/rust_src/committed/src/git.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.14/rust_src/committed/src/main.rs` & `committed-1.0.15/rust_src/committed/src/main.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.14/rust_src/committed/src/no_style.rs` & `committed-1.0.15/rust_src/committed/src/no_style.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.14/rust_src/committed/src/report.rs` & `committed-1.0.15/rust_src/committed/src/report.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.14/Cargo.lock` & `committed-1.0.15/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,50 +24,59 @@
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.2.3"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd0982309face56a044e935a18bbffcddeb1ce72e69a3ecc3bafb56d4e959f37"
+checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
 dependencies = [
  "anstyle",
  "anstyle-parse",
+ "anstyle-query",
  "anstyle-wincon",
- "concolor-override",
- "concolor-query 0.3.2",
+ "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "0.3.0"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d06b7594c4a4a9b15b4333938b437614e39a5d25ac542657a27e33e448bd799"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7d1bb534e9efed14f3e5f44e7dd1a4f709384023a4165199a4241e18dff0116"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "anstyle-wincon"
-version = "0.2.0"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3127af6145b149f3287bb9a0d10ad9c5692dba8c53ad48285e5bec4063834fa"
+checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
 dependencies = [
  "anstyle",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
@@ -135,69 +144,80 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.1.8"
+version = "4.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d7ae14b20b94cb02149ed21a86c423859cbe18dc7ed69845cace50e52b40a5"
+checksum = "9b802d85aaf3a1cdb02b224ba472ebdea62014fccfcb269b95a4d76443b5ee5a"
 dependencies = [
- "bitflags",
+ "clap_builder",
  "clap_derive",
- "clap_lex",
- "is-terminal",
  "once_cell",
- "strsim",
- "termcolor",
 ]
 
 [[package]]
 name = "clap-verbosity-flag"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23e2b6c3dcdb73299f48ae05b294da14e2f560b3ed2c09e742269eb1b22af231"
 dependencies = [
  "clap",
  "log",
 ]
 
 [[package]]
+name = "clap_builder"
+version = "4.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14a1a858f532119338887a4b8e1af9c60de8249cd7bafd68036a489e261e37b6"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "bitflags",
+ "clap_lex",
+ "strsim",
+]
+
+[[package]]
 name = "clap_derive"
-version = "4.1.8"
+version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44bec8e5c9d09e439c4335b1af0abaab56dcf3b94999a936e1bb47b9134288f0"
+checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
 dependencies = [
  "heck",
- "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.3.2"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "350b9cf31731f9957399229e9b2adc51eeabdfbe9d71d9a0552275fd12710d09"
-dependencies = [
- "os_str_bytes",
-]
+checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "committed"
-version = "1.0.14"
+version = "1.0.15"
 dependencies = [
  "anstream",
  "anstyle",
  "anyhow",
  "clap",
  "clap-verbosity-flag",
- "concolor 0.1.1",
+ "concolor",
  "concolor-clap",
  "derive_more",
  "env_logger",
  "git-conventional",
  "git2",
  "grep-cli",
  "human-panic",
@@ -212,64 +232,47 @@
  "toml",
  "unicase",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "concolor"
-version = "0.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7b3e3c41e9488eeda196b6806dbf487742107d61b2e16485bcca6c25ed5755b"
-dependencies = [
- "bitflags",
- "concolor-query 0.1.0",
- "is-terminal",
-]
-
-[[package]]
-name = "concolor"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b946244a988c390a94667ae0e3958411fa40cc46ea496a929b263d883f5f9c3"
 dependencies = [
  "bitflags",
  "concolor-override",
- "concolor-query 0.3.2",
+ "concolor-query",
  "is-terminal",
 ]
 
 [[package]]
 name = "concolor-clap"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435ff0007a3bb04099fe1beedc6b76e7dd5340c90b168008ac0d7e87441de1bf"
 dependencies = [
  "clap",
- "concolor 0.1.1",
+ "concolor",
 ]
 
 [[package]]
 name = "concolor-override"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a855d4a1978dc52fb0536a04d384c2c0c1aa273597f08b77c8c4d3b2eec6037f"
 
 [[package]]
 name = "concolor-query"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82a90734b3d5dcf656e7624cca6bce9c3a90ee11f900e80141a7427ccfb3d317"
-
-[[package]]
-name = "concolor-query"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b20c6ac2524cb0ddc8ceac2368f2208399dad8fa31175f14b08ae28b9d07766"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
@@ -280,15 +283,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
@@ -444,24 +447,24 @@
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "human-panic"
-version = "1.1.1"
+version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d13dc3bae03e53a5e81a3944773631df2c5a33c060e195c1f7bf3fd0d2a696"
+checksum = "c16465f6227e18e5a64eba488245d7b2974d4db0c4404ca5a69b550defa18d0a"
 dependencies = [
+ "anstream",
+ "anstyle",
  "backtrace",
- "concolor 0.0.12",
  "os_info",
  "serde",
  "serde_derive",
- "termcolor",
  "toml",
  "uuid",
 ]
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
@@ -501,27 +504,27 @@
 [[package]]
 name = "io-lifetimes"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfa919a82ea574332e2de6e74b4c36e74d41982b335080fa59d4ef31be20fdf3"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "is-terminal"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21b6b32576413a8e69b90e952e4a026476040d81017b80445deda5f2d3921857"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -633,20 +636,14 @@
 dependencies = [
  "log",
  "serde",
  "winapi",
 ]
 
 [[package]]
-name = "os_str_bytes"
-version = "6.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
-
-[[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "phf"
@@ -675,51 +672,27 @@
 [[package]]
 name = "proc-exit"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2d778539881515d37cd91925d169f4a351120c5a1b44fce2b7c462b0d7f4ec6"
 
 [[package]]
-name = "proc-macro-error"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
-dependencies = [
- "proc-macro-error-attr",
- "proc-macro2",
- "quote",
- "syn",
- "version_check",
-]
-
-[[package]]
-name = "proc-macro-error-attr"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
-dependencies = [
- "proc-macro2",
- "quote",
- "version_check",
-]
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.7.1"
@@ -775,15 +748,15 @@
 checksum = "fd5c6ff11fecd55b40746d1995a02f2eb375bf8c00d192d521ee09f42bef37bc"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
@@ -816,15 +789,15 @@
 name = "serde_derive"
 version = "1.0.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fc80d722935453bcafdc2c9a73cd6fac4dc1938f0346035d84bf99fa9e33217"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
@@ -863,14 +836,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
@@ -1037,75 +1021,141 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.1",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.1",
+ "windows_aarch64_msvc 0.42.1",
+ "windows_i686_gnu 0.42.1",
+ "windows_i686_msvc 0.42.1",
+ "windows_x86_64_gnu 0.42.1",
+ "windows_x86_64_gnullvm 0.42.1",
+ "windows_x86_64_msvc 0.42.1",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winnow"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee7b2c67f962bf5042bfd8b6a916178df33a26eec343ae064cb8e069f638fa6f"
 dependencies = [
  "memchr",
 ]
```

### Comparing `committed-1.0.14/PKG-INFO` & `committed-1.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: committed
-Version: 1.0.14
+Version: 1.0.15
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Nitpicking commit history since beabf39
 Keywords: development
@@ -41,15 +41,15 @@
 
 To use `committed` with [`pre-commit`](https://pre-commit.com), point its
 config at this repository:
 
 ```yaml
 repos:
   - repo: https://github.com/crate-ci/committed
-    rev: v1.0.14
+    rev: v1.0.15
     hooks:
       - id: committed
 ```
 
 The `committed` id installs a prebuilt executable from GitHub releases. If
 one does not exist for the target platform, or if one built from
 sources is preferred, use `committed-src` as the hook id instead.
```

