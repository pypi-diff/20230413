# Comparing `tmp/pyriksprot-2022.3.2.tar.gz` & `tmp/pyriksprot-2022.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot-2022.3.2.tar", max compression
+gzip compressed data, was "pyriksprot-2022.5.2.tar", max compression
```

## Comparing `pyriksprot-2022.3.2.tar` & `pyriksprot-2022.5.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2022.3.2/LICENSE
--rw-r--r--   0        0        0     6675 2022-03-14 19:05:38.857587 pyriksprot-2022.3.2/README.md
--rw-r--r--   0        0        0     3365 2022-03-31 11:44:40.862164 pyriksprot-2022.3.2/pyproject.toml
--rw-r--r--   0        0        0     1362 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/__init__.py
--rw-r--r--   0        0        0      112 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/__init__.py
--rw-r--r--   0        0        0     3621 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/corpus_index.py
--rw-r--r--   0        0        0    10645 2022-03-31 11:43:17.389668 pyriksprot-2022.3.2/pyriksprot/corpus/iterate.py
--rw-r--r--   0        0        0      326 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/__init__.py
--rw-r--r--   0        0        0     3500 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/convert.py
--rw-r--r--   0        0        0     3651 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/iterate.py
--rw-r--r--   0        0        0    10088 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/parse.py
--rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/__init__.py
--rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
--rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
--rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
--rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
--rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
--rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
--rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
--rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
--rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
--rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/tf.py
--rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/tagged/__init__.py
--rw-r--r--   0        0        0     1556 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/tagged/iterate.py
--rw-r--r--   0        0        0     5761 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/corpus/tagged/persist.py
--rw-r--r--   0        0        0      141 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/dehyphenation/__init__.py
--rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/dehyphenation/flair_dehyphen.py
--rw-r--r--   0        0        0     7891 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/dehyphenation/swe_dehyphen.py
--rw-r--r--   0        0        0      403 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/dispatch/__init__.py
--rw-r--r--   0        0        0    16531 2022-03-31 11:43:17.389668 pyriksprot-2022.3.2/pyriksprot/dispatch/dispatch.py
--rw-r--r--   0        0        0     2098 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/dispatch/item.py
--rw-r--r--   0        0        0     5844 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/dispatch/merge.py
--rw-r--r--   0        0        0     2127 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/dispatch/utility.py
--rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/README.md
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/__init__.py
--rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/bettertokenizer.sv
--rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
--rw-r--r--   0        0        0    12240 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/foss/pos_tags.py
--rw-r--r--   0        0        0     7548 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/sparv_tokenize.py
--rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/stopwords.py
--rw-r--r--   0        0        0     6129 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/foss/untangle.py
--rw-r--r--   0        0        0    11564 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/interface.py
--rw-r--r--   0        0        0      494 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/metadata/__init__.py
--rw-r--r--   0        0        0     4720 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/metadata/codecs.py
--rw-r--r--   0        0        0    12647 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/metadata/generate.py
--rw-r--r--   0        0        0    11888 2022-03-31 11:43:17.389668 pyriksprot-2022.3.2/pyriksprot/metadata/person.py
--rw-r--r--   0        0        0     5176 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/metadata/utility.py
--rw-r--r--   0        0        0     1557 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/metadata/utterance.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2022.3.2/pyriksprot/scripts/__init__.py
--rw-r--r--   0        0        0     2359 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/metadata2db.py
--rw-r--r--   0        0        0     2579 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2speech.py
--rw-r--r--   0        0        0     2779 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2tagged.py
--rw-r--r--   0        0        0     2123 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2text.py
--rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2tfs.py
--rw-r--r--   0        0        0     1506 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/speakerhash.py
--rw-r--r--   0        0        0     4134 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/speech_index.py
--rw-r--r--   0        0        0     4795 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/scripts/utils.py
--rw-r--r--   0        0        0     6391 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/to_speech.py
--rw-r--r--   0        0        0    15773 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/utility.py
--rw-r--r--   0        0        0      133 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/workflows/__init__.py
--rw-r--r--   0        0        0     6369 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/workflows/extract_tags.py
--rw-r--r--   0        0        0     4805 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/workflows/extract_text.py
--rw-r--r--   0        0        0     4302 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/workflows/tag.py
--rw-r--r--   0        0        0     4056 2022-03-31 10:06:39.806371 pyriksprot-2022.3.2/pyriksprot/workflows/tf.py
--rw-r--r--   0        0        0     8333 2022-03-31 11:44:42.285895 pyriksprot-2022.3.2/setup.py
--rw-r--r--   0        0        0     7604 2022-03-31 11:44:42.286361 pyriksprot-2022.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2022.5.2/LICENSE
+-rw-r--r--   0        0        0     6675 2022-03-14 19:05:38.857587 pyriksprot-2022.5.2/README.md
+-rw-r--r--   0        0        0     3365 2022-05-11 05:27:50.057256 pyriksprot-2022.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1377 2022-05-08 09:29:23.979544 pyriksprot-2022.5.2/pyriksprot/__init__.py
+-rw-r--r--   0        0        0      112 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/__init__.py
+-rw-r--r--   0        0        0     3621 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/corpus_index.py
+-rw-r--r--   0        0        0    10663 2022-05-05 14:02:18.800048 pyriksprot-2022.5.2/pyriksprot/corpus/iterate.py
+-rw-r--r--   0        0        0      326 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/__init__.py
+-rw-r--r--   0        0        0     3503 2022-05-05 14:02:18.800048 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/convert.py
+-rw-r--r--   0        0        0     3651 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/iterate.py
+-rw-r--r--   0        0        0    11197 2022-05-10 09:30:30.108299 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/parse.py
+-rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/__init__.py
+-rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
+-rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
+-rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
+-rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
+-rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
+-rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
+-rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
+-rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
+-rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/tf.py
+-rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/tagged/__init__.py
+-rw-r--r--   0        0        0     1556 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/tagged/iterate.py
+-rw-r--r--   0        0        0     5797 2022-05-05 14:02:18.800048 pyriksprot-2022.5.2/pyriksprot/corpus/tagged/persist.py
+-rw-r--r--   0        0        0      141 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/dehyphenation/__init__.py
+-rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/dehyphenation/flair_dehyphen.py
+-rw-r--r--   0        0        0     7891 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/dehyphenation/swe_dehyphen.py
+-rw-r--r--   0        0        0      403 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/__init__.py
+-rw-r--r--   0        0        0    16531 2022-03-31 11:43:17.389668 pyriksprot-2022.5.2/pyriksprot/dispatch/dispatch.py
+-rw-r--r--   0        0        0     2098 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/item.py
+-rw-r--r--   0        0        0     5844 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/merge.py
+-rw-r--r--   0        0        0     2127 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/utility.py
+-rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/README.md
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/__init__.py
+-rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv
+-rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
+-rw-r--r--   0        0        0    12240 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/foss/pos_tags.py
+-rw-r--r--   0        0        0     7548 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/sparv_tokenize.py
+-rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/stopwords.py
+-rw-r--r--   0        0        0     6129 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/untangle.py
+-rw-r--r--   0        0        0    11716 2022-05-09 14:28:04.150091 pyriksprot-2022.5.2/pyriksprot/interface.py
+-rw-r--r--   0        0        0      494 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/__init__.py
+-rw-r--r--   0        0        0     4720 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/codecs.py
+-rw-r--r--   0        0        0    13692 2022-05-07 15:02:41.744714 pyriksprot-2022.5.2/pyriksprot/metadata/generate.py
+-rw-r--r--   0        0        0    11888 2022-03-31 11:43:17.389668 pyriksprot-2022.5.2/pyriksprot/metadata/person.py
+-rw-r--r--   0        0        0     5176 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/utility.py
+-rw-r--r--   0        0        0     1557 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/utterance.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/scripts/__init__.py
+-rw-r--r--   0        0        0     1648 2022-05-06 13:38:30.301815 pyriksprot-2022.5.2/pyriksprot/scripts/fix_speaker_notes.py
+-rw-r--r--   0        0        0     2359 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/metadata2db.py
+-rw-r--r--   0        0        0     2579 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2speech.py
+-rw-r--r--   0        0        0     2779 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2tagged.py
+-rw-r--r--   0        0        0     2123 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2text.py
+-rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2tfs.py
+-rw-r--r--   0        0        0     2176 2022-05-06 13:08:46.764962 pyriksprot-2022.5.2/pyriksprot/scripts/speech_index.py
+-rw-r--r--   0        0        0     4795 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/utils.py
+-rw-r--r--   0        0        0     6493 2022-05-09 08:27:29.314102 pyriksprot-2022.5.2/pyriksprot/to_speech.py
+-rw-r--r--   0        0        0    15777 2022-05-09 13:51:49.761315 pyriksprot-2022.5.2/pyriksprot/utility.py
+-rw-r--r--   0        0        0      196 2022-05-08 09:29:48.639724 pyriksprot-2022.5.2/pyriksprot/workflows/__init__.py
+-rw-r--r--   0        0        0     6369 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/workflows/extract_tags.py
+-rw-r--r--   0        0        0     4805 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/workflows/extract_text.py
+-rw-r--r--   0        0        0     3160 2022-05-06 13:38:30.317816 pyriksprot-2022.5.2/pyriksprot/workflows/speech_index.py
+-rw-r--r--   0        0        0     5411 2022-05-08 10:53:49.052959 pyriksprot-2022.5.2/pyriksprot/workflows/tag.py
+-rw-r--r--   0        0        0     4056 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/workflows/tf.py
+-rw-r--r--   0        0        0     8333 2022-05-11 05:27:51.333917 pyriksprot-2022.5.2/setup.py
+-rw-r--r--   0        0        0     7604 2022-05-11 05:27:51.334318 pyriksprot-2022.5.2/PKG-INFO
```

### Comparing `pyriksprot-2022.3.2/LICENSE` & `pyriksprot-2022.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/README.md` & `pyriksprot-2022.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyproject.toml` & `pyriksprot-2022.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot"
-version = "2022.3.2"
+version = "2022.5.2"
 description = "Python API for Riksdagens Protokoll"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/__init__.py` & `pyriksprot-2022.5.2/pyriksprot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,8 @@
     sync_delta_names,
     temporary_file,
     touch,
     ts_data_path,
     unlink,
 )
 from .workflows import compute_term_frequencies, extract_corpus_tags, extract_corpus_text
-from .workflows.tag import ITagger, TaggedDocument, tag_protocol, tag_protocol_xml
+from .workflows.tag import ITagger, TaggedDocument, tag_protocol, tag_protocol_xml, tag_protocols
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/corpus_index.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/corpus_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/iterate.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/iterate.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     id: str
     data: str
     page_number: str
     year: int
     u_id: str
     n_utterances: int = 0
     speaker_info: SpeakerInfo = None
-    speaker_hash: str = None
+    speaker_note_id: str = None
     speech_index: int = None
 
     def __len__(self) -> int:
         """IDispatchItem interface"""
         return 1
 
     def data_z64(self) -> bytes:
@@ -50,15 +50,15 @@
             'period': self.year,
             'who': self.who,
             'protocol_name': self.protocol_name,
             'document_name': self.name,
             'filename': self.filename,
             'n_tokens': self.n_tokens,
             'n_utterances': self.n_utterances,
-            'speaker_hash': self.speaker_hash,
+            'speaker_note_id': self.speaker_note_id,
             'speech_index': self.speech_index,
             'page_number': self.page_number,
             **({} if not self.speaker_info else self.speaker_info.to_dict()),
         }
 
     @staticmethod
     def dtypes() -> dict:
@@ -95,15 +95,15 @@
             id=protocol.name,
             u_id=None,
             data=protocol.text,
             page_number='0',
             n_tokens=0,
             n_utterances=len(protocol.utterances),
             speaker_info=None,
-            speaker_hash=None,
+            speaker_note_id=None,
         )
     ]
 
 
 def to_speech_segments(
     *,
     protocol: Protocol,
@@ -122,15 +122,15 @@
             who=s.who,
             id=s.speech_id,
             u_id=s.speech_id,
             data=s.to_content_str(content_type),
             page_number=s.page_number,
             n_tokens=0 if not s.has_tagged_text else s.tagged_text.count("\n"),
             n_utterances=len(s),
-            speaker_hash=s.speaker_hash,
+            speaker_note_id=s.speaker_note_id,
             speech_index=s.speech_index,
         )
         for s in mu.to_speeches(protocol=protocol, merge_strategy=merge_strategy, skip_size=segment_skip_size)
     ]
 
 
 def to_who_segments(
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/convert.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         return text
 
 
 def convert_protocol(
     input_filename: str = None,
     output_filename: str = None,
     template_name: str = None,
-    merge_strategy: to_speech.MergeStrategyType = to_speech.MergeStrategyType.who_speaker_hash_sequence,
+    merge_strategy: to_speech.MergeStrategyType = to_speech.MergeStrategyType.who_speaker_note_id_sequence,
     **dehyphen_cfg,
 ):
     """Convert protocol in `input_filename' using template `template_name`. Store result in `output_filename`.
 
     Args:
         input_filename (str, optional): Source file. Defaults to None.
         output_filename (str, optional): Target file. Defaults to None.
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/iterate.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/parse.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from loguru import logger
 
 from pyriksprot import interface
 from pyriksprot.foss import untangle
 from pyriksprot.utility import dedent as dedent_text
 from pyriksprot.utility import deprecated
 
+XML_ID: str = '{http://www.w3.org/XML/1998/namespace}id'
+
+MISSING_SPEAKER_NOTE_ID: str = "missing"
+
+# pylint: disable=too-many-statements
+
 
 class XmlProtocol(abc.ABC):
     def __init__(self, data: str, segment_skip_size: int = 0, delimiter: str = '\n'):
 
         self.data: str = data
         self.segment_skip_size: bool = segment_skip_size
         self.delimiter: str = delimiter
@@ -80,37 +86,59 @@
 
         super().__init__(data, segment_skip_size, delimiter)
 
     def create_iterator(self) -> Iterable[interface.Utterance]:
         return []
 
     def create_utterances(self) -> List[interface.Utterance]:
+
         utterances: List[interface.Utterance] = []
         page_number: str = None
 
         parent: untangle.Element = self.get_content_root()
         if parent is None:
             return utterances
 
-        speaker_hash: str = ''
+        speaker_note_id: str = MISSING_SPEAKER_NOTE_ID
+        previous_who: str = None
 
         for child in parent.children:
+
             if child.name == 'pb':
                 page_number = child['n']
+
             elif child.name == "note":
+
                 if child['type'] == "speaker":
-                    speaker_hash = child["n"]
-                    if speaker_hash:
-                        self.speaker_notes[speaker_hash] = " ".join(child.cdata.split())
+                    speaker_note_id = child["xml:id"]
+
+                    if not speaker_note_id:
+                        raise ValueError("no xml:id in speaker's note tag")
+
+                    self.speaker_notes[speaker_note_id] = " ".join(child.cdata.split())
+
+                    previous_who: str = None
+
             elif child.name == 'u':
+
+                who: str = child.get_attribute('who')
+
+                if previous_who and previous_who != who:
+                    speaker_note_id = MISSING_SPEAKER_NOTE_ID
+
+                previous_who: str = who
+
                 utterances.append(
-                    UtteranceMapper.create(element=child, page_number=page_number, speaker_hash=speaker_hash)
+                    UtteranceMapper.create(
+                        element=child,
+                        page_number=page_number,
+                        speaker_note_id=speaker_note_id,
+                    )
                 )
-            # else:
-            #     speaker_hash = None
+
         return utterances
 
     def get_date(self) -> str:
         try:
             docDate = self.data.teiCorpus.TEI.text.front.div.docDate
             return docDate[0]['when'] if isinstance(docDate, list) else docDate['when']
         except (AttributeError, KeyError):
@@ -138,20 +166,20 @@
     """Wraps a single ParlaClarin XML utterance tag."""
 
     @staticmethod
     def create(
         *,
         element: untangle.Element,
         page_number: str,
-        speaker_hash: str,
+        speaker_note_id: str,
         dedent: bool = True,
     ) -> interface.Utterance:
         utterance: interface.Utterance = interface.Utterance(
             u_id=element.get_attribute('xml:id'),
-            speaker_hash=speaker_hash,
+            speaker_note_id=speaker_note_id,
             who=element.get_attribute('who') or "undefined",
             page_number=page_number,
             prev_id=element.get_attribute('prev'),
             next_id=element.get_attribute('next'),
             paragraphs=UtteranceMapper.to_paragraphs(element, dedent),
             n=element.get_attribute('n'),
         )
@@ -226,17 +254,18 @@
 
         def create_iterator(self) -> Iterable[interface.Utterance]:
 
             context = ET.iterparse(self.filename, events=("start", "end"))
 
             context = iter(context)
             current_page: int = 0
-            current_utterance: dict = None
-            speaker_hash: str = ''
+            current_utterance: interface.Utterance = None
+            speaker_note_id: str = MISSING_SPEAKER_NOTE_ID
             is_preface: bool = False
+            previous_who: str = None
 
             for event, elem in context:
 
                 tag = elem.tag.rpartition('}')[2]
                 value = elem.text
 
                 if event == 'start':
@@ -244,47 +273,55 @@
                     if tag == 'head' and is_preface:
                         self.doc_name = value
 
                     elif tag == 'docDate' and is_preface:
                         self.doc_date = elem.attrib.get('when')
 
                     elif tag == "note" and elem.attrib.get('type') == "speaker":
-                        speaker_hash = elem.attrib['n']
-                        if speaker_hash:
+                        speaker_note_id = elem.attrib.get(XML_ID)
+                        previous_who: str = None
+                        if not speaker_note_id:
+                            raise ValueError("no xml:id in speaker's note")
+                        if speaker_note_id:
                             if value:
-                                self.speaker_notes[speaker_hash] = " ".join(value.split())
+                                self.speaker_notes[speaker_note_id] = " ".join(value.split())
                             else:
                                 pass
 
                     elif tag == "pb":
                         current_page = elem.attrib['n']
 
                     elif tag == "u":
                         is_preface = False
+                        who: str = elem.attrib.get('who')
+                        if previous_who and previous_who != who:
+                            speaker_note_id = MISSING_SPEAKER_NOTE_ID
+
                         current_utterance: interface.Utterance = interface.Utterance(
                             page_number=current_page,
-                            speaker_hash=speaker_hash,
-                            u_id=elem.attrib.get('{http://www.w3.org/XML/1998/namespace}id'),
+                            speaker_note_id=speaker_note_id,
+                            u_id=elem.attrib.get(XML_ID),
                             who=elem.attrib.get('who'),
                             prev_id=elem.attrib.get('prev'),
                             next_id=elem.attrib.get('next'),
                             n=elem.attrib.get('n'),
                             paragraphs=[],
                         )
-                        # speaker_hash = None
+                        previous_who = elem.attrib.get('who')
+                        # speaker_note_id = None
                     elif tag == "seg" and value is not None:
                         value = (dedent_text(value) if self.dedent else value).strip()
                         if value:
                             current_utterance.paragraphs.append(value)
 
                     elif tag == 'div' and elem.attrib.get('type') == 'preface':
                         is_preface = True
 
                     # else:
-                    #     speaker_hash = None
+                    #     speaker_note_id = None
 
                 elif event == 'end':
 
                     if tag == "seg" and value is not None:
                         value = (dedent_text(value) if self.dedent else value).strip()
                         if value:
                             current_utterance.paragraphs.append(value)
@@ -293,10 +330,10 @@
                         yield current_utterance
                         current_utterance = None
 
                     elif tag == 'div' and elem.attrib.get('type') == 'preface':
                         is_preface = False
 
                     # elif tag == "note" and elem.attrib.get('type') == "speaker":
-                    #     self.speaker_notes[speaker_hash] = " ".join(value.split())
+                    #     self.speaker_notes[speaker_note_id] = " ".join(value.split())
 
                 elem.clear()
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/parlaclarin/tf.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/tagged/iterate.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/tagged/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/corpus/tagged/persist.py` & `pyriksprot-2022.5.2/pyriksprot/corpus/tagged/persist.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,17 +137,17 @@
         return False
     metadata: dict = load_metadata(filename)
     if metadata is None:
         return False
     return checksum == metadata.get('checksum', 'oo')
 
 
-def update_speaker_hash(speaker_hash_lookup: dict[str, str], source_folder: str, target_folder: str):
-    """Updates `speaker_hash` in an existing PoS-tagged corpus
-    speaker_hash_lookup = SpeakerInfoService(database_filename).utterance_index.utterances['speaker_hash'].to_dict()
+def update_speaker_note_id(speaker_note_id_lookup: dict[str, str], source_folder: str, target_folder: str):
+    """Updates speaker's note's xml:id in an existing PoS-tagged corpus
+    speaker_note_id_lookup = SpeakerInfoService(database_filename).utterance_index.utterances['speaker_note_id'].to_dict()
     """
 
     os.makedirs(target_folder, exist_ok=True)
 
     for filename in tqdm(glob.glob(jj(source_folder, "**/*.zip"), recursive=True)):
         target_filename: str = jj(target_folder, relpath(filename, source_folder))
         ensure_path(target_filename)
@@ -157,14 +157,14 @@
                 protocol_str = fp.read(json_name).decode('utf-8')
                 metadata_str = fp.read("metadata.json").decode('utf-8')
         except zipfile.BadZipFile:
             touch(target_filename)
             continue
         protocol: list[dict] = json.loads(protocol_str)
         for u in protocol:
-            speaker_hash: str = speaker_hash_lookup.get(u['u_id'])
-            if speaker_hash:
-                u['speaker_hash'] = speaker_hash
+            speaker_note_id: str = speaker_note_id_lookup.get(u['u_id'])
+            if speaker_note_id:
+                u['speaker_note_id'] = speaker_note_id
         utterances_csv_str: str = json.dumps(protocol)
         with zipfile.ZipFile(target_filename, "w", compression=zipfile.ZIP_DEFLATED) as fp:
             fp.writestr(json_name, utterances_csv_str or "")
             fp.writestr("metadata.json", metadata_str or "")
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/dehyphenation/flair_dehyphen.py` & `pyriksprot-2022.5.2/pyriksprot/dehyphenation/flair_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/dehyphenation/swe_dehyphen.py` & `pyriksprot-2022.5.2/pyriksprot/dehyphenation/swe_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/dispatch/dispatch.py` & `pyriksprot-2022.5.2/pyriksprot/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/dispatch/item.py` & `pyriksprot-2022.5.2/pyriksprot/dispatch/item.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/dispatch/merge.py` & `pyriksprot-2022.5.2/pyriksprot/dispatch/merge.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/dispatch/utility.py` & `pyriksprot-2022.5.2/pyriksprot/dispatch/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/foss/bettertokenizer.sv` & `pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens` & `pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/foss/pos_tags.py` & `pyriksprot-2022.5.2/pyriksprot/foss/pos_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/foss/sparv_tokenize.py` & `pyriksprot-2022.5.2/pyriksprot/foss/sparv_tokenize.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/foss/stopwords.py` & `pyriksprot-2022.5.2/pyriksprot/foss/stopwords.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/foss/untangle.py` & `pyriksprot-2022.5.2/pyriksprot/foss/untangle.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/interface.py` & `pyriksprot-2022.5.2/pyriksprot/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from enum import Enum
 from io import StringIO
 from typing import Any, Callable, Mapping, Optional, Union
 
 import pandas as pd
 from pandas.io import json
 
+from pyriksprot.corpus.parlaclarin.parse import MISSING_SPEAKER_NOTE_ID
+
 from .utility import flatten, merge_tagged_csv, strip_extensions
 
 # pylint: disable=too-many-arguments, no-member
 
-EMPTY_SPEAKER_HASH: str = "unknown"
-
 
 class ParlaClarinError(ValueError):
     ...
 
 
 class TemporalKey(str, Enum):
     NONE = None
@@ -99,42 +99,44 @@
 
     delimiter: str = '\n'
 
     def __init__(
         self,
         *,
         u_id: str,
-        speaker_hash: str,
+        speaker_note_id: str,
         who: str,
         n: str = "",
         prev_id: str = None,
         next_id: str = None,
         paragraphs: Union[list[str], str] = None,
         annotation: Optional[str] = None,
         page_number: Optional[str] = '',
         **_,
     ):
 
-        if not speaker_hash:
-            speaker_hash = EMPTY_SPEAKER_HASH
-            # FIXME #15 Exists utterances in data not preceeded by a SPEAKER_HASH
-            # logger.warning(f"utterance {u_id}: empty speaker_hash")
-            # raise ValueError(f"utterance {u_id}: empty speaker_hash not allowed")
+        if not speaker_note_id:
+            speaker_note_id = MISSING_SPEAKER_NOTE_ID
+            # FIXME #15 Exists utterances in data not preceeded by a speakers's intro note
+            # logger.warning(f"utterance {u_id}: empty speaker_note_id")
+            # raise ValueError(f"utterance {u_id}: empty speaker_note_id not allowed")
 
         self.u_id: str = u_id
         self.n: str = n
         self.who: str = who
         self.prev_id: str = prev_id if isinstance(prev_id, str) else None
         self.next_id: str = next_id if isinstance(next_id, str) else None
         self.paragraphs: list[str] = (
             [] if not paragraphs else paragraphs if isinstance(paragraphs, list) else paragraphs.split(PARAGRAPH_MARKER)
         )
         self.annotation: Optional[str] = annotation if isinstance(annotation, str) else None
         self.page_number: Optional[str] = page_number if isinstance(page_number, str) else ''
-        self.speaker_hash: Optional[str] = speaker_hash if isinstance(speaker_hash, str) else ''
+        self.speaker_note_id: Optional[str] = (
+            speaker_note_id if isinstance(speaker_note_id, str) else MISSING_SPEAKER_NOTE_ID
+        )
 
     @property
     def is_unknown(self) -> bool:
         return self.who == "unknown"
 
     @property
     def document_name(self) -> str:
@@ -170,15 +172,15 @@
     def to_dict(utterances: list[Utterance]) -> list[Mapping[str, Any]]:
         """Convert list of utterances to a list of dicts. Return the list."""
         return [
             {
                 'u_id': u.u_id,
                 'n': u.n,
                 'who': u.who,
-                'speaker_hash': u.speaker_hash,
+                'speaker_note_id': u.speaker_note_id,
                 'prev_id': u.prev_id,
                 'next_id': u.next_id,
                 'annotation': u.tagged_text,
                 'paragraphs': PARAGRAPH_MARKER.join(u.paragraphs),
                 'page_number': u.page_number or '',
                 'checksum': u.checksum(),
             }
@@ -327,17 +329,17 @@
 
     @property
     def speech_name(self):
         """Generate a unique name for speech."""
         return f"{strip_extensions(self.document_name)}@{self.speech_index}"
 
     @property
-    def speaker_hash(self):
-        """Hash for preceeding speaker-note."""
-        return None if not self.utterances else self.utterances[0].speaker_hash
+    def speaker_note_id(self):
+        """xml:id for preceeding speaker-note."""
+        return MISSING_SPEAKER_NOTE_ID if not self.utterances else self.utterances[0].speaker_note_id
 
     def add(self, item: Utterance) -> "Speech":
         self.utterances.append(item)
         return self
 
 
 class Protocol(UtteranceMixIn):
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/metadata/codecs.py` & `pyriksprot-2022.5.2/pyriksprot/metadata/codecs.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/metadata/generate.py` & `pyriksprot-2022.5.2/pyriksprot/metadata/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     """IParser = parse.ProtocolMapper """
 
     @dataclass
     class IUtterance:
         u_id: str
         who: str
-        speaker_hash: str
+        speaker_note_id: str
 
     @dataclass
     class IProtocol:
         name: str
         date: str
         utterances: list[IParser.IUtterance]
 
@@ -97,44 +97,67 @@
         'party': 'text',
         'abbreviation': 'text',
         'ocr_correction': 'text',
     },
     'party_affiliation': {
         'person_id': 'text references person (person_id) not null',
         'party': 'text',
+        'start': 'int',
+        'end': 'int',
+        # ':loaded_hook:': _to_year_period
     },
     'person': {
         'person_id': 'text primary key',
         'born': 'int',
         'dead': 'int',
         'gender': 'text',
         'wiki_id': 'text',
         'riksdagen_guid': 'text',
         'riksdagen_id': 'text',
+        ':drop_duplicates:': 'person_id',
     },
     'speaker': {
         'person_id': 'text references person (person_id) not null',
         'role': 'text',
         'start': 'date',
         'end': 'date',
     },
     'twitter': {
         'twitter': 'text',  # primary key',
         'person_id': 'text references person (person_id) not null',
     },
     'unknowns': {
         'protocol_id': 'text',  # primary key',
-        'hash': 'text',
+        'uuid': 'text',
         'gender': 'text',
         'party': 'text',
         'other': 'text',
         ':url:': input_unknown_url,
     },
 }
 
+EXTRA_TABLES = {
+    'speech_index': {
+        'document_id': 'int primary key',
+        'document_name': 'text',
+        'year': 'int',
+        'who': 'text',
+        'gender_id': 'int',
+        'party_id': 'int',
+        'office_type_id': 'int',
+        'sub_office_type_id': 'int',
+        'n_tokens': 'int',
+        'filename': 'text',
+        'u_id': 'text',
+        'n_utterances': 'int',
+        'speaker_note_id': 'text',
+        'speach_index': 'int',
+    },
+}
+
 
 def register_numpy_adapters():
     for dt in [np.int8, np.int16, np.int32, np.int64]:
         sqlite3.register_adapter(dt, int)
     for dt in [np.float16, np.float32, np.float64]:
         sqlite3.register_adapter(dt, float)
     sqlite3.register_adapter(np.nan, lambda _: "'NaN'")
@@ -215,68 +238,77 @@
     unknowns.to_csv(jj(target_folder, "unknowns.csv"), sep=',', index=False)
 
 
 def fx_or_url(url: Any, tag: str) -> str:
     return url(tag) if callable(url) else url
 
 
+def sql_ddl_create(*, tablename: str, specification: dict[str, str]) -> str:
+    lf = '\n' + (12 * ' ')
+    sql_ddl: str = f"""
+        create table {tablename} (
+            {(','+lf).join(f"{k.removeprefix('+')} {t}" for k, t in specification.items() if not k.startswith(":"))}
+        );
+    """
+    return sql_ddl
+
+
+def sql_ddl_insert(*, tablename: str, columns: list[str]) -> str:
+    insert_sql = f"""
+    insert into {tablename} ({', '.join(columns)})
+        values ({', '.join(['?'] * len(columns))});
+    """
+    return insert_sql
+
+
 def create_database(
     database_filename: str,
     branch: str = None,
     folder: str = None,
     force: bool = False,
 ):
-    logger.info("Creating database.")
-    logger.info(f"  target: {database_filename}")
-    logger.info(f"     tag: {branch}")
-    logger.info(f"  folder: {folder}")
+    logger.info(f"Creating database {database_filename}, using source {branch}/{folder} (tag/folder).")
 
     os.makedirs(dirname(database_filename), exist_ok=True)
 
     if isfile(database_filename):
         if not force:
             raise ValueError("DB exists, use `force=True` to overwrite")
         os.remove(database_filename)
 
     db = sqlite3.connect(database_filename)
 
     register_numpy_adapters()
 
-    lf = '\n' + (12 * ' ')
-
     for tablename, specification in RIKSPROT_METADATA_TABLES.items():
-        sql_ddl: str = f"""
-            create table {tablename} (
-                {(','+lf).join(f"{k.removeprefix('+')} {t}" for k, t in specification.items() if not k.startswith(":"))}
-            );
-        """
         with closing(db.cursor()) as cursor:
-            cursor.executescript(sql_ddl)
+            cursor.executescript(sql_ddl_create(tablename=tablename, specification=specification))
 
     for tablename, specification in RIKSPROT_METADATA_TABLES.items():
         logger.info(f"loading table: {tablename}")
 
-        column_names: list[str] = [k for k in specification if k[0] not in "+:"]
-
         if ':url:' in specification and folder is None:
             table: pd.DataFrame = pd.read_csv(fx_or_url(specification[':url:'], branch), sep=',')
         else:
             table: pd.DataFrame = smart_load_table(tablename=tablename, folder=folder, branch=branch, sep=',')
 
+        if ':drop_duplicates:' in specification:
+            table = table.drop_duplicates(subset='person_id', keep='first')
+
+        # if ':loaded_hook:' in specification:
+        #     table = specification[':loaded_hook:'](table)
+
         for c in table.columns:
             if table.dtypes[c] == np.dtype('bool'):  # pylint: disable=no-member
                 table[c] = [int(x) for x in table[c]]
 
-        data = table[column_names].to_records(index=False)
-
         with closing(db.cursor()) as cursor:
-            insert_sql = f"""
-            insert into {tablename} ({', '.join(column_names)})
-                values ({', '.join(['?'] * len(column_names))});
-            """
+            columns: list[str] = [k for k in specification if k[0] not in "+:"]
+            data = table[columns].to_records(index=False)
+            insert_sql = sql_ddl_insert(tablename=tablename, columns=columns)
             cursor.executemany(insert_sql, data)
 
     db.commit()
     return db
 
 
 def generate_corpus_indexes(
@@ -292,25 +324,25 @@
     filenames = glob.glob(jj(corpus_folder, "protocols", "**/*.xml"), recursive=True)
     speaker_notes: dict[str, str] = {}
 
     for document_id, filename in tqdm(enumerate(filenames)):
         protocol: IParser.IProtocol = parser.to_protocol(filename, segment_skip_size=0, ignore_tags={"teiHeader"})
         protocol_data.append((document_id, protocol.name, protocol.date, int(protocol.date[:4])))
         for u in protocol.utterances:
-            utterance_data.append(tuple([document_id, u.u_id, u.who, u.speaker_hash]))
+            utterance_data.append(tuple([document_id, u.u_id, u.who, u.speaker_note_id]))
         speaker_notes.update(protocol.get_speaker_notes())
 
     data: tuple[pd.DataFrame, pd.DataFrame] = (
         pd.DataFrame(data=protocol_data, columns=['document_id', 'document_name', 'date', 'year']).set_index(
             "document_id"
         ),
-        pd.DataFrame(data=utterance_data, columns=['document_id', 'u_id', 'person_id', 'speaker_hash']).set_index(
+        pd.DataFrame(data=utterance_data, columns=['document_id', 'u_id', 'person_id', 'speaker_note_id']).set_index(
             "u_id"
         ),
-        pd.DataFrame(speaker_notes.items(), columns=['speaker_hash', 'speaker_note']).set_index('speaker_hash'),
+        pd.DataFrame(speaker_notes.items(), columns=['speaker_note_id', 'speaker_note']).set_index('speaker_note_id'),
     )
 
     if target_folder:
 
         os.makedirs(target_folder, exist_ok=True)
 
         for df, tablename in zip(data, ["protocols", "utterances", "speaker_notes"]):
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/metadata/person.py` & `pyriksprot-2022.5.2/pyriksprot/metadata/person.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/metadata/utility.py` & `pyriksprot-2022.5.2/pyriksprot/metadata/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/metadata/utterance.py` & `pyriksprot-2022.5.2/pyriksprot/metadata/utterance.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/metadata2db.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/metadata2db.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2speech.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2tagged.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2tagged.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/riksprot2text.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/speakerhash.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/fix_speaker_notes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import os
 import sys
 
 import click
 
 from pyriksprot import metadata as md
-from pyriksprot.corpus.tagged.persist import update_speaker_hash
+from pyriksprot.corpus.tagged.persist import update_speaker_note_id
 
 jj = os.path.join
 relpath = os.path.relpath
 
 # FIXME #20 Tagging does not assign correct speaker hashes to utterances
 def temporary_update(tag: str, target_tag: str):
 
     source_folder: str = f"/data/riksdagen_corpus_data/tagged_frames_{tag}"
     target_folder: str = f"/data/riksdagen_corpus_data/tagged_frames_{target_tag}"
     database_filename: str = f"/data/riksdagen_corpus_data/metadata/riksprot_metadata.{tag}.db"
 
     service = md.SpeakerInfoService(database_filename)
-    speaker_hash_lookup = service.utterance_index.utterances['speaker_hash'].to_dict()
-    update_speaker_hash(speaker_hash_lookup, source_folder, target_folder)
+    speaker_note_id_lookup = service.utterance_index.utterances['speaker_note_id'].to_dict()
+    update_speaker_note_id(speaker_note_id_lookup, source_folder, target_folder)
 
 
 @click.command()
 @click.argument('source-folder', type=click.STRING)
 @click.argument('target-folder', type=click.STRING)
 @click.argument('database-filename', type=click.STRING)
 def main(source_folder: str = None, target_folder: str = None, database_filename: str = None):
+    """Updates missing or wrong speaker note identities in an exist speech corpus (stored as zipped JSON files)"""
     try:
         service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename)
-        speaker_hash_lookup: dict[str, str] = service.utterance_index.utterances['speaker_hash'].to_dict()
-        update_speaker_hash(speaker_hash_lookup, source_folder, target_folder)
+        speaker_note_id_lookup: dict[str, str] = service.utterance_index.utterances['speaker_note_id'].to_dict()
+        update_speaker_note_id(speaker_note_id_lookup, source_folder, target_folder)
     except Exception as ex:
         click.echo(ex)
         sys.exit(1)
 
 
 if __name__ == "__main__":
     # main()
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/speech_index.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/speech_index.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,24 @@
 from __future__ import annotations
 
 import os
 import sys
-import typing as t
 
 import click
-import pandas as pd
-from loguru import logger
-from tqdm import tqdm
-
-from pyriksprot import interface
-from pyriksprot import metadata as md
-from pyriksprot import to_speech
-from pyriksprot.corpus import corpus_index, iterate, tagged
+
+from pyriksprot import interface, to_speech
 from pyriksprot.scripts.utils import option2, update_arguments_from_options_file
+from pyriksprot.workflows.speech_index import extract_speech_index
 
 jj = os.path.join
 relpath = os.path.relpath
 
 # pylint: disable=too-many-arguments, W0613
 
 
-def extract_speech_index(
-    *,
-    source_folder: str,
-    database_filename: str,
-    target_name: str,
-    content_type: interface.ContentType = interface.ContentType.TaggedFrame,
-    segment_level: interface.SegmentLevel = None,
-    segment_skip_size: int = 1,
-    years: str = None,
-    multiproc_keep_order: str = None,
-    multiproc_processes: int = 1,
-    multiproc_chunksize: int = 100,
-    merge_strategy: to_speech.MergeStrategyType = 'chain',
-) -> None:
-
-    logger.info("extracting corpus speech index...")
-
-    source_index: corpus_index.CorpusSourceIndex = corpus_index.CorpusSourceIndex.load(
-        source_folder=source_folder, source_pattern='**/prot-*.zip', years=years
-    )
-    logger.info("loading parliamentary metadata...")
-
-    # FIXME: How to ensure metadata tag is the same as corpus??? Add tag to DB?
-    speaker_service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename=database_filename)
-
-    def get_speaker(item: iterate.ProtocolSegment) -> None:
-        item.speaker_info = speaker_service.get_speaker_info(u_id=item.u_id, person_id=item.who, year=item.year)
-
-    preprocess: t.Callable[[iterate.ProtocolSegment], None] = (
-        get_speaker if segment_level not in ('protocol', None) else None
-    )
-
-    speeches: iterate.ProtocolSegmentIterator = tagged.ProtocolIterator(
-        filenames=source_index.paths,
-        content_type=content_type,
-        segment_level=segment_level,
-        segment_skip_size=segment_skip_size,
-        multiproc_keep_order=multiproc_keep_order,
-        multiproc_processes=multiproc_processes,
-        multiproc_chunksize=multiproc_chunksize,
-        merge_strategy=merge_strategy,
-        preprocess=preprocess,
-    )
-
-    data: list[dict] = []
-    for speech in tqdm(speeches):
-        data.append(speech.to_dict())
-
-    pd.DataFrame(data=data).to_csv('speech_index.csv.gz', sep='\t')
-
-
 @click.command()
 @click.argument('source-folder', type=click.STRING)
 @click.argument('target-name', type=click.STRING)
 @click.argument('database-filename', type=click.STRING)
 @option2('--options-filename')
 @option2('--merge-strategy')
 @option2('--multiproc-processes')
@@ -83,14 +26,15 @@
     options_filename: str = None,
     source_folder: str = None,
     target_name: str = None,
     database_filename: str = None,
     merge_strategy: str = 'chain',
     multiproc_processes: int = 1,
 ):
+    """Extracts a speech index from given speech corpus"""
     arguments: dict = update_arguments_from_options_file(arguments=locals(), filename_key='options_filename')
     arguments['merge_strategy'] = to_speech.MergeStrategyType(arguments['merge_strategy'])
 
     try:
         extract_speech_index(
             **arguments,
             **dict(
@@ -107,15 +51,15 @@
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
 
     # arguments = {
-    #     'source_folder': '/data/riksdagen_corpus_data/tagged_frames_v0.4.1',
+    #     'source_folder': '/data/riksdagen_corpus_data/tagged_frames_vx.x.x',
     #     'target_name': 'speech_index.csv.gz',
     #     'database_filename': '/data/riksdagen_corpus_data/metadata/riksprot_metadata.main.db',
     #     'merge_strategy': 'chain',
     #     'multiproc_processes': None,
     #     'segment_skip_size': 0,
     #     'years': None,
     #     'content_type': "tagged_frame",
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/scripts/utils.py` & `pyriksprot-2022.5.2/pyriksprot/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/to_speech.py` & `pyriksprot-2022.5.2/pyriksprot/to_speech.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # pylint: disable=too-many-arguments, no-member
 
 
 class MergeStrategyType(str, Enum):
     who = 'who'
     who_sequence = 'who_sequence'
     chain = 'chain'
-    who_speaker_hash_sequence = 'who_speaker_hash_sequence'
-    speaker_hash_sequence = 'speaker_hash_sequence'
+    who_speaker_note_id_sequence = 'who_speaker_note_id_sequence'
+    speaker_note_id_sequence = 'speaker_note_id_sequence'
     undefined = 'undefined'
 
 
 def to_speeches(
     *, protocol: Protocol, merge_strategy: MergeStrategyType | Type[IMergeStrategy], skip_size: int = 1
 ) -> list[Speech]:
 
@@ -74,28 +74,28 @@
     """Merge sequences with same `who` into a speech """
 
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         groups: list[list[Utterance]] = [list(g) for _, g in groupby(utterances or [], key=lambda x: x.who)]
         return groups
 
 
-class MergeBySpeakerHashSequence(IMergeStrategy):
-    """Merge sequences with same `who` into a speech """
+class MergeBySpeakerNoteIdSequence(IMergeStrategy):
+    """Merge sequences with same `speaker_note_id` into a speech """
 
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
-        groups: list[list[Utterance]] = [list(g) for _, g in groupby(utterances or [], key=lambda x: x.speaker_hash)]
+        groups: list[list[Utterance]] = [list(g) for _, g in groupby(utterances or [], key=lambda x: x.speaker_note_id)]
         return groups
 
 
-class MergeByWhoSpeakerHashSequence(IMergeStrategy):
-    """Merge sequences with same `who` into a speech """
+class MergeByWhoSpeakerNoteIdSequence(IMergeStrategy):
+    """Merge sequences with same `who` & 'speaker_note_id' into a speech """
 
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         groups: list[list[Utterance]] = [
-            list(g) for _, g in groupby(utterances or [], key=lambda x: f"{x.who}_{x.speaker_hash}")
+            list(g) for _, g in groupby(utterances or [], key=lambda x: f"{x.who}_{x.speaker_note_id}")
         ]
         return groups
 
 
 class MergeByChain(IMergeStrategy):
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         groups: list[list[Utterance]] = MergeByChain.group_utterances_by_chain(utterances)
@@ -117,15 +117,17 @@
             """
 
             if bool(u.prev_id) and bool(u.next_id):
                 raise ValueError(f"logic error: {u.u_id} has both prev/next attrbutes set")
 
             is_part_of_chain: bool = bool(u.prev_id) or bool(u.next_id)
             is_unknown_continuation: bool = (
-                bool(speech) and u.who == "unknown" == speech[-1].who and u.speaker_hash == speech[-1].speaker_hash
+                bool(speech)
+                and u.who == "unknown" == speech[-1].who
+                and u.speaker_note_id == speech[-1].speaker_note_id
             )
 
             start_of_speech: bool = (
                 True
                 if bool(u.next_id)
                 else not is_unknown_continuation
                 if not is_part_of_chain
@@ -164,16 +166,16 @@
 
 
 class MergerFactory:
 
     strategies: dict[MergeStrategyType, IMergeStrategy] = {
         'who': MergeByWho(),
         'who_sequence': MergeByWhoSequence(),
-        'who_speaker_hash_sequence': MergeByWhoSpeakerHashSequence(),
-        'speaker_hash_sequence': MergeBySpeakerHashSequence(),
+        'who_speaker_note_id_sequence': MergeByWhoSpeakerNoteIdSequence(),
+        'speaker_note_id_sequence': MergeBySpeakerNoteIdSequence(),
         'chain': MergeByChain(),
         'undefined': UndefinedMerge(),
     }
 
     @staticmethod
     def get(strategy: str | Type[IMergeStrategy]) -> IMergeStrategy:
         return (
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/utility.py` & `pyriksprot-2022.5.2/pyriksprot/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
 def store_dict(data: dict, filename: str):
     with open(filename, 'wb') as fp:
         pickle.dump(data, fp, pickle.HIGHEST_PROTOCOL)
 
 
 def load_dict(filename: str) -> defaultdict(int):
-    logger.info(f"loading {filename}")
+    # logger.info(f"loading {filename}")
     if isfile(filename):
         with open(filename, 'rb') as fp:
             return pickle.load(fp)
     return defaultdict(int)
 
 
 @contextlib.contextmanager
@@ -265,15 +265,15 @@
 def unlink(f: str) -> None:
 
     fo = pathlib.Path(f)
 
     if fo.is_dir():
         shutil.rmtree(f)
 
-    if fo.is_file():
+    elif fo.is_file():
         fo.unlink(missing_ok=True)
 
 
 def touch(f: str) -> None:
     pathlib.Path(f).touch()
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/workflows/extract_tags.py` & `pyriksprot-2022.5.2/pyriksprot/workflows/extract_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/workflows/extract_text.py` & `pyriksprot-2022.5.2/pyriksprot/workflows/extract_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/pyriksprot/workflows/tag.py` & `pyriksprot-2022.5.2/pyriksprot/workflows/tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from __future__ import annotations
+
 import abc
 import itertools
 from functools import reduce
+from glob import glob
+from os.path import getmtime, isfile, join
 from typing import Any, Callable, List, Mapping, Union
 
 from loguru import logger
+from tqdm import tqdm
 
 from pyriksprot.corpus.parlaclarin import parse
 from pyriksprot.corpus.tagged import persist
 
 from .. import interface
 from ..utility import ensure_path, strip_path_and_extension, touch, unlink
 
@@ -116,18 +121,41 @@
         checksum: str = protocol.checksum()
 
         # print(f"checksum: {checksum}")
         # print(f"   force: {force}")
         # print(f"filename: {os.path.abspath(output_filename)}  {os.path.isfile(os.path.abspath(output_filename))}")
 
         if not force and persist.validate_checksum(output_filename, checksum):
-            logger.info(f"SKIPPING {strip_path_and_extension(input_filename)} (checksum validates OK)")
+            logger.info(f"skipped: {strip_path_and_extension(input_filename)} (checksum validates OK)")
             touch(output_filename)
         else:
             unlink(output_filename)
+            logger.info(f"tagging: {strip_path_and_extension(input_filename)}")
             protocol = tag_protocol(tagger, protocol=protocol)
             persist.store_protocol(output_filename, protocol=protocol, checksum=checksum, storage_format=storage_format)
 
     except Exception:
         logger.error(f"FAILED: {input_filename}")
         unlink(output_filename)
         raise
+
+
+def tag_protocols(tagger: ITagger, source_folder: str, target_folder: str, force: bool):
+    """Tags protocols in `source_folder`. Stores result in `target_folder`.
+    Note: not used by Snakemake workflow (used by tag CLI script)
+    """
+
+    source_files: list[str] = glob(join(source_folder, "prot-*.xml"))
+    for source_file in tqdm(source_files):
+        target_file = join(target_folder, f"{strip_path_and_extension(source_file)}.zip")
+        if force or expired(target_file, source_file):
+            tag_protocol_xml(source_file, target_file, tagger, storage_format="json", force=force)
+        else:
+            touch(target_file)
+
+
+def expired(filename: str, expiry_instance: float | str) -> bool:
+    if isfile(filename):
+        if isinstance(expiry_instance, str):
+            expiry_instance = getmtime(expiry_instance)
+        return expiry_instance > getmtime(filename)
+    return True
```

### Comparing `pyriksprot-2022.3.2/pyriksprot/workflows/tf.py` & `pyriksprot-2022.5.2/pyriksprot/workflows/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.3.2/setup.py` & `pyriksprot-2022.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 entry_points = \
 {'console_scripts': ['riksprot2any = pyriksprot.scripts.riksprot2any:main',
                      'riksprot2text = pyriksprot.scripts.riksprot2text:main',
                      'riksprot2tfs = pyriksprot.scripts.riksprot2tfs:main']}
 
 setup_kwargs = {
     'name': 'pyriksprot',
-    'version': '2022.3.2',
+    'version': '2022.5.2',
     'description': 'Python API for Riksdagens Protokoll',
     'long_description': '# Python package for reading and tagging Riksdagens Protokoll\n\nBatteries (tagger) not included.\n\n## Overview\n\nThis package is intended to cover the following use cases:\n\n### Extract "text documents" from the Parla-CLARIN XML files\n\nText can be extracted from the XML files at different granularity (paragraphs, utterance, speech, who, protocol). The text can be grouped (combined) into larger temporal blocks based on time (year, lustrum, decade or custom periods). Within each of these block the text in turn can be grouped by speaker attributes (who, party, gender).\n\nThe text extraction can done using the `riksprot2text` utility, which is a CLI interface installed with the package, or in Python code using the API that this package exposes. The Python API exposed both streaming (SAX based) methods and a domain model API (i.e. Python classes representing protocols, speeches and utterances).\n\nBoth the CLI and the API supports dehyphenation using method described in [Anföranden: Annotated and Augmented Parliamentary Debates from Sweden, Stian Rødven Eide, 2020](https://gup.ub.gu.se/publication/302449). The API also supports user defined text transformations.\n\n### Extract PoS-tagged versions of the Parla-CLARIN XML files\n\nPart-of-speech tagged versions of the protocols can be extracted with the same granularity and aggregation as described above for the raw text. The returned documents are tab-separated files with fields for text, baseform and pos-tag (UPOS, XPOS). Note that the actual part-of-speech tagging is done using tools found in the `pyriksprot_tagging` repository ([link](https://github.com/welfare-state-analytics/westac_parlaclarin_pipeline)).\n\nCurrently there are no open-source tagged versions of the corpos avaliable. The tagging is done using [Stanza](https://stanfordnlp.github.io/stanza/) with Swedish language models produced and made publically avaliable by Språkbanken Text.\n\n### Store extracted text\n\nThe extracted text can be stored as optionally compressed plain text files on disk, or in a ZIP-archive.\n\n## Pre-requisites\n\n- Python >=3.8\n- A folder containing the Riksdagen Protokoll (parliamentary protocols) Github repository.\n\n```bash\ncd some-folder \\\ngit clone --branch "tag" tags/"tag" --depth 1 https://github.com/welfare-state-analytics/riksdagen-corpus.git\ncd riksdagen-corpus\ngit config core.quotepath off\n\n```\n\n## Installation (Linux)\n\nCreate an new isolated virtual environment for pyriksprot:\n\n```bash\nmkdir /path/to/new/pyriksprot-folder\ncd /path/to/new/pyriksprot-folder\npython -m venv .venv\n```\n\nActivate the environment:\n\n```bash\ncd /path/to/new/pyriksprot-folder\nsource .venv/bin/activate\n```\n\nInstall `pyriksprot` in activated virtual environment.\n\n```bash\npip install pyriksprot\n```\n\n## CLI riksprot2text:  Extract aggregated text corpus from Parla-CLARIN XML files\n\n```bash\n\nλ riksprot2text --help\n\nUsage: riksprot2text [OPTIONS] SOURCE_FOLDER TARGET\n\nOptions:\n  -m, --mode [plain|zip|gzip|bz2|lzma]\n                                  Target type\n  -t, --temporal-key TEXT         Temporal partition key(s)\n  -y, --years TEXT                Years to include in output\n  -g, --group-key TEXT            Partition key(s)\n  -p, --processes INTEGER RANGE   Number of processes to use\n  -l, --segment-level [protocol|speech|utterance|paragraph|who]\n                                  Protocol extract segment level\n  -e, --keep-order                Keep output in filename order (slower, multiproc)\n\n  -s, --skip-size INTEGER RANGE   Skip blocks of char length less than\n  -d, --dedent                    Remove indentation\n  -k, --dehyphen                  Dehyphen text\n  --help                          Show this message and exit.\n\n```\n\n### Examples CLI\n\nAggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.\n\n```python\nriksprot2text /path/to/corpus output.zip -m zip -t year -l protocol -g who --skip-size 50\n```\n\nAggregate text per decade grouped by speaker. Store result in a single zip. Remove indentations and hyphenations.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t decade -l who -g who --dedent --dehyphen\n```\n\nAggregate text using customized temporal periods and grouped by party.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t "1920-1938,1929-1945,1946-1989,1990-2020" -l who -g party\n```\n\nAggregate text per document and group by gender and party.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t protocol -l who -g party -g gender\n```\n\nAggregate text per year grouped by gender and party and include only 1946-1989.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t year -l who -g party -g gender -y 1946-1989\n```\n\n## Python API - Iterate XML protocols\n\nAggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.\n\n<!--pytest-codeblocks:skip-->\n```python\nimport pyriksprot\n\ntarget_filename: str = f\'output.zip\'\nopts = {\n    \'source_folder\': \'/path/to/corpus\',\n    \'target\': \'outout.zip\',\n    \'target_type\': \'files-in-zip\',\n    \'segment_level\': SegmentLevel.Who,\n    \'dedent\': True,\n    \'dehyphen\': False,\n    \'years\': \'1955-1965\',\n    \'temporal_key\': TemporalKey.Protocol,\n    \'group_keys\': (GroupingKey.Party, GroupingKey.Gender),\n}\n\npyriksprot.extract_corpus_text(**opts)\n\n```\n\n\nIterate over protocol and speaker:\n\n```python\n\nfrom pyriksprot import interface, iterstors\n\nitems: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(\n    filenames=filenames, segment_level=SegmentLevel.Who, segment_skip_size=0, processes=4\n)\n\nfor item in items:\n    print(item.who, len(item.text))\n\n```\n\nIterate over protocol and speech, skip empty:\n\n```python\n\nfrom pyriksprot import interface, iterstors\n\nitems: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(\n    filenames=filenames, segment_level=SegmentLevel.Who, segment_skip_size=1, processes=4\n)\n\nfor item in items:\n    print(item.who, len(item.text))\n\n```\n\nIterate over protocol and speech, apply preprocess function(s):\n\n```python\n\nfrom pyriksprot import interface, iterstors\nimport ftfy  # pip install ftfy\nimport unidecode\n\nfix_text: Callable[[str], str] = pyriksprot.compose(\n    [str.lower, pyriksprot.dedent, ftfy.fix_character_width, unidecode.unidecode ]\n)\nitems: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(\n    filenames=filenames, segment_level=SegmentLevel.Speech, segment_skip_size=1, processes=4, preprocessor=fix_text,\n)\n\nfor item in items:\n    print(item.who, len(item.text))\n\n```\n\n## Python API - Iterate protocols as domain entities\n\n## CLI riksprot2tags:  Extract aggregated part-of-speech tagged corpus\n',
     'author': 'Roger Mähler',
     'author_email': 'roger.mahler@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://westac.se',
```

### Comparing `pyriksprot-2022.3.2/PKG-INFO` & `pyriksprot-2022.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot
-Version: 2022.3.2
+Version: 2022.5.2
 Summary: Python API for Riksdagens Protokoll
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: ==3.9.10
 Classifier: License :: OSI Approved :: Apache Software License
```

