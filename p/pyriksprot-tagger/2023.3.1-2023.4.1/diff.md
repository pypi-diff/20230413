# Comparing `tmp/pyriksprot_tagger-2023.3.1.tar.gz` & `tmp/pyriksprot_tagger-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot_tagger-2023.3.1.tar", max compression
+gzip compressed data, was "pyriksprot_tagger-2023.4.1.tar", max compression
```

## Comparing `pyriksprot_tagger-2023.3.1.tar` & `pyriksprot_tagger-2023.4.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:45.701621 pyriksprot_tagger-2023.3.1/LICENSE
--rw-r--r--   0        0        0     3694 2023-03-27 14:40:27.622646 pyriksprot_tagger-2023.3.1/README.md
--rw-r--r--   0        0        0     4571 2023-03-27 14:48:01.056018 pyriksprot_tagger-2023.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/scripts/__init__.py
--rw-r--r--   0        0        0     7224 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.3.1/scripts/git-timesync
--rwxr-xr-x   0        0        0     1786 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.3.1/scripts/git_update_mtime.sh
--rw-r--r--   0        0        0      563 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.3.1/scripts/move_empty_files.sh
--rwxr-xr-x   0        0        0      251 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.3.1/scripts/setup-pipeline
--rwxr-xr-x   0        0        0     1071 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.3.1/scripts/stanza_models.sh
--rw-r--r--   0        0        0      995 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/scripts/tag.py
--rw-r--r--   0        0        0      857 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/scripts/tag_info.py
--rw-r--r--   0        0        0     4335 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/Makefile
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.3.1/workflow/README.md
--rw-r--r--   0        0        0     1807 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/Snakefile
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.3.1/workflow/__init__.py
--rw-r--r--   0        0        0     6453 2023-03-27 14:40:27.626646 pyriksprot_tagger-2023.3.1/workflow/config.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.3.1/workflow/rules/__init__.py
--rw-r--r--   0        0        0      188 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.3.1/workflow/rules/__paths__.py
--rw-r--r--   0        0        0      738 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/rules/compute_frequency.smk
--rw-r--r--   0        0        0      911 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/rules/extract_speeches.smk
--rw-r--r--   0        0        0      111 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.3.1/workflow/rules/help.smk
--rw-r--r--   0        0        0     1350 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/rules/tag_protocols.smk
--rw-r--r--   0        0        0     1784 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/rules/update_repository.smk
--rw-r--r--   0        0        0      121 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.3.1/workflow/taggers/__init__.py
--rw-r--r--   0        0        0     1740 2023-03-27 14:40:27.626646 pyriksprot_tagger-2023.3.1/workflow/taggers/registry.py
--rw-r--r--   0        0        0     1991 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.3.1/workflow/taggers/spacy2.py
--rw-r--r--   0        0        0     4235 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.3.1/workflow/taggers/stanza.py
--rw-r--r--   0        0        0     5575 2023-03-27 14:40:27.626646 pyriksprot_tagger-2023.3.1/workflow/utility.py
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 pyriksprot_tagger-2023.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:45.701621 pyriksprot_tagger-2023.4.1/LICENSE
+-rw-r--r--   0        0        0     3694 2023-03-27 14:40:27.622646 pyriksprot_tagger-2023.4.1/README.md
+-rw-r--r--   0        0        0     4593 2023-04-13 13:21:06.650320 pyriksprot_tagger-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.4.1/scripts/__init__.py
+-rw-r--r--   0        0        0     7224 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/git-timesync
+-rwxr-xr-x   0        0        0     1786 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/git_update_mtime.sh
+-rw-r--r--   0        0        0      563 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/move_empty_files.sh
+-rwxr-xr-x   0        0        0      251 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.1/scripts/setup-pipeline
+-rwxr-xr-x   0        0        0      196 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/snake-it.sh
+-rwxr-xr-x   0        0        0     1071 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/stanza-models.sh
+-rwxr-xr-x   0        0        0     4244 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/tag-it.sh
+-rw-r--r--   0        0        0      995 2023-03-28 10:59:30.619948 pyriksprot_tagger-2023.4.1/scripts/tag.py
+-rw-r--r--   0        0        0      846 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.1/scripts/tag_info.py
+-rw-r--r--   0        0        0     4328 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/Makefile
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/README.md
+-rw-r--r--   0        0        0     1714 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/__init__.py
+-rw-r--r--   0        0        0     5274 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/config.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/rules/__init__.py
+-rw-r--r--   0        0        0      188 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.1/workflow/rules/__paths__.py
+-rw-r--r--   0        0        0      735 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/compute_frequency.smk
+-rw-r--r--   0        0        0      892 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/extract_speeches.smk
+-rw-r--r--   0        0        0      111 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.1/workflow/rules/help.smk
+-rw-r--r--   0        0        0     1302 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/tag_protocols.smk
+-rw-r--r--   0        0        0     1758 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/rules/update_repository.smk
+-rw-r--r--   0        0        0      121 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.1/workflow/taggers/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.1/workflow/taggers/registry.py
+-rw-r--r--   0        0        0     1991 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.1/workflow/taggers/spacy2.py
+-rw-r--r--   0        0        0     4235 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.4.1/workflow/taggers/stanza.py
+-rw-r--r--   0        0        0     5575 2023-03-27 14:40:27.626646 pyriksprot_tagger-2023.4.1/workflow/utility.py
+-rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 pyriksprot_tagger-2023.4.1/PKG-INFO
```

### Comparing `pyriksprot_tagger-2023.3.1/LICENSE` & `pyriksprot_tagger-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/README.md` & `pyriksprot_tagger-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/pyproject.toml` & `pyriksprot_tagger-2023.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot_tagger"
-version = "2023.3.1"
+version = "2023.4.1"
 description = "Pipeline that tags pyriksprot Parla-Clarin XML files"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "workflow" },
     { include = "scripts" },
 ]
 classifiers = [
@@ -32,15 +32,16 @@
 snakemake = "*"
 loguru = "*"
 stanza = "*"
 # torch = "==1.11.0+cu113"
 
 # pip install torch==1.7.0 torchvision==0.8.1 -f https://download.pytorch.org/whl/cu101/torch_stable.html
 # beräkningsserver: pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
-pyriksprot = "0.6.1"
+poetry = "^1.4.2"
+pyriksprot = "^2023.4.1"
 
 [tool.poetry.dev-dependencies]
 black = "==20.*,>=20.8.0.b1"
 coverage = "==5.*,>=5.4.0"
 flake8 = "==3.*,>=3.8.4"
 flake8-black = "==0.*,>=0.2.1"
 isort = "==5.*,>=5.7.0"
```

### Comparing `pyriksprot_tagger-2023.3.1/scripts/git-timesync` & `pyriksprot_tagger-2023.4.1/scripts/git-timesync`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/scripts/git_update_mtime.sh` & `pyriksprot_tagger-2023.4.1/scripts/git_update_mtime.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/scripts/move_empty_files.sh` & `pyriksprot_tagger-2023.4.1/scripts/move_empty_files.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/scripts/stanza_models.sh` & `pyriksprot_tagger-2023.4.1/scripts/stanza-models.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/scripts/tag.py` & `pyriksprot_tagger-2023.4.1/scripts/tag.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/scripts/tag_info.py` & `pyriksprot_tagger-2023.4.1/scripts/tag_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Prints tag & commit info (SHA & tag) for a Git repository.
 
 """
 import click
 
-from pyriksprot.gitchen import GitUtility
+from pyriksprot.gitchen import GitInfo
 from pyriksprot.utility import write_yaml
 
 # pylint: disable=too-many-arguments, unused-argument
 
 
 @click.command()
 @click.argument('folder', type=click.STRING)
@@ -16,16 +16,16 @@
 @click.option(
     '--key',
     type=click.Choice(["tag", "ref", "sha", "sha8", "tag_url", "commit_url"], case_sensitive=False),
     help='Prints value for given key',
     default=None,
 )
 def main(folder: str = None, tag: str = None, key: str = None):
-    data: dict = GitUtility(folder).tag_info(source='workdir', tag=tag)
+    data: dict = GitInfo(folder).tag_info(source='workdir', tag=tag)
     if key:
         print(data.get(key, ""))
     else:
-        write_yaml(filename="-", data=data)
+        write_yaml(data=data,file="-")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/Makefile` & `pyriksprot_tagger-2023.4.1/workflow/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 # 	@$(POETRY) snakemake -j1 update_repository_timestamps
 
 .PHONY: annotate
 .PHONY: help-workflow clean-workflow
 .PHONY: extract-speeches-workflow
 .PHONY: dag-workflow dag-pdf-workflow
 
-annotate: unlock
+annotate:
 	@$(POETRY) snakemake -j$(PROCESSES_COUNT) --keep-going --keep-target-files --rerun-incomplete $(OPTS)
 
 extract-speeches-workflows:
 	@echo "This recipe is deprecated"
 	@echo "$(POETRY) snakemake -p -j4"
 
 workflow-dag:
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/Snakefile` & `pyriksprot_tagger-2023.4.1/workflow/Snakefile`

 * *Files 8% similar despite different names*

```diff
@@ -25,43 +25,42 @@
 
 
 setup_logging()
 
 if sys.platform not in ["win32"]:
     shell.prefix("set -o pipefail; ")
 
-config_filename: str = (config or {}).get("config_filename", "config.yml")
-typed_config: Config = Config.load(source=config_filename)
+typed_config: Config = Config.load(source=(config or {}).get("config_filename"))
 
 rule all:
     input:
         expand_target_files(
-            typed_config.corpus.source_folder,
-            typed_config.source_extension,
-            typed_config.tagged_frames_folder,
-            typed_config.target_extension,
+            typed_config.source.folder,
+            typed_config.source.extension,
+            typed_config.target.folder,
+            typed_config.target.extension,
             years=config.get("year_filter", None)
         )
 
 
 include: jj("rules", "help.smk")
 include: jj("rules", "update_repository.smk")
 include: jj("rules", "compute_frequency.smk")
 include: jj("rules", "tag_protocols.smk")
 # include: jj("rules", "extract_speeches.smk")
 
 
 onstart:
     loguru_logger.info("Workflow started")
-    os.makedirs(typed_config.tagged_frames_folder, exist_ok=True)
+    os.makedirs(typed_config.target.folder, exist_ok=True)
     os.makedirs(typed_config.data_folder, exist_ok=True)
     os.makedirs(typed_config.log_folder, exist_ok=True)
-    # os.makedirs(typed_config.extract_opts.folder, exist_ok=True)
+    # os.makedirs(typed_config.extract.folder, exist_ok=True)
 
 
 onsuccess:
-    sync_delta_names(typed_config.corpus.source_folder, "xml", typed_config.tagged_frames_folder, "xml", delete=True)
+    sync_delta_names(typed_config.source.folder, "xml", typed_config.target.folder, "xml", delete=True)
     loguru_logger.info("Workflow ended")
 
 
 onerror:
     loguru_logger.error("Workflow FAILED")
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/config.py` & `pyriksprot_tagger-2023.4.1/workflow/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,151 +19,122 @@
     def let_unknown_through(self, node):  # pylint: disable=unused-argument
         return None
 
 
 SafeLoaderIgnoreUnknown.add_constructor(None, SafeLoaderIgnoreUnknown.let_unknown_through)
 
 
-class ParlaClarinConfig:
+class SourceConfig:
 
     REPOSITORY_URL: str = "https://github.com/welfare-state-analytics/riksdagen-corpus.git"
 
-    def __init__(self, *, repository_folder: str, repository_tag: str, folder: str = None):
+    def __init__(self, *, repository_folder: str, repository_tag: str, extension: str = "xml"):
+
+        if not repository_tag:
+            raise ValueError("Corpus tag cannot be empty")
+
         self.repository_folder: str = nj(repository_folder)
         self.repository_tag: str = repository_tag
         self.repository_url: str = self.REPOSITORY_URL
-        self.source_folder: str = folder or jj(self.repository_folder, "corpus/protocols")
+        self.extension: str = extension
 
     def __repr__(self):
-        return f"{self.__class__.__name__}(repository_folder={self.repository_folder},repository_url={self.repository_url},repository_tag={self.repository_tag},folder={self.source_folder})"
+        return f"{self.__class__.__name__}(repository_folder={self.repository_folder},repository_url={self.repository_url},repository_tag={self.repository_tag},folder={self.folder},extension={self.extension})"
+
+    @property
+    def folder(self) -> str:
+        return jj(self.repository_folder, "corpus/protocols")
 
     @property
-    def parent_folder(self):
+    def parent_folder(self) -> str:
         return os.path.abspath(nj(self.repository_folder, '..'))
 
 
-class TransformedSpeechesConfig:
-    def __init__(self, folder: str, template: str = "", extension: str = "xml"):
+class TargetConfig:
+    def __init__(self, folder: str, extension: str = "xml"):
         self.folder: str = nj(folder) if folder else None
-        self.template: str = template
         self.extension: str = extension
 
     def __repr__(self):
-        return f"{self.__class__.__name__}(folder={self.folder},template={self.template},extension={self.extension})"
+        return f"{self.__class__.__name__}(folder={self.folder},extension={self.extension})"
 
 
-class WordFrequencyConfig:
-    def __init__(self, data_folder: str):
-        self.data_folder: str = nj(data_folder)
-        self.basename: str = "riksdagen-corpus-term-frequencies.pkl"
-
-    @property
-    def filename(self) -> str:
-        return jj(self.data_folder, self.basename)
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(data_folder={self.data_folder},filename={self.basename})"
+class DehyphenConfig:
+    def __init__(self, folder: str, tf_filename: str = None):
+        self.folder: str = folder
+        self.tf_filename: str = tf_filename or jj(folder, "riksdagen-corpus-term-frequencies.pkl")
 
 
-class DehyphenConfig:
-    def __init__(self, data_folder: str):
-        self.data_folder: str = nj(data_folder)
-        self.whitelist_filename: str = jj(data_folder, "dehyphen_whitelist.txt.gz")
-        self.whitelist_log_filename: str = jj(data_folder, "dehyphen_whitelist_log.pkl")
-        self.unresolved_filename: str = jj(data_folder, "dehyphen_unresolved.txt.gz")
+class ExtractConfig:
+    def __init__(self, folder: str, template: str = "", extension: str = "xml"):
+        self.folder: str = nj(folder) if folder else None
+        self.template: str = template
+        self.extension: str = extension
 
     def __repr__(self):
-        return (
-            f"{self.__class__.__name__}"
-            f"(data_folder={self.data_folder},"
-            f"whitelist_filename={self.whitelist_filename},"
-            f"whitelist_log_filename={self.whitelist_log_filename},"
-            f"unresolved_filename={self.unresolved_filename})"
-        )
-
-    @property
-    def opts(self) -> dict:
-        return dict(
-            whitelist_filename=self.whitelist_filename,
-            whitelist_log_filename=self.whitelist_log_filename,
-            unresolved_filename=self.unresolved_filename,
-        )
+        return f"{self.__class__.__name__}(folder={self.folder},template={self.template},extension={self.extension})"
 
 
 class Config:
     def __init__(
         self,
         data_folder: str,
-        target_folder: str,
-        parla_opts: ParlaClarinConfig = None,
-        source_extension: str = "xml",
-        target_extension: str = "zip",
-        extract_opts: TransformedSpeechesConfig = None,
+        source_opts: SourceConfig = None,
+        target_opts: TargetConfig = None,
+        extract_opts: ExtractConfig = None,
         dehyphen_opts: DehyphenConfig = None,
-        tf_opts: WordFrequencyConfig = None,
     ):
         self.data_folder: str = nj(data_folder)
-        self.tagged_frames_folder: str = target_folder
-        self.source_extension: str = source_extension
-        self.target_extension: str = target_extension
-
-        self.corpus: ParlaClarinConfig = parla_opts
-        self.extract_opts: TransformedSpeechesConfig = extract_opts
-        self.tf_opts: WordFrequencyConfig = tf_opts
+        self.source: SourceConfig = source_opts
+        self.target: TargetConfig = target_opts
+        self.extract: ExtractConfig = extract_opts
         self.dehyphen: DehyphenConfig = dehyphen_opts
-
         self.log_basename: str = f'parla_clarin_{time.strftime("%Y%m%d%H%M")}.log'
 
     @staticmethod
     def load(source: str) -> "Config":
         """Load YAML configuration named `config_name` in resources folder. Return typed config."""
 
+        if source is None:
+            raise ValueError("Config source cannot be None")
+
+        if source.endswith("yml") and not os.path.isfile(source):
+            raise FileNotFoundError(f"Config file {source} not found")
+
         data: dict = (
             yaml.load(Path(source).read_text(encoding="utf-8"), Loader=SafeLoaderIgnoreUnknown)
             if os.path.isfile(source)
             else yaml.load(io.StringIO(source), Loader=SafeLoaderIgnoreUnknown)
         )
 
         data_folder: str = dget(data, "data_folder", "root_folder")
-        repository_tag: str = dget(data, "repository.tag", "repository_tag") or os.environ.get(
-            "RIKSPROT_REPOSITORY_TAG"
-        )
 
-        if not repository_tag:
-            raise ValueError(
-                "Corpus tag not found. Looked in (config: repository.tag, repository_tag, environ: RIKSPROT_REPOSITORY_TAG)"
-            )
-
-        repository_folder: str = dget(data, "repository.folder", "repository_folder") or jj(
-            data_folder, "riksdagen-corpus"
-        )
-        parla_folder: str = dget(data, "repository.source_folder", "source_folder") or jj(
-            repository_folder, "corpus/protocols"
-        )
-
-        parla_opts: ParlaClarinConfig = ParlaClarinConfig(
-            repository_folder=repository_folder,
-            repository_tag=repository_tag,
-            folder=parla_folder,
-        )
-        extract_opts: TransformedSpeechesConfig = TransformedSpeechesConfig(
-            folder=dget(data, "export.folder", "export_folder"),
-            template=dget(data, "export.template", "export_template"),
-            extension=dget(data, "export.extension", "export_extension"),
-        )
-        dehyphen_opts: DehyphenConfig = DehyphenConfig(data_folder)
-        tf_opts: WordFrequencyConfig = WordFrequencyConfig(data_folder)
-        target_folder: str = dget(data, "target_folder", "target.folder")
         return Config(
             data_folder=data_folder,
-            target_folder=target_folder,
-            parla_opts=parla_opts,
-            extract_opts=extract_opts,
-            dehyphen_opts=dehyphen_opts,
-            tf_opts=tf_opts,
+            target_opts=TargetConfig(
+                folder=dget(data, "target_folder", "target.folder"),
+                extension=dget(data, "target_extension", "target.extension", default="zip"),
+            ),
+            source_opts=SourceConfig(
+                repository_folder=dget(
+                    data, "repository.folder", "repository_folder", default=jj(data_folder, "riksdagen-corpus")
+                ),
+                repository_tag=dget(
+                    data, "tag", "repository.tag", "repository_tag", default=os.environ.get("RIKSPROT_REPOSITORY_TAG")
+                ),
+            ),
+            extract_opts=ExtractConfig(
+                folder=dget(data, "export.folder", "export_folder"),
+                template=dget(data, "export.template", "export_template"),
+                extension=dget(data, "export.extension", "export_extension"),
+            ),
+            dehyphen_opts=DehyphenConfig(
+                folder=dget(data, "dehyphen_folder", "dehypen.folder", default=data_folder),
+                tf_filename=dget(data, "tf_filename", "dehyphen.tf_filename", default=None),
+            ),
         )
 
     @property
     def stanza_dir(self):
         return stanza_dir(self.data_folder)
 
     @property
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/rules/compute_frequency.smk` & `pyriksprot_tagger-2023.4.1/workflow/rules/compute_frequency.smk`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 Computes global word frequency
 """
 import glob
 from pyriksprot import compute_term_frequencies
 
 # TODO: Apply optional wildcard constraint (if any)
-WORD_FREQUENCY_SOURCE_FILES = glob.glob(jj(typed_config.corpus.source_folder, "*", "*.xml"))
+WORD_FREQUENCY_SOURCE_FILES = glob.glob(jj(typed_config.source.folder, "*", "*.xml"))
 
 rule word_frequency:
     message:
         "step: word_frequency"
     input:
         filenames=WORD_FREQUENCY_SOURCE_FILES,
     output:
-        filename=typed_config.tf_opts.filename,
+        filename=typed_config.dehyphen.tf_filename,
     run:
         compute_term_frequencies(
             source=input.filenames,
             filename=output.filename,
             segment_skip_size=10,
             multiproc_processes=config.get('processes', 1),
             multiproc_keep_order=False,
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/rules/extract_speeches.smk` & `pyriksprot_tagger-2023.4.1/workflow/rules/extract_speeches.smk`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 rule extract_speeches:
     message:
         "step: extract_speeches"
     # log:
     #     typed_config.log_filename,
     params:
-        template=typed_config.extract_opts.template,
+        template=typed_config.extract.template,
     input:
-        filename=jj(typed_config.corpus.source_folder, "{year}", "{basename}.xml"),
+        filename=jj(typed_config.source.folder, "{year}", "{basename}.xml"),
     output:
-        filename=jj(typed_config.tagged_frames_folder, "{year}", f"{{basename}}.{typed_config.target_extension}"),
+        filename=jj(typed_config.target.folder, "{year}", f"{{basename}}.{typed_config.target.extension}"),
     run:
         try:
             convert_protocol(input.filename, output.filename, params.template)
         except Exception as ex:
             print(
                 f"failed: parla_transform {input.filename} --output-filename {output.filename} --template-name {params.template}"
             )
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/rules/tag_protocols.smk` & `pyriksprot_tagger-2023.4.1/workflow/rules/tag_protocols.smk`

 * *Files 7% similar despite different names*

```diff
@@ -14,30 +14,29 @@
 from workflow.utility import check_cuda
 
 typed_config: Config = typed_config
 disable_gpu: bool = config.get("disable_gpu", 0) == 1
 
 check_cuda()
 
-ANNOTATION_FOLDER = typed_config.tagged_frames_folder
-makedirs(ANNOTATION_FOLDER, exist_ok=True)
+makedirs(typed_config.target.folder, exist_ok=True)
 
 def tagger():
     return TaggerRegistry.stanza(typed_config, disable_gpu=disable_gpu)
 
 rule tag_protocols:
     message:
         "step: tag_protocols"
     params:
-        template=typed_config.extract_opts.template,
+        template=typed_config.extract.template,
     # threads: workflow.cores * 0.75
     input:
-        filename=jj(typed_config.corpus.source_folder, "{year}", "{basename}.xml"),
+        filename=jj(typed_config.source.folder, "{year}", "{basename}.xml"),
     output:
-        filename=jj(ANNOTATION_FOLDER, "{year}", "{basename}.zip"),
+        filename=jj(typed_config.target.folder, "{year}", "{basename}.zip"),
     # message: "Tagging {input.filename}."
     run:
         try:
             tag_protocol_xml(
                 input.filename,
                 output.filename,
                 tagger(),
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/rules/update_repository.smk` & `pyriksprot_tagger-2023.4.1/workflow/rules/update_repository.smk`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # type: ignore
 # pylint: skip-file, disable-all
 import os
 
-repository_name = os.path.basename(typed_config.corpus.repository_folder)
+repository_name = os.path.basename(typed_config.source.repository_folder)
 
 
 rule init_repository:
     log:
         typed_config.log_filename,
     message:
         "step: create shallow copy of ParlaClarin repository"
     output:
-        directory(typed_config.corpus.repository_folder),
+        directory(typed_config.source.repository_folder),
     log:
         "init_repository.log",
     shell:
         f"""
            pushd . \
-        && cd {typed_config.corpus.parent_folder} \
-        && git clone --branch {typed_config.corpus.repository_tag} --depth 1 {typed_config.corpus.repository_url} \
+        && cd {typed_config.source.parent_folder} \
+        && git clone --branch {typed_config.source.repository_tag} --depth 1 {typed_config.source.repository_url} \
         && cd {repository_name} \
         && git config core.quotepath off \
         && popd
         """
 
 
 rule update_repository:
     log:
         typed_config.log_filename,
     message:
         "step: do a shallow update of ParlaClarin repository"
     shell:
         f"""\
            pushd . \
-        && cd {typed_config.corpus.repository_folder} \
+        && cd {typed_config.source.repository_folder} \
         && git fetch --depth 1 \
         && git reset --hard origin \
         && git clean -dfx \
         && git config core.quotepath off \
         && popd \
         """
 
@@ -45,20 +45,20 @@
 rule update_repository_timestamps:
     # log:
     #     typed_config.log_filename,
     message:
         "step: sets timestamp of repository files to last commit"
     shell:
         """
-        {PACKAGE_PATH}/scripts/git_update_mtime.sh {typed_config.corpus.repository_folder}
+        {PACKAGE_PATH}/scripts/git_update_mtime.sh {typed_config.source.repository_folder}
         """
 
 
 rule sync_deleted_files:
     # log:
     #     typed_config.log_filename,
     run:
-        utility.sync_delta_names(typed_config.corpus.source_folder, "xml", typed_config.tagged_frames_folder, "zip", delete=True)
+        utility.sync_delta_names(typed_config.source.folder, "xml", typed_config.target.folder, "zip", delete=True)
         # utility.sync_delta_names(
-        #     typed_config.corpus.source_folder, "xml", typed_config.extract_opts.folder, "txt", delete=True
+        #     typed_config.source.folder, "xml", typed_config.extract.folder, "txt", delete=True
         # )
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/taggers/registry.py` & `pyriksprot_tagger-2023.4.1/workflow/taggers/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,11 +45,11 @@
 
     @staticmethod
     def stanza(cfg: Config, disable_gpu: bool) -> ITagger:
         """Get tagger from registry."""
         return TaggerRegistry.get(
             tagger_cls=StanzaTagger,
             model=cfg.stanza_dir,
-            dehyphen_folder=cfg.dehyphen.data_folder,
-            word_frequencies=cfg.tf_opts.filename,
+            dehyphen_folder=cfg.dehyphen.folder,
+            word_frequencies=cfg.dehyphen.tf_filename,
             use_gpu=not disable_gpu,
         )
```

### Comparing `pyriksprot_tagger-2023.3.1/workflow/taggers/spacy2.py` & `pyriksprot_tagger-2023.4.1/workflow/taggers/spacy2.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/workflow/taggers/stanza.py` & `pyriksprot_tagger-2023.4.1/workflow/taggers/stanza.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/workflow/utility.py` & `pyriksprot_tagger-2023.4.1/workflow/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.3.1/PKG-INFO` & `pyriksprot_tagger-2023.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot-tagger
-Version: 2023.3.1
+Version: 2023.4.1
 Summary: Pipeline that tags pyriksprot Parla-Clarin XML files
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,16 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: dehyphen
 Requires-Dist: loguru
 Requires-Dist: pandas
+Requires-Dist: poetry (>=1.4.2,<2.0.0)
 Requires-Dist: pygit2
-Requires-Dist: pyriksprot (==0.6.1)
+Requires-Dist: pyriksprot (>=2023.4.1,<2024.0.0)
 Requires-Dist: snakefmt
 Requires-Dist: snakemake
 Requires-Dist: stanza
 Project-URL: Repository, https://github.com/welfare-state-analytics/pyriksprot_tagger
 Description-Content-Type: text/markdown
 
 # Riksdagens Protokoll Part-Of-Speech Tagging
```

