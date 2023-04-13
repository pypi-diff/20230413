# Comparing `tmp/typos-1.14.5.tar.gz` & `tmp/typos-1.14.6.tar.gz`

## Comparing `typos-1.14.5.tar` & `typos-1.14.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.14.5/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.14.5/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44797 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.14.5/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  5965618 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.14.5/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 typos-1.14.5/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-04-04 14:29:52.000000 typos-1.14.5/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.14.5/pyproject.toml
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 typos-1.14.5/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8514 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9783 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12553 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21534 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32485 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5359 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-04-04 14:29:52.000000 typos-1.14.5/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123    49816 2023-04-04 14:29:52.000000 typos-1.14.5/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.14.5/PKG-INFO
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44797 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  5965618 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.14.6/pyproject.toml
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 typos-1.14.6/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12565 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21534 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32485 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     5359 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123    51732 2023-04-13 16:36:44.000000 typos-1.14.6/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.14.6/PKG-INFO
```

### Comparing `typos-1.14.5/local_dependencies/dictgen/Cargo.toml` & `typos-1.14.6/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/dictgen/src/map.rs` & `typos-1.14.6/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/dictgen/src/table.rs` & `typos-1.14.6/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/dictgen/src/trie.rs` & `typos-1.14.6/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos/Cargo.toml` & `typos-1.14.6/local_dependencies/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos/src/check.rs` & `typos-1.14.6/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos/src/dict.rs` & `typos-1.14.6/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos/src/tokens.rs` & `typos-1.14.6/local_dependencies/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos-dict/Cargo.toml` & `typos-1.14.6/local_dependencies/typos-dict/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.14.6/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/varcon-core/Cargo.toml` & `typos-1.14.6/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.14.6/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/varcon-core/src/lib.rs` & `typos-1.14.6/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/varcon-core/src/parser.rs` & `typos-1.14.6/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos-vars/Cargo.toml` & `typos-1.14.6/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.14.6/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/Cargo.toml` & `typos-1.14.6/rust_src/typos-cli/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.14.5"
+version = "1.14.6"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
@@ -60,16 +60,14 @@
 clap-verbosity-flag = "2.0"
 ignore = "0.4"
 serde = { version = "1.0", features = ["derive"] }
 toml = "0.7.3"
 log = "0.4"
 env_logger = { version = "0.10", default-features = false, features = ["auto-color"] }
 atty = "0.2.14"
-concolor = { version = "0.1.1" }
-concolor-clap = { version = "0.1.0", features = ["api"] }
 bstr = "1.4"
 once_cell = "1.17.1"
 ahash = "0.8"
 difflib = "0.4"
 proc-exit = "2.0"
 human-panic = "1.1.3"
 content_inspector = "0.2.4"
@@ -81,16 +79,17 @@
 kstring = { version = "2.0.0", features = ["serde"] }
 typed-arena = "2.0.2"
 maplit = "1.0"
 unicode-width = "0.1.10"
 unic-emoji-char = "0.9.0"
 thread_local = "1.1.7"
 globset = "0.4.10"
-anstyle = "0.3.5"
-anstream = "0.2.6"
+anstyle = "1.0.0"
+anstream = "0.3.0"
+colorchoice-clap = "1.0.0"
 serde_regex = "1.1.0"
 regex = "1.7.3"
 encoding_rs = "0.8.32"
 
 [[bench]]
 name = "checks"
 harness = false
```

### Comparing `typos-1.14.5/rust_src/typos-cli/benches/checks.rs` & `typos-1.14.6/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/benches/corrections.rs` & `typos-1.14.6/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/benches/data.rs` & `typos-1.14.6/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.14.6/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,14 @@
         Format::Long
     }
 }
 
 #[derive(Debug, Parser)]
 #[command(rename_all = "kebab-case")]
 #[command(about, author, version)]
-#[command(
-        color = concolor_clap::color_choice(),
-    )]
 #[command(group = clap::ArgGroup::new("mode").multiple(false))]
 pub(crate) struct Args {
     /// Paths to check with `-` for stdin
     #[arg(default_value = ".")]
     pub(crate) path: Vec<std::path::PathBuf>,
 
     /// Custom config file
@@ -97,15 +94,15 @@
     #[arg(short = 'j', long = "threads", default_value = "0")]
     pub(crate) threads: usize,
 
     #[command(flatten)]
     pub(crate) config: ConfigArgs,
 
     #[command(flatten)]
-    pub(crate) color: concolor_clap::Color,
+    pub(crate) color: colorchoice_clap::Color,
 
     #[command(flatten)]
     pub(crate) verbose: clap_verbosity_flag::Verbosity,
 }
 
 #[derive(Debug, Clone, clap::Args)]
 #[command(rename_all = "kebab-case")]
```

### Comparing `typos-1.14.5/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         }
         Err(e) => {
             let _ = e.print();
             return proc_exit::Code::SUCCESS.ok();
         }
     };
 
-    args.color.apply();
+    args.color.write_global();
 
     init_logging(args.verbose.log_level());
 
     if let Some(output_path) = args.dump_config.as_ref() {
         run_dump_config(&args, output_path)
     } else if args.type_list {
         run_type_list(&args)
@@ -269,19 +269,19 @@
     }
 }
 
 fn init_logging(level: Option<log::Level>) {
     if let Some(level) = level {
         let mut builder = env_logger::Builder::new();
 
-        let colored = concolor::get(concolor::Stream::Stderr).ansi_color();
-        builder.write_style(if colored {
-            env_logger::WriteStyle::Always
-        } else {
+        let choice = anstream::AutoStream::choice(&std::io::stderr());
+        builder.write_style(if matches!(choice, anstream::ColorChoice::Never) {
             env_logger::WriteStyle::Never
+        } else {
+            env_logger::WriteStyle::Always
         });
 
         builder.filter(None, level.to_level_filter());
 
         if level == log::LevelFilter::Trace {
             builder.format_timestamp_secs();
         } else {
```

### Comparing `typos-1.14.5/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     info: anstyle::Style,
     strong: anstyle::Style,
 }
 
 impl Palette {
     pub fn colored() -> Self {
         Self {
-            error: anstyle::AnsiColor::Red.into(),
-            info: anstyle::AnsiColor::Blue.into(),
+            error: anstyle::AnsiColor::Red.on_default(),
+            info: anstyle::AnsiColor::Blue.on_default(),
             strong: anstyle::Effects::BOLD.into(),
         }
     }
 
     pub(crate) fn error<D: std::fmt::Display>(self, display: D) -> Styled<D> {
         Styled::new(display, self.error)
     }
```

### Comparing `typos-1.14.5/rust_src/typos-cli/src/config.rs` & `typos-1.14.6/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/default_types.rs` & `typos-1.14.6/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/dict.rs` & `typos-1.14.6/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/file.rs` & `typos-1.14.6/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/file_type.rs` & `typos-1.14.6/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/policy.rs` & `typos-1.14.6/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/rust_src/typos-cli/src/report.rs` & `typos-1.14.6/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.5/Cargo.lock` & `typos-1.14.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -42,50 +42,59 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstream"
-version = "0.2.6"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "342258dd14006105c2b75ab1bd7543a03bdf0cfc94383303ac212a04939dff6f"
+checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
 dependencies = [
  "anstyle",
  "anstyle-parse",
+ "anstyle-query",
  "anstyle-wincon",
- "concolor-override",
- "concolor-query",
+ "colorchoice",
  "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "0.3.5"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23ea9e81bd02e310c216d080f6223c179012256e5151c41db88d12c88a1684d2"
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
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "216261ddc8289130e551ddcd5ce8a064710c0d064a4d2895c67151c92b5443f6"
@@ -220,38 +229,38 @@
  "strsim 0.10.0",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.1"
+version = "4.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "046ae530c528f252094e4a77886ee1374437744b2bff1497aa898bbddbbb29b3"
+checksum = "9b802d85aaf3a1cdb02b224ba472ebdea62014fccfcb269b95a4d76443b5ee5a"
 dependencies = [
  "clap_builder",
  "clap_derive 4.2.0",
  "once_cell",
 ]
 
 [[package]]
 name = "clap-verbosity-flag"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23e2b6c3dcdb73299f48ae05b294da14e2f560b3ed2c09e742269eb1b22af231"
 dependencies = [
- "clap 4.2.1",
+ "clap 4.2.2",
  "log",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.1"
+version = "4.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "223163f58c9a40c3b0a43e1c4b50a9ce09f007ea2cb1ec258a687945b4b7929f"
+checksum = "14a1a858f532119338887a4b8e1af9c60de8249cd7bafd68036a489e261e37b6"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex 0.4.1",
  "strsim 0.10.0",
 ]
@@ -316,48 +325,27 @@
  "dictgen",
  "itertools",
  "snapbox",
  "unicase",
 ]
 
 [[package]]
-name = "concolor"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b946244a988c390a94667ae0e3958411fa40cc46ea496a929b263d883f5f9c3"
-dependencies = [
- "bitflags",
- "concolor-override",
- "concolor-query",
- "is-terminal",
-]
-
-[[package]]
-name = "concolor-clap"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435ff0007a3bb04099fe1beedc6b76e7dd5340c90b168008ac0d7e87441de1bf"
-dependencies = [
- "clap 4.2.1",
- "concolor",
-]
-
-[[package]]
-name = "concolor-override"
+name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a855d4a1978dc52fb0536a04d384c2c0c1aa273597f08b77c8c4d3b2eec6037f"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
-name = "concolor-query"
-version = "0.3.3"
+name = "colorchoice-clap"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d11d52c3d7ca2e6d0040212be9e4dbbcd78b6447f535b6b561f449427944cf"
+checksum = "412e88a3a3a3f52e436909b49beb467a05649e8b0dda0e6202bd05c1b63dbc49"
 dependencies = [
- "windows-sys 0.45.0",
+ "clap 4.2.2",
+ "colorchoice",
 ]
 
 [[package]]
 name = "content_inspector"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7bda66e858c683005a53a9a60c69a4aca7eeaa45d124526e389f7aec8e62f38"
@@ -752,17 +740,17 @@
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "human-panic"
-version = "1.1.3"
+version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a6557b29bbdc9d6c7a5cdbe2962e78eaf48115e8d55b0b62282956981c1f605"
+checksum = "c16465f6227e18e5a64eba488245d7b2974d4db0c4404ca5a69b550defa18d0a"
 dependencies = [
  "anstream",
  "anstyle",
  "backtrace",
  "os_info",
  "serde",
  "serde_derive",
@@ -1381,17 +1369,17 @@
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "snapbox"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9615402f9cff539301119bdf2c2f328739cf2b45c2116666618fb6ac399f75bb"
+checksum = "f6bccd62078347f89a914e3004d94582e13824d4e3d8a816317862884c423835"
 dependencies = [
  "anstream",
  "anstyle",
  "content_inspector",
  "dunce",
  "filetime",
  "libc",
@@ -1403,17 +1391,17 @@
  "wait-timeout",
  "walkdir",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "snapbox-macros"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8e40c667388ed1cb5060f545d0013bf0a23efdfa6c5c3e9ef592de391cd860f"
+checksum = "eaaf09df9f0eeae82be96290918520214530e738a7fe5a351b0f24cf77c0ca31"
 dependencies = [
  "anstream",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
@@ -1560,17 +1548,17 @@
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "trycmd"
-version = "0.14.15"
+version = "0.14.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32564b3f936a9ebedf5cc07dcf1e7e661204766d35f92c03bf347b099d84e783"
+checksum = "2925e71868a12b173c1eb166018c2d2f9dfaedfcaec747bdb6ea2246785d258e"
 dependencies = [
  "glob",
  "humantime",
  "humantime-serde",
  "rayon",
  "serde",
  "shlex",
@@ -1598,27 +1586,26 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.14.5"
+version = "1.14.6"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
  "bstr",
- "clap 4.2.1",
+ "clap 4.2.2",
  "clap-verbosity-flag",
- "concolor",
- "concolor-clap",
+ "colorchoice-clap",
  "content_inspector",
  "criterion",
  "derive_more",
  "derive_setters",
  "difflib",
  "encoding_rs",
  "env_logger",
@@ -1923,90 +1910,156 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
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
 ]
 
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
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
 dependencies = [
  "memchr",
 ]
```

### Comparing `typos-1.14.5/PKG-INFO` & `typos-1.14.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.14.5
+Version: 1.14.6
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

