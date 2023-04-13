# Comparing `tmp/TheengsDecoder-1.3.7.tar.gz` & `tmp/TheengsDecoder-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheengsDecoder-1.3.7.tar", last modified: Tue Mar 28 12:37:27 2023, max compression
+gzip compressed data, was "TheengsDecoder-1.4.0.tar", last modified: Thu Apr 13 16:30:41 2023, max compression
```

## Comparing `TheengsDecoder-1.3.7.tar` & `TheengsDecoder-1.4.0.tar`

### file list

```diff
@@ -1,270 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.344149 TheengsDecoder-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-03-28 12:37:27.344149 TheengsDecoder-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.312149 TheengsDecoder-1.3.7/TheengsDecoder/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/TheengsDecoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/TheengsDecoder/_decoder.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.312149 TheengsDecoder-1.3.7/TheengsDecoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-03-28 12:37:27.000000 TheengsDecoder-1.3.7/TheengsDecoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11368 2023-03-28 12:37:27.000000 TheengsDecoder-1.3.7/TheengsDecoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 12:37:27.000000 TheengsDecoder-1.3.7/TheengsDecoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-28 12:37:27.000000 TheengsDecoder-1.3.7/TheengsDecoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 12:37:27.344149 TheengsDecoder-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-03-28 12:37:25.000000 TheengsDecoder-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.316149 TheengsDecoder-1.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.316149 TheengsDecoder-1.3.7/src/arduino_json/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-03-28 12:37:18.000000 TheengsDecoder-1.3.7/src/arduino_json/.git
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/.mbedignore
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/ArduinoJson.h
--rw-r--r--   0 runner    (1001) docker     (122)    40084 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)    10845 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (122)    32515 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/banner.svg
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/component.mk
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/keywords.txt
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/library.json
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/library.properties
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.316149 TheengsDecoder-1.3.7/src/arduino_json/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.316149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.320149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.320149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Collection/
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Configuration.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.320149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/
--rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.320149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStringReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.320149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/
--rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.324149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/Latch.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.324149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Memory/
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.324149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Misc/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Misc/Visitable.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.324149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/
--rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/ieee754.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Namespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.324149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/Float.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.324149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/Pair.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.328149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/assert.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/ctype.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/integer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/math.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.328149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/mpl/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.332149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/conditional.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/declval.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/enable_if.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/integral_constant.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_array.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_const.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_floating_point.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_same.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_void.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_const.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_cv.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_reference.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/type_identity.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.332149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.332149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/DummyWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/measure.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.332149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.332149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.336149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/StoragePolicy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/String.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.336149 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/Converter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5651 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10885 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantTag.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/compatibility.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/version.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson.h
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-03-28 12:37:19.000000 TheengsDecoder-1.3.7/src/arduino_json/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    29794 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/decoder.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 12:37:27.344149 TheengsDecoder-1.3.7/src/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/ABN03_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/ABTemp_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/APPLE_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/Amphiro_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BC08_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BM1IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BM2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BM3IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BM4IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BPARASITE_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/BWBSDOO_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGD1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGDK2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGDN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     6309 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGG1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGH1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGP1W_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/CGPR1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/GAEN_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/H5055_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/H5072_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/H5074_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/H5102_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2792 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/H5106_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/HHCCJCY01HHCC_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/HHCCPOT002_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/IBS_THBP01B_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/IBT_2X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/IBT_4XS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/IBT_6XS_SOLIS6_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/JHT_F525_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/JQJCY01YM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/LYWSD02_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/LYWSD03MMC_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/LYWSDCGQ_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3892 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/MBXPRO_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/MS_CDP_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/MUE4094RT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/Miband_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/Mokobeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/Mopeka_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/PH10_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     8958 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/RDL52832_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/RuuviTag_RAWv1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/RuuviTag_RAWv2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SBCS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SBCU_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SBMS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SBMT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SBS1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SCD4X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SHT4X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/ServiceData_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/Skale_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/SmartDry_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/T201_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/T301_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/TPMS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/TPTH_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/ThermoBeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/XMTZC04HM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/XMTZC05HM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/common_props.h
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/iBeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/iNodeEM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices/tracker_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     6265 2023-03-28 12:37:17.000000 TheengsDecoder-1.3.7/src/devices.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.237486 TheengsDecoder-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-04-13 16:30:41.237486 TheengsDecoder-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.197485 TheengsDecoder-1.4.0/TheengsDecoder/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/TheengsDecoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/TheengsDecoder/_decoder.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.197485 TheengsDecoder-1.4.0/TheengsDecoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-04-13 16:30:41.000000 TheengsDecoder-1.4.0/TheengsDecoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11397 2023-04-13 16:30:41.000000 TheengsDecoder-1.4.0/TheengsDecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 16:30:41.000000 TheengsDecoder-1.4.0/TheengsDecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-13 16:30:41.000000 TheengsDecoder-1.4.0/TheengsDecoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 16:30:41.237486 TheengsDecoder-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-13 16:30:40.000000 TheengsDecoder-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.197485 TheengsDecoder-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.201485 TheengsDecoder-1.4.0/src/arduino_json/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-13 16:30:33.000000 TheengsDecoder-1.4.0/src/arduino_json/.git
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/.mbedignore
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/ArduinoJson.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40084 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10845 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    32515 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/banner.svg
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/component.mk
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/library.json
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/library.properties
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.201485 TheengsDecoder-1.4.0/src/arduino_json/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.205485 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.209485 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.209485 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Collection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Configuration.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.209485 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/
+-rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.209485 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStringReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.209485 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/
+-rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.213486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.213486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Memory/
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.213486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Misc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Misc/Visitable.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.213486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/
+-rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/ieee754.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Namespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.213486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/Float.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.213486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.217486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/assert.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/ctype.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/integer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/math.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.217486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.221486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/conditional.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/declval.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/enable_if.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/integral_constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_array.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_const.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_floating_point.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_same.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_void.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_const.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_cv.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/type_identity.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.221486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.221486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/DummyWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/measure.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.221486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.221486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.225486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/StoragePolicy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/String.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.225486 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/Converter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5651 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10885 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantTag.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/compatibility.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/version.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-04-13 16:30:34.000000 TheengsDecoder-1.4.0/src/arduino_json/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    29794 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/decoder.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 16:30:41.237486 TheengsDecoder-1.4.0/src/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/ABN03_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/ABTemp_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/APPLE_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/Amphiro_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BC08_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BM1IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BM2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BM3IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BM4IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BPARASITE_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/BWBSDOO_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGD1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGDK2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGDN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6309 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGG1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGH1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGP1W_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/CGPR1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/GAEN_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/H5055_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/H5072_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/H5074_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/H5102_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/H5106_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/HHCCJCY01HHCC_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/HHCCJCY10_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/HHCCPOT002_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/IBS_THBP01B_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/IBT_2X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/IBT_4XS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/IBT_6XS_SOLIS6_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/JHT_F525_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/JQJCY01YM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/LYWSD02_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/LYWSD03MMC_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/LYWSDCGQ_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3892 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/MBXPRO_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/MS_CDP_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/MUE4094RT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/Miband_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/Mokobeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/Mopeka_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/PH10_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8958 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/RDL52832_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/RuuviTag_RAWv1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/RuuviTag_RAWv2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SBCS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SBCU_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SBMS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SBMT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SBS1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SCD4X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SHT4X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/ServiceData_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/Skale_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/SmartDry_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/T201_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/T301_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/TPMS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/TPTH_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/ThermoBeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/XMTZC04HM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/XMTZC05HM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/common_props.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/iBeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/iNodeEM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices/tracker_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6347 2023-04-13 16:30:32.000000 TheengsDecoder-1.4.0/src/devices.h
```

### Comparing `TheengsDecoder-1.3.7/CMakeLists.txt` & `TheengsDecoder-1.4.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/LICENSE.txt` & `TheengsDecoder-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/PKG-INFO` & `TheengsDecoder-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: TheengsDecoder
-Version: 1.3.7
-Summary: A message decoder for the Internet of Things
-Author: Theengs
-License:  GPL-3.0 License
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 Theengs Decoder project aims to provide an efficient, portable and lightweight library for Internet of Things messages decoding.
 
 ![Iot](https://github.com/theengs/decoder/raw/development//docs/img/Theengs_decoder_iot_chain.jpg)
 
 Sensors and devices use chains of data to communicate to gateways, computers, servers. Enabling them to have lightweight and fast communication.
 On the other hand we have a huge diversity of communication methods, resulting in the sensors or devices being closed to one ecosystem or a few.
```

### Comparing `TheengsDecoder-1.3.7/README.md` & `TheengsDecoder-1.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: TheengsDecoder
+Version: 1.4.0
+Summary: A message decoder for the Internet of Things
+Author: Theengs
+License:  GPL-3.0 License
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 Theengs Decoder project aims to provide an efficient, portable and lightweight library for Internet of Things messages decoding.
 
 ![Iot](https://github.com/theengs/decoder/raw/development//docs/img/Theengs_decoder_iot_chain.jpg)
 
 Sensors and devices use chains of data to communicate to gateways, computers, servers. Enabling them to have lightweight and fast communication.
 On the other hand we have a huge diversity of communication methods, resulting in the sensors or devices being closed to one ecosystem or a few.
```

### Comparing `TheengsDecoder-1.3.7/TheengsDecoder/_decoder.cpp` & `TheengsDecoder-1.4.0/TheengsDecoder/_decoder.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -19,22 +19,14 @@
   if (!err) {
     TheengsDecoder decoder;
     JsonObject bleObject;
     bleObject = doc.as<JsonObject>();
 
     if (decoder.decodeBLEJson(bleObject) >= 0) {
       std::string buf;
-      bleObject.remove("servicedata");
-      bleObject.remove("manufacturerdata");
-      bleObject.remove("servicedatauuid");
-      bleObject.remove("type");
-      bleObject.remove("cidc");
-      bleObject.remove("acts");
-      bleObject.remove("cont");
-      bleObject.remove("track");
       serializeJson(bleObject, buf);
       return Py_BuildValue("s", buf.c_str());
     }
   }
 
   Py_RETURN_NONE;
 }
```

### Comparing `TheengsDecoder-1.3.7/TheengsDecoder.egg-info/PKG-INFO` & `TheengsDecoder-1.4.0/TheengsDecoder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheengsDecoder
-Version: 1.3.7
+Version: 1.4.0
 Summary: A message decoder for the Internet of Things
 Author: Theengs
 License:  GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Theengs Decoder project aims to provide an efficient, portable and lightweight library for Internet of Things messages decoding.
```

### Comparing `TheengsDecoder-1.3.7/TheengsDecoder.egg-info/SOURCES.txt` & `TheengsDecoder-1.4.0/TheengsDecoder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 src/devices/GAEN_json.h
 src/devices/H5055_json.h
 src/devices/H5072_json.h
 src/devices/H5074_json.h
 src/devices/H5102_json.h
 src/devices/H5106_json.h
 src/devices/HHCCJCY01HHCC_json.h
+src/devices/HHCCJCY10_json.h
 src/devices/HHCCPOT002_json.h
 src/devices/IBS_THBP01B_json.h
 src/devices/IBT_2X_json.h
 src/devices/IBT_4XS_json.h
 src/devices/IBT_6XS_SOLIS6_json.h
 src/devices/JHT_F525_json.h
 src/devices/JQJCY01YM_json.h
```

### Comparing `TheengsDecoder-1.3.7/setup.py` & `TheengsDecoder-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if version.parse(get_cmake_version()) < version.parse("3.4"):
         setup_requires.append("cmake")
 except SKBuildError:
     setup_requires.append("cmake")
 
 setup(
     name="TheengsDecoder",
-    version="v1.3.7",
+    version="v1.4.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A message decoder for the Internet of Things",
     author='Theengs',
     license=" GPL-3.0 License",
     packages=['TheengsDecoder'],
     setup_requires=setup_requires,
```

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/CHANGELOG.md` & `TheengsDecoder-1.4.0/src/arduino_json/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/CMakeLists.txt` & `TheengsDecoder-1.4.0/src/arduino_json/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/LICENSE.md` & `TheengsDecoder-1.4.0/src/arduino_json/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/README.md` & `TheengsDecoder-1.4.0/src/arduino_json/README.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/SUPPORT.md` & `TheengsDecoder-1.4.0/src/arduino_json/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/appveyor.yml` & `TheengsDecoder-1.4.0/src/arduino_json/appveyor.yml`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/banner.svg` & `TheengsDecoder-1.4.0/src/arduino_json/banner.svg`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/keywords.txt` & `TheengsDecoder-1.4.0/src/arduino_json/keywords.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/library.json` & `TheengsDecoder-1.4.0/src/arduino_json/library.json`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/library.properties` & `TheengsDecoder-1.4.0/src/arduino_json/library.properties`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Configuration.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Configuration.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/Latch.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Namespace.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Namespace.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Object/Pair.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/String.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/String.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson/compatibility.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson/compatibility.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/ArduinoJson.hpp` & `TheengsDecoder-1.4.0/src/arduino_json/src/ArduinoJson.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/arduino_json/src/CMakeLists.txt` & `TheengsDecoder-1.4.0/src/arduino_json/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/decoder.cpp` & `TheengsDecoder-1.4.0/src/decoder.cpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/decoder.h` & `TheengsDecoder-1.4.0/src/decoder.h`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     CGPR1,
     THERMOBEACON,
     H5055,
     H5072,
     H5074,
     H5102,
     H5106,
+    HHCCJCY10,
     MUE4094RT,
     MOKOBEACON,
     MOKOBEACONXPRO,
     INODEEM,
     RUUVITAG_RAWV1,
     RUUVITAG_RAWV2,
     SBCS,
@@ -135,13 +136,13 @@
   uint8_t     getBinaryData(char ch);
   bool        evaluateDatalength(std::string op, size_t data_len, size_t req_len);
   bool        checkPropCondition(const JsonArray& prop, const char* svc_data, const char* mfg_data);
   bool        checkDeviceMatch(const JsonArray& condition, const char* svc_data, const char* mfg_data,
                                const char* dev_name, const char* svc_uuid, const char* mac_id);
   std::string sanitizeJsonKey(const char* key_in);
 
-  size_t m_docMax = 12000;
+  size_t m_docMax = 13000;
   size_t m_minSvcDataLen = 20;
   size_t m_minMfgDataLen = 16;
 };
 
 #endif
```

### Comparing `TheengsDecoder-1.3.7/src/devices/ABN03_json.h` & `TheengsDecoder-1.4.0/src/devices/ABN03_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/ABTemp_json.h` & `TheengsDecoder-1.4.0/src/devices/ABTemp_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/APPLE_json.h` & `TheengsDecoder-1.4.0/src/devices/APPLE_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/Amphiro_json.h` & `TheengsDecoder-1.4.0/src/devices/Amphiro_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BC08_json.h` & `TheengsDecoder-1.4.0/src/devices/BC08_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BM1IN1_json.h` & `TheengsDecoder-1.4.0/src/devices/BM1IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BM2_json.h` & `TheengsDecoder-1.4.0/src/devices/BM2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BM3IN1_json.h` & `TheengsDecoder-1.4.0/src/devices/BM3IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BM4IN1_json.h` & `TheengsDecoder-1.4.0/src/devices/BM4IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BPARASITE_json.h` & `TheengsDecoder-1.4.0/src/devices/BPARASITE_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/BWBSDOO_json.h` & `TheengsDecoder-1.4.0/src/devices/BWBSDOO_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGD1_json.h` & `TheengsDecoder-1.4.0/src/devices/CGD1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGDK2_json.h` & `TheengsDecoder-1.4.0/src/devices/CGDK2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGDN1_json.h` & `TheengsDecoder-1.4.0/src/devices/CGDN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGG1_json.h` & `TheengsDecoder-1.4.0/src/devices/CGG1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGH1_json.h` & `TheengsDecoder-1.4.0/src/devices/CGH1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGP1W_json.h` & `TheengsDecoder-1.4.0/src/devices/CGP1W_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/CGPR1_json.h` & `TheengsDecoder-1.4.0/src/devices/CGPR1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/GAEN_json.h` & `TheengsDecoder-1.4.0/src/devices/GAEN_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/H5055_json.h` & `TheengsDecoder-1.4.0/src/devices/H5055_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/H5072_json.h` & `TheengsDecoder-1.4.0/src/devices/H5072_json.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #include "common_props.h"
 
-const char* _H5072_json = "{\"brand\":\"Govee\",\"model\":\"Thermo Hygrometer\",\"model_id\":\"H5072/75\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"GVH5072\",\"|\",\"name\",\"index\",0,\"GVH5075\",\"&\",\"manufacturerdata\",\"=\",16,\"index\",0,\"88ec\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",6,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,6,false,false],\"post_proc\":[\"/\",1000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",6,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,6,false,false],\"post_proc\":[\"-\",8388608,\"/\",10000,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,6,false,false],\"post_proc\":[\"%\",1000,\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",12,2,false,false]}}}";
+const char* _H5072_json = "{\"brand\":\"Govee\",\"model\":\"Thermo Hygrometer\",\"model_id\":\"H5072/75\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"GVH5072\",\"|\",\"name\",\"index\",0,\"GVH5075\",\"&\",\"manufacturerdata\",\">=\",16,\"index\",0,\"88ec\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",6,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,6,false,false],\"post_proc\":[\"/\",1000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",6,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,6,false,false],\"post_proc\":[\"-\",8388608,\"/\",10000,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,6,false,false],\"post_proc\":[\"%\",1000,\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",12,2,false,false]}}}";
 
 /* R""""(
 {
    "brand":"Govee",
    "model":"Thermo Hygrometer",
    "model_id":"H5072/75",
    "tag":"0103",
-   "condition":["name", "index", 0, "GVH5072", "|", "name", "index", 0, "GVH5075", "&", "manufacturerdata", "=", 16, "index", 0, "88ec"],
+   "condition":["name", "index", 0, "GVH5072", "|", "name", "index", 0, "GVH5075", "&", "manufacturerdata", ">=", 16, "index", 0, "88ec"],
    "properties":{
       "tempc":{
          "condition":["manufacturerdata", 6, "bit", 3, 0],
          "decoder":["value_from_hex_data", "manufacturerdata", 6, 6, false, false],
          "post_proc":["/", 1000, ">", 0, "/", 10]
       },
       "_tempc":{
```

### Comparing `TheengsDecoder-1.3.7/src/devices/H5074_json.h` & `TheengsDecoder-1.4.0/src/devices/H5074_json.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #include "common_props.h"
 
-const char* _H5074_json = "{\"brand\":\"Govee\",\"model\":\"Thermo Hygrometer\",\"model_id\":\"H5074\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"Govee_H5074\",\"&\",\"manufacturerdata\",\"=\",18,\"index\",0,\"88ec\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,4,true,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,4,true,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,2,false,false]}}}";
+const char* _H5074_json = "{\"brand\":\"Govee\",\"model\":\"Thermo Hygrometer\",\"model_id\":\"H5074\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"Govee_H5074\",\"&\",\"manufacturerdata\",\">=\",18,\"index\",0,\"88ec\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,4,true,true],\"post_proc\":[\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,4,true,false],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,2,false,false]}}}";
 
 /* R""""(
 {
    "brand":"Govee",
    "model":"Thermo Hygrometer",
    "model_id":"H5074",
    "tag":"0103",
-   "condition":["name", "index", 0, "Govee_H5074", "&", "manufacturerdata", "=", 18, "index", 0, "88ec"],
+   "condition":["name", "index", 0, "Govee_H5074", "&", "manufacturerdata", ">=", 18, "index", 0, "88ec"],
    "properties":{
       "tempc":{
          "decoder":["value_from_hex_data", "manufacturerdata", 6, 4, true, true],
          "post_proc":["/", 100]
       },
       "hum":{
          "decoder":["value_from_hex_data", "manufacturerdata", 10, 4, true, false],
```

### Comparing `TheengsDecoder-1.3.7/src/devices/H5102_json.h` & `TheengsDecoder-1.4.0/src/devices/H5102_json.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #include "common_props.h"
 
-const char* _H5102_json = "{\"brand\":\"Govee\",\"model\":\"Smart Thermo Hygrometer\",\"model_id\":\"H5101/02/74/77\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"GVH5101\",\"|\",\"name\",\"index\",0,\"GVH5102\",\"|\",\"name\",\"index\",0,\"GVH5174\",\"|\",\"name\",\"index\",0,\"GVH5177\",\"&\",\"manufacturerdata\",\"=\",16,\"index\",0,\"0100\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,6,false,false],\"post_proc\":[\"/\",1000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,6,false,false],\"post_proc\":[\"&\",8388607,\"/\",1000,\">\",0,\"/\",10,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,6,false,false],\"post_proc\":[\"%\",1000,\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,2,false,false]}}}";
+const char* _H5102_json = "{\"brand\":\"Govee\",\"model\":\"Smart Thermo Hygrometer\",\"model_id\":\"H5101/02/74/77\",\"tag\":\"0103\",\"condition\":[\"name\",\"index\",0,\"GVH5101\",\"|\",\"name\",\"index\",0,\"GVH5102\",\"|\",\"name\",\"index\",0,\"GVH5174\",\"|\",\"name\",\"index\",0,\"GVH5177\",\"&\",\"manufacturerdata\",\">=\",16,\"index\",0,\"0100\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,6,false,false],\"post_proc\":[\"/\",1000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,6,false,false],\"post_proc\":[\"&\",8388607,\"/\",1000,\">\",0,\"/\",10,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,6,false,false],\"post_proc\":[\"%\",1000,\"/\",10]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",14,2,false,false]}}}";
 
 /* R""""(
 {
    "brand":"Govee",
    "model":"Smart Thermo Hygrometer",
    "model_id":"H5101/02/74/77",
    "tag":"0103",
-   "condition":["name", "index", 0, "GVH5101", "|", "name", "index", 0, "GVH5102", "|", "name", "index", 0, "GVH5174", "|", "name", "index", 0, "GVH5177", "&", "manufacturerdata", "=", 16, "index", 0, "0100"],
+   "condition":["name", "index", 0, "GVH5101", "|", "name", "index", 0, "GVH5102", "|", "name", "index", 0, "GVH5174", "|", "name", "index", 0, "GVH5177", "&", "manufacturerdata", ">=", 16, "index", 0, "0100"],
    "properties":{
       "tempc":{
          "condition":["manufacturerdata", 8, "bit", 3, 0],
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 6, false, false],
          "post_proc":["/", 1000, ">", 0, "/", 10]
       },
       "_tempc":{
```

### Comparing `TheengsDecoder-1.3.7/src/devices/H5106_json.h` & `TheengsDecoder-1.4.0/src/devices/H5106_json.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-const char* _H5106_json = "{\"brand\":\"Govee\",\"model\":\"Smart Air Quality Monitor\",\"model_id\":\"H5106\",\"tag\":\"0f03\",\"condition\":[\"name\",\"index\",0,\"GVH5106\",\"&\",\"manufacturerdata\",\"=\",16,\"index\",0,\"0100\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"/\",1000000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000000,\">\",0,\"/\",10,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"%\",1000000,\"/\",10000,\">\",0]},\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000,\">\",0,\"*\",1000]},\"pm25\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"-\",\".cal\"]}}}";
+const char* _H5106_json = "{\"brand\":\"Govee\",\"model\":\"Smart Air Quality Monitor\",\"model_id\":\"H5106\",\"tag\":\"0f03\",\"condition\":[\"name\",\"index\",0,\"GVH5106\",\"&\",\"manufacturerdata\",\">=\",16,\"index\",0,\"0100\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"/\",1000000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000000,\">\",0,\"/\",10,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"%\",1000000,\"/\",10000,\">\",0]},\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000,\">\",0,\"*\",1000]},\"pm25\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"-\",\".cal\"]}}}";
 /* R""""(
 {
    "brand":"Govee",
    "model":"Smart Air Quality Monitor",
    "model_id":"H5106",
    "tag":"0f03",
-   "condition":["name", "index", 0, "GVH5106", "&", "manufacturerdata", "=", 16, "index", 0, "0100"],
+   "condition":["name", "index", 0, "GVH5106", "&", "manufacturerdata", ">=", 16, "index", 0, "0100"],
    "properties":{
       "tempc":{
          "condition":["manufacturerdata", 8, "bit", 3, 0],
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 8, false, false],
          "post_proc":["/", 1000000, ">", 0, "/", 10]
       },
       "_tempc":{
```

### Comparing `TheengsDecoder-1.3.7/src/devices/HHCCJCY01HHCC_json.h` & `TheengsDecoder-1.4.0/src/devices/HHCCJCY01HHCC_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/HHCCPOT002_json.h` & `TheengsDecoder-1.4.0/src/devices/HHCCPOT002_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/IBS_THBP01B_json.h` & `TheengsDecoder-1.4.0/src/devices/IBS_THBP01B_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/IBT_2X_json.h` & `TheengsDecoder-1.4.0/src/devices/IBT_2X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/IBT_4XS_json.h` & `TheengsDecoder-1.4.0/src/devices/IBT_4XS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/IBT_6XS_SOLIS6_json.h` & `TheengsDecoder-1.4.0/src/devices/IBT_6XS_SOLIS6_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/JHT_F525_json.h` & `TheengsDecoder-1.4.0/src/devices/JHT_F525_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/JQJCY01YM_json.h` & `TheengsDecoder-1.4.0/src/devices/JQJCY01YM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/LYWSD02_json.h` & `TheengsDecoder-1.4.0/src/devices/LYWSD02_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/LYWSD03MMC_json.h` & `TheengsDecoder-1.4.0/src/devices/LYWSD03MMC_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/LYWSDCGQ_json.h` & `TheengsDecoder-1.4.0/src/devices/LYWSDCGQ_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/MBXPRO_json.h` & `TheengsDecoder-1.4.0/src/devices/MBXPRO_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/MS_CDP_json.h` & `TheengsDecoder-1.4.0/src/devices/MS_CDP_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/MUE4094RT_json.h` & `TheengsDecoder-1.4.0/src/devices/MUE4094RT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/Miband_json.h` & `TheengsDecoder-1.4.0/src/devices/Miband_json.h`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       },
       "device":{
          "decoder":["static_value", "Xiaomi/Amazfit Tracker"]
       }
    }
 })"""";*/
 
-const char* _Miband_json_props = "{\"properties\":{\"steps\":{\"unit\":\"int\",\"name\":\"step-count\"},\"act_bpm\":{\"unit\":\"bpm\",\"name\":\"activity heart rate\"},\"device\":{\"unit\":\"string\",\"name\":\"tracker device\"}}}}";
+const char* _Miband_json_props = "{\"properties\":{\"steps\":{\"unit\":\"int\",\"name\":\"step-count\"},\"act_bpm\":{\"unit\":\"bpm\",\"name\":\"activity heart rate\"},\"device\":{\"unit\":\"string\",\"name\":\"tracker device\"}}}";
 /*R""""(
 {
    "properties":{
       "steps":{
          "unit":"int",
          "name":"step-count"
       },
```

### Comparing `TheengsDecoder-1.3.7/src/devices/Mokobeacon_json.h` & `TheengsDecoder-1.4.0/src/devices/Mokobeacon_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/Mopeka_json.h` & `TheengsDecoder-1.4.0/src/devices/Mopeka_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/PH10_json.h` & `TheengsDecoder-1.4.0/src/devices/PH10_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/RDL52832_json.h` & `TheengsDecoder-1.4.0/src/devices/RDL52832_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/RuuviTag_RAWv1_json.h` & `TheengsDecoder-1.4.0/src/devices/RuuviTag_RAWv1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/RuuviTag_RAWv2_json.h` & `TheengsDecoder-1.4.0/src/devices/RuuviTag_RAWv2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SBCS_json.h` & `TheengsDecoder-1.4.0/src/devices/SBCS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SBCU_json.h` & `TheengsDecoder-1.4.0/src/devices/SBCU_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SBMS_json.h` & `TheengsDecoder-1.4.0/src/devices/SBMS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SBMT_json.h` & `TheengsDecoder-1.4.0/src/devices/SBMT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SBS1_json.h` & `TheengsDecoder-1.4.0/src/devices/SBS1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SCD4X_json.h` & `TheengsDecoder-1.4.0/src/devices/SCD4X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SHT4X_json.h` & `TheengsDecoder-1.4.0/src/devices/SHT4X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/ServiceData_json.h` & `TheengsDecoder-1.4.0/src/devices/ServiceData_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/Skale_json.h` & `TheengsDecoder-1.4.0/src/devices/Skale_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/SmartDry_json.h` & `TheengsDecoder-1.4.0/src/devices/SmartDry_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/T201_json.h` & `TheengsDecoder-1.4.0/src/devices/T201_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/T301_json.h` & `TheengsDecoder-1.4.0/src/devices/T301_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/TPMS_json.h` & `TheengsDecoder-1.4.0/src/devices/TPMS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/TPTH_json.h` & `TheengsDecoder-1.4.0/src/devices/TPTH_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/ThermoBeacon_json.h` & `TheengsDecoder-1.4.0/src/devices/ThermoBeacon_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/XMTZC04HM_json.h` & `TheengsDecoder-1.4.0/src/devices/XMTZC04HM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/XMTZC05HM_json.h` & `TheengsDecoder-1.4.0/src/devices/XMTZC05HM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/common_props.h` & `TheengsDecoder-1.4.0/src/devices/common_props.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/iBeacon_json.h` & `TheengsDecoder-1.4.0/src/devices/iBeacon_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/iNodeEM_json.h` & `TheengsDecoder-1.4.0/src/devices/iNodeEM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices/tracker_json.h` & `TheengsDecoder-1.4.0/src/devices/tracker_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.3.7/src/devices.h` & `TheengsDecoder-1.4.0/src/devices.h`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 #include "devices/CGPR1_json.h"
 #include "devices/GAEN_json.h"
 #include "devices/H5055_json.h"
 #include "devices/H5072_json.h"
 #include "devices/H5074_json.h"
 #include "devices/H5102_json.h"
 #include "devices/H5106_json.h"
+#include "devices/HHCCJCY10_json.h"
 #include "devices/HHCCJCY01HHCC_json.h"
 #include "devices/HHCCPOT002_json.h"
 #include "devices/IBS_THBP01B_json.h"
 #include "devices/IBT_2X_json.h"
 #include "devices/IBT_4XS_json.h"
 #include "devices/IBT_6XS_SOLIS6_json.h"
 #include "devices/JQJCY01YM_json.h"
@@ -116,14 +117,15 @@
     {_CGPR1_json, _CGPR1_json_props},
     {_ThermoBeacon_json, _ThermoBeacon_json_props},
     {_H5055_json, _H5055_json_props},
     {_H5072_json, _H5072_json_props},
     {_H5074_json, _H5074_json_props},
     {_H5102_json, _H5102_json_props},
     {_H5106_json, _H5106_json_props},
+    {_HHCCJCY10_json, _HHCCJCY10_json_props},
     {_MUE4094RT_json, _MUE4094RT_json_props},
     {_Mokobeacon_json, _Mokobeacon_json_props},
     {_MBXPRO_json, _MBXPRO_json_props},
     {_iNodeEM_json, _iNodeEM_json_props},
     {_RuuviTag_RAWv1_json, _RuuviTag_RAWv1_json_props},
     {_RuuviTag_RAWv2_json, _RuuviTag_RAWv2_json_props},
     {_SBCS_json, _SBCS_json_props},
```

