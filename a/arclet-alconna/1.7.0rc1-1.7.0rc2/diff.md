# Comparing `tmp/arclet-alconna-1.7.0rc1.tar.gz` & `tmp/arclet-alconna-1.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.0rc1.tar", last modified: Thu Mar 16 09:50:41 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.0rc2.tar", last modified: Thu Apr 13 10:49:38 2023, max compression
```

## Comparing `arclet-alconna-1.7.0rc1.tar` & `arclet-alconna-1.7.0rc2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc1/LICENSE
--rw-r--r--   0        0        0     2913 2023-03-16 09:45:07.980569 arclet-alconna-1.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5191 2023-03-14 09:21:21.005535 arclet-alconna-1.7.0rc1/README-EN.md
--rw-r--r--   0        0        0      950 2023-03-16 09:46:06.457842 arclet-alconna-1.7.0rc1/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0     3394 2023-02-22 15:46:15.231924 arclet-alconna-1.7.0rc1/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    15509 2023-03-14 09:15:36.509822 arclet-alconna-1.7.0rc1/src/arclet/alconna/analyser.py
--rw-r--r--   0        0        0    10804 2023-03-15 15:32:21.477157 arclet-alconna-1.7.0rc1/src/arclet/alconna/args.py
--rw-r--r--   0        0        0    12771 2023-02-27 09:35:42.844270 arclet-alconna-1.7.0rc1/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0     6872 2023-02-18 14:11:39.220598 arclet-alconna-1.7.0rc1/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     4383 2023-02-22 15:46:15.071359 arclet-alconna-1.7.0rc1/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     5148 2023-03-06 15:29:44.184409 arclet-alconna-1.7.0rc1/src/arclet/alconna/config.py
--rw-r--r--   0        0        0     6458 2023-03-07 04:04:26.923811 arclet-alconna-1.7.0rc1/src/arclet/alconna/container.py
--rw-r--r--   0        0        0    13651 2023-03-04 08:15:53.161084 arclet-alconna-1.7.0rc1/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     9828 2023-02-15 09:48:32.677640 arclet-alconna-1.7.0rc1/src/arclet/alconna/default.lang
--rw-r--r--   0        0        0     2501 2023-02-20 10:22:52.103947 arclet-alconna-1.7.0rc1/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-03-01 12:44:08.622779 arclet-alconna-1.7.0rc1/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0      825 2023-02-18 14:11:04.504003 arclet-alconna-1.7.0rc1/src/arclet/alconna/executor.py
--rw-r--r--   0        0        0     9728 2023-02-22 15:46:15.162360 arclet-alconna-1.7.0rc1/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0    19388 2023-03-08 06:52:19.038179 arclet-alconna-1.7.0rc1/src/arclet/alconna/handlers.py
--rw-r--r--   0        0        0     4812 2023-02-26 11:08:52.490124 arclet-alconna-1.7.0rc1/src/arclet/alconna/header.py
--rw-r--r--   0        0        0    12901 2023-03-07 14:57:52.623163 arclet-alconna-1.7.0rc1/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1311 2023-03-07 03:39:35.849142 arclet-alconna-1.7.0rc1/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1020 2023-02-15 09:48:32.678482 arclet-alconna-1.7.0rc1/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc1/src/arclet/alconna/output.py
--rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc1/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     2409 2023-02-26 05:18:00.275234 arclet-alconna-1.7.0rc1/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     6446 2023-03-14 08:57:31.959828 arclet-alconna-1.7.0rc1/src/arclet/alconna/util.py
--rw-r--r--   0        0        0     5991 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.0rc2/LICENSE
+-rw-r--r--   0        0        0     2934 2023-04-12 14:50:52.114697 arclet-alconna-1.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5110 2023-04-13 04:57:01.774375 arclet-alconna-1.7.0rc2/README-EN.md
+-rw-r--r--   0        0        0      986 2023-04-13 03:53:01.217815 arclet-alconna-1.7.0rc2/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0     3419 2023-04-09 14:04:25.832070 arclet-alconna-1.7.0rc2/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    15690 2023-04-13 03:53:01.241816 arclet-alconna-1.7.0rc2/src/arclet/alconna/analyser.py
+-rw-r--r--   0        0        0    11073 2023-04-13 03:53:01.202851 arclet-alconna-1.7.0rc2/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0    12635 2023-04-13 03:53:01.266816 arclet-alconna-1.7.0rc2/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0     6728 2023-04-13 03:53:01.232845 arclet-alconna-1.7.0rc2/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     4383 2023-02-22 15:46:15.071359 arclet-alconna-1.7.0rc2/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     3506 2023-04-13 03:56:31.540007 arclet-alconna-1.7.0rc2/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     3086 2023-04-13 04:07:03.467875 arclet-alconna-1.7.0rc2/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0     6293 2023-04-13 03:56:31.510993 arclet-alconna-1.7.0rc2/src/arclet/alconna/container.py
+-rw-r--r--   0        0        0    13398 2023-04-13 03:56:31.527968 arclet-alconna-1.7.0rc2/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     9715 2023-04-01 15:40:45.569486 arclet-alconna-1.7.0rc2/src/arclet/alconna/default.lang
+-rw-r--r--   0        0        0     2498 2023-03-31 19:18:40.743939 arclet-alconna-1.7.0rc2/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-03-31 14:01:42.790537 arclet-alconna-1.7.0rc2/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0      823 2023-04-08 10:00:51.776731 arclet-alconna-1.7.0rc2/src/arclet/alconna/executor.py
+-rw-r--r--   0        0        0     9771 2023-04-13 03:35:02.154387 arclet-alconna-1.7.0rc2/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0    19282 2023-04-13 03:59:55.614916 arclet-alconna-1.7.0rc2/src/arclet/alconna/handlers.py
+-rw-r--r--   0        0        0     5828 2023-04-12 12:26:51.391339 arclet-alconna-1.7.0rc2/src/arclet/alconna/header.py
+-rw-r--r--   0        0        0     2487 2023-04-13 10:49:13.979099 arclet-alconna-1.7.0rc2/src/arclet/alconna/lang.py
+-rw-r--r--   0        0        0    13354 2023-04-13 03:59:55.575869 arclet-alconna-1.7.0rc2/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1505 2023-04-13 03:35:02.200010 arclet-alconna-1.7.0rc2/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1144 2023-04-12 12:33:00.784350 arclet-alconna-1.7.0rc2/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     2942 2023-02-22 15:46:15.130357 arclet-alconna-1.7.0rc2/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:18:05.731268 arclet-alconna-1.7.0rc2/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     4805 2023-02-22 15:46:15.253359 arclet-alconna-1.7.0rc2/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     2397 2023-03-31 14:01:42.844114 arclet-alconna-1.7.0rc2/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0      895 2023-04-11 10:30:01.832860 arclet-alconna-1.7.0rc2/src/arclet/alconna/util.py
+-rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 arclet-alconna-1.7.0rc2/PKG-INFO
```

### Comparing `arclet-alconna-1.7.0rc1/LICENSE` & `arclet-alconna-1.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc1/pyproject.toml` & `arclet-alconna-1.7.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 name = "arclet-alconna"
 description = "A High-performance, Generality, Humane Command Line Arguments Parser Library."
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "nepattern<0.6.0, >=0.5.0",
+    "nepattern<0.6.0, >=0.5.2",
+    "tarina>=0.2.3",
 ]
 dynamic = []
 requires-python = ">=3.8"
 readme = "README-EN.md"
 keywords = [
     "command",
     "argparse",
@@ -33,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.0rc1"
+version = "1.7.0rc2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.0rc1/README-EN.md` & `arclet-alconna-1.7.0rc2/README-EN.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2Fu%2F42648639%3Fs%3D400%26u%3Da81d93f3683d0a3b7d38ea8e6a4903355986e8c7%26v%3D4&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Light)
-
+![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
 <div align="center"> 
 
 # Alconna
 
 </div>
 
 ![Alconna](https://img.shields.io/badge/Arclet-Alconna-2564c2.svg)
@@ -52,14 +51,15 @@
 ```
 
 Output as follows:
 ```
 value=None args={'pak_name': 'numpy'} options={'upgrade': value=Ellipsis args={}} subcommands={}
 ```
 
+
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
 * High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Alconna 概览"""
 
-from nepattern import AllParam as AllParam, Empty as Empty, AnyOne as AnyOne  # noqa
-from .util import split_once, split, LruCache
+from nepattern import AllParam as AllParam, AnyOne as AnyOne  # noqa
+from tarina import Empty as Empty # noqa
 from .typing import MultiVar, KeyWordVar, Kw, Nargs
 from .args import Args, Field, ArgFlag, Arg
 from .base import CommandNode, Option, Subcommand
+from .completion import CompInterface
 from .exceptions import ParamsUnmatched, NullMessage, InvalidParam
 from .analyser import Analyser
 from .container import DataCollectionContainer
 from .core import Alconna, CommandMeta
 from .arparma import Arparma, ArparmaBehavior
 from .manager import command_manager, ShortcutArgs
-from .config import config, load_lang_file, namespace, Namespace
+from .config import config, namespace, Namespace
+from .lang import load_lang_file
 
 from .builtin import store_value, set_default, store_true, store_false
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.0rc1"
+__version__ = "1.7.0rc2"
 
 Arpamar = Arparma
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/action.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
 from types import LambdaType
 from typing import Any, Callable, Dict
 from nepattern import AllParam, AnyOne
+from tarina import is_coroutinefunction
 
 from .args import Args
 from .exceptions import InvalidParam
 from .model import OptionResult, SubcommandResult
-from .util import is_async
 
 
 @dataclass(init=True, unsafe_hash=True)
 class ArgAction:
     """负责封装action的类"""
     action: Callable[..., Any]
 
@@ -26,15 +26,15 @@
             varargs: 可变参数
             kwargs: 关键字参数
             raise_exc: 是否抛出异常
         """
         _varargs = list(params.values()) + (varargs or [])
         kwargs = kwargs or {}
         try:
-            if is_async(self.action):
+            if is_coroutinefunction(self.action):
                 loop = asyncio.get_event_loop()
                 if loop.is_running():
                     loop.create_task(self.action(*_varargs, **kwargs))
                     return params
                 additional_values = loop.run_until_complete(self.action(*_varargs, **kwargs))
             else:
                 additional_values = self.action(*_varargs, **kwargs)
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/analyser.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/analyser.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 import re
 import traceback
 from re import Match
 from typing import TYPE_CHECKING, Any, Generic, Callable
 from dataclasses import dataclass, field, InitVar
 from typing_extensions import Self, TypeVar
 
-from nepattern import BasePattern
-from nepattern.util import TPattern
-
 from .manager import command_manager, ShortcutArgs
 from .exceptions import (
     ParamsUnmatched,
     ArgumentMissing,
     FuzzyMatchSuccess,
     PauseTriggered,
     SpecialOptionTriggered,
     NullMessage
 )
 from .args import Args
-from .header import handle_header, Pair, Double
+from .header import Header
 from .base import Option, Subcommand
+from .completion import comp_ctx
 from .model import Sentence, HeadResult, OptionResult, SubcommandResult
 from .arparma import Arparma
 from .typing import TDataCollection
-from .config import config, Namespace
+from .config import Namespace
+from .lang import lang
 from .output import output_manager
-from .handlers import analyse_args, analyse_param, analyse_header, handle_help, handle_shortcut, handle_completion
+from .handlers import analyse_args, analyse_param, analyse_header, handle_help, handle_shortcut, handle_completion, prompt
 from .container import DataCollectionContainer, TContainer
 
 if TYPE_CHECKING:
     from .core import Alconna
 
 
 def _compile_opts(option: Option, data: dict[str, Sentence | list[Option] | SubAnalyser]):
@@ -112,16 +111,20 @@
             self.value_result, self.args_result.copy(), self.options_result.copy(), self.subcommands_result.copy()
         )
         self.reset()
         return res
 
     def reset(self):
         """重置分析器"""
-        self.args_result, self.options_result, self.subcommands_result = {}, {}, {}
-        self.sentences, self.value_result, self.header_result = [], None, None
+        self.args_result = {}
+        self.options_result = {}
+        self.subcommands_result = {}
+        self.sentences = []
+        self.value_result = None
+        self.header_result = None
 
     def __handle_args__(self):
         if self.command.nargs > 0 and self.command.nargs > self.self_args.optional_count:
             self.need_main_args = True  # 如果need_marg那么match的元素里一定得有main_argument
         _de_count = sum(arg.field.default_gen is not None for arg in self.self_args.argument)
         if _de_count and _de_count == self.command.nargs:
             self.default_main_only = True
@@ -146,32 +149,32 @@
             return self
         return self.analyse()
 
     def analyse(self) -> Self:
         for _ in self.part_len:
             analyse_param(self, *self.container.popitem(self.command.separators, move=False))
         if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(self, self.self_args, self.command.nargs)
+            self.args_result = analyse_args(self, self.self_args)
         if not self.args_result and self.need_main_args:
-            raise ArgumentMissing(config.lang.subcommand_args_missing.format(name=self.command.dest))
+            raise ArgumentMissing(lang.subcommand.args_missing.format(name=self.command.dest))
         return self
 
-    def get_sub_analyser(self, target: Subcommand):
+    def get_sub_analyser(self, target: Subcommand) -> SubAnalyser[TContainer] | None:
         if target == self.command:
             return self
         for param in self.compile_params.values():
             if isinstance(param, SubAnalyser):
                 return param.get_sub_analyser(target)
 
 
 class Analyser(SubAnalyser[TContainer], Generic[TContainer, TDataCollection]):
     command: Alconna  # Alconna实例
     used_tokens: set[int]  # 已使用的token
     # 命令头部
-    command_header: TPattern | BasePattern | list[Pair] | Double
+    command_header: Header
     _global_container_type = DataCollectionContainer
 
     def __init__(self, alconna: Alconna, container_type: type[TContainer] | None = None):
         _type: type[TContainer] = container_type or self.__class__._global_container_type  # type: ignore
         super().__init__(
             alconna,
             _type(
@@ -180,15 +183,15 @@
                 message_cache=alconna.namespace_config.enable_message_cache,
                 filter_crlf=not alconna.meta.keep_crlf,
             ),
             alconna.namespace_config
         )
         self.fuzzy_match = alconna.meta.fuzzy_match
         self.used_tokens = set()
-        self.command_header = handle_header(alconna.command, alconna.headers)
+        self.command_header = Header.generate(alconna.command, alconna.headers)
 
     @classmethod
     def default_container(cls, __t: type[TContainer] | None = None) -> type[Analyser[TContainer, TDataCollection]]:
         """配置 Analyser 的默认容器"""
         if __t is not None:
             cls._global_container_type = __t
         return cls
@@ -203,15 +206,15 @@
 
     def __repr__(self):
         return f"<{self.__class__.__name__} of {self.command.path}>"
 
     def shortcut(self, data: list[Any], short: Arparma | ShortcutArgs, reg: Match | None) -> Arparma[TDataCollection]:
         if isinstance(short, Arparma):
             return short
-        self.container.build(short['command'])
+        self.container.build(short.get('command', self.command.command or self.command.name))
         data_index = 0
         for i, unit in enumerate(self.container.raw_data):
             if not data:
                 break
             if not isinstance(unit, str):
                 continue
             if unit == f"{{%{data_index}}}":
@@ -238,22 +241,19 @@
                 for k, v in gdict.items():
                     unit = unit.replace(f"{{{k}}}", v)
                 self.container.raw_data[j] = unit
         if self.container.message_cache:
             self.container.temp_token = self.container.generate_token(self.container.raw_data)
         return self.process()
 
-    def process(self, message: TDataCollection | None = None, interrupt: bool = False) -> Arparma[TDataCollection]:
+    def process(self, message: TDataCollection | None = None) -> Arparma[TDataCollection]:
         """主体解析函数, 应针对各种情况进行解析"""
-        if command_manager.is_disable(self.command):
-            return self.export(fail=True)
-
         if self.container.ndata == 0:
             if not message:
-                raise NullMessage(config.lang.analyser_handle_null_message.format(target=message))
+                raise NullMessage(lang.analyser.handle_null_message.format(target=message))
             try:
                 self.container.build(message)
             except Exception as e:
                 return self.export(fail=True, exception=e)
         if (
             self.container.message_cache and
             self.container.temp_token in self.used_tokens and
@@ -278,78 +278,85 @@
                 self.container.reset()
                 return self.shortcut(data, *_res)
 
         except FuzzyMatchSuccess as Fuzzy:
             output_manager.send(self.command.name, lambda: str(Fuzzy))
             return self.export(fail=True)
 
-        if fail := self.analyse(interrupt):
+        if fail := self.analyse():
             return fail
 
         if self.container.done and (not self.need_main_args or self.args_result):
             return self.export()
 
         rest = self.container.release()
         if len(rest) > 0:
             if isinstance(rest[-1], str) and rest[-1] in self.completion_names:
+                last = self.container.bak_data[-1]
+                self.container.bak_data[-1] = last[:last.rfind(rest[-1])]
                 return handle_completion(self, rest[-2])
-            exc = ParamsUnmatched(config.lang.analyser_param_unmatched.format(target=self.container.popitem(move=False)[0]))
+            exc = ParamsUnmatched(lang.analyser.param_unmatched.format(target=self.container.popitem(move=False)[0]))
         else:
-            exc = ArgumentMissing(config.lang.analyser_param_missing)
-        if interrupt and isinstance(exc, ArgumentMissing):
-            raise PauseTriggered(self)
+            exc = ArgumentMissing(lang.analyser.param_missing)
+        if isinstance(exc, ArgumentMissing) and comp_ctx.get(None):
+            raise PauseTriggered(prompt(self))
         if self.command.meta.raise_exception:
             raise exc
         return self.export(fail=True, exception=exc)
 
-    def analyse(self, interrupt: bool = False) -> Arparma[TDataCollection] | None:
+    def analyse(self) -> Arparma[TDataCollection] | None:
         for _ in self.part_len:
             try:
                 analyse_param(self, *self.container.popitem(move=False))
             except FuzzyMatchSuccess as e:
                 output_manager.send(self.command.name, lambda: str(e))
                 return self.export(fail=True)
             except SpecialOptionTriggered as sot:
                 return sot.args[0](self)
             except (ParamsUnmatched, ArgumentMissing) as e1:
                 if (rest := self.container.release()) and isinstance(rest[-1], str):
                     if rest[-1] in self.completion_names:
+                        last = self.container.bak_data[-1]
+                        self.container.bak_data[-1] = last[:last.rfind(rest[-1])]
                         return handle_completion(self)
                     if handler := self.special.get(rest[-1]):
                         return handler(self)
-                if interrupt and isinstance(e1, ArgumentMissing):
-                    raise PauseTriggered(self) from e1
+                if isinstance(e1, ArgumentMissing) and comp_ctx.get(None):
+                    raise PauseTriggered(prompt(self)) from e1
                 if self.command.meta.raise_exception:
                     raise
                 return self.export(fail=True, exception=e1)
             if self.container.done:
                 break
 
         if self.default_main_only and not self.args_result:
-            self.args_result = analyse_args(self, self.self_args, self.command.nargs)
+            self.args_result = analyse_args(self, self.self_args)
 
     def export(self, exception: BaseException | None = None, fail: bool = False) -> Arparma[TDataCollection]:
         """创建arpamar, 其一定是一次解析的最后部分"""
         result = Arparma(self.command.path, self.container.origin, not fail, self.header_result)
         if fail:
             result.error_info = repr(exception or traceback.format_exc(limit=1))
             result.error_data = self.container.release()
         else:
-            result.encapsulate_result(self.args_result, self.options_result, self.subcommands_result)
+            result.main_args = self.args_result
+            result.options = self.options_result
+            result.subcommands = self.subcommands_result
+            result.unpack()
             if self.container.message_cache:
                 command_manager.record(self.container.temp_token, result)
                 self.used_tokens.add(self.container.temp_token)
         self.reset()
         return result  # type: ignore
 
     @classmethod
     def compile(
         cls: type[TAnalyser],
-        command: Alconna[TAnalyser],
+        command: Alconna[Any],
         compiler: Callable[[TAnalyser, Namespace], None] = default_compiler
     ) -> TAnalyser:
-        _analyser = command.analyser_type(command)
+        _analyser = cls(command)
         compiler(_analyser, command.namespace_config)
         return _analyser
 
 
 TAnalyser = TypeVar("TAnalyser", bound=Analyser, default=Analyser)
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/args.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/args.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,109 +1,112 @@
 from __future__ import annotations
 
 import inspect
 import re
 from copy import deepcopy
-from dataclasses import dataclass
 from dataclasses import field as dc_field
 from enum import Enum
 from functools import partial
-from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union
-from nepattern import AllParam, AnyOne, BasePattern, Empty, UnionPattern, type_parser
+from typing import Any, Callable, Generic, Iterable, Sequence, TypeVar, Union, TYPE_CHECKING
+from tarina import Empty
+from nepattern import AllParam, AnyOne, BasePattern, UnionPattern, type_parser
 from typing_extensions import Self
+from tarina import get_signature
 
-from .config import config
+from .lang import lang
 from .exceptions import InvalidParam
 from .typing import KeyWordVar, MultiVar
-from .util import _safe_dcs_args, get_signature
+
+if TYPE_CHECKING:
+    from dataclasses import dataclass
+else:
+    from .util import dataclass
 
 _T = TypeVar("_T")
 TAValue = Union[BasePattern, AllParam.__class__, type, str]
 
 
 class ArgFlag(str, Enum):
     OPTIONAL = '?'
     HIDDEN = "/"
     ANTI = "!"
 
 
-@dataclass(**_safe_dcs_args(slots=True))
+@dataclass(slots=True)
 class Field(Generic[_T]):
     """标识参数单元字段"""
-    default: _T = dc_field(default=None)
-    default_factory: Callable[[], _T] = dc_field(default=lambda: None)
+    default: _T | None = dc_field(default=None)
+    default_factory: Callable[[], _T | None] = dc_field(default=lambda: None)
     alias: str | None = dc_field(default=None)
     completion: Callable[[], str | list[str]] | None = dc_field(default=None)
+    display: Any = dc_field(init=False)
+    default_gen: _T | None = dc_field(init=False)
 
-    @property
-    def display(self):
-        return self.alias or self.default_gen
-
-    @property
-    def default_gen(self) -> _T:
-        return self.default if self.default is not None else self.default_factory()
+    def __post_init__(self):
+        self.default_gen = self.default if self.default is not None else self.default_factory()
+        self.display = self.alias or self.default_gen
 
 
-@dataclass(**_safe_dcs_args(init=False, eq=True, unsafe_hash=True, slots=True))
+@dataclass(init=False, eq=True, unsafe_hash=True, slots=True)
 class Arg:
     name: str = dc_field(compare=True, hash=True)
-    value: TAValue = dc_field(compare=False, hash=True)
-    field: Field[_T] = dc_field(compare=False, hash=False)
+    value: Union[BasePattern, AllParam.__class__] = dc_field(compare=False, hash=True)
+    field: Field[Any] = dc_field(compare=False, hash=False)
     notice: str | None = dc_field(compare=False, hash=False)
     flag: set[ArgFlag] = dc_field(compare=False, hash=False)
     separators: tuple[str, ...] = dc_field(compare=False, hash=False)
+    optional: bool = dc_field(compare=False, hash=False)
+    hidden: bool = dc_field(compare=False, hash=False)
+    anonymous: bool = dc_field(compare=False, hash=False)
 
     def __init__(
         self,
         name: str,
         value: TAValue | None = None,
         field: Field[_T] | _T | None = None,
         seps: str | Iterable[str] = " ",
         notice: str | None = None,
         flags: list[ArgFlag] | None = None,
     ):
         if not isinstance(name, str) or name.startswith('$'):
-            raise InvalidParam(config.lang.args_name_error)
+            raise InvalidParam(lang.args.name_error)
         if not name.strip():
-            raise InvalidParam(config.lang.args_name_empty)
+            raise InvalidParam(lang.args.name_empty)
         self.name = name
         _value = type_parser(value or name)
         default = field if isinstance(field, Field) else Field(field)
         if isinstance(_value, UnionPattern) and _value.optional:
             default.default = Empty if default.default is None else default.default
         if default.default == "...":
             default.default = Empty
         if _value is Empty:
-            raise InvalidParam(config.lang.args_value_error.format(target=name))
+            raise InvalidParam(lang.args.value_error.format(target=name))
         self.value = _value
         self.field = default
         self.notice = notice
         self.separators = (seps,) if isinstance(seps, str) else tuple(seps)
         flags = flags or []
         if res := re.match(r"^.+?#(?P<notice>[^;?!/#]+)", name):
             self.notice = res["notice"]
             self.name = name.replace(f"#{res['notice']}", "")
         if res := re.match(r"^.+?;(?P<flag>[?!/]+)", self.name):
             flags.extend(ArgFlag(c) for c in res["flag"])
             self.name = self.name.replace(f";{res['flag']}", "")
         self.flag = set(flags)
+        self.optional = ArgFlag.OPTIONAL in self.flag
+        self.hidden = ArgFlag.HIDDEN in self.flag
+        self.anonymous = self.name.startswith("_key_")
+        if ArgFlag.ANTI in self.flag and self.value not in (AnyOne, AllParam):
+            self.value = deepcopy(self.value).reverse()
 
     def __repr__(self):
         return (n if (n := f"'{self.name}'") == (v := str(self.value)) else f"{n}: {v}") + (
             f" = '{self.field.display}'" if self.field.display is not None else ""
         )
 
-    @property
-    def optional(self):
-        return ArgFlag.OPTIONAL in self.flag
-
-    @property
-    def hidden(self):
-        return ArgFlag.HIDDEN in self.flag
-
 
 class ArgsMeta(type):
     """Args 类的元类"""
 
     def __getattr__(self, name):
         return type("_S", (), {"__getitem__": partial(self.__class__.__getitem__, self, key=name), "__call__": None})()
 
@@ -207,53 +210,51 @@
                 continue
             _tmp.append(arg)
             _visit.add(arg.name)
             if arg.name in self._visit:
                 continue
             self._visit.add(arg.name)
             _limit = False
-            if ArgFlag.ANTI in arg.flag and arg.value not in (AnyOne, AllParam):
-                arg.value = deepcopy(arg.value).reverse()
             if isinstance(arg.value, MultiVar) and not _limit:
                 if isinstance(arg.value.base, KeyWordVar):
                     if self.var_keyword:
-                        raise InvalidParam(config.lang.args_duplicate_kwargs)
+                        raise InvalidParam(lang.args.duplicate_kwargs)
                     self.var_keyword = arg.name
                 elif self.var_positional:
-                    raise InvalidParam(config.lang.args_duplicate_varargs)
+                    raise InvalidParam(lang.args.duplicate_varargs)
                 else:
                     self.var_positional = arg.name
                 _limit = True
             if isinstance(arg.value, KeyWordVar):
                 if self.var_keyword or self.var_positional:
-                    raise InvalidParam(config.lang.args_exclude_mutable_args)
+                    raise InvalidParam(lang.args.exclude_mutable_args)
                 self.keyword_only.append(arg.name)
                 if arg.value.sep in arg.separators:
                     _tmp.insert(-1, Arg(f"_key_{arg.name}", value=f"-*{arg.name}"))
                     _tmp[-1].value = arg.value.base
             if ArgFlag.OPTIONAL in arg.flag:
                 if self.var_keyword or self.var_positional:
-                    raise InvalidParam(config.lang.args_exclude_mutable_args)
+                    raise InvalidParam(lang.args.exclude_mutable_args)
                 self.optional_count += 1
         self.argument.clear()
         self.argument.extend(_tmp)
         del _tmp
         del _visit
 
     def __len__(self):
         return len(self.argument)
 
     def __getitem__(self, item) -> Self | Arg:
         if isinstance(item, str) and (res := next(filter(lambda x: x.name == item, self.argument), None)):
             return res
         data = item if isinstance(item, tuple) else (item,)
         if isinstance(data[0], Arg):
-            self.argument.extend(data)
+            self.argument.extend(data)  # type: ignore
         else:
-            self.argument.append(Arg(*data))
+            self.argument.append(Arg(*data))  # type: ignore
         self.__check_vars__()
         return self
 
     def __merge__(self, other) -> Self:
         if isinstance(other, Args):
             self.argument.extend(other.argument)
             self.__check_vars__()
@@ -275,14 +276,14 @@
         return self
 
     def __eq__(self, other):
         return self.argument == other.argument
 
     def __repr__(self):
         return (
-            f"Args({', '.join([f'{arg}' for arg in self.argument if not arg.name.startswith('_key_')])})"
+            f"Args({', '.join([f'{arg}' for arg in self.argument if not arg.anonymous])})"
             if self.argument else "Empty"
         )
 
     @property
     def empty(self) -> bool:
         return not self.argument
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/arparma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from contextlib import suppress
 from dataclasses import dataclass, field
 from functools import lru_cache
-from inspect import Signature
 from types import MappingProxyType
 from typing import Any, Callable, Generic, Mapping, TypeVar, overload
+from tarina import get_signature, generic_isinstance, Empty
 
-from nepattern import Empty, generic_isinstance
 from typing_extensions import Self
 
-from .config import config
+from .lang import lang
 from .exceptions import BehaveCancelled, OutBoundsBehave
 from .model import HeadResult, OptionResult, SubcommandResult
 from .typing import TDataCollection
-from .util import get_signature
 
 T = TypeVar('T')
 D = TypeVar('D')
 
 
 def _handle_opt(_pf: str, _parts: list[str], _opts: dict[str, OptionResult]):
     if _pf == "options":
@@ -43,19 +41,19 @@
     elif not (__src := _subs.get(_pf)):
         return _subs, _pf
     if (_end := _parts.pop(0)) == "value":
         return __src, _end
     if _end == 'args':
         return (__src.args, _parts.pop(0)) if _parts else (__src, _end)
     if _end == "options" and (_end in __src.options or not _parts):
-        raise RuntimeError(config.lang.arpamar_ambiguous_name.format(target=f"{_pf}.{_end}"))
+        raise RuntimeError(lang.arpamar.ambiguous_name.format(target=f"{_pf}.{_end}"))
     if _end == "options" or _end in __src.options:
         return _handle_opt(_end, _parts, __src.options)
     if _end == "subcommands" and (_end in __src.subcommands or not _parts):
-        raise RuntimeError(config.lang.arpamar_ambiguous_name.format(target=f"{_pf}.{_end}"))
+        raise RuntimeError(lang.arpamar.ambiguous_name.format(target=f"{_pf}.{_end}"))
     if _end == "subcommands" or _end in __src.subcommands:
         return _handle_sub(_end, _parts, __src.subcommands)
     return __src.args, _end
 
 
 class Arparma(Generic[TDataCollection]):
     """承载解析结果与操作数据的接口类"""
@@ -66,39 +64,42 @@
     def __init__(
         self,
         source: str,
         origin: TDataCollection,
         matched: bool = False,
         header_match: HeadResult | None = None,
         error_info: type[BaseException] | BaseException | str = '',
-        error_data: list[str | Any] | None = None
+        error_data: list[str | Any] | None = None,
+        main_args: dict[str, Any] | None = None,
+        options: dict[str, OptionResult] | None = None,
+        subcommands: dict[str, SubcommandResult] | None = None,
     ):
         self._source = source
         self.origin = origin
         self.matched = matched
         self.header_match = header_match or HeadResult()
         self.error_info = error_info
         self.error_data = error_data or []
-        self.main_args = {}
+        self.main_args = main_args or {}
         self.other_args = {}
-        self.options = {}
-        self.subcommands = {}
+        self.options = options or {}
+        self.subcommands = subcommands or {}
 
     def _clr(self):
         ks = list(self.__dict__.keys())
         for k in ks:
             delattr(self, k)
 
     @property
     def source(self):
         from .manager import command_manager
         return command_manager.get_command(self._source)
 
     @property
-    def header(self) -> dict[str, str]:
+    def header(self) -> dict[str, Any]:
         """返回可能解析到的命令头中的信息"""
         return self.header_match.groups
 
     @property
     def head_matched(self):
         return self.header_match.matched
 
@@ -132,23 +133,20 @@
         for _v in _data.values():
             self.other_args = {**self.other_args, **_v.args}
             if _v.options:
                 self._unpack_opts(_v.options)
             if _v.subcommands:
                 self._unpack_subs(_v.subcommands)
 
-    def encapsulate_result(
-        self, main_args: dict[str, Any], options: dict[str, OptionResult], subcommands: dict[str, SubcommandResult]
+    def unpack(
+        self,
     ) -> None:
         """处理 Arparma 中的数据"""
-        self.main_args = main_args.copy()
-        self.options = options.copy()
-        self.subcommands = subcommands.copy()
-        self._unpack_opts(options)
-        self._unpack_subs(subcommands)
+        self._unpack_opts(self.options)
+        self._unpack_subs(self.subcommands)
 
     @staticmethod
     def behave_cancel():
         raise BehaveCancelled
 
     @staticmethod
     def behave_fail():
@@ -187,28 +185,32 @@
                 if part in src:
                     return src, part
             if part in {"options", "subcommands", "main_args", "other_args"}:
                 return getattr(self, part, {}), ''
             return (self.all_matched_args, '') if part == "args" else (None, part)
         prefix = parts.pop(0)  # parts[0]
         if prefix in {"options", "subcommands"} and prefix in self.components:
-            raise RuntimeError(config.lang.arpamar_ambiguous_name.format(target=prefix))
+            raise RuntimeError(lang.arpamar.ambiguous_name.format(target=prefix))
         if prefix == "options" or prefix in self.options:
             return _handle_opt(prefix, parts, self.options)
         if prefix == "subcommands" or prefix in self.subcommands:
             return _handle_sub(prefix, parts, self.subcommands)
         prefix = prefix.replace("$main", "main_args").replace("$other", "other_args")
         if prefix in {"main_args", "other_args"}:
             return getattr(self, prefix, {}), parts.pop(0)
         return None, prefix
 
     @overload
-    def query(self, path: str) -> Mapping[str, Any] | Any | None: ...
+    def query(self, path: str) -> Mapping[str, Any] | Any | None:
+        ...
+
     @overload
-    def query(self, path: str, default: T) -> T | Mapping[str, Any] | Any: ...
+    def query(self, path: str, default: T) -> T | Mapping[str, Any] | Any:
+        ...
+
     def query(self, path: str, default: T | None = None) -> Any | Mapping[str, Any] | T | None:
         """根据path查询值"""
         source, endpoint = self.__require__(path.split('.'))
         if source is None:
             return default
         if isinstance(source, (OptionResult, SubcommandResult)):
             return getattr(source, endpoint, default) if endpoint else source
@@ -272,36 +274,36 @@
         if not (_record := self.record.get(interface.token, None)):
             return
         for path, (past, current) in _record.items():
             source, end = interface.__require__(path.split("."))
             if source is None:
                 continue
             if isinstance(source, dict):
-                if past != Signature.empty:
+                if past != Empty:
                     source[end] = past
-                elif source.get(end, Signature.empty) != current:
+                elif source.get(end, Empty) != current:
                     source.pop(end)
-            elif past != Signature.empty:
+            elif past != Empty:
                 setattr(source, end, past)
-            elif getattr(source, end, Signature.empty) != current:
+            elif getattr(source, end, Empty) != current:
                 delattr(source, end)
         _record.clear()
 
     @abstractmethod
     def operate(self, interface: Arparma):
         ...
 
     def update(self, interface: Arparma, path: str, value: Any):
         def _update(tkn, src, pth, ep, val):
             _record = self.record.setdefault(tkn, {})
             if isinstance(src, dict):
-                _record[pth] = (src.get(ep, Signature.empty), val)
+                _record[pth] = (src.get(ep, Empty), val)
                 src[ep] = val
             else:
-                _record[pth] = (getattr(src, ep, Signature.empty), val)
+                _record[pth] = (getattr(src, ep, Empty), val)
                 setattr(src, ep, val)
 
         source, end = interface.__require__(path.split("."))
         if source is None:
             return
         if end:
             _update(interface.token, source, path, end, value)
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/base.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Alconna 的基础内容相关"""
 from __future__ import annotations
 
-import re
 from functools import reduce
 from typing import Callable, Iterable, Sequence, overload
 from typing_extensions import Self
 
 from .action import ArgAction
 from .args import Arg, Args
-from .config import config
+from .lang import lang
 from .exceptions import InvalidParam
 
 
 class CommandNode:
     """命令体基类, 规定基础命令的参数"""
     name: str
     dest: str
@@ -36,17 +35,15 @@
             name(str): 命令节点名称
             args(Arg | Args): 命令节点参数
             action(ArgAction): 命令节点响应动作
             separators(str | Sequence[str] | Set[str]): 命令分隔符
             help_text(str): 命令帮助信息
         """
         if not name:
-            raise InvalidParam(config.lang.node_name_empty)
-        if re.match(r"^[`~?/.,<>;\':\"|!@#$%^&*()_+=\[\]}{]+.*$", name):
-            raise InvalidParam(config.lang.node_name_error)
+            raise InvalidParam(lang.node.name_empty)
         _parts = name.split(" ")
         self.name = _parts[-1]
         self.requires = ([requires] if isinstance(requires, str) else list(requires)) if requires else []
         self.requires.extend(_parts[:-1])
         self.args = Args() + args
         self.action = ArgAction.__validator__(action, self.args)
         self.separators = (' ',) if separators is None else (
@@ -80,26 +77,27 @@
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.__hash__() == other.__hash__()
 
 
 class Option(CommandNode):
     """命令选项, 可以使用别名"""
+    aliases: list[str]
     priority: int
 
     def __init__(
         self,
         name: str, args: Arg | Args | None = None, alias: Iterable[str] | None = None,
         dest: str | None = None, action: ArgAction | Callable | None = None,
         separators: str | Sequence[str] | set[str] | None = None,
         help_text: str | None = None,
         requires: str | list[str] | tuple[str, ...] | set[str] | None = None,
         priority: int = 0
     ):
-        self.aliases: list[str] = list(alias or [])
+        self.aliases = list(alias or [])
         _name = name.split(" ")[-1]
         if "|" in _name:
             _aliases = _name.split('|')
             _aliases.sort(key=len, reverse=True)
             name = name.replace(_name, _aliases[0])
             _name = _aliases[0]
             self.aliases.extend(_aliases[1:])
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/container.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Callable, TypeVar
 from typing_extensions import Self
+from tarina import split, split_once
 
 from .args import Arg
 from .base import Option, Subcommand
-from .config import config
+from .lang import lang
 from .exceptions import NullMessage
 from .typing import DataCollection
-from .util import split, split_once
 
 _cache: dict[type, dict[str, Any]] = {}
 
 
 @dataclass(repr=True)
 class DataCollectionContainer:
     preprocessors: dict[str, Callable[..., Any]] = field(default_factory=dict)
@@ -26,72 +26,73 @@
     param_ids: set[str] = field(default_factory=set)
 
     context: Arg | Subcommand | Option | None = field(init=False)
     current_index: int = field(init=False)  # 当前数据的index
     ndata: int = field(init=False)  # 原始数据的长度
     bak_data: list[str | Any] = field(init=False)
     raw_data: list[str | Any] = field(init=False)
-    temporary_data: dict[str, Any] = field(init=False)  # 临时数据
     temp_token: int = field(init=False)  # 临时token
+    origin: DataCollection[Any] = field(init=False)
+    _sep: tuple[str, ...] | None = field(init=False)
 
     @classmethod
     def config(
         cls,
         preprocessors: dict[str, Callable[..., Any]] | None = None,
-        to_text: Callable[[Any], str | None] = None,
+        to_text: Callable[[Any], str | None] | None = None,
         filter_out: list[str] | None = None
     ):
         _cache.setdefault(cls, {}).update(locals())
 
     def __post_init__(self):
         self.reset()
         if __cache := _cache.get(self.__class__, {}):
             self.preprocessors.update(__cache["preprocessors"] or {})
             self.filter_out.extend(__cache["filter_out"] or [])
             self.to_text = __cache["to_text"] or self.to_text
 
     def reset(self):
-        self.current_index, self.ndata, self.temp_token = 0, 0, 0
-        self.temporary_data = {}
-        self.raw_data, self.bak_data = [], []
+        self.current_index = 0
+        self.ndata = 0
+        self.bak_data = []
+        self.raw_data = []
+        self.temp_token = 0
+        self.origin = "None"
+        self._sep = None
         self.context = None
 
     @staticmethod
     def generate_token(data: list[Any | list[str]]) -> int:
         return hash(str(data))
 
     @property
-    def origin(self) -> DataCollection:
-        return self.temporary_data.get("origin", "None")
-
-    @property
     def done(self) -> bool:
         return self.current_index == self.ndata
 
     def build(self, data: DataCollection[str | Any]) -> Self:
-        """命令分析功能, 传入字符串或消息链, 应当在失败时返回fail的arpamar"""
+        """命令分析功能, 传入字符串或消息链"""
         self.reset()
-        self.temporary_data["origin"] = data
+        self.origin = data
         if isinstance(data, str):
             data = [data]
         i, raw_data = 0, self.raw_data
         for unit in data:
             if (uname := unit.__class__.__name__) in self.filter_out:
                 continue
             if (proc := self.preprocessors.get(uname)) and (res := proc(unit)):
                 unit = res
-            if text := self.to_text(unit):
-                if not (res := text.strip()):
-                    continue
-                raw_data.append(res)
-            else:
+            if (text := self.to_text(unit)) is None:
                 raw_data.append(unit)
+            elif not (res := text.strip()):
+                continue
+            else:
+                raw_data.append(res)
             i += 1
         if i < 1:
-            raise NullMessage(config.lang.analyser_handle_null_message.format(target=data))
+            raise NullMessage(lang.analyser_handle_null_message.format(target=data))
         self.ndata = i
         self.bak_data = raw_data.copy()
         if self.message_cache:
             self.temp_token = self.generate_token(raw_data)
         return self
 
     def rebuild(self, *data: str | Any) -> Self:
@@ -108,52 +109,52 @@
         self.bak_data = self.raw_data.copy()
         if self.message_cache:
             self.temp_token = self.generate_token(self.raw_data)
         return self
 
     def popitem(self, separate: tuple[str, ...] | None = None, move: bool = True) -> tuple[str | Any, bool]:
         """获取解析需要的下个数据"""
-        if 'sep' in self.temporary_data:
-            del self.temporary_data['sep']
+        if self._sep:
+            self._sep = None
         if self.current_index == self.ndata:
             return "", True
         separate = separate or self.separators
         _current_data = self.raw_data[self.current_index]
         if isinstance(_current_data, str):
             _text, _rest_text = split_once(_current_data, separate, self.filter_crlf)
             if move:
                 if _rest_text:
-                    self.temporary_data['sep'] = separate
+                    self._sep = separate
                     self.raw_data[self.current_index] = _rest_text
                 else:
                     self.current_index += 1
             return _text, True
         if move:
             self.current_index += 1
         return _current_data, False
 
     def pushback(self, data: str | Any, replace: bool = False):
         """把 pop的数据放回 (实际只是‘指针’移动)"""
         if data in ("", None):
             return
-        if 'sep' in self.temporary_data:
+        if self._sep:
             _current_data = self.raw_data[self.current_index]
-            self.raw_data[self.current_index] = f"{data}{self.temporary_data['sep'][0]}{_current_data}"
+            self.raw_data[self.current_index] = f"{data}{self._sep[0]}{_current_data}"
             return
         if self.current_index >= 1:
             self.current_index -= 1
         if replace:
             self.raw_data[self.current_index] = data
 
     def release(self, separate: tuple[str, ...] | None = None, recover: bool = False) -> list[str | Any]:
         _result = []
         data = self.bak_data if recover else self.raw_data[self.current_index:]
         for _data in data:
             if isinstance(_data, str):
-                _result.extend(split(_data, separate))
+                _result.extend(split(_data, separate or (' ',)))
             else:
                 _result.append(_data)
         return _result
 
     def data_set(self):
         return self.raw_data.copy(), self.current_index
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/core.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Alconna 主体"""
 from __future__ import annotations
 
 import sys
 from dataclasses import InitVar, dataclass, field
 from functools import reduce
-from typing import Any, Callable, Generic, Literal, Sequence, TypeVar, overload
+from typing import Any, Callable, Generic, Sequence, TypeVar, overload
+
+from tarina import init_spec
 from typing_extensions import Self
 
 from .action import ArgAction, exec_, exec_args
-from .analyser import Analyser, TAnalyser
+from .analyser import Analyser
 from .args import Arg, Args
 from .arparma import Arparma, ArparmaBehavior
 from .base import Option, Subcommand
 from .config import Namespace, config
+from .lang import lang
 from .duplication import Duplication
-from .exceptions import PauseTriggered
+from .exceptions import NullMessage
 from .executor import ArparmaExecutor, T
 from .formatter import TextFormatter
 from .manager import ShortcutArgs, command_manager
 from .typing import TDataCollection, THeader
-from .util import init_spec
 
 T_Duplication = TypeVar('T_Duplication', bound=Duplication)
 
 
 @dataclass
 class ActionHandler(ArparmaBehavior):
     source: InitVar[Alconna]
@@ -60,15 +62,15 @@
     author: str | None = field(default=None)
     fuzzy_match: bool = field(default=False)
     raise_exception: bool = field(default=False)
     hide: bool = field(default=False)
     keep_crlf: bool = field(default=False)
 
 
-class Alconna(Subcommand, Generic[TAnalyser]):
+class Alconna(Subcommand, Generic[TDataCollection]):
     """
     更加精确的命令解析
 
     Examples:
 
         >>> from arclet.alconna import Alconna
         >>> alc = Alconna(
@@ -82,40 +84,40 @@
         ...     ),
         ...     Args["main_args", "main_args"],
         ...  )
         >>> alc.parse("name opt opt_arg")
     """
     headers: THeader
     command: str | Any
-    analyser_type: type[TAnalyser]
+    analyser_type: type[Analyser]
     formatter: TextFormatter
     namespace: str
     meta: CommandMeta
     behaviors: list[ArparmaBehavior]
 
     global_analyser_type: type[Analyser] = Analyser
 
-    def compile(self) -> TAnalyser:
+    def compile(self) -> Analyser:
         return self.analyser_type.compile(self)
 
     @classmethod
-    def default_analyser(cls, __t: type[TAnalyser] | None = None) -> type[Alconna[TAnalyser]]:
+    def default_analyser(cls, __t: type[Analyser] | None = None):
         """配置 Alconna 的默认解析器"""
         if __t is not None:
             cls.global_analyser_type = __t
         return cls
 
     def __init__(
         self,
         *args: Option | Subcommand | str | THeader | Any | Args | Arg,
         action: ArgAction | Callable | None = None,
         meta: CommandMeta | None = None,
         namespace: str | Namespace | None = None,
         separators: str | set[str] | Sequence[str] | None = None,
-        analyser_type: type[TAnalyser] | None = None,
+        analyser_type: type[Analyser] | None = None,
         behaviors: list[ArparmaBehavior] | None = None,
         formatter_type: type[TextFormatter] | None = None
     ):
         """
         以标准形式构造 Alconna
 
         Args:
@@ -141,70 +143,70 @@
             self.command = "" if self.headers else sys.argv[0]
         self.namespace = np_config.name
         self.analyser_type = analyser_type or self.__class__.global_analyser_type  # type: ignore
         self.formatter = (formatter_type or np_config.formatter_type or TextFormatter)()
         self.meta = meta or CommandMeta()
         self.meta.fuzzy_match = self.meta.fuzzy_match or np_config.fuzzy_match
         self.meta.raise_exception = self.meta.raise_exception or np_config.raise_exception
-        super().__init__(
-            command_manager.sign,
-            reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
-            action=action,
-            separators=separators or np_config.separators,
+        options = [i for i in args if isinstance(i, (Option, Subcommand))]
+        options.append(
+            Option("|".join(np_config.builtin_option_name['help']), help_text=lang.builtin.option_help),
         )
-        self.options = [i for i in args if isinstance(i, (Option, Subcommand))]
-        self.options.append(
-            Option("|".join(np_config.builtin_option_name['help']), help_text=config.lang.builtin_option_help),
-        )
-        self.options.append(
+        options.append(
             Option(
                 "|".join(np_config.builtin_option_name['shortcut']),
                 Args["delete;?", "delete"]["name", str]["command", str, "_"],
-                help_text=config.lang.builtin_option_shortcut
+                help_text=lang.builtin.option_shortcut
             )
         )
-        self.options.append(
+        options.append(
             Option(
-                "|".join(np_config.builtin_option_name['completion']), help_text=config.lang.builtin_option_completion
+                "|".join(np_config.builtin_option_name['completion']), help_text=lang.builtin.option_completion
             )
         )
+        name = f"{self.command or self.headers[0]}".replace(command_manager.sign, "")  # type: ignore
+        self.path = f"{self.namespace}::{name}"
+        super().__init__(
+            "ALCONNA::",
+            reduce(lambda x, y: x + y, [Args()] + [i for i in args if isinstance(i, (Arg, Args))]),  # type: ignore
+            *options,
+            dest=name,
+            action=action,
+            separators=separators or np_config.separators,
+        )
+        self.name = name
         self.behaviors = behaviors or []
         self.behaviors.insert(0, ActionHandler(self))
-        self.name = f"{self.command or self.headers[0]}".replace(command_manager.sign, "")  # type: ignore
-        self._hash = self._calc_hash()
         command_manager.register(self)
         self._executors: list[ArparmaExecutor] = []
         self.union = set()
 
     @property
-    def path(self) -> str:
-        return f"{self.namespace}::{self.name.replace(command_manager.sign, '')}"
-
-    @property
     def namespace_config(self) -> Namespace:
         return config.namespaces[self.namespace]
 
     def reset_namespace(self, namespace: Namespace | str, header: bool = True) -> Self:
         """重新设置命名空间"""
         command_manager.delete(self)
         if isinstance(namespace, str):
             namespace = config.namespaces.setdefault(namespace, Namespace(namespace))
         self.namespace = namespace.name
+        self.path = f"{self.namespace}::{self.name}"
         if header:
             self.headers = namespace.headers.copy()
         self.options[-3] = Option(
-            "|".join(namespace.builtin_option_name['help']), help_text=config.lang.builtin_option_help
+            "|".join(namespace.builtin_option_name['help']), help_text=lang.builtin.option_help
         )
         self.options[-2] = Option(
             "|".join(namespace.builtin_option_name['shortcut']),
             Args["delete;?", "delete"]["name", str]["command", str, "_"],
-            help_text=config.lang.builtin_option_shortcut
+            help_text=lang.builtin.option_shortcut
         )
         self.options[-1] = Option(
-            "|".join(namespace.builtin_option_name['completion']), help_text=config.lang.builtin_option_completion
+            "|".join(namespace.builtin_option_name['completion']), help_text=lang.builtin.option_completion
         )
         self.meta.fuzzy_match = namespace.fuzzy_match or self.meta.fuzzy_match
         self.meta.raise_exception = namespace.raise_exception or self.meta.raise_exception
         self._hash = self._calc_hash()
         command_manager.register(self)
         return self
 
@@ -213,34 +215,33 @@
         self.behaviors[1:] = behaviors
         return self
 
     def get_help(self) -> str:
         """返回该命令的帮助信息"""
         return self.formatter.format_node()
 
-    def shortcut(self, key: str, args: ShortcutArgs | None = None, delete: bool = False):
+    def shortcut(self, key: str, args: ShortcutArgs[TDataCollection] | None = None, delete: bool = False):
         """添加快捷命令"""
         try:
             if delete:
                 command_manager.delete_shortcut(self, key)
-                return config.lang.shortcut_delete_success.format(shortcut=key, target=self.path)
+                return lang.shortcut.delete_success.format(shortcut=key, target=self.path)
             if args:
                 command_manager.add_shortcut(self, key, args)
-                return config.lang.shortcut_add_success.format(shortcut=key, target=self.path)
+                return lang.shortcut.add_success.format(shortcut=key, target=self.path)
             elif cmd := command_manager.recent_message:
                 alc = command_manager.last_using
                 if alc and alc == self:
                     command_manager.add_shortcut(self, key, {"command": cmd})
-                    return config.lang.shortcut_add_success.format(shortcut=key, target=self.path)
+                    return lang.shortcut.add_success.format(shortcut=key, target=self.path)
                 raise ValueError(
-                    config.lang.shortcut_recent_command_error.format(
-                        target=self.path, source=getattr(alc, "path", "Unknown"))
+                    lang.shortcut.recent_command_error.format(target=self.path, source=getattr(alc, "path", "Unknown"))
                 )
             else:
-                raise ValueError(config.lang.shortcut_no_recent_command)
+                raise ValueError(lang.shortcut.no_recent_command)
         except Exception as e:
             if self.meta.raise_exception:
                 raise e
             return str(e)
 
     def __repr__(self):
         return f"{self.namespace}::{self.name}(args={self.args}, options={self.options})"
@@ -257,37 +258,42 @@
     def option(self, opt: Option) -> Self:
         return self.add(opt)
 
     @init_spec(Subcommand, True)
     def subcommand(self, sub: Subcommand) -> Self:
         return self.add(sub)
 
-    def _parse(self, message: TDataCollection, interrupt: bool = False) -> Arparma[TDataCollection]:
+    def _parse(self, message: TDataCollection) -> Arparma[TDataCollection]:
         if self.union:
             for ana in command_manager.requires(*self.union):
                 ana.container.build(message)
-                if (res := ana.process(interrupt=interrupt)).matched:
+                if (res := ana.process()).matched:
                     return res
         analyser = command_manager.require(self)
         analyser.container.build(message)
-        return analyser.process(interrupt=interrupt)
-    @overload
-    def parse(self, message: TDataCollection) -> Arparma[TDataCollection]: ...
+        return analyser.process()
+
     @overload
-    def parse(self, message, *, duplication: type[T_Duplication]) -> T_Duplication: ...
+    def parse(self, message: TDataCollection) -> Arparma[TDataCollection]:
+        ...
+
     @overload
-    def parse(self, message: TDataCollection, *, interrupt: Literal[True]) -> Arparma[TDataCollection] | TAnalyser: ...
+    def parse(self, message, *, duplication: type[T_Duplication]) -> T_Duplication:
+        ...
+
     def parse(
-        self, message: TDataCollection, *, duplication: type[T_Duplication] | None = None, interrupt: bool = False
-    ) -> TAnalyser | Arparma[TDataCollection] | T_Duplication:
+        self, message: TDataCollection, *, duplication: type[T_Duplication] | None = None
+    ) -> Arparma[TDataCollection] | T_Duplication:
         """命令分析功能, 传入字符串或消息链, 返回一个特定的数据集合类"""
         try:
-            arp = self._parse(message, interrupt)
-        except PauseTriggered as e:
-            return e.args[0]
+            arp = self._parse(message)
+        except NullMessage as e:
+            if self.meta.raise_exception:
+                raise e
+            return Arparma(self.path, message, False, error_info=e)
         if arp.matched:
             self.behaviors[0].operate(arp)
             arp = arp.execute()
         return duplication(arp) if duplication else arp
 
     def bind(self, target: Callable[..., T]) -> ArparmaExecutor[T]:
         ext = ArparmaExecutor(target)
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/default.lang` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/default.lang`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920634920634921%*

 * *Differences: {"'en-US'": "{'common.completion_node': 'suggest input follows:', delete: "*

 * *            "['common.completion_arg']}",*

 * * "'zh-CN'": "{'common.completion_node': '以下是建议的输入：', delete: ['common.completion_arg']}"}*

```diff
@@ -27,16 +27,15 @@
         "builtin.option_shortcut": "set a shortcut command",
         "cli.command_matched": "Your command is successfully matched!\nThe results:\n - Header: {header}\n - Command: {main_args}\n - Options: {options}\n - Arguments: {all_args}",
         "cli.command_not_found": "Please create a command first",
         "cli.command_not_matched": "Your command matched failed.\nError Data: {data}\nError Info: {exception}",
         "cli.lang_type_set_failed": "The default language type set failed.",
         "cli.lang_type_set_success": "The default language type is set to {type}",
         "cli.not_found": "Cannot found the target component of Alconna",
-        "common.completion_arg": "suggest next arg:",
-        "common.completion_node": "next input maybe:",
+        "common.completion_node": "suggest input follows:",
         "common.custom_type_error": "The custom parameter type {target} can't be a type.",
         "common.fuzzy_matched": "{target} is not matched. Do you mean \"{source}\"?",
         "construct.decorate_error": "This action must behind a @xxx.command()",
         "construct.function_name_error": "function name can not start with '_'",
         "duplication.stub_type_error": "{value} is not a valid stub",
         "header.error": "{target} dose not matched",
         "lang.name_error": "{target} is not a valid Alconna Lang Config name",
@@ -92,16 +91,15 @@
         "builtin.option_shortcut": "\u8bbe\u7f6e\u5feb\u6377\u547d\u4ee4",
         "cli.command_matched": "\u4f60\u7684\u547d\u4ee4\u89e3\u6790\u6210\u529f\u4e86\uff01\n\u89e3\u6790\u7ed3\u679c\u662f\n - \u547d\u4ee4\u5934\u90e8: {header}\n - \u547d\u4ee4\u53c2\u6570: {main_args}\n - \u547d\u4ee4\u9009\u9879: {options}\n - \u6240\u6709\u53c2\u6570: {all_args}",
         "cli.command_not_found": "\u8bf7\u5148\u521b\u5efa\u547d\u4ee4",
         "cli.command_not_matched": "\u4f60\u7684\u547d\u4ee4\u89e3\u6790\u5931\u8d25\u4e86\n\u9519\u8bef\u6570\u636e\u662f: {data}\n\u9519\u8bef\u4fe1\u606f\u662f: {exception}",
         "cli.lang_type_set_failed": "\u8bed\u8a00\u914d\u7f6e\u7c7b\u578b\u66f4\u6539\u5931\u8d25",
         "cli.lang_type_set_success": "\u8bed\u8a00\u914d\u7f6e\u7c7b\u578b\u66f4\u6539\u6210\u529f, \u5df2\u7ecf\u66f4\u6539\u4e3a {type}",
         "cli.not_found": "\u6ca1\u6709\u627e\u5230\u6307\u5b9a\u7684\u7ec4\u4ef6",
-        "common.completion_arg": "\u4e0b\u4e00\u4e2a\u53c2\u6570\u5e94\u5f53\u4e3a\uff1a",
-        "common.completion_node": "\u4e0b\u4e00\u4e2a\u8f93\u5165\u53ef\u80fd\u662f\u4ee5\u4e0b\uff1a",
+        "common.completion_node": "\u4ee5\u4e0b\u662f\u5efa\u8bae\u7684\u8f93\u5165\uff1a",
         "common.custom_type_error": "\u81ea\u5b9a\u4e49\u53c2\u6570\u7c7b\u578b\u4f20\u5165\u7684\u4e0d\u662f\u7c7b\u578b\u800c\u662f {target}, \u8fd9\u662f\u6709\u610f\u800c\u4e3a\u4e4b\u7684\u5417?",
         "common.fuzzy_matched": "\u65e0\u6cd5\u89e3\u6790 {target}\u3002\u60a8\u60f3\u8981\u8f93\u5165\u7684\u662f\u4e0d\u662f \"{source}\" ?",
         "construct.decorate_error": "\u8be5\u884c\u4e3a\u5fc5\u987b\u5728 @xxx.command() \u4e4b\u540e",
         "construct.function_name_error": "\u51fd\u6570\u540d\u4e0d\u80fd\u4ee5 '_' \u5f00\u5934",
         "duplication.stub_type_error": "{value} \u4e0d\u662f\u4e00\u4e2a\u5408\u6cd5\u7684 Stub \u5b50\u7c7b",
         "header.error": "\u547d\u4ee4\u5934\u90e8 {target} \u5339\u914d\u5931\u8d25",
         "lang.name_error": "{target} \u4e0d\u662f\u5408\u6cd5\u7684 Alconna \u8bed\u8a00\u914d\u7f6e\u540d\u79f0",
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/duplication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from inspect import isclass
 from typing import cast
-from nepattern import Empty
+from tarina import Empty
 
 from .arparma import Arparma
 from .stub import ArgsStub, BaseStub, OptionStub, SubcommandStub
 
 
 class Duplication:
     """用以更方便的检查、调用解析结果的类。"""
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/executor.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,13 @@
     binding: Callable[..., list[Arparma]] = field(default=lambda: [], repr=False)
 
     @property
     def result(self) -> T:
         if not self.binding:
             raise ExecuteFailed(None)
         arps = self.binding()
-        if not arps or not arps[-1].matched:
+        if not arps or not arps[0].matched:
             raise ExecuteFailed("Unmatched")
         try:
-            return arps[-1].call(self.target)
+            return arps[0].call(self.target)
         except Exception as e:
             raise ExecuteFailed(e) from e
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any
-from nepattern import AllParam, BasePattern, Empty
+from tarina import Empty
+from nepattern import AllParam, BasePattern
 
 from .args import Arg, Args
 from .base import Option, Subcommand
 
 if TYPE_CHECKING:
     from .core import Alconna
 
@@ -80,15 +81,15 @@
 
     def add(self, base: Alconna):
         self.ignore_names.update(base.namespace_config.builtin_option_name['help'])
         self.ignore_names.update(base.namespace_config.builtin_option_name['shortcut'])
         self.ignore_names.update(base.namespace_config.builtin_option_name['completion'])
         hds = base.headers.copy()
         if base.name in hds:
-            hds.remove(base.name)
+            hds.remove(base.name)  # type: ignore
         res = Trace(
             {
                 'name': base.name, 'header': hds or [], 'description': base.meta.description,
                 'usage': base.meta.usage, 'example': base.meta.example
             },
             base.args, base.separators, base.options.copy()
         )
@@ -139,15 +140,15 @@
             if isinstance(_cache, Subcommand):
                 return self.format(Trace(
                     {"name": _cache.name, "header": [], "description": _cache.help_text}, _cache.args,
                     _cache.separators, _cache.options  # type: ignore
                 ))
             return self.format(trace)
 
-        return "\n".join(map(_handle, self.data.values()))
+        return "\n".join([_handle(v) for v in self.data.values()])
 
     def format(self, trace: Trace) -> str:
         """help text的生成入口"""
         header = self.header(trace.head, trace.separators)
         param = self.parameters(trace.args)
         body = self.body(trace.body)
         return header % (param, body)
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/handlers.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Any, Iterable
-
-from nepattern import AllParam, BasePattern, Empty
+from tarina import Empty, split_once
+from nepattern import AllParam, BasePattern
 from nepattern.util import TPattern
 
 from .args import Arg, Args
 from .header import Double
 from .base import Option, Subcommand
 from .config import config
-from .exceptions import ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, SpecialOptionTriggered
+from .lang import lang
+from .completion import Prompt, comp_ctx
+from .exceptions import ArgumentMissing, FuzzyMatchSuccess, ParamsUnmatched, SpecialOptionTriggered, PauseTriggered
 from .model import OptionResult, Sentence, HeadResult
 from .output import output_manager
 from .typing import KeyWordVar, MultiVar
-from .util import levenshtein_norm, split_once
+from .util import levenshtein_norm
 
 if TYPE_CHECKING:
     from .analyser import SubAnalyser, DataCollectionContainer, Analyser
 
 
 def _handle_keyword(
-    analyser: SubAnalyser,
+    container: DataCollectionContainer,
     value: KeyWordVar,
     may_arg: Any,
     seps: tuple[str, ...],
     result_dict: dict[str, Any],
     default_val: Any,
     optional: bool,
     key: str | None = None,
+    fuzzy: bool = False,
 ):
     if _kwarg := re.match(fr'^([^{value.sep}]+){value.sep}(.*?)$', may_arg):
         key = key or _kwarg[1]
         if (_key := _kwarg[1]) != key:
-            analyser.container.pushback(may_arg)
-            if analyser.fuzzy_match and levenshtein_norm(_key, key) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(config.lang.common_fuzzy_matched.format(source=_key, target=key))
+            container.pushback(may_arg)
+            if fuzzy and levenshtein_norm(_key, key) >= config.fuzzy_threshold:
+                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_key, target=key))
             if default_val is None:
-                raise ParamsUnmatched(config.lang.common_fuzzy_matched.format(source=_key, target=key))
+                raise ParamsUnmatched(lang.common.fuzzy_matched.format(source=_key, target=key))
             result_dict[_key] = None if default_val is Empty else default_val
             return
         if not (_m_arg := _kwarg[2]):
-            may_arg, _str = analyser.container.popitem(seps)
-        res = value.base(_kwarg[2], default_val)
+            _m_arg, _ = container.popitem(seps)
+        res = value.base(_m_arg, default_val)
         if res.flag != 'valid':
-            analyser.container.pushback(may_arg)
+            container.pushback(may_arg)
         if res.flag == 'error':
             if optional:
                 return
             raise ParamsUnmatched(*res.error.args)
         result_dict[_kwarg[1]] = res._value  # type: ignore
         return
-    analyser.container.pushback(may_arg)
-    raise ParamsUnmatched(config.lang.args_key_missing.format(target=may_arg, key=key))
+    container.pushback(may_arg)
+    raise ParamsUnmatched(lang.args.key_missing.format(target=may_arg, key=key))
 
 
 def _loop_kw(
-    analyser: SubAnalyser,
+    container: DataCollectionContainer,
     _loop: int,
-    rest_arg: int,
     seps: tuple[str, ...],
     value: MultiVar,
     default: Any
 ):
     result = {}
     for _ in range(_loop):
-        _m_arg, _m_str = analyser.container.popitem(seps)
+        _m_arg, _m_str = container.popitem(seps)
         if not _m_arg:
             continue
-        if _m_str and _m_arg in analyser.container.param_ids:
-            analyser.container.pushback(_m_arg)
-            for _ in range(min(len(result), rest_arg - 1)):
-                arg = result.popitem()  # type: ignore
-                analyser.container.pushback(f'{arg[0]}={arg[1]}')
+        if _m_str and _m_arg in container.param_ids:
+            container.pushback(_m_arg)
             break
         try:
-            _handle_keyword(analyser, value.base, _m_arg, seps, result, default, False)  # type: ignore
+            _handle_keyword(container, value.base, _m_arg, seps, result, default, False)  # type: ignore
         except ParamsUnmatched:
             break
     if not result:
         if value.flag == '+':
             raise ParamsUnmatched
         result = [default] if default else []
     return result
 
 
 def _loop(
     container: DataCollectionContainer,
     _loop: int,
-    rest_arg: int,
     seps: tuple[str, ...],
     value: MultiVar,
-    default: Any
+    default: Any,
+    args: Args
 ):
+    kw = args[args.var_keyword].value.base if args.var_keyword else None
     result = []
     for _ in range(_loop):
         _m_arg, _m_str = container.popitem(seps)
         if not _m_arg:
             continue
-        if _m_str and (_m_arg in container.param_ids or re.match(fr'^(.+)=\s?$', _m_arg)):
+        if _m_str and (
+            _m_arg in container.param_ids or
+            (kw and re.match(fr'^([^{kw.sep}]+){kw.sep}(.*?)$', _m_arg))
+        ):
             container.pushback(_m_arg)
-            for _ in range(min(len(result), rest_arg - 1)):
-                container.pushback(result.pop(-1))
             break
         if (res := value.base(_m_arg)).flag != 'valid':
             container.pushback(_m_arg)
             break
         result.append(res._value)  # type: ignore
     if not result:
         if value.flag == '+':
@@ -115,134 +116,139 @@
 
 
 def multi_arg_handler(
     analyser: SubAnalyser,
     args: Args,
     arg: Arg,
     result_dict: dict[str, Any],
-    nargs: int
 ):
     seps = arg.separators
     value = arg.value
     key = arg.name
     default = arg.field.default_gen
     kw = value.base.__class__ == KeyWordVar
-    _m_rest_arg = nargs - len(result_dict)
+    _m_rest_arg = len(args) - len(result_dict)
     _m_rest_all_param_count = len(analyser.container.release(seps))
     if not kw and not args.var_keyword or kw and not args.var_positional:
-        loop = _m_rest_all_param_count - (_m_rest_arg - (value.flag == "+"))
+        loop = _m_rest_all_param_count - _m_rest_arg + 1
     elif not kw:
-        loop = _m_rest_all_param_count - (_m_rest_arg - (args[args.var_keyword].value.flag == "*"))
+        loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_keyword].value.flag == "*"))
     else:
-        loop = _m_rest_all_param_count - (_m_rest_arg - (args[args.var_positional].value.flag == "*"))
+        loop = _m_rest_all_param_count - (_m_rest_arg - 2*(args[args.var_positional].value.flag == "*"))
     if value.length > 0:
         loop = min(loop, value.length)
     result_dict[key] = (
-        _loop_kw(analyser, loop, _m_rest_arg, seps, value, default) if kw
-        else _loop(analyser.container, loop, _m_rest_arg, seps, value, default)
+        _loop_kw(analyser.container, loop, seps, value, default) if kw
+        else _loop(analyser.container, loop, seps, value, default, args)
     )
 
 
-def analyse_args(analyser: SubAnalyser, args: Args, nargs: int) -> dict[str, Any]:
+def analyse_args(analyser: SubAnalyser, args: Args) -> dict[str, Any]:
     """
     分析 Args 部分
 
     Args:
         analyser: 使用的分析器
         args: 目标Args
-        nargs: 目标Args的参数个数
 
     Returns:
         Dict: 解析结果
     """
     result: dict[str, Any] = {}
     for arg in args.argument:
         analyser.container.context = arg
-        key, value, default_val, optional = arg.name, arg.value, arg.field.default_gen, arg.optional
+        key = arg.name
+        value = arg.value
+        default_val = arg.field.default_gen
+        optional = arg.optional
         seps = arg.separators
         may_arg, _str = analyser.container.popitem(seps)
-        if _str and (handler := analyser.special.get(may_arg)):
-            raise SpecialOptionTriggered(handler)
-        if not may_arg or (_str and may_arg in analyser.container.param_ids):
+        if _str and may_arg in analyser.special:
+            raise SpecialOptionTriggered(analyser.special[may_arg])
+        if (
+            (not may_arg or (_str and may_arg in analyser.container.param_ids))
+            and (value.__class__ != MultiVar or value.__class__ is MultiVar and value.flag == '+')
+        ):
             analyser.container.pushback(may_arg)
             if default_val is not None:
                 result[key] = None if default_val is Empty else default_val
             elif not optional:
-                raise ArgumentMissing(config.lang.args_missing.format(key=key))
+                raise ArgumentMissing(lang.args.missing.format(key=key))
             continue
         if value.__class__ is MultiVar:
             analyser.container.pushback(may_arg)
-            multi_arg_handler(analyser, args, arg, result, nargs)  # type: ignore
+            multi_arg_handler(analyser, args, arg, result)  # type: ignore
         elif value.__class__ is KeyWordVar:
-            _handle_keyword(analyser, value, may_arg, seps, result, default_val, optional, key)  # type: ignore
-        elif isinstance(value, BasePattern):
-            res = value(may_arg, default_val)
+            _handle_keyword(
+                analyser.container, value, may_arg, seps, result, default_val, optional, key, analyser.fuzzy_match  # type: ignore
+            )
+        elif value is AllParam:
+            analyser.container.pushback(may_arg)
+            result[key] = analyser.container.release(seps)
+            analyser.container.current_index = analyser.container.ndata
+            return result
+        else:
+            res = (
+                value.invalidate(may_arg, default_val)
+                if value.anti
+                else value.validate(may_arg, default_val)
+            )
             if res.flag != 'valid':
                 analyser.container.pushback(may_arg)
             if res.flag == 'error':
                 if optional:
                     continue
                 raise ParamsUnmatched(*res.error.args)
-            if not key.startswith('_key'):
+            if not arg.anonymous:
                 result[key] = res._value  # type: ignore
-        elif value is AllParam:
-            analyser.container.pushback(may_arg)
-            result[key] = analyser.container.release(seps)
-            analyser.container.current_index = analyser.container.ndata
-            return result
-        elif may_arg == value:
-            result[key] = may_arg
-        elif default_val is not None:
-            result[key] = None if default_val is Empty else default_val
-        elif not optional:
-            raise ParamsUnmatched(config.lang.args_error.format(target=may_arg))
     if args.var_keyword:
         kwargs = result[args.var_keyword]
         if not isinstance(kwargs, dict):
             kwargs = {args.var_keyword: kwargs}
         result['$kwargs'] = (kwargs, args.var_keyword)
     if args.var_positional:
         varargs = result[args.var_positional]
         if not isinstance(varargs, Iterable):
             varargs = [varargs]
         elif not isinstance(varargs, list):
             varargs = list(varargs)
         result['$varargs'] = (varargs, args.var_positional)
     if args.keyword_only:
         result['$kwonly'] = {k: v for k, v in result.items() if k in args.keyword_only}
+    analyser.container.context = None
     return result
 
 
 def analyse_unmatch_params(analyser: SubAnalyser, text: str):
     for _p in analyser.compile_params.values():
         if isinstance(_p, list):
             res = []
             for _o in _p:
                 _may_param, _ = split_once(text, _o.separators)
                 if _may_param in _o.aliases or any(map(_may_param.startswith, _o.aliases)):
                     analyser.compile_params.setdefault(text, res)
                     res.append(_o)
                     continue
                 if analyser.fuzzy_match and levenshtein_norm(_may_param, _o.name) >= config.fuzzy_threshold:
-                    raise FuzzyMatchSuccess(config.lang.common_fuzzy_matched.format(source=_may_param, target=_o.name))
+                    raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_o.name))
             if res:
                 return res
         elif isinstance(_p, Sentence):
             if (_may_param := split_once(text, _p.separators)[0]) == _p.name:
                 analyser.compile_params.setdefault(text, _p)
                 return _p
             if analyser.fuzzy_match and levenshtein_norm(_may_param, _p.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(config.lang.common_fuzzy_matched.format(source=_may_param, target=_p.name))
+                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_p.name))
         else:
             _may_param, _ = split_once(text, _p.command.separators)
             if _may_param == _p.command.name or _may_param.startswith(_p.command.name):
                 analyser.compile_params.setdefault(text, _p)
                 return _p
             if analyser.fuzzy_match and levenshtein_norm(_may_param, _p.command.name) >= config.fuzzy_threshold:
-                raise FuzzyMatchSuccess(config.lang.common_fuzzy_matched.format(source=_may_param, target=_p.command.name))
+                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(source=_may_param, target=_p.command.name))
 
 
 def analyse_option(analyser: SubAnalyser, param: Option) -> tuple[str, OptionResult]:
     """
     分析 Option 部分
 
     Args:
@@ -264,26 +270,33 @@
     else:
         name, _ = analyser.container.popitem(param.separators)
         if name not in param.aliases:  # 先匹配选项名称
             raise ParamsUnmatched(f"{name} dose not matched with {param.name}")
     name = param.dest
     if param.nargs == 0:
         return name, OptionResult()
-    return name, OptionResult(None, analyse_args(analyser, param.args, param.nargs))
+    return name, OptionResult(None, analyse_args(analyser, param.args))
 
 
 def analyse_param(analyser: SubAnalyser, _text: Any, _str: bool):
-    if handler := analyser.special.get(_text if _str else Ellipsis):
-        raise SpecialOptionTriggered(handler)
+    if _str and _text in analyser.special:
+        if _text in analyser.completion_names:
+            if analyser.container.current_index < analyser.container.ndata:
+                analyser.container.bak_data = analyser.container.bak_data[:analyser.container.current_index+1]
+            last = analyser.container.bak_data[-1]
+            analyser.container.bak_data[-1] = last[:last.rfind(_text)]
+        raise SpecialOptionTriggered(analyser.special[_text])
     if not _str or not _text:
-        _param = Ellipsis
-    elif not (_param := analyser.compile_params.get(_text)):
+        _param = None
+    elif _text in analyser.compile_params:
+        _param = analyser.compile_params[_text]
+    else:
         _param = None if analyser.container.default_separate else analyse_unmatch_params(analyser, _text)
-    if (not _param or _param is Ellipsis) and not analyser.args_result:
-        analyser.args_result = analyse_args(analyser, analyser.self_args, analyser.command.nargs)
+    if not _param and not analyser.args_result:
+        analyser.args_result = analyse_args(analyser, analyser.self_args)
     elif isinstance(_param, list):
         for opt in _param:
             _data, _index = analyser.container.data_set()
             try:
                 opt_n, opt_v = analyse_option(analyser, opt)
                 analyser.options_result[opt_n] = opt_v
                 _data.clear()
@@ -292,165 +305,160 @@
                 exc = e
                 analyser.container.data_reset(_data, _index)
                 continue
         else:
             raise exc  # type: ignore  # noqa
     elif isinstance(_param, Sentence):
         analyser.sentences.append(analyser.container.popitem()[0])
-    elif _param not in (None, Ellipsis):
+    elif _param:
         _param.process()
         analyser.subcommands_result.setdefault(_param.command.dest, _param.export())
+    analyser.container.context = None
 
 
 def analyse_header(analyser: Analyser) -> HeadResult:
-    command = analyser.command_header
+    header = analyser.command_header
+    content = header.content
+    mapping = header.mapping
     head_text, _str = analyser.container.popitem()
-    if isinstance(command, TPattern) and _str and (mat := command.fullmatch(head_text)):
-        return HeadResult(head_text, head_text, True, mat.groupdict())
-    elif isinstance(command, BasePattern) and (val := command(head_text, Empty)).success:
-        return HeadResult(head_text, val.value, True)
+    if isinstance(content, TPattern) and _str and (mat := content.fullmatch(head_text)):
+        return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
+    elif isinstance(content, BasePattern) and (val := content(head_text, Empty)).success:
+        return HeadResult(head_text, val.value, True, fixes=mapping)
 
     may_command, _m_str = analyser.container.popitem()
-    if isinstance(command, list) and _m_str:
-        for pair in command:
+    if isinstance(content, list) and _m_str:
+        for pair in content:
             if res := pair.match(head_text, may_command):
-                return HeadResult(*res)
-    if isinstance(command, Double) and (
-        res := command.match(head_text, may_command, _str, _m_str, analyser.container.pushback)
+                return HeadResult(*res, fixes=mapping)
+    if isinstance(content, Double) and (
+        res := content.match(head_text, may_command, _str, _m_str, analyser.container.pushback)
     ):
-        return HeadResult(*res)
+        return HeadResult(*res, fixes=mapping)
 
     if _str and analyser.fuzzy_match:
         headers_text = []
         if analyser.command.headers and analyser.command.headers != [""]:
             headers_text.extend(f"{i}{analyser.command.command}" for i in analyser.command.headers)
         elif analyser.command.command:
             headers_text.append(str(analyser.command.command))
-        if isinstance(command, (TPattern, BasePattern)):
+        if isinstance(content, (TPattern, BasePattern)):
             source = head_text
         else:
             source = head_text + analyser.container.separators[0] + str(may_command)
         if source == analyser.command.command:
             analyser.header_result = HeadResult(source, source, False)
-            raise ParamsUnmatched(config.lang.header_error.format(target=head_text))
+            raise ParamsUnmatched(lang.header.error.format(target=head_text))
         for ht in headers_text:
             if levenshtein_norm(source, ht) >= config.fuzzy_threshold:
                 analyser.header_result = HeadResult(source, ht, True)
-                raise FuzzyMatchSuccess(config.lang.common_fuzzy_matched.format(target=source, source=ht))
-    raise ParamsUnmatched(config.lang.header_error.format(target=head_text))
+                raise FuzzyMatchSuccess(lang.common.fuzzy_matched.format(target=source, source=ht))
+    raise ParamsUnmatched(lang.header.error.format(target=head_text))
 
 
 def handle_help(analyser: Analyser):
     _help_param = [str(i) for i in analyser.container.release(recover=True) if str(i) not in analyser.special]
     output_manager.send(
         analyser.command.name,
         lambda: analyser.command.formatter.format_node(_help_param),
     )
     return analyser.export(fail=True)
 
 
 def handle_shortcut(analyser: Analyser):
     analyser.container.popitem()
-    opt_v = analyse_args(analyser, Args["delete;?", "delete"]["name", str]["command", str, "_"], 3)
+    opt_v = analyse_args(analyser, Args["delete;?", "delete"]["name", str]["command", str, "_"])
     try:
         msg = analyser.command.shortcut(
             opt_v["name"],
             None if opt_v["command"] == "_" else {"command": analyser.converter(opt_v["command"])},
             bool(opt_v.get("delete"))
         )
         output_manager.send(analyser.command.name, lambda: msg)
     except Exception as e:
         output_manager.send(analyser.command.name, lambda: str(e))
     return analyser.export(fail=True)
 
 
-def _handle_unit(analyser: Analyser, trigger: Arg):
-    if gen := trigger.field.completion:
-        comp = gen()
+def _prompt_unit(analyser: Analyser, trigger: Arg):
+    if trigger.field.completion:
+        comp = trigger.field.completion()
         if isinstance(comp, str):
-            return output_manager.send(analyser.command.name, lambda: comp)
-        target = str(analyser.container.release(recover=True)[-2])
-        o = "\n- ".join(list(filter(lambda x: target in x, comp)) or comp)
-        return output_manager.send(
-            analyser.command.name, lambda: f"{config.lang.common_completion_arg}\n- {o}"
-        )
+            return [Prompt(comp, False)]
+        releases = analyser.container.release(recover=True)
+        target = str(releases[-1]) or str(releases[-2])
+        o = list(filter(lambda x: target in x, comp)) or comp
+        return [Prompt(i, False, target) for i in o]
     default = trigger.field.default_gen
     o = f"[{trigger.name}]{trigger.value}{'' if default is None else f' default:({None if default is Empty else default})'}"
-    return output_manager.send(
-        analyser.command.name, lambda: f"{config.lang.common_completion_arg}\n{o}"
-    )
+    return [Prompt(o, False)]
 
 
-def _handle_sentence(analyser: Analyser):
+def _prompt_sentence(analyser: Analyser):
     res: list[str] = []
     s_len = len(stc := analyser.sentences)
     for opt in filter(
         lambda x: len(x.requires) >= s_len and x.requires[s_len - 1] == stc[-1],
         analyser.command.options,
     ):
         if len(opt.requires) > s_len:
             res.append(opt.requires[s_len])
         else:
             res.extend(opt.aliases if isinstance(opt, Option) else [opt.name])
-    return res
+    return [Prompt(i) for i in res]
 
 
-def _handle_none(analyser: Analyser, got: list[str]):
-    res: list[str] = []
+def _prompt_none(analyser: Analyser, got: list[str]):
+    res: list[Prompt] = []
     if not analyser.args_result and analyser.self_args.argument:
         unit = analyser.self_args.argument[0]
         if gen := unit.field.completion:
-            res.append(comp if isinstance(comp := gen(), str) else "\n- ".join(comp))
+            res.extend([Prompt(comp, False)] if isinstance(comp := gen(), str) else [Prompt(i, False) for i in comp])
         else:
             default = unit.field.default_gen
             res.append(
-                f"[{unit.name}]{unit.value}{'' if default is None else f' ({None if default is Empty else default})'}"
+                Prompt(
+                    f"[{unit.name}]{unit.value}{'' if default is None else f' ({None if default is Empty else default})'}",
+                    False
+                )
             )
     for opt in filter(
         lambda x: x.name not in analyser.completion_names,
         analyser.command.options,
     ):
         if opt.requires and all(opt.requires[0] not in i for i in got):
-            res.append(opt.requires[0])
+            res.append(Prompt(opt.requires[0]))
         elif opt.dest not in got:
-            res.extend(opt.aliases if isinstance(opt, Option) else [opt.name])
+            res.extend([Prompt(al) for al in opt.aliases] if isinstance(opt, Option) else [Prompt(opt.name)])
     return res
 
 
-def handle_completion(analyser: Analyser, trigger: str | None = None):
+def prompt(analyser: Analyser, trigger: str | None = None):
     trigger = trigger or analyser.container.context
     got = [*analyser.options_result.keys(), *analyser.subcommands_result.keys(), *analyser.sentences]
     if isinstance(trigger, Arg):
-        _handle_unit(analyser, trigger)
+        return _prompt_unit(analyser, trigger)
     elif isinstance(trigger, Subcommand):
-        output_manager.send(
-            analyser.command.name,
-            lambda: f"{config.lang.common_completion_node}\n- " +
-                    "\n- ".join(analyser.get_sub_analyser(trigger).compile_params),
-        )
+        return [Prompt(i) for i in analyser.get_sub_analyser(trigger).compile_params]
     elif isinstance(trigger, str):
         res = list(filter(lambda x: trigger in x, analyser.compile_params))
         if not res:
-            return analyser.export(
-                fail=True,
-                exception=ParamsUnmatched(config.lang.analyser_param_unmatched.format(target=trigger)),
-            )
+            return []
         out = [i for i in res if i not in got]
+        return [Prompt(i, True, trigger) for i in (out or res)]
+    releases = analyser.container.release(recover=True)
+    target = str(releases[-1]) or str(releases[-2])
+    if _res := list(filter(lambda x: target in x and target != x, analyser.compile_params)):
+        out = [i for i in _res if i not in got]
+        return [Prompt(i, True, target) for i in (out or _res)]
+    return _prompt_sentence(analyser) if analyser.sentences else _prompt_none(analyser, got)
+
+
+def handle_completion(analyser: Analyser, trigger: str | None = None):
+    if res := prompt(analyser, trigger):
+        if comp_ctx.get(None):
+            raise PauseTriggered(res)
         output_manager.send(
             analyser.command.name,
-            lambda: f"{config.lang.common_completion_node}\n- " + "\n- ".join(out or res),
+            lambda: f"{lang.common.completion_node}\n* " + "\n* ".join([i.text for i in res]),
         )
-    else:
-        target = str(analyser.container.release(recover=True)[-1])
-        if _res := list(filter(lambda x: target in x and target != x, analyser.compile_params)):
-            out = [i for i in _res if i not in got]
-            output_manager.send(
-                analyser.command.name,
-                lambda: f"{config.lang.common_completion_node}\n- " + "\n- ".join(out or _res),
-            )
-        else:
-            res = _handle_sentence(analyser) if analyser.sentences else _handle_none(analyser, got)
-            output_manager.send(
-                analyser.command.name,
-                lambda: f"{config.lang.common_completion_node}\n- " + "\n- ".join(set(res)),
-            )
     return analyser.export(fail=True, exception='NoneType: None\n')  # type: ignore
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/header.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/header.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from __future__ import annotations
 
-from inspect import isclass
-from nepattern.util import TPattern
-from nepattern import all_patterns, type_parser, BasePattern, Empty, UnionPattern
 import re
-from typing import Any, Callable
-from dataclasses import dataclass, field
 from copy import deepcopy
+from dataclasses import dataclass, field
+from inspect import isclass
+from typing import Any, Callable
+
+from nepattern import BasePattern, UnionPattern, all_patterns, type_parser
+from nepattern.util import TPattern
+from tarina import Empty
 
 
 def handle_bracket(name: str):
     pattern_map = all_patterns()
+    mapping = {}
     if len(parts := re.split(r"(\{.*?})", name)) <= 1:
-        return name
+        return name, mapping
     for i, part in enumerate(parts):
         if not part:
             continue
-        if part.startswith('{') and part.endswith('}'):
-            res = part[1:-1].split(':')
+        if part.startswith("{") and part.endswith("}"):
+            res = part[1:-1].split(":")
             if not res or (len(res) > 1 and not res[1] and not res[0]):
                 parts[i] = ".+?"
             elif len(res) == 1 or not res[1]:
                 parts[i] = f"(?P<{res[0]}>.+?)"
             elif not res[0]:
-                parts[i] = f"{pattern_map[res[1]].pattern if res[1] in pattern_map else res[1]}"
+                parts[
+                    i
+                ] = f"{pattern_map[res[1]].pattern if res[1] in pattern_map else res[1]}"
+            elif res[1] in pattern_map:
+                mapping[res[0]] = pattern_map[res[1]]
+                parts[i] = f"(?P<{res[0]}>{pattern_map[res[1]].pattern})"
             else:
-                parts[i] = f"(?P<{res[0]}>{pattern_map[res[1]].pattern if res[1] in pattern_map else res[1]})"
-    return "".join(parts)
+                parts[i] = f"(?P<{res[0]}>{res[1]})"
+    return "".join(parts), mapping
 
 
 @dataclass
 class Pair:
     prefix: Any
     pattern: TPattern
     is_prefix_pat: bool = field(default=False, init=False)
@@ -38,79 +46,118 @@
     def __post_init__(self):
         self.is_prefix_pat = isinstance(self.prefix, BasePattern)
 
     def match(self, prefix: Any, command: str):
         if mat := self.pattern.fullmatch(command):
             if self.is_prefix_pat and (val := self.prefix(prefix, Empty)).success:
                 return (prefix, command), (val.value, command), True, mat.groupdict()
-            if not isclass(prefix) and prefix == self.prefix or type(prefix) == self.prefix:
+            if (
+                not isclass(prefix)
+                and prefix == self.prefix
+                or type(prefix) == self.prefix
+            ):
                 return (prefix, command), (prefix, command), True, mat.groupdict()
 
 
 @dataclass
 class Double:
     elements: list[Any]
     patterns: UnionPattern | None
     prefix: TPattern | None
     command: BasePattern | TPattern
 
-    def match(self, prefix: Any, command: Any, prefix_str: bool, command_str: bool, pushback_fn: Callable[[str], ...]):
+    def match(
+        self,
+        prefix: Any,
+        command: Any,
+        prefix_str: bool,
+        command_str: bool,
+        pushback_fn: Callable[[str], ...],
+    ):
         if self.prefix and prefix_str:
             if command_str:
                 pat = re.compile(self.prefix.pattern + self.command.pattern)
                 if mat := pat.fullmatch(prefix):
                     pushback_fn(command)
                     return prefix, prefix, True, mat.groupdict()
                 elif mat := pat.fullmatch(name := (prefix + command)):
                     return name, name, True, mat.groupdict()
-            if (mat := self.prefix.fullmatch(prefix)) and (_val := self.command(command, Empty)).success:
+            if (mat := self.prefix.fullmatch(prefix)) and (
+                _val := self.command(command, Empty)
+            ).success:
                 return (prefix, command), (prefix, _val.value), True, mat.groupdict()
         if self.patterns and (val := self.patterns.validate(prefix, Empty)).success:
             _po, _pr = prefix, val.value
-        elif self.elements and not isclass(prefix) and (prefix in self.elements or type(prefix) in self.elements):
+        elif (
+            self.elements
+            and not isclass(prefix)
+            and (prefix in self.elements or type(prefix) in self.elements)
+        ):
             _po, _pr = prefix, prefix
         else:
             return
-        if isinstance(self.command, TPattern) and command_str and (mat := self.command.fullmatch(command)):
+        if (
+            isinstance(self.command, TPattern)
+            and command_str
+            and (mat := self.command.fullmatch(command))
+        ):
             return (_po, command), (_pr, command), True, mat.groupdict()
-        elif isinstance(self.command, BasePattern) and (_val := self.command(command, Empty)).success:
+        elif (
+            isinstance(self.command, BasePattern)
+            and (_val := self.command(command, Empty)).success
+        ):
             return (_po, command), (_pr, _val.value), True
 
 
-def handle_header(
-    command: str | type | BasePattern,
-    headers: list[Any] | list[tuple[Any, str]]
-) -> TPattern | BasePattern | list[Pair] | Double:
-    if isinstance(command, str):
-        command = handle_bracket(command)
-    _cmd_name: TPattern | BasePattern
-    _cmd_str: str
-    _cmd_name, _cmd_str = (
-        (re.compile(command), command) if isinstance(command, str) else
-        (deepcopy(type_parser(command)), str(command))
-    )
-    if not headers:
-        return _cmd_name
-    if isinstance(headers[0], tuple):
-        return [Pair(h[0], re.compile(re.escape(h[1]) + _cmd_str)) for h in headers]
-    elements = []
-    patterns = []
-    ch_text = ""
-    for h in headers:
-        if isinstance(h, str):
-            ch_text += f"{re.escape(h)}|"
-        elif isinstance(h, BasePattern):
-            patterns.append(h)
-        else:
-            elements.append(h)
-    if not elements and not patterns:
-        if isinstance(_cmd_name, TPattern):
-            return re.compile(f"(?:{ch_text[:-1]}){_cmd_str}")
-        _cmd_name.pattern = f"(?:{ch_text[:-1]}){_cmd_name.pattern}"  # type: ignore
-        _cmd_name.regex_pattern = re.compile(_cmd_name.pattern)  # type: ignore
-        return _cmd_name
-    return Double(
-        elements,
-        UnionPattern(patterns) if patterns else None,
-        re.compile(f"(?:{ch_text[:-1]})") if ch_text else None,
-        _cmd_name
-    )
+@dataclass
+class Header:
+    content: TPattern | BasePattern | list[Pair] | Double
+    mapping: dict[str, BasePattern] = field(default_factory=dict)
+
+    @classmethod
+    def generate(
+        cls,
+        command: str | type | BasePattern,
+        headers: list[Any] | list[tuple[Any, str]],
+    ):
+        mapping = {}
+        if isinstance(command, str):
+            command, mapping = handle_bracket(command)
+        _cmd_name: TPattern | BasePattern
+        _cmd_str: str
+        _cmd_name, _cmd_str = (
+            (re.compile(command), command)
+            if isinstance(command, str)
+            else (deepcopy(type_parser(command)), str(command))
+        )
+        if not headers:
+            return cls(_cmd_name, mapping)
+        if isinstance(headers[0], tuple):
+            return cls(
+                [Pair(h[0], re.compile(re.escape(h[1]) + _cmd_str)) for h in headers],
+                mapping,
+            )
+        elements = []
+        patterns = []
+        ch_text = ""
+        for h in headers:
+            if isinstance(h, str):
+                ch_text += f"{re.escape(h)}|"
+            elif isinstance(h, BasePattern):
+                patterns.append(h)
+            else:
+                elements.append(h)
+        if not elements and not patterns:
+            if isinstance(_cmd_name, TPattern):
+                return cls(re.compile(f"(?:{ch_text[:-1]}){_cmd_str}"), mapping)
+            _cmd_name.pattern = f"(?:{ch_text[:-1]}){_cmd_name.pattern}"  # type: ignore
+            _cmd_name.regex_pattern = re.compile(_cmd_name.pattern)  # type: ignore
+            return cls(_cmd_name)
+        return cls(
+            Double(
+                elements,
+                UnionPattern(patterns) if patterns else None,
+                re.compile(f"(?:{ch_text[:-1]})") if ch_text else None,
+                _cmd_name,
+            ),
+            mapping,
+        )
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 """Alconna 负责记录命令的部分"""
+
 from __future__ import annotations
 
 import contextlib
 import re
 import shelve
 import weakref
 from copy import copy
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload
+from typing import TYPE_CHECKING, Any, Match, TypedDict, Union, overload, Generic
 from typing_extensions import NotRequired
+from tarina import LRU
+from weakref import WeakKeyDictionary, WeakValueDictionary
 
 from .arparma import Arparma
 from .config import Namespace, config
+from .lang import lang
 from .exceptions import ExceedMaxCount
 from .typing import DataCollection, TDataCollection
-from .util import LruCache
+
 
 if TYPE_CHECKING:
-    from .analyser import Analyser, TAnalyser
+    from .analyser import Analyser
     from .core import Alconna, CommandMeta
 
 
-class ShortcutArgs(TypedDict):
-    command: NotRequired[DataCollection[Any]]
-    args: NotRequired[list[Any]]
+    class ShortcutArgs(TypedDict, Generic[TDataCollection]):
+        command: NotRequired[TDataCollection]
+        args: NotRequired[list[Any]]
+else:
+    class ShortcutArgs(TypedDict):
+        command: NotRequired[DataCollection[Any]]
+        args: NotRequired[list[Any]]
 
 
 class CommandManager:
     """
     Alconna 命令管理器
 
     命令管理器负责记录命令, 并存储快捷指令。
     """
 
     sign: str
     current_count: int
     max_count: int
 
-    __commands: dict[str, dict[str, Alconna]]
-    __analysers: dict[Alconna, Analyser]
+    __commands: dict[str, WeakValueDictionary[str, Alconna]]
+    __analysers: WeakKeyDictionary[Alconna, Analyser]
     __abandons: list[Alconna]
-    __record: LruCache[int, Arparma]
+    __record: LRU[int, Arparma]
     __shortcuts: dict[str, Union[Arparma, ShortcutArgs]]
 
     def __init__(self):
         self.cache_path = f"{__file__.replace('manager.py', '')}manager_cache.db"
         self.sign = "ALCONNA::"
         self.max_count = config.command_max_count
         self.current_count = 0
 
         self.__commands = {}
-        self.__analysers = {}
+        self.__analysers = WeakKeyDictionary()
         self.__abandons = []
         self.__shortcuts = {}
-        self.__record = LruCache(config.message_max_cache)
+        self.__record = LRU(config.message_max_cache)
 
         def _del():
             self.__commands.clear()
             for ana in self.__analysers.values():
                 ana._clr()
             self.__analysers.clear()
             self.__abandons.clear()
@@ -99,32 +107,32 @@
 
     def register(self, command: Alconna) -> None:
         """注册命令解析器, 会同时记录解析器对应的命令"""
         if self.current_count >= self.max_count:
             raise ExceedMaxCount
         self.__analysers.pop(command, None)
         self.__analysers[command] = command.compile()
-        namespace = self.__commands.setdefault(command.namespace, {})
+        namespace = self.__commands.setdefault(command.namespace, WeakValueDictionary())
         if _cmd := namespace.get(command.name):
             if _cmd == command:
                 return
             _cmd.formatter.add(command)
             command.formatter = _cmd.formatter
         else:
             command.formatter.add(command)
             namespace[command.name] = command
             self.current_count += 1
 
-    def require(self, command: Alconna[TAnalyser]) -> TAnalyser:
+    def require(self, command: Alconna) -> Analyser:
         """获取命令解析器"""
         try:
             return self.__analysers[command]  # type: ignore
         except KeyError as e:
             namespace, name = self._command_part(command.path)
-            raise ValueError(config.lang.manager_undefined_command.format(target=f"{namespace}.{name}")) from e
+            raise ValueError(lang.manager.undefined_command.format(target=f"{namespace}.{name}")) from e
 
     def requires(self, *paths: str) -> list[Analyser]:
         return [v for k, v in self.__analysers.items() if k.path in paths]
 
     def delete(self, command: Alconna | str) -> None:
         """删除命令"""
         namespace, name = self._command_part(command if isinstance(command, str) else command.path)
@@ -156,36 +164,40 @@
         namespace, name = self._command_part(target.path)
         if isinstance(source, dict):
             source['command'] = source.get('command', target.command or target.name)
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         elif source.matched:
             self.__shortcuts[f"{namespace}.{name}::{key}"] = source
         else:
-            raise ValueError(config.lang.manager_incorrect_shortcut.format(target=f"{key}"))
+            raise ValueError(lang.manager.incorrect_shortcut.format(target=f"{key}"))
 
     @overload
-    def find_shortcut(self, target: Alconna) -> list[Union[Arparma, ShortcutArgs]]:
+    def find_shortcut(
+        self, target: Alconna[TDataCollection]
+    ) -> list[Union[Arparma[TDataCollection], ShortcutArgs[TDataCollection]]]:
         ...
 
     @overload
-    def find_shortcut(self, target: Alconna, query: str) -> tuple[Arparma | ShortcutArgs, Match | None]:
+    def find_shortcut(
+        self, target: Alconna[TDataCollection], query: str
+    ) -> tuple[Arparma[TDataCollection] | ShortcutArgs[TDataCollection], Match[str] | None]:
         ...
 
-    def find_shortcut(self, target: Alconna, query: str | None = None):
+    def find_shortcut(self, target: Alconna[TDataCollection], query: str | None = None):
         """查找快捷命令"""
         namespace, name = self._command_part(target.path)
         if query:
             try:
                 return self.__shortcuts[f"{namespace}.{name}::{query}"], None
             except KeyError as e:
                 for k in self.__shortcuts.keys():
                     if mat := re.match(k.split("::")[1], query):
                         return self.__shortcuts[k], mat
                 raise ValueError(
-                    config.lang.manager_target_command_error.format(target=f"{namespace}.{name}", shortcut=query)
+                    lang.manager.target_command_error.format(target=f"{namespace}.{name}", shortcut=query)
                 ) from e
         return [self.__shortcuts[k] for k in self.__shortcuts.keys() if f"{namespace}.{name}" in k]
 
     def delete_shortcut(self, target: Alconna, key: str | None = None):
         """删除快捷命令"""
         for res in [self.find_shortcut(target, key)[0]] if key else self.find_shortcut(target):
             with contextlib.suppress(StopIteration):
@@ -232,17 +244,17 @@
             namespace: 指定的命名空间, 如果为None则选择所有命令
             header: 帮助信息的页眉
             pages: 帮助信息的页码
             footer: 帮助信息的页脚
             max_length: 单个页面展示的最大长度
             page: 当前页码
         """
-        pages = pages or config.lang.manager_help_pages
+        pages = pages or lang.manager.help_pages
         cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
-        header = header or config.lang.manager_help_header
+        header = header or lang.manager.help_header
         if max_length < 1:
             command_string = "\n".join(
                 f" {str(index).rjust(len(str(len(cmds))), '0')} {slot.name} : {slot.meta.description}"
                 for index, slot in enumerate(cmds)
             ) if show_index else "\n".join(
                 f" - {cmd.name} : {cmd.meta.description}"
                 for cmd in cmds
@@ -260,68 +272,67 @@
             ) if show_index else "\n".join(
                 f" - {cmd.name} : {cmd.meta.description}"
                 for cmd in cmds[(page - 1) * max_length: page * max_length]
             )
         help_names = set()
         for i in cmds:
             help_names.update(i.namespace_config.builtin_option_name['help'])
-        footer = footer or config.lang.manager_help_footer.format(help="|".join(help_names))
+        footer = footer or lang.manager.help_footer.format(help="|".join(help_names))
         return f"{header}\n{command_string}\n{footer}"
 
     def all_command_raw_help(self, namespace: str | Namespace | None = None) -> dict[str, CommandMeta]:
         """获取所有命令的原始帮助信息"""
         cmds = list(filter(lambda x: not x.meta.hide, self.get_commands(namespace or '')))
         return {cmd.path: copy(cmd.meta) for cmd in cmds}
 
     def command_help(self, command: str) -> str | None:
         """获取单个命令的帮助"""
         if cmd := self.get_command(command):
             return cmd.get_help()
 
     def record(self, token: int, result: Arparma):
-        self.__record.set(token, result)
+        self.__record[token] = result
 
     def get_record(self, token: int) -> Arparma | None:
-        if not token:
-            return
-        return self.__record.get(token)
+        if token in self.__record:
+            return self.__record[token]
 
     def get_token(self, result: Arparma) -> int:
         return next((token for token, res in self.__record.items() if res == result), 0)
 
     def get_result(self, command: Alconna) -> list[Arparma]:
         return [v for v in self.__record.values() if v.source == command]
 
     @property
     def recent_message(self) -> DataCollection[str | Any] | None:
-        if rct := self.__record.recent:
-            return rct.origin
+        if rct := self.__record.peek_first_item():
+            return rct[1].origin  # type: ignore
 
     @property
     def last_using(self):
-        if rct := self.__record.recent:
-            return rct.source
+        if rct := self.__record.peek_first_item():
+            return rct[1].source  # type: ignore
 
     @property
-    def records(self) -> LruCache:
+    def records(self) -> LRU[int, Arparma]:
         return self.__record
 
     def reuse(self, index: int = -1):
-        key = list(self.__record.cache.keys())[index]
+        key = self.__record.keys()[index]
         return self.__record[key]
 
     def __repr__(self):
         return (
             f"Current: {hex(id(self))} in {datetime.now().strftime('%Y/%m/%d %H:%M:%S')}\n" +
             "Commands:\n" +
-            f"[{', '.join(map(lambda x: x.path, self.get_commands()))}]" +
+            f"[{', '.join([cmd.path for cmd in self.get_commands()])}]" +
             "\nShortcuts:\n" +
             "\n".join([f" {k} => {v}" for k, v in self.__shortcuts.items()]) +
             "\nRecords:\n" +
-            "\n".join([f" [{k}]: {v[1].origin}" for k, v in enumerate(self.__record.items(20))]) +
+            "\n".join([f" [{k}]: {v[1].origin}" for k, v in enumerate(self.__record.items()[:20])]) +
             "\nDisabled Commands:\n" +
             f"[{', '.join(map(lambda x: x.path, self.__abandons))}]"
         )
 
 
 command_manager = CommandManager()
 __all__ = ["ShortcutArgs", "command_manager"]
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/model.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-_repr_ = lambda self: " ".join(f"{k}={getattr(self, k, ...)!r}" for k in self.__slots__)
+_repr_ = lambda self: "(" + " ".join([f"{k}={getattr(self, k, ...)!r}" for k in self.__slots__]) + ")"
 
 
 @dataclass(init=False, eq=True)
 class Sentence:
     __slots__ = ("name", "separators")
     __repr__ = _repr_
     def __init__(self, name, separators=None):
@@ -31,12 +31,16 @@
         self.subcommands = subcommands or {}
 
 
 @dataclass(init=False, eq=True)
 class HeadResult:
     __slots__ = ("origin", "result", "matched", "groups")
     __repr__ = _repr_
-    def __init__(self, origin=None, result=None, matched=False, groups=None):
+    def __init__(self, origin=None, result=None, matched=False, groups=None, fixes=None):
         self.origin = origin
         self.result = result
         self.matched = matched
         self.groups = groups or {}
+        if fixes:
+            self.groups.update(
+                {k: v(self.groups[k])._value for k, v in fixes.items() if k in self.groups}  # noqa
+            )
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/model.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from typing import Any
+from nepattern import BasePattern
 
 class Sentence:
     name: str
     separators: tuple[str, ...]
     def __init__(self, name: str, separators: tuple[str, ...] | None = ...) -> None: ...
 
 class OptionResult:
@@ -24,11 +25,16 @@
         subcommands: dict[str, SubcommandResult] | None = ...
     ) -> None: ...
 
 class HeadResult:
     origin: Any
     result: Any
     matched: bool
-    groups: dict[str, str]
+    groups: dict[str, Any]
     def __init__(
-        self, origin: Any = ..., result: Any = ..., matched: bool = ..., groups: dict[str, str] | None = ...
+        self,
+        origin: Any = ...,
+        result: Any = ...,
+        matched: bool = ...,
+        groups: dict[str, str] | None = ...,
+        fixes: dict[str, BasePattern] | None = ...
     ) -> None: ...
```

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/output.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.0rc1/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.0rc2/src/arclet/alconna/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class DataCollection(Protocol[DataUnit]):
     """数据集合协议"""
     def __repr__(self) -> str: ...
     def __iter__(self) -> Iterator[DataUnit]: ...
     def __len__(self) -> int: ...
 
 
-TDataCollection = TypeVar("TDataCollection", bound=DataCollection[Union[str, Any]])
+TDataCollection = TypeVar("TDataCollection", bound=DataCollection[Any])
 
 
 class KeyWordVar(BasePattern):
     """对具名参数的包装"""
     base: BasePattern
 
     def __init__(self, value: BasePattern | Any, sep: str = '='):
```

### Comparing `arclet-alconna-1.7.0rc1/PKG-INFO` & `arclet-alconna-1.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.0rc1
+Version: 1.7.0rc2
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -18,16 +18,15 @@
 Provides-Extra: cli
 Provides-Extra: full
 Provides-Extra: graia
 Project-URL: documentation, https://arcletproject.github.io/docs/alconna/tutorial
 Project-URL: repository, https://github.com/ArcletProject/Alconna
 Description-Content-Type: text/markdown
 
-![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2Fu%2F42648639%3Fs%3D400%26u%3Da81d93f3683d0a3b7d38ea8e6a4903355986e8c7%26v%3D4&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Light)
-
+![](https://socialify.git.ci/ArcletProject/Alconna/image?description=1&descriptionEditable=A%20High-performance%2C%20Generality%2C%20Humane%20Command%20Line%20Arguments%20Parser%20Library.&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Farclet.top%2Fimg%2Farclet.png&name=1&owner=1&pattern=Brick%20Wall&stargazers=1&theme=Auto)
 <div align="center"> 
 
 # Alconna
 
 </div>
 
 ![Alconna](https://img.shields.io/badge/Arclet-Alconna-2564c2.svg)
@@ -76,14 +75,15 @@
 ```
 
 Output as follows:
 ```
 value=None args={'pak_name': 'numpy'} options={'upgrade': value=Ellipsis args={}} subcommands={}
 ```
 
+
 ## Communication
 
 QQ Group: [Link](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 ## Features
 
 * High Performance. On i5-10210U, performance is about `71000~289000 msg/s`; test script: [benchmark](benchmark.py)
```

