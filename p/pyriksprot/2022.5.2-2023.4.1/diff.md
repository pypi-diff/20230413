# Comparing `tmp/pyriksprot-2022.5.2.tar.gz` & `tmp/pyriksprot-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot-2022.5.2.tar", max compression
+gzip compressed data, was "pyriksprot-2023.4.1.tar", max compression
```

## Comparing `pyriksprot-2022.5.2.tar` & `pyriksprot-2023.4.1.tar`

### file list

```diff
@@ -1,67 +1,90 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2022.5.2/LICENSE
--rw-r--r--   0        0        0     6675 2022-03-14 19:05:38.857587 pyriksprot-2022.5.2/README.md
--rw-r--r--   0        0        0     3365 2022-05-11 05:27:50.057256 pyriksprot-2022.5.2/pyproject.toml
--rw-r--r--   0        0        0     1377 2022-05-08 09:29:23.979544 pyriksprot-2022.5.2/pyriksprot/__init__.py
--rw-r--r--   0        0        0      112 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/__init__.py
--rw-r--r--   0        0        0     3621 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/corpus_index.py
--rw-r--r--   0        0        0    10663 2022-05-05 14:02:18.800048 pyriksprot-2022.5.2/pyriksprot/corpus/iterate.py
--rw-r--r--   0        0        0      326 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/__init__.py
--rw-r--r--   0        0        0     3503 2022-05-05 14:02:18.800048 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/convert.py
--rw-r--r--   0        0        0     3651 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/iterate.py
--rw-r--r--   0        0        0    11197 2022-05-10 09:30:30.108299 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/parse.py
--rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/__init__.py
--rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
--rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
--rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
--rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
--rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
--rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
--rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
--rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
--rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
--rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/tf.py
--rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/tagged/__init__.py
--rw-r--r--   0        0        0     1556 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/corpus/tagged/iterate.py
--rw-r--r--   0        0        0     5797 2022-05-05 14:02:18.800048 pyriksprot-2022.5.2/pyriksprot/corpus/tagged/persist.py
--rw-r--r--   0        0        0      141 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/dehyphenation/__init__.py
--rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/dehyphenation/flair_dehyphen.py
--rw-r--r--   0        0        0     7891 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/dehyphenation/swe_dehyphen.py
--rw-r--r--   0        0        0      403 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/__init__.py
--rw-r--r--   0        0        0    16531 2022-03-31 11:43:17.389668 pyriksprot-2022.5.2/pyriksprot/dispatch/dispatch.py
--rw-r--r--   0        0        0     2098 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/item.py
--rw-r--r--   0        0        0     5844 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/merge.py
--rw-r--r--   0        0        0     2127 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/dispatch/utility.py
--rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/README.md
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/__init__.py
--rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv
--rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
--rw-r--r--   0        0        0    12240 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/foss/pos_tags.py
--rw-r--r--   0        0        0     7548 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/sparv_tokenize.py
--rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/stopwords.py
--rw-r--r--   0        0        0     6129 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/foss/untangle.py
--rw-r--r--   0        0        0    11716 2022-05-09 14:28:04.150091 pyriksprot-2022.5.2/pyriksprot/interface.py
--rw-r--r--   0        0        0      494 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/__init__.py
--rw-r--r--   0        0        0     4720 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/codecs.py
--rw-r--r--   0        0        0    13692 2022-05-07 15:02:41.744714 pyriksprot-2022.5.2/pyriksprot/metadata/generate.py
--rw-r--r--   0        0        0    11888 2022-03-31 11:43:17.389668 pyriksprot-2022.5.2/pyriksprot/metadata/person.py
--rw-r--r--   0        0        0     5176 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/utility.py
--rw-r--r--   0        0        0     1557 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/metadata/utterance.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2022.5.2/pyriksprot/scripts/__init__.py
--rw-r--r--   0        0        0     1648 2022-05-06 13:38:30.301815 pyriksprot-2022.5.2/pyriksprot/scripts/fix_speaker_notes.py
--rw-r--r--   0        0        0     2359 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/metadata2db.py
--rw-r--r--   0        0        0     2579 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2speech.py
--rw-r--r--   0        0        0     2779 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2tagged.py
--rw-r--r--   0        0        0     2123 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2text.py
--rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2tfs.py
--rw-r--r--   0        0        0     2176 2022-05-06 13:08:46.764962 pyriksprot-2022.5.2/pyriksprot/scripts/speech_index.py
--rw-r--r--   0        0        0     4795 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/scripts/utils.py
--rw-r--r--   0        0        0     6493 2022-05-09 08:27:29.314102 pyriksprot-2022.5.2/pyriksprot/to_speech.py
--rw-r--r--   0        0        0    15777 2022-05-09 13:51:49.761315 pyriksprot-2022.5.2/pyriksprot/utility.py
--rw-r--r--   0        0        0      196 2022-05-08 09:29:48.639724 pyriksprot-2022.5.2/pyriksprot/workflows/__init__.py
--rw-r--r--   0        0        0     6369 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/workflows/extract_tags.py
--rw-r--r--   0        0        0     4805 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/workflows/extract_text.py
--rw-r--r--   0        0        0     3160 2022-05-06 13:38:30.317816 pyriksprot-2022.5.2/pyriksprot/workflows/speech_index.py
--rw-r--r--   0        0        0     5411 2022-05-08 10:53:49.052959 pyriksprot-2022.5.2/pyriksprot/workflows/tag.py
--rw-r--r--   0        0        0     4056 2022-03-31 10:06:39.806371 pyriksprot-2022.5.2/pyriksprot/workflows/tf.py
--rw-r--r--   0        0        0     8333 2022-05-11 05:27:51.333917 pyriksprot-2022.5.2/setup.py
--rw-r--r--   0        0        0     7604 2022-05-11 05:27:51.334318 pyriksprot-2022.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.1/LICENSE
+-rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.1/README.md
+-rw-r--r--   0        0        0     3406 2023-04-13 12:57:03.282516 pyriksprot-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1163 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/__init__.py
+-rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/corpus/__init__.py
+-rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/corpus_index.py
+-rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/iterate.py
+-rw-r--r--   0        0        0      243 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/__init__.py
+-rw-r--r--   0        0        0     3526 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/convert.py
+-rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/iterate.py
+-rw-r--r--   0        0        0     5365 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/parse.py
+-rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/__init__.py
+-rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
+-rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
+-rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
+-rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
+-rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
+-rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
+-rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
+-rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
+-rw-r--r--   0        0        0     2266 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/tf.py
+-rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/corpus/tagged/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/tagged/iterate.py
+-rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/tagged/persist.py
+-rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/corpus/utility.py
+-rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/dehyphenation/__init__.py
+-rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/dehyphenation/flair_dehyphen.py
+-rw-r--r--   0        0        0     7718 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dehyphenation/swe_dehyphen.py
+-rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/dehyphenation/utility.py
+-rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.1/pyriksprot/dispatch/__init__.py
+-rw-r--r--   0        0        0    21549 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dispatch/dispatch.py
+-rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/dispatch/item.py
+-rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dispatch/merge.py
+-rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/dispatch/utility.py
+-rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/README.md
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/__init__.py
+-rw-r--r--   0        0        0     2335 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv
+-rw-r--r--   0        0        0      945 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv.saldo-tokens
+-rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/foss/pos_tags.py
+-rw-r--r--   0        0        0     7546 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/foss/sparv_tokenize.py
+-rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/foss/stopwords.py
+-rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/foss/untangle.py
+-rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/gitchen.py
+-rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/interface.py
+-rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/metadata/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/codecs.py
+-rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/config.py
+-rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/generate.py
+-rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/person.py
+-rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/repository.py
+-rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/subset.py
+-rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/utility.py
+-rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/utterance.py
+-rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/metadata/verify.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.1/pyriksprot/scripts/__init__.py
+-rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/csv2pgsql.py
+-rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/fix_speaker_notes.py
+-rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/metadata2db.py
+-rw-r--r--   0        0        0     2695 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech.py
+-rw-r--r--   0        0        0     3475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech_text.py
+-rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2tagged.py
+-rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2text.py
+-rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2tfs.py
+-rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/speaker_note2csv
+-rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/speech_index.py
+-rw-r--r--   0        0        0     1196 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/scripts/subset_corpus.py
+-rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/utils.py
+-rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.1/pyriksprot/scripts/xml2csv
+-rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/00_rename.sql
+-rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/01_data_updates.sql
+-rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/02_code_tables.sql
+-rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/03_persons_of_interest.sql
+-rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/04_terms_of_office.sql
+-rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/05_person_party.sql
+-rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/06_unknown.sql
+-rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/09_cleanup.sql
+-rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/sql/__init__.py
+-rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/to_speech.py
+-rw-r--r--   0        0        0    12385 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/utility.py
+-rw-r--r--   0        0        0      250 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/workflows/__init__.py
+-rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/_extract_speech_ids.py
+-rw-r--r--   0        0        0     4425 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/extract_speech_text.py
+-rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/extract_tags.py
+-rw-r--r--   0        0        0     4552 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/extract_text.py
+-rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.1/pyriksprot/workflows/speech_index.py
+-rw-r--r--   0        0        0     2230 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/subset_corpus.py
+-rw-r--r--   0        0        0     5313 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/tag.py
+-rw-r--r--   0        0        0     4137 2023-04-13 10:55:09.503216 pyriksprot-2023.4.1/pyriksprot/workflows/tf.py
+-rw-r--r--   0        0        0     8732 1970-01-01 00:00:00.000000 pyriksprot-2023.4.1/PKG-INFO
```

### Comparing `pyriksprot-2022.5.2/LICENSE` & `pyriksprot-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/README.md` & `pyriksprot-2023.4.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ### Store extracted text
 
 The extracted text can be stored as optionally compressed plain text files on disk, or in a ZIP-archive.
 
 ## Pre-requisites
 
-- Python >=3.8
+- Python >=3.11
 - A folder containing the Riksdagen Protokoll (parliamentary protocols) Github repository.
 
 ```bash
 cd some-folder \
 git clone --branch "tag" tags/"tag" --depth 1 https://github.com/welfare-state-analytics/riksdagen-corpus.git
 cd riksdagen-corpus
 git config core.quotepath off
@@ -80,16 +80,52 @@
   -e, --keep-order                Keep output in filename order (slower, multiproc)
 
   -s, --skip-size INTEGER RANGE   Skip blocks of char length less than
   -d, --dedent                    Remove indentation
   -k, --dehyphen                  Dehyphen text
   --help                          Show this message and exit.
 
+  λ metadata2db --help
+Usage: metadata2db.py [OPTIONS] COMMAND [ARGS]...
+
+  CLI tool to manage riksprot metadata
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  columns
+  database
+  download
+  filenames
+  index
+
+  λ metadata2db.py database --help
+Usage: metadata2db.py database [OPTIONS] TARGET
+
+Options:
+  --tag TEXT             Metadata version
+  --source-folder TEXT
+  --force                Force overwrite
+  --load-index           Load utterance index
+  --scripts-folder TEXT  Apply scripts in specified folder to DB. If not
+                         specified the scripts are loaded from SQL-module.
+  --skip-scripts         Skip loading SQL scripts
+  --help                 Show this message and exit.
+
+
+  λ metadata2db index --help
+Usage: metadata2db.py index [OPTIONS] CORPUS_FOLDER TARGET_FOLDER
+
+Options:
+  --help  Show this message and exit.
+
 ```
 
+
 ### Examples CLI
 
 Aggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.
 
 ```python
 riksprot2text /path/to/corpus output.zip -m zip -t year -l protocol -g who --skip-size 50
 ```
```

### Comparing `pyriksprot-2022.5.2/pyproject.toml` & `pyriksprot-2023.4.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 [tool.poetry]
 name = "pyriksprot"
-version = "2022.5.2"
+version = "2023.4.1"
 description = "Python API for Riksdagens Protokoll"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     'Topic :: Software Development',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.11',
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://westac.se"
 repository = "https://github.com/welfare-state-analytics/pyriksprot"
 
 [tool.poetry.dependencies]
-python = "==3.9.10"
+python = "==3.11.*"
 Jinja2 = "*"
 click = "*"
 pandas = "*"
 loguru = "*"
 lz4 = "*"
 pdoc = "*"
 requests = "*"
 tqdm = "*"
-Unidecode = "*"
 pyarrow = "*"
 more-itertools = "*"
 python-dotenv = "*"
+unidecode = "^1.3.6"
+pygit2 = "^1.11.1"
+sqlalchemy = "^2.0.6"
+psycopg2-binary = "^2.9.5"
 
 [tool.poetry.dev-dependencies]
-black = "==20.*,>=20.8.0.b1"
-coverage = "==5.*,>=5.4.0"
-flake8 = "==3.*,>=3.8.4"
-flake8-black = "==0.*,>=0.2.1"
-isort = "==5.*,>=5.7.0"
-mypy = "==0.*,>=0.812.0"
-pre-commit = "==2.*,>=2.10.1"
-pycodestyle = "==2.*,>=2.6.0"
-pyflakes = "==2.*,>=2.2.0"
-pylint = "==2.*,>=2.7.1"
-pytest = "==6.*,>=6.2.2"
-pytest-cov = "==2.*,>=2.11.1"
-pyinstrument = "^4.0.3"
-ipykernel = "^6.6.0"
-pytest-codeblocks = "^0.12.2"
+black = "*"
+coverage = "*"
+flake8 = "*"
+flake8-black = "*"
+isort = "*"
+pre-commit = "*"
+pycodestyle = "*"
+pyflakes = "*"
+pylint = "*"
+pytest = "*"
+pytest-cov = "*"
+pyinstrument = "*"
+pytest-codeblocks = "*"
 
 [tool.poetry.scripts]
 riksprot2any = "pyriksprot.scripts.riksprot2any:main"
 riksprot2tfs = "pyriksprot.scripts.riksprot2tfs:main"
 riksprot2text = "pyriksprot.scripts.riksprot2text:main"
+subset-corpus = "pyriksprot.scripts.subset_corpus:main"
+speech-index = "pyriksprot.scripts.speech_index:main"
+metadata2db = "pyriksprot.scripts.metadata2db:main"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-rfE", "-q", "-s"]
 log_cli = "False"
 testpaths = ["tests"]
 python_files = "*_test.py"
@@ -141,8 +145,8 @@
 reportMissingImports = true
 reportMissingTypeStubs = false
 reportUntypedFunctionDecorator = false
 reportUntypedClassDecorator = true
 reportOptionalSubscript = false
 reportOptionalMemberAccess = false
 reportOptionalCall = false
-pythonVersion = "3.9"
+pythonVersion = "3.11"
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/__init__.py` & `pyriksprot-2023.4.1/pyriksprot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 # type: ignore
 
 from . import metadata
-from .corpus.corpus_index import CorpusSourceIndex, CorpusSourceItem
+from .corpus.corpus_index import CorpusSourceIndex, ICorpusSourceItem
 from .corpus.iterate import ProtocolSegment, ProtocolSegmentIterator
 from .corpus.parlaclarin import pretokenize
-from .dehyphenation import SwedishDehyphenator, SwedishDehyphenatorService
+from .dehyphenation import SwedishDehyphenator
 from .dispatch import DispatchItem, SegmentMerger, create_grouping_hashcoder
 from .interface import ParlaClarinError, Protocol, SegmentLevel, Speech, Utterance
 from .to_speech import MergerFactory, MergeStrategyType, to_speeches
 from .utility import (
     compose,
-    data_path_ts,
     dedent,
     deprecated,
-    dict_get_by_path,
-    download_protocols,
-    download_url,
     ensure_path,
     flatten,
     hasattr_path,
     is_empty,
-    load_dict,
-    load_token_set,
     lookup,
     norm_join,
     parse_range_list,
     path_add_date,
     path_add_sequence,
     path_add_suffix,
     path_add_timestamp,
+    reset_file,
+    reset_folder,
     sanitize,
     slugify,
-    split_properties_by_dataclass,
-    store_dict,
-    store_token_set,
     strip_extensions,
-    strip_path_and_add_counter,
     strip_path_and_extension,
     strip_paths,
     sync_delta_names,
     temporary_file,
     touch,
     ts_data_path,
     unlink,
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/corpus_index.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/corpus_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,90 +15,103 @@
 
 """
 Creates a recursive index of files in a source folder that match given pattern.
 """
 
 
 @dataclass
-class CorpusSourceItem:
-
+class ICorpusSourceItem:
     path: str
     filename: str = None
     name: str = None
     subfolder: str = None
     year: Optional[int] = None
-    metadata: dict | None = None
 
     def __post_init__(self):
-
         self.filename = basename(self.path)
         self.name = utility.strip_path_and_extension(self.path)
         self.subfolder = basename(dirname(self.path))
-        self.metadata = load_metadata(self.path)
 
         if not self.name.startswith("prot-"):
             raise ValueError(f"illegal filename {self.name}")
 
         """Year extracted from filename"""
         self.year = int(self.filename.split("-")[1][:4])
 
-        """Year from data in metadata (the actual year)"""
-        self.actual_year = int(self.metadata['date'][:4]) if self.metadata else self.year
-
     @property
     def is_empty(self) -> bool:
-        return not bool(self.metadata)
+        return False
 
     def to_dict(self) -> dict:
-
         return asdict(self)
 
 
 @dataclass
-class CorpusSourceIndex:
-    def __init__(self, source_items: List[CorpusSourceItem]):
+class TaggedCorpusSourceItem(ICorpusSourceItem):
+    metadata: dict | None = None
+    # actual_year: int = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.metadata = load_metadata(self.path)
+        """Year from data in metadata (the actual year)"""
+        # self.actual_year = int(self.metadata['date'][:4]) if self.metadata else self.year
+
+    @property
+    def is_empty(self) -> bool:
+        """Checks if file is empty. Only valid for tagged ZIP files"""
+        return not bool(self.metadata)
 
-        self.source_items: List[CorpusSourceItem] = source_items
+
+@dataclass
+class CorpusSourceIndex:
+    def __init__(self, source_items: list[ICorpusSourceItem]):
+        self.source_items: list[ICorpusSourceItem] = source_items
         self.lookup: dict = {x.name: x for x in self.source_items}
 
-    def __getitem__(self, key: str) -> CorpusSourceItem:
+    def __getitem__(self, key: str) -> ICorpusSourceItem:
         return self.lookup.get(key)
 
     def __contains__(self, key: str) -> bool:
         return key in self.lookup
 
     def __len__(self) -> int:
         return len(self.source_items)
 
     @staticmethod
     def load(
         *, source_folder: str, source_pattern: str, years: Optional[str | Set[int]] = None, skip_empty: bool = True
     ) -> "CorpusSourceIndex":
-
         if not isdir(source_folder):
             raise ValueError(f"folder {source_folder} not found")
 
         paths: List[str] = glob.glob(jj(source_folder, source_pattern), recursive=True)
 
         target_years: Set[int] = (
             None if years is None else (set(utility.parse_range_list(years)) if isinstance(years, str) else set(years))
         )
 
-        source_items = [CorpusSourceItem(path=path) for path in paths]
+        source_items = [CorpusSourceIndex.create(path=path) for path in paths]
 
         if target_years is not None:
             source_items = [x for x in source_items if x.year in target_years]
 
         if skip_empty:
             source_items = [x for x in source_items if not x.is_empty]
 
         source_index: CorpusSourceIndex = CorpusSourceIndex(source_items)
 
         return source_index
 
+    @staticmethod
+    def create(path: str) -> ICorpusSourceItem:
+        if path.endswith("zip"):
+            return TaggedCorpusSourceItem(path)
+        return ICorpusSourceItem(path)
+
     @property
     def filenames(self) -> List[str]:
         return sorted([x.filename for x in self.source_items])
 
     @property
     def paths(self) -> List[str]:
         return sorted([x.path for x in self.source_items])
@@ -109,10 +122,10 @@
 
     def to_csv(self, filename: str = None) -> Optional[str]:
         return self.to_pandas().to_csv(filename, sep='\t', index=None)
 
     @staticmethod
     def read_csv(filename: str) -> "CorpusSourceIndex":
         df: pd.DataFrame = pd.read_csv(filename, sep="\t", index_col=None)
-        source_items: List[CorpusSourceItem] = [CorpusSourceItem(**d) for d in df.to_dict('records')]
+        source_items: list[ICorpusSourceItem] = [ICorpusSourceItem(**d) for d in df.to_dict('records')]
         source_index: CorpusSourceIndex = CorpusSourceIndex(source_items)
         return source_index
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/iterate.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/iterate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass
 from multiprocessing import get_context
-from typing import TYPE_CHECKING, Callable, Iterable
+from typing import TYPE_CHECKING, Callable, Iterable, Literal
 
 import numpy as np
+import tqdm
 
 from .. import to_speech as mu
-from ..interface import ContentType, IDispachItem, Protocol, SegmentLevel
+from ..interface import ContentType, IDispatchItem, Protocol, SegmentLevel
 from ..utility import compress
 
 if TYPE_CHECKING:
     from ..metadata import SpeakerInfo
 
 # pylint: disable=too-many-arguments, no-member
 
 
 @dataclass
-class ProtocolSegment(IDispachItem):
+class ProtocolSegment(IDispatchItem):
     """Container for a subset of utterances within a single protocol"""
 
     protocol_name: str
     name: str
     who: str
     id: str
     data: str
-    page_number: str
+    page_number: int
     year: int
     u_id: str
     n_utterances: int = 0
     speaker_info: SpeakerInfo = None
     speaker_note_id: str = None
     speech_index: int = None
 
@@ -53,15 +54,24 @@
             'document_name': self.name,
             'filename': self.filename,
             'n_tokens': self.n_tokens,
             'n_utterances': self.n_utterances,
             'speaker_note_id': self.speaker_note_id,
             'speech_index': self.speech_index,
             'page_number': self.page_number,
-            **({} if not self.speaker_info else self.speaker_info.to_dict()),
+            **(
+                {}
+                if not self.speaker_info
+                else {
+                    'gender_id': self.speaker_info.gender_id,
+                    'party_id': self.speaker_info.party_id,
+                    'office_type_id': self.speaker_info.term_of_office.office_type_id,
+                    'sub_office_type_id': self.speaker_info.term_of_office.sub_office_type_id,
+                }  # FIXME: Call self.speaker_info.to_dict() instead
+            ),
         }
 
     @staticmethod
     def dtypes() -> dict:
         return {
             'year': np.int16,
             'n_tokens': np.int32,
@@ -79,49 +89,52 @@
         return f'{self.name}.{self.extension}'
 
     @property
     def text(self) -> str:
         return self.data
 
 
-def to_protocol_segment(*, protocol: Protocol, content_type: ContentType, **_) -> list[ProtocolSegment]:
+def to_protocol_segment(
+    *, protocol: Protocol, content_type: ContentType, which_year: Literal["filename", "date"] = "filename", **_
+) -> list[ProtocolSegment]:
     return [
         ProtocolSegment(
             protocol_name=protocol.name,
             content_type=content_type,
             segment_level=SegmentLevel.Protocol,
-            year=protocol.year,
+            year=protocol.get_year(which=which_year),
             name=protocol.name,
             who=None,
             id=protocol.name,
             u_id=None,
             data=protocol.text,
-            page_number='0',
+            page_number=0,
             n_tokens=0,
             n_utterances=len(protocol.utterances),
             speaker_info=None,
             speaker_note_id=None,
         )
     ]
 
 
 def to_speech_segments(
     *,
     protocol: Protocol,
     content_type: ContentType,
     segment_skip_size: int,
     merge_strategy: mu.MergeStrategyType,
+    which_year: Literal["filename", "date"] = "filename",
     **_,
 ) -> list[ProtocolSegment]:
     return [
         ProtocolSegment(
             protocol_name=protocol.name,
             content_type=content_type,
             segment_level=SegmentLevel.Speech,
-            year=protocol.year,
+            year=protocol.get_year(which=which_year),
             name=s.document_name,
             who=s.who,
             id=s.speech_id,
             u_id=s.speech_id,
             data=s.to_content_str(content_type),
             page_number=s.page_number,
             n_tokens=0 if not s.has_tagged_text else s.tagged_text.count("\n"),
@@ -130,62 +143,71 @@
             speech_index=s.speech_index,
         )
         for s in mu.to_speeches(protocol=protocol, merge_strategy=merge_strategy, skip_size=segment_skip_size)
     ]
 
 
 def to_who_segments(
-    *, protocol: Protocol, content_type: ContentType, segment_skip_size: int, **_
+    *,
+    protocol: Protocol,
+    content_type: ContentType,
+    segment_skip_size: int,
+    which_year: Literal["filename", "date"] = "filename",
+    **_,
 ) -> list[ProtocolSegment]:
     return [
         ProtocolSegment(
             protocol_name=protocol.name,
             content_type=content_type,
             segment_level=SegmentLevel.Who,
-            year=protocol.year,
+            year=protocol.get_year(which=which_year),
             name=s.document_name,
             who=s.who,
             id=s.speech_id,
             u_id=s.speech_id,
             data=s.to_content_str(content_type),
             page_number=s.page_number,
             n_tokens=0,
             n_utterances=len(s),
         )
         for s in mu.to_speeches(protocol=protocol, merge_strategy=mu.MergeStrategyType.who, skip_size=segment_skip_size)
     ]
 
 
-def to_utterance_segments(*, protocol: Protocol, content_type: ContentType, **_) -> list[ProtocolSegment]:
+def to_utterance_segments(
+    *, protocol: Protocol, content_type: ContentType, which_year: Literal["filename", "date"] = "filename", **_
+) -> list[ProtocolSegment]:
     return [
         ProtocolSegment(
             protocol_name=protocol.name,
             content_type=content_type,
             segment_level=SegmentLevel.Utterance,
-            year=protocol.year,
+            year=protocol.get_year(which=which_year),
             name=f'{protocol.name}_{i+1:03}',
             who=u.who,
             id=u.u_id,
             u_id=u.u_id,
             data=u.to_str(content_type),
             page_number=u.page_number,
             n_tokens=0,
             n_utterances=1,
         )
         for i, u in enumerate(protocol.utterances)
     ]
 
 
-def to_paragraph_segments(*, protocol: Protocol, content_type: ContentType, **_) -> list[ProtocolSegment]:
+def to_paragraph_segments(
+    *, protocol: Protocol, content_type: ContentType, which_year: Literal["filename", "date"] = "filename", **_
+) -> list[ProtocolSegment]:
     return [
         ProtocolSegment(
             protocol_name=protocol.name,
             content_type=content_type,
             segment_level=SegmentLevel.Paragraph,
-            year=protocol.year,
+            year=protocol.get_year(which=which_year),
             name=f'{protocol.name}_{j+1:03}_{i+1:03}',
             who=u.who,
             id=f"{u.u_id}@{i}",
             u_id=u.u_id,
             data=p,
             page_number=u.page_number,
             n_tokens=0,
@@ -200,14 +222,15 @@
     *,
     protocol: Protocol,
     content_type: ContentType,
     segment_level: SegmentLevel,
     merge_strategy: mu.MergeStrategyType,
     segment_skip_size: int = 1,
     preprocess: Callable[[str], str] = None,
+    which_year: Literal["filename", "date"] = "filename",
 ) -> Iterable[ProtocolSegment]:
     """Splits protocol to sequence of text/tagged text segments
 
     Args:
         content_type (ContentType): Text' or 'TaggedFrame'
         segment_level (SegmentLevel): [description]
         segment_skip_size (int, optional): [description]. Defaults to 1.
@@ -218,14 +241,15 @@
     """
 
     segments: list[ProtocolSegment] = SEGMENT_FUNCTIONS.get(segment_level)(
         protocol=protocol,
         content_type=content_type,
         segment_skip_size=segment_skip_size,
         merge_strategy=merge_strategy,
+        which_year=which_year,
     )
 
     if preprocess is not None:
         for x in segments:
             x.data = preprocess(x.data)
 
     if segment_skip_size > 0:
@@ -241,81 +265,88 @@
     SegmentLevel.Who: to_who_segments,
     SegmentLevel.Utterance: to_utterance_segments,
     SegmentLevel.Paragraph: to_paragraph_segments,
 }
 
 
 class ProtocolSegmentIterator(abc.ABC):
-    ...
-
     def __init__(
         self,
         *,
         filenames: list[str],
         content_type: ContentType = ContentType.Text,
         segment_level: SegmentLevel = SegmentLevel.Protocol,
         segment_skip_size: int = 1,
         multiproc_processes: int = None,
         multiproc_chunksize: int = 100,
         multiproc_keep_order: bool = False,
         merge_strategy: str = 'chain',
         preprocess: Callable[[str], str] = None,
+        which_year: Literal["filename", "date"] = "filename",
     ):
         """Merge utterances within protocols to segments.
 
         Args:
             filenames (list[str]): files to read
             content_type (ContentType, optional): Content type Text or TaggedFrame . Defaults to TaggedFrame.
             segment_level (SegmentLevel, optional): Iterate segment level. Defaults to Protocol.
             segment_skip_size (int, optional): Skip segments having char count below threshold. Defaults to 1.
             multiproc_processes (int, optional): Number of read processes. Defaults to None.
             multiproc_chunksize (int, optional): Multiprocessing multiproc_chunksize. Defaults to 100.
             multiproc_keep_order (bool, optional): Keep doc order. Defaults to False.
             merge_strategy (str, optional): Speech merge strategy. Defaults to 'chain'.
             preprocess (Callable[[str], str], optional): Preprocess funcion, only used for text. Defaults to None.
+            which_year (Literal["filename", "date"]): Take year from filename or XML tag `date` in content
         """
         self.filenames: list[str] = sorted(filenames)
         self.iterator = None
         self.content_type: ContentType = content_type
         self.segment_level: SegmentLevel = segment_level
         self.segment_skip_size: int = segment_skip_size
         self.merge_strategy: str = merge_strategy  # FIXME: used??
         self.multiproc_processes: int = multiproc_processes or 1
         self.multiproc_chunksize: int = multiproc_chunksize
         self.multiproc_keep_order: bool = multiproc_keep_order
         self.preprocess: Callable[[ProtocolSegment], str] = preprocess
+        self.which_year: str = which_year
 
     def __iter__(self):
         self.iterator = self.create_iterator()
         return self
 
     def __next__(self):
         return next(self.iterator)
 
     def create_iterator(self) -> Iterable[ProtocolSegment]:
-
         item: ProtocolSegment
         fx = self.preprocess
         # speaker_service: SpeakerInfoService = self.speaker_service
 
         if self.multiproc_processes > 1:
             args: list[tuple[str, str, str, int]] = [
-                (name, self.content_type, self.segment_level, self.segment_skip_size, self.merge_strategy)
+                (
+                    name,
+                    self.content_type,
+                    self.segment_level,
+                    self.segment_skip_size,
+                    self.merge_strategy,
+                    self.which_year,
+                )
                 for name in self.filenames
             ]
             with get_context("spawn").Pool(processes=self.multiproc_processes) as executor:
                 imap = executor.imap if self.multiproc_keep_order else executor.imap_unordered
                 futures = self.map_futures(imap=imap, args=args)
                 for payload in futures:
                     for item in payload:
                         if fx:
                             fx(item)
                         yield item
         else:
-            for filename in self.filenames:
+            for filename in tqdm.tqdm(self.filenames):
                 for item in self.load(filename=filename):
                     if fx:
                         fx(item)
                     yield item
 
     @abc.abstractmethod
     def load(self, filename: str) -> Iterable[ProtocolSegment]:
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/convert.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 import os
 from typing import TYPE_CHECKING, List, Union
 
 from click import echo
 from jinja2 import Environment, PackageLoader, Template, select_autoescape
 
 from pyriksprot import to_speech
-from pyriksprot.dehyphenation import SwedishDehyphenatorService
+from pyriksprot.dehyphenation import SwedishDehyphenator
 from pyriksprot.foss.sparv_tokenize import default_tokenize
 from pyriksprot.utility import dedent, strip_paths
 
 from . import parse
 
 if TYPE_CHECKING:
     from .. import interface
 
-__dehyphenator: SwedishDehyphenatorService = None
+__dehyphenator: SwedishDehyphenator = None
 
 
-def get_dehyphenator() -> SwedishDehyphenatorService:
+def get_dehyphenator() -> SwedishDehyphenator:
     return __dehyphenator
 
 
-def set_dehyphenator(**opts) -> None:
+def set_dehyphenator(data_folder: str) -> SwedishDehyphenator:
     global __dehyphenator
-    __dehyphenator = SwedishDehyphenatorService(**opts)
+    __dehyphenator = SwedishDehyphenator(data_folder=data_folder, word_frequencies=None)
 
 
 def dehyphen(text: str) -> str:
     """Remove hyphens from `text`."""
-    dehyphenated_text = get_dehyphenator().dehyphenator.dehyphen_text(text)
+    dehyphenated_text = get_dehyphenator().dehyphen_text(text)
     return dehyphenated_text
 
 
 def pretokenize(text: str) -> str:
     """Tokenize `text`, then join resulting tokens."""
     return ' '.join(default_tokenize(text))
 
@@ -75,25 +75,25 @@
 
 
 def convert_protocol(
     input_filename: str = None,
     output_filename: str = None,
     template_name: str = None,
     merge_strategy: to_speech.MergeStrategyType = to_speech.MergeStrategyType.who_speaker_note_id_sequence,
-    **dehyphen_cfg,
+    dehyphen_folder: str = None,
 ):
     """Convert protocol in `input_filename' using template `template_name`. Store result in `output_filename`.
 
     Args:
         input_filename (str, optional): Source file. Defaults to None.
         output_filename (str, optional): Target file. Defaults to None.
         template_name (str, optional): Template name (found in resource-folder). Defaults to None.
     """
-    set_dehyphenator(**dehyphen_cfg)
-    protocol: interface.Protocol = parse.ProtocolMapper.to_protocol(input_filename, segment_skip_size=5)
+    set_dehyphenator(data_folder=dehyphen_folder)
+    protocol: interface.Protocol = parse.ProtocolMapper.parse(input_filename)
     content: str = ""
 
     if protocol.has_text:
         converter: ProtocolConverter = ProtocolConverter(template_name)
         speeches: List[interface.Speech] = to_speech.to_speeches(protocol=protocol, merge_strategy=merge_strategy)
         content: str = converter.convert(protocol, speeches, strip_paths(input_filename))
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/iterate.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/iterate.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,94 +2,68 @@
 
 from typing import Iterable, List, Tuple
 
 from pyriksprot.corpus import iterate
 from pyriksprot.interface import ContentType
 from pyriksprot.utility import deprecated
 
-from .parse import ProtocolMapper, XmlIterParseProtocol, XmlUntangleProtocol
+from .parse import ProtocolMapper
 
 
 def multiprocessing_xml_load(args) -> Iterable[iterate.ProtocolSegment]:
     """Load protocol from XML. Aggregate text to `segment_level`. Return (name, who, id, text)."""
     return iterate.to_segments(
         content_type=ContentType.Text,
-        protocol=XmlUntangleProtocol(data=args[0], segment_skip_size=args[3]),
+        protocol=ProtocolMapper.parse(filename=args[0]),
         segment_level=args[2],
         merge_strategy=args[4],
         segment_skip_size=args[3],
+        which_year=args[5],
     )
 
 
 class XmlUntangleSegmentIterator(iterate.ProtocolSegmentIterator):
     """Iterate ParlaClarin XML files using `untangle` wrapper."""
 
     def load(self, filename: str) -> Iterable[iterate.ProtocolSegment]:
         """Load protocol from XML. Aggregate text to `segment_level`. Return sequence of segment.ProtocolSegment."""
         return iterate.to_segments(
             content_type=ContentType.Text,
-            protocol=XmlUntangleProtocol(data=filename, segment_skip_size=self.segment_skip_size),
+            protocol=ProtocolMapper.parse(filename=filename),
             segment_level=self.segment_level,
             merge_strategy=self.merge_strategy,
             segment_skip_size=self.segment_skip_size,
+            which_year=self.which_year,
         )
 
     def map_futures(self, imap, args: List[Tuple[str, str, int]]):
         return imap(multiprocessing_xml_load, args)
 
 
 @deprecated
 def multiprocessing_load(args):
     return iterate.to_segments(
-        protocol=ProtocolMapper.to_protocol(data=args[0]),
+        protocol=ProtocolMapper.parse(filename=args[0]),
         content_type=args[1],
         segment_level=args[2],
         segment_skip_size=args[3],
         merge_strategy=args[4],
+        which_year=args[5],
     )
 
 
 # @deprecated
 class XmlProtocolSegmentIterator(iterate.ProtocolSegmentIterator):
     """Reads xml files using Protocol entity and returns a stream of `segment.ProtocolSegment`"""
 
     def load(self, filename: str) -> List[iterate.ProtocolSegment]:
         return iterate.to_segments(
-            protocol=ProtocolMapper.to_protocol(data=filename, segment_skip_size=self.segment_skip_size),
+            protocol=ProtocolMapper.parse(filename=filename),
             content_type=self.content_type,
             segment_level=self.segment_level,
             segment_skip_size=self.segment_skip_size,
             merge_strategy=self.merge_strategy,
+            which_year=self.which_year,
         )
 
     def map_futures(self, imap, args):
         return imap(multiprocessing_load, args, chunksize=self.multiproc_chunksize)
-
-
-@deprecated
-def multiprocessing_xml_iter_load(args) -> Iterable[iterate.ProtocolSegment]:
-    """Load protocol from XML. Aggregate text to `segment_level`. Return (name, who, id, text)."""
-    return iterate.to_segments(
-        content_type=ContentType.Text,
-        protocol=XmlIterParseProtocol(data=args[0], segment_skip_size=args[3]),
-        segment_level=args[2],
-        merge_strategy=args[4],
-        segment_skip_size=args[3],
-    )
-
-
-# @deprecated
-class XmlSaxSegmentIterator(iterate.ProtocolSegmentIterator):
-    """Reads xml files and returns a stream of (name, who, id, text, page_number).
-    Uses SAX streaming"""
-
-    def load(self, filename: str) -> List[iterate.ProtocolSegment]:
-        return iterate.to_segments(
-            content_type=ContentType.Text,
-            protocol=XmlIterParseProtocol(data=filename, segment_skip_size=self.segment_skip_size),
-            segment_level=self.segment_level,
-            merge_strategy=self.merge_strategy,
-            segment_skip_size=self.segment_skip_size,
-        )
-
-    def map_futures(self, imap, args):
-        return imap(multiprocessing_xml_iter_load, args, chunksize=self.multiproc_chunksize)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt` & `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt` & `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt` & `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/parlaclarin/tf.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/parlaclarin/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/tagged/iterate.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/tagged/iterate.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 import pandas as pd
 
 from .. import iterate
 from . import persist
 
 
 def multiprocessing_load(args) -> Iterable[iterate.ProtocolSegment]:
-
     protocol: iterate.Protocol = persist.load_protocol(filename=args[0])
     return (
         []
         if protocol is None
         else iterate.to_segments(
             protocol=protocol,
             content_type=args[1],
             segment_level=args[2],
             segment_skip_size=args[3],
             merge_strategy=args[4],
+            which_year=args[5],
         )
     )
 
 
 class ProtocolIterator(iterate.ProtocolSegmentIterator):
     """Reads xml files and returns a stream of `ProtocolSegment`"""
 
     def load(self, filename: str) -> List[Tuple[str, str, int]]:
-
         protocol: iterate.Protocol = persist.load_protocol(filename=filename)
 
         return (
             []
             if protocol is None
             else iterate.to_segments(
                 protocol=protocol,
                 content_type=self.content_type,
                 segment_level=self.segment_level,
                 segment_skip_size=self.segment_skip_size,
                 merge_strategy=self.merge_strategy,
+                which_year=self.which_year,
             )
         )
 
     def map_futures(self, imap, args):
         return imap(multiprocessing_load, args, chunksize=self.multiproc_chunksize)
 
     def to_segment_index(self) -> pd.DataFrame:
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/corpus/tagged/persist.py` & `pyriksprot-2023.4.1/pyriksprot/corpus/tagged/persist.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     protocol: interface.Protocol,
     checksum: str,
     storage_format: interface.StorageFormat = interface.StorageFormat.JSON,
 ) -> None:
     """Store tagged protocol in `output_filename`, with metadata."""
 
     if output_filename.endswith("zip"):
-
         with zipfile.ZipFile(output_filename, 'w', zipfile.ZIP_DEFLATED) as fp:
-
             metadata: dict = dict(name=protocol.name, date=protocol.date, checksum=checksum)
             fp.writestr(METADATA_FILENAME, json.dumps(metadata, indent=4))
 
             if storage_format == interface.StorageFormat.CSV:
                 utterances_csv_str: str = protocol.to_csv()
                 fp.writestr(f'{protocol.name}.csv', utterances_csv_str or "")
 
@@ -47,20 +45,19 @@
             #     .set_index('document_name', drop=False)
             #     .rename_axis('')
             #     .assign(document_id=range(0, len(speeches)))
             # )
             # fp.writestr('document_index.csv', document_index.to_csv(sep='\t', header=True))
 
     else:
-
         raise ValueError("Only Zip store currently implemented")
 
 
 def load_metadata(filename: str) -> Optional[dict]:
-    """Read metadata attributes stored in `metadata.json` """
+    """Read metadata attributes stored in `metadata.json`"""
 
     try:
         with zipfile.ZipFile(filename, 'r') as fp:
             filenames: List[str] = [f.filename for f in fp.filelist]
             if METADATA_FILENAME not in filenames:
                 return None
             json_str = fp.read(METADATA_FILENAME).decode('utf-8')
@@ -90,36 +87,33 @@
 
     metadata: dict = load_metadata(filename)
 
     if metadata is None:
         return None
 
     with zipfile.ZipFile(filename, 'r') as fp:
-
         basename: str = metadata['name']
 
         filenames: List[str] = [f.filename for f in fp.filelist]
 
         for ext in PROTOCOL_LOADERS:
-
             stored_filename: str = f"{basename}.{ext}"
 
             if not stored_filename in filenames:
                 continue
 
             data_str: str = fp.read(stored_filename).decode('utf-8')
             utterances: List[interface.Utterance] = PROTOCOL_LOADERS.get(ext)(data_str)
 
             protocol: interface.Protocol = interface.Protocol(utterances=utterances, **metadata, speaker_notes={})
 
             return protocol
 
 
 def load_protocols(source: str | List, file_pattern: str = 'prot-*.zip') -> Iterable[interface.Protocol]:
-
     return (p for p in (load_protocol(filename) for filename in glob_protocols(source, file_pattern)) if p is not None)
 
 
 def glob_protocols(source: str, file_pattern: str, strip_path: bool = False):
     filenames: List[str] = (
         glob.glob(os.path.join(source, file_pattern), recursive=True)
         if isinstance(source, str)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/dehyphenation/flair_dehyphen.py` & `pyriksprot-2023.4.1/pyriksprot/dehyphenation/flair_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/dehyphenation/swe_dehyphen.py` & `pyriksprot-2023.4.1/pyriksprot/dehyphenation/swe_dehyphen.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 License: https://gitlab.com/Julipan/swedish-de-hyphenator/-/blob/master/LICENSE
 
 """
 import os
 import re
 from dataclasses import dataclass, field
 from enum import IntEnum
-from typing import Callable, Dict, Set
+from typing import Callable
 
-from ..utility import load_dict, load_token_set, store_dict, store_token_set
+from .utility import load_dict, load_token_set, store_dict, store_token_set
 
 PARAGRAPH_MARKER = '##PARAGRAPH##'
 
 # pylint: disable=too-many-arguments
+jj = os.path.join
 
 
 class WhitelistReason(IntEnum):
     Undefined = 0
     HyphenatedCompound = 1
     Frequency = 2
     UnknownParts = 3
 
 
-IGNORE_CONJUNCTION_WORDS: Set[str] = {
+IGNORE_CONJUNCTION_WORDS: set[str] = {
     'än',
     'eller',
     'framför',
     'inklusive',
     'kontra',
     'liksom',
     'men',
@@ -53,90 +54,62 @@
 }
 
 
 def is_ignored_by_conjunction_word(dashed_word: str) -> bool:
     return any(dashed_word.endswith(f' {w}') for w in IGNORE_CONJUNCTION_WORDS)
 
 
-def find_dashed_words(text: str) -> Set[str]:
+def find_dashed_words(text: str) -> set[str]:
     dashed_words = [d for d in re.findall(r'\w+- \w+', text) if not is_ignored_by_conjunction_word(d)]
     return dashed_words
 
 
-class SwedishDehyphenatorService:
-    """Dehyphen text"""
-
-    def __init__(
-        self,
-        word_frequency_filename: str,
-        whitelist_filename: str,
-        whitelist_log_filename: str,
-        unresolved_filename: str,
-        word_frequencies: dict = None,
-        whitelist: Set = None,
-        whitelist_log: dict = None,
-        unresolved: Set = None,
-    ):
-
-        self.word_frequency_filename: str = word_frequency_filename
-        self.whitelist_filename: str = whitelist_filename
-        self.whitelist_log_filename: str = whitelist_log_filename
-        self.unresolved_filename: str = unresolved_filename
-
-        if not word_frequencies:
-            if not os.path.isfile(self.word_frequency_filename):
-                raise FileNotFoundError(self.word_frequency_filename)
-
-        # FIXME: Use PersistentDict to load/store dicts
-        self.dehyphenator: SwedishDehyphenator = SwedishDehyphenator(
-            word_frequencies=load_dict(self.word_frequency_filename) if word_frequencies is None else word_frequencies,
-            whitelist=load_token_set(self.whitelist_filename) if whitelist is None else whitelist,
-            whitelist_log=load_dict(self.whitelist_log_filename) if whitelist_log is None else whitelist_log,
-            unresolved=load_token_set(self.unresolved_filename) if unresolved is None else unresolved,
-        )
-
-    def flush(self):
-        store_token_set(self.dehyphenator.whitelist, self.whitelist_filename)
-        store_token_set(self.dehyphenator.unresolved, self.unresolved_filename)
-        store_dict(self.dehyphenator.whitelist_log, self.whitelist_log_filename)
-
-    @staticmethod
-    def create_dehypen(**opts) -> Callable[[str], str]:
-        """Create a dehypen service. Return wrapped dehypen function."""
-        service = SwedishDehyphenatorService(**opts)
-
-        def dehyphen(text: str) -> str:
-            """Remove hyphens from `text`."""
-            dehyphenated_text = service.dehyphenator.dehyphen_text(text)
-
-            return dehyphenated_text
-
-        return dehyphen
-
-
 class ParagraphMergeStrategy(IntEnum):
     DoNotMerge = (0,)
     MergeIfWordsOnlySeparatedByTwoNewlines = (1,)
     MergeAll = 2
 
 
 @dataclass
 class SwedishDehyphenator:
     """Dehyphens Swedish text"""
 
-    # External data
-    word_frequencies: Dict[str, int]
+    data_folder: str
+    word_frequencies: dict[str, int]
 
     # Internal data
-    whitelist: Set[str] = field(default_factory=set)
-    whitelist_log: Dict[str, int] = field(default_factory=dict)
-    unresolved: Set[str] = field(default_factory=set)
+    whitelist: set[str] = field(default_factory=set)
+    whitelist_log: dict[str, int] = field(default_factory=dict)
+    unresolved: set[str] = field(default_factory=set)
 
     paragraph_merge_strategy: ParagraphMergeStrategy = 0
 
+    def __post_init__(self) -> "SwedishDehyphenator":
+        if self.word_frequencies is None:
+            self.word_frequencies = os.path.join(self.data_folder, 'riksdagen-corpus-term-frequencies.pkl')
+
+        if isinstance(self.word_frequencies, str):
+            if not os.path.isfile(self.word_frequencies):
+                raise FileNotFoundError(self.word_frequencies)
+            self.word_frequencies = load_dict(self.word_frequencies)
+
+        self.load()
+
+    @property
+    def whitelist_filename(self) -> str:
+        return jj(self.data_folder, 'dehyphen_whitelist.txt.gz')
+
+    @property
+    def whitelist_log_filename(self) -> str:
+        return jj(self.data_folder, 'dehyphen_whitelist_log.pkl')
+
+    @property
+    def unresolved_filename(self) -> str:
+        return jj(self.data_folder, 'dehyphen_unresolved.txt.gz')
+
     def is_whitelisted(self, word: str) -> bool:
         return word.lower() in self.whitelist
 
     def is_known_word(self, word: str) -> bool:
         return word in self.whitelist
 
     def add_to_whitelist(self, word: str, reason_code: WhitelistReason = WhitelistReason.Undefined):
@@ -146,40 +119,40 @@
         self.whitelist_log[word] = int(reason_code)
         return word
 
     @staticmethod
     def is_hyphenated_compound(dashed_word: str) -> bool:
         """Test if is compund"""
         if re.match(
-            r'[A-ZÅÄÖ]+-[a-zåäö]+|' r'[A-ZÅÄÖ][a-zåäö]+-[A-ZÅÄÖ][a-zåäö]+|' r'\d+-\w+|' r'icke-\w+',
+            r'[A-ZÅÄÖ]+-[a-zåäö]+|' + r'[A-ZÅÄÖ][a-zåäö]+-[A-ZÅÄÖ][a-zåäö]+|' + r'\d+-\w+|' + r'icke-\w+',
             dashed_word,
         ):
             return True
 
         return None
 
     def dehyphen_dashed_word(self, dash: str) -> str:  # pylint: disable=too-many-return-statements
         """Remove hyphen from word if rules are satisfied"""
         compound_word: str = re.sub('- ', '', dash)
         dashed_word: str = re.sub('- ', '-', dash)
 
-        _compound_word = compound_word.lower()
-        _dashed_word = dashed_word.lower()
+        _compound_word: str = compound_word.lower()
+        _dashed_word: str = dashed_word.lower()
 
         if self.is_whitelisted(_compound_word):
             return compound_word
 
         if self.is_whitelisted(_dashed_word):
             return dashed_word
 
         if self.is_hyphenated_compound(dashed_word):
             return self.add_to_whitelist(dashed_word, WhitelistReason.HyphenatedCompound)
 
-        _compound_word_frequency = self.word_frequencies.get(_compound_word, 0)
-        _dashed_word_frequency = self.word_frequencies.get(_dashed_word, 0)
+        _compound_word_frequency: int = self.word_frequencies.get(_compound_word, 0)
+        _dashed_word_frequency: int = self.word_frequencies.get(_dashed_word, 0)
 
         if _compound_word_frequency > _dashed_word_frequency:
             return self.add_to_whitelist(compound_word, WhitelistReason.Frequency)
 
         if _dashed_word_frequency > _compound_word_frequency:
             return self.add_to_whitelist(dashed_word, WhitelistReason.Frequency)
 
@@ -198,15 +171,15 @@
 
         self.unresolved.add(dash)
 
         return dash
 
     def dehyphen_text(self, text: str) -> str:
         """Remove dehyphens in text"""
-        text = re.sub(r'\n{3,}', r'\n\n', text)
+        text: str = re.sub(r'\n{3,}', r'\n\n', text)
 
         # add paragraph markers:
         text = re.sub(r'\n\n', PARAGRAPH_MARKER, text)
 
         # remove paragraph marker if previous line is ELH (end-of-line hyphenation)
         text = re.sub(rf'-\s*{PARAGRAPH_MARKER}', '- ', text)
 
@@ -223,14 +196,39 @@
         text = text.strip()
         text = re.sub(PARAGRAPH_MARKER, '\n\n', text)
 
         text = merge_paragraphs(text, self.paragraph_merge_strategy)
 
         return text
 
+    def flush(self):
+        store_token_set(self.whitelist, self.whitelist_filename)
+        store_token_set(self.unresolved, self.unresolved_filename)
+        store_dict(self.whitelist_log, self.whitelist_log_filename)
+
+    def load(self) -> None:
+        self.whitelist = load_token_set(self.whitelist_filename)
+        self.whitelist_log = load_dict(self.whitelist_log_filename)
+        self.unresolved = load_token_set(self.unresolved_filename)
+
+    @staticmethod
+    def create_dehypen(data_folder: str, word_frequencies: str | dict = None) -> Callable[[str], str]:
+        """Create a dehypen service. Return wrapped dehypen function."""
+        dehyphenator: SwedishDehyphenator = SwedishDehyphenator(
+            data_folder=data_folder, word_frequencies=word_frequencies
+        )
+
+        def dehyphen(text: str) -> str:
+            """Remove hyphens from `text`."""
+            dehyphenated_text = dehyphenator.dehyphen_text(text)
+
+            return dehyphenated_text
+
+        return dehyphen
+
 
 def merge_paragraphs(text: str, paragraph_merge_strategy: ParagraphMergeStrategy) -> str:
     """Merge paragraphs"""
     if paragraph_merge_strategy == ParagraphMergeStrategy.MergeIfWordsOnlySeparatedByTwoNewlines:
         return re.sub(r"(\w+)(\n\n)(\w+)", r"\1 \3", text)
 
     if paragraph_merge_strategy == ParagraphMergeStrategy.MergeAll:
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/dispatch/dispatch.py` & `pyriksprot-2023.4.1/pyriksprot/dispatch/dispatch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from __future__ import annotations
 
 import abc
 import os
+import string
 import sys
 import zipfile
 from collections import defaultdict
 from enum import Enum
 from io import StringIO
 from typing import Any, Literal, Type
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 
+from pyriksprot.corpus.iterate import ProtocolSegment
 from pyriksprot.dispatch.item import DispatchItem
+from pyriksprot.dispatch.utility import decode_protocol_segment_filename, to_temporal_category
 from pyriksprot.foss.pos_tags import PoS_Tag_Scheme, PoS_TAGS_SCHEMES
+from pyriksprot.foss.sparv_tokenize import default_tokenize
 from pyriksprot.foss.stopwords import STOPWORDS
+from pyriksprot.metadata import Codecs
 
 from .. import utility
-from ..interface import IDispachItem, SegmentLevel
+from ..interface import IDispatchItem, SegmentLevel
 
 jj = os.path.join
 
 TargetTypeKey = Literal[
     'files-in-zip',
     'single-tagged-frame-per-group',
     'single-id-tagged-frame-per-group',
     'single-id-tagged-frame',
     'checkpoint-per-group',
     'files-in-folder',
     'one-hot-sparse',
+    'sorted-speeches-in-zip',
 ]
 
+PERSON_ATTRIBUTES = {'sub_office_type_id', 'office_type_id', 'protocol_name', 'gender_id', 'party_id'}
+
 
 class CompressType(str, Enum):
     Plain = 'csv'
     Zip = 'zip'
     Gzip = 'gzip'
     Bz2 = 'bz2'
     Lzma = 'lzma'
@@ -52,31 +60,31 @@
 
     @classmethod
     def values(cls) -> list[str]:
         return [e.value for e in cls]
 
 
 class IDispatcher(abc.ABC):
-
     name: str = 'parent'
 
-    def __init__(self, *, target_name: str, compress_type: CompressType, **kwargs):
+    def __init__(self, *, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
         """Dispatches text blocks to a target_name zink.
 
         Args:
             target_name (str): Target filename or folder.
             compress_type ([str]): Target compress format.
         """
         self.target_name: str = target_name
         self.document_data: list[dict] = []
         self.document_id: int = 0
         self.compress_type: CompressType = compress_type
         self.kwargs: dict = kwargs
         self.lowercase: bool = kwargs.get('lowercase', False)
         self.skip_stopwords: bool = kwargs.get('skip_stopwords', False)
+        self.lookups: Codecs = lookups
 
     def __enter__(self) -> IDispatcher:
         self.open_target(self.target_name)
         return self
 
     def __exit__(self, _type, _value, _traceback):  # pylint: disable=unused-argument
         """If the suite was exited due to an exception, and the return value from the __exit__() method was false,
@@ -84,40 +92,38 @@
         continues with the statement following the with statement."""
         self.close_target()
         return False
 
     @abc.abstractmethod
     def open_target(self, target_name: Any) -> None:
         """Open zink."""
-        ...
 
     def close_target(self) -> None:
         """Close zink."""
         self.dispatch_index()
 
     def dispatch_index(self) -> None:
         """Dispatch an index of dispatched documents."""
-        ...
 
-    def dispatch(self, dispatch_items: list[IDispachItem]) -> None:
+    def dispatch(self, dispatch_items: list[IDispatchItem]) -> None:
         for item in dispatch_items:
             self._dispatch_index_item(item)
             self._dispatch_item(item)
 
     def _reset_index(self) -> None:
         self.document_data = []
         self.document_id: int = 0
 
-    def _dispatch_index_item(self, item: IDispachItem) -> None:
+    def _dispatch_index_item(self, item: IDispatchItem) -> None:
         """Default one document per group"""
         self.document_data.append({**item.to_dict(), **{'document_id': self.document_id}})
         self.document_id += 1
 
     @abc.abstractmethod
-    def _dispatch_item(self, item: IDispachItem) -> None:
+    def _dispatch_item(self, item: IDispatchItem) -> None:
         ...
 
     def document_index(self) -> pd.DataFrame:
         document_index: pd.DataFrame = pd.DataFrame(self.document_data)
         return document_index
 
     def document_index_str(self) -> str:
@@ -127,15 +133,14 @@
     def store(self, filename: str, data: str | pd.DataFrame) -> None:
         """Store text to file."""
 
         if not os.path.split(filename)[0]:
             filename = jj(self.target_name, f"{filename}")
 
         if isinstance(data, pd.DataFrame):
-
             if self.compress_type == 'feather':
                 data.to_feather(utility.replace_extension(filename, 'feather'))
                 return
 
             data = data.to_csv(sep='\t')
 
         if isinstance(data, str):
@@ -159,42 +164,74 @@
     def dispatcher_keys() -> list[str]:
         return [d.name for d in IDispatcher.dispatchers()]
 
     def to_lower(self, text: str) -> str:
         # FIXME: PoS tags gets lowercased???
         return text.lower() if self.lowercase else text
 
+    # FIXME: Consolidate this code!
+
+    def get_filename(self, item: IDispatchItem) -> str:
+        if isinstance(item, DispatchItem):
+            return self.decoded_filename(item)
+        return item.filename
+
+    def decoded_group_name(self, item: DispatchItem) -> str:
+        group_name: str = ""
+        for key, key_id in item.group_values.items():
+            try:
+                value_name: str = self.lookups.lookup_name(key, int(key_id), None)
+                group_name = (
+                    f"{group_name}_{key_id}"
+                    if value_name is None
+                    else f"{group_name}_unknown"
+                    if value_name == "?"
+                    else f"{group_name}_{value_name}"
+                )
+            except Exception as _:
+                group_name = f"{group_name}_{key_id}"
+        return group_name
+
+    def decoded_document_name(self, item: DispatchItem) -> str:
+        group_name: str = self.decoded_group_name(item)
+        if group_name != "":
+            group_name = f"_{group_name}"
+        return f'{item.group_temporal_value}{self.decoded_group_name(item)}'
+
+    def decoded_filename(self, item: DispatchItem) -> str:
+        return f'{self.decoded_document_name(item=item)}.{item.extension}'
+
 
 class FilesInFolderDispatcher(IDispatcher):
     """Dispatch text to filesystem as single files (optionally compressed)"""
 
-    def __init__(self, target_name: str, compress_type: CompressType, **kwargs):
-        super().__init__(target_name=target_name, compress_type=compress_type, **kwargs)
+    def __init__(self, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
 
     name: str = 'files-in-folder'
 
     def open_target(self, target_name: Any) -> None:
         os.makedirs(target_name, exist_ok=True)
 
-    def _dispatch_item(self, item: IDispachItem) -> None:
-        self.store(item.filename, self.to_lower(item.text))
+    def _dispatch_item(self, item: IDispatchItem) -> None:
+        self.store(self.get_filename(item), self.to_lower(item.text))
 
     def dispatch_index(self) -> None:
         """Write index of documents to disk."""
         self.store('document_index.csv', self.document_index_str())
 
 
 class FilesInZipDispatcher(IDispatcher):
     """Dispatch text to a single zip file."""
 
     name: str = 'files-in-zip'
 
-    def __init__(self, target_name: str, compress_type: CompressType, **kwargs):
+    def __init__(self, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
         self.zup: zipfile.ZipFile = None
-        super().__init__(target_name=target_name, compress_type=compress_type, **kwargs)
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
 
     def open_target(self, target_name: Any) -> None:
         """Create and open a new zip file."""
         if os.path.isdir(target_name):
             raise ValueError("zip mode: target_name must be name of zip file (not folder)")
         self.zup = zipfile.ZipFile(  # pylint: disable=consider-using-with
             self.target_name, mode="w", compression=self.compress_type.to_zipfile_compression()
@@ -208,125 +245,188 @@
     def dispatch_index(self) -> None:
         """Write index of documents to zip file."""
         if len(self.document_data) == 0:
             return
         csv_str: str = self.document_index_str()
         self.zup.writestr('document_index.csv', csv_str)
 
-    def _dispatch_item(self, item: IDispachItem) -> None:
-        self.zup.writestr(item.filename, self.to_lower(item.text))
+    def _dispatch_item(self, item: IDispatchItem) -> None:
+        self.zup.writestr(self.get_filename(item), self.to_lower(item.text))
+
+
+class SortedSpeechesInZipDispatcher(FilesInZipDispatcher):
+    """Dispatch speeches to files in a single zip file."""
+
+    name: str = 'sorted-speeches-in-zip'
+
+    def __init__(
+        self,
+        target_name: str,
+        compress_type: CompressType,
+        lookups: Codecs,
+        subfolder_key: str = None,
+        naming_keys: list[str] = None,
+        **kwargs,
+    ):
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
+        self.subfolder_key: str = subfolder_key
+        self.naming_keys: list[str] = naming_keys
+
+    def to_speech_segment(self, item: IDispatchItem) -> ProtocolSegment:
+        if item.segment_level != SegmentLevel.Speech:
+            raise ValueError(f"{type(self).__name__}: requires speech segment level")
+
+        if issubclass(type(item), ProtocolSegment):
+            return item
+
+        if hasattr(item, "protocol_segments"):
+            segments: list[ProtocolSegment] = getattr(item, "protocol_segments")
+            if len(segments) > 0:
+                return segments[0]
+
+        raise ValueError(f"{type(self).__name__}: item has no protocol segments")
+
+    def _dispatch_index_item(self, item: IDispatchItem) -> None:
+        tokens: list[str] = default_tokenize(item.text)
+        tokens = [t for t in tokens if len(t) > 1 or t not in string.punctuation]
+        item.n_tokens = len(tokens)
+        return super()._dispatch_index_item(item)
+
+    def _dispatch_item(self, item: IDispatchItem) -> None:
+        speech: ProtocolSegment = self.to_speech_segment(item)
+
+        subfolder: str = to_temporal_category(self.subfolder_key, speech.year, speech.protocol_name)
+
+        filename: str = jj(subfolder or "", decode_protocol_segment_filename(self.lookups, speech, self.naming_keys))
+
+        self.zup.writestr(filename, self.to_lower(speech.text))
 
 
 class CheckpointPerGroupDispatcher(IDispatcher):
     """Store as sequence of zipped CSV files (stream of Checkpoint)."""
 
-    def __init__(self, target_name: str, compress_type: CompressType, **kwargs):
-        super().__init__(target_name=target_name, compress_type=compress_type, **kwargs)
+    def __init__(self, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
 
     name: str = 'checkpoint-per-group'
 
     def open_target(self, target_name: Any) -> None:
         return
 
     def close_target(self) -> None:
         return
 
-    def _dispatch_item(self, item: IDispachItem) -> None:
+    def _dispatch_item(self, item: IDispatchItem) -> None:
         return
 
     def dispatch_index(self) -> None:
         return
 
-    def dispatch(self, dispatch_items: list[IDispachItem]) -> None:
-
+    def dispatch(self, dispatch_items: list[IDispatchItem]) -> None:
         self._reset_index()
 
         if len(dispatch_items) == 0:
             return
 
         checkpoint_name: str = f'{dispatch_items[0].group_temporal_value}.zip'
-        sub_folder: str = dispatch_items[0].group_temporal_value.split('-')[1]
-        path: str = jj(self.target_name, sub_folder)
+        subfolder: str = dispatch_items[0].group_temporal_value.split('-')[1]
+        path: str = jj(self.target_name, subfolder)
 
         os.makedirs(path, exist_ok=True)
 
         with zipfile.ZipFile(
             jj(path, checkpoint_name), mode="w", compression=self.compress_type.to_zipfile_compression()
         ) as fp:
-
             for item in dispatch_items:
                 fp.writestr(item.filename, self.to_lower(item.text))
                 self._dispatch_index_item(item)
 
             if len(self.document_data) > 0:
                 fp.writestr('document_index.csv', self.document_index_str())
                 self._reset_index()
 
 
 class TaggedFramePerGroupDispatcher(FilesInFolderDispatcher):
     """Store merged group items in a single tagged frame.
     NOTE! This dispatcher is ONLY valid for Speech level segments.
     """
 
-    def __init__(self, target_name: str, compress_type: CompressType, **kwargs):
-        super().__init__(target_name=target_name, compress_type=compress_type, **kwargs)
+    def __init__(self, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
         self.skip_text: bool = kwargs.get('skip_text', False)
         self.skip_lemma: bool = kwargs.get('skip_lemma', False)
         self.skip_puncts: bool = kwargs.get('skip_puncts', False)
 
     name: str = 'single-tagged-frame-per-group'
 
-    def _dispatch_item(self, item: IDispachItem) -> None:
+    def _dispatch_item(self, item: IDispatchItem) -> None:
         return
 
-    def _dispatch_index_item(self, item: IDispachItem) -> None:
-
+    def _dispatch_index_item(self, item: IDispatchItem) -> None:
         item: DispatchItem = item
 
         if item.segment_level != SegmentLevel.Speech:
             raise ValueError(f"TaggedFramePerGroupDispatcher: expected Speech, found {item.segment_level}")
 
-        if len(item.protocol_segments) != 1:
-            raise ValueError(
-                f"TaggedFramePerGroupDispatcher: expected exacly one Speech, found {len(item.protocol_segments)}"
-            )
-
-        for speech_segment in item.protocol_segments:
-            self.document_data.append(
-                {**{'document_id': self.document_id}, **item.to_dict(), **speech_segment.to_dict()}
-            )
-            self.document_id += 1
+        if item.group_values == {}:
+            """Speech level segments and no grouping => Add all speech metadata to index"""
+            if len(item.protocol_segments) > 1:
+                raise ValueError(
+                    f"TaggedFramePerGroupDispatcher: expected exacly one Speech, found {len(item.protocol_segments)}"
+                )
+            speech_data: dict = item.protocol_segments[0].to_dict()
+            item_data: dict = {**{'document_id': self.document_id}, **item.to_dict(), **speech_data}
+        else:
+            item_data: dict = {**{'document_id': self.document_id}, **item.to_dict()}
+            speech_data: dict = item.protocol_segments[0].to_dict()
+            if 'who' in item.group_values:
+                """If `who` in grouping attributes => add person attribute from first speech"""
+                for key in PERSON_ATTRIBUTES:
+                    if key in speech_data:
+                        item_data[key] = speech_data[key]
+            if 'n_tokens' in speech_data:
+                n_tokens: int = 0
+                for sd in item.protocol_segments:
+                    n_tokens += sd.n_tokens
+                item_data['n_tokens'] = n_tokens
+
+            # FIXME #39 Protocol segements must be merged into one Document index item.
+            # for speech_segment in item.protocol_segments:
+            #     self.document_data.append(
+            #         {**{'document_id': self.document_id}, **item.to_dict(), **speech_segment.to_dict()}
+            #     )
+            #     self.document_id += 1
 
-    def dispatch(self, dispatch_items: list[IDispachItem]) -> None:
+        self.document_data.append(item_data)
+        self.document_id += 1
 
+    def dispatch(self, dispatch_items: list[IDispatchItem]) -> None:
         if len(dispatch_items) == 0:
             return
 
         tagged_frames: list[pd.DataFrame] = []
         for item in dispatch_items:
-
             tagged_frame: pd.DataFrame = self.create_tagged_frame(item)
             tagged_frames.append(tagged_frame)
             item.n_tokens = len(tagged_frame)
             self._dispatch_index_item(item)
 
         if len(tagged_frames) > 0:
             total_frame: pd.DataFrame = pd.concat(tagged_frames, ignore_index=True)
             self.flush(total_frame, dispatch_items)
 
-    def flush(self, tagged_frame: pd.DataFrame, dispatch_items: list[IDispachItem]):
+    def flush(self, tagged_frame: pd.DataFrame, dispatch_items: list[IDispatchItem]):
         temporal_value: str = dispatch_items[0].group_temporal_value
-        sub_folder: str = temporal_value.split('-')[1] if '-' in temporal_value else temporal_value
-        path: str = jj(self.target_name, sub_folder)
+        subfolder: str = temporal_value.split('-')[1] if '-' in temporal_value else temporal_value
+        path: str = jj(self.target_name, subfolder)
         os.makedirs(path, exist_ok=True)
         target_name: str = jj(path, f'{temporal_value}.csv')
         self.store(filename=target_name, data=tagged_frame)
 
-    def create_tagged_frame(self, item: IDispachItem) -> pd.DataFrame:
-
+    def create_tagged_frame(self, item: IDispatchItem) -> pd.DataFrame:
         pads: set = {'MID', 'MAD', 'PAD'}
 
         tagged_frame: pd.DataFrame = pd.read_csv(StringIO(item.text), sep='\t', quoting=3, dtype=str)
         tagged_frame['document_id'] = self.document_id
 
         if self.lowercase:
             tagged_frame["token"] = tagged_frame["token"].str.lower()
@@ -389,25 +489,25 @@
 class IdTaggedFramePerGroupDispatcher(TaggedFramePerGroupDispatcher):
     """Store merged group items in a single tagged frame.
     NOTE! This dispatcher is ONLY valid for Speech level segments.
     """
 
     name: str = 'single-id-tagged-frame-per-group'
 
-    def __init__(self, target_name: str, compress_type: CompressType, **kwargs):
-        super().__init__(target_name=target_name, compress_type=compress_type, **kwargs)
+    def __init__(self, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
         self.token2id: defaultdict = defaultdict()
         self.tfs: defaultdict = defaultdict()
         self.token2id.default_factory = self.token2id.__len__
         self.pos_schema: PoS_Tag_Scheme = PoS_TAGS_SCHEMES.SUC
 
-    def create_tagged_frame(self, item: IDispachItem) -> pd.DataFrame:
+    def create_tagged_frame(self, item: IDispatchItem) -> pd.DataFrame:
         tagged_frame: pd.DataFrame = super().create_tagged_frame(item)
-        fg = lambda t: self.token2id[t]
-        pg = self.pos_schema.pos_to_id.get
+        fg = self.token2id.get  # lambda t: self.token2id[t]
+        pg = self.pos_schema.pos_to_id.get  # pylint: disable=unnecessary-lambda-assignment
 
         if not self.skip_text:
             tagged_frame['token_id'] = tagged_frame.token.apply(fg)
 
         if not self.skip_lemma:
             tagged_frame['lemma_id'] = tagged_frame.lemma.apply(fg)
 
@@ -431,19 +531,19 @@
 
 class SingleIdTaggedFrameDispatcher(IdTaggedFramePerGroupDispatcher):
     """Store merged group items in a single, global tagged frame."""
 
     name: str = 'single-id-tagged-frame'
     corpus_name: str = "corpus.feather"
 
-    def __init__(self, target_name: str, compress_type: CompressType, **kwargs):
-        super().__init__(target_name=target_name, compress_type=compress_type, **kwargs)
+    def __init__(self, target_name: str, compress_type: CompressType, lookups: Codecs, **kwargs):
+        super().__init__(target_name=target_name, compress_type=compress_type, lookups=lookups, **kwargs)
         self.tagged_frames: list[pd.DataFrame] = []
 
-    def flush(self, tagged_frame: pd.DataFrame, dispatch_items: list[IDispachItem]):
+    def flush(self, tagged_frame: pd.DataFrame, dispatch_items: list[IDispatchItem]):
         self.tagged_frames.append(tagged_frame)
 
     def close_target(self) -> None:
         super().close_target()
         total_frame: pd.DataFrame = pd.concat(self.tagged_frames, ignore_index=True)
         self.store(filename=self.corpus_name, data=total_frame)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/dispatch/item.py` & `pyriksprot-2023.4.1/pyriksprot/dispatch/item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
 from ..corpus import ProtocolSegment
-from ..interface import ContentType, IDispachItem
-from ..utility import merge_tagged_csv
+from ..interface import ContentType, IDispatchItem
+from ..utility import merge_csv_strings
 
 
 @dataclass
-class DispatchItem(IDispachItem):
+class DispatchItem(IDispatchItem):
     """Groups segments for dispatch to a zink.
     One item corresponds to either...
      - A single document made up of the aggregate of contained segments
      - A set of documents, one for each contained segment
     """
 
     year: int
@@ -34,20 +34,20 @@
     def document_name(self) -> str:
         if self.group_name.startswith(self.group_temporal_value or ""):
             return self.group_name
         return f'{self.group_temporal_value}_{self.group_name}'
 
     @property
     def filename(self) -> str:
-        return f'{self.document_name}.{self._extension}'
+        return f'{self.document_name}.{self.extension}'
 
     @property
     def text(self) -> str:
         return (
-            merge_tagged_csv(self._get_texts(), sep='\n')
+            merge_csv_strings(self._get_texts(), sep='\n')
             if self.content_type == ContentType.TaggedFrame
             else '\n'.join(self._get_texts())
         )
 
     def to_dict(self):
         return {
             'year': self.year,
@@ -60,14 +60,14 @@
 
     """Not public"""
 
     def _get_texts(self) -> list[str]:
         return [s.data for s in self.protocol_segments]
 
     @property
-    def _extension(self) -> str:
+    def extension(self) -> str:
         return 'txt' if self.content_type == ContentType.Text else 'csv'
 
     """Not used"""
     # @property
     # def group_keys(self) -> list[str]:
     #     return list(self.group_values.keys())
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/dispatch/merge.py` & `pyriksprot-2023.4.1/pyriksprot/dispatch/utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,140 @@
 from __future__ import annotations
 
-from typing import Iterable
-
-from loguru import logger
+import hashlib
+from os.path import splitext
+from typing import Any, Callable
 
+from .. import metadata as md
+from .. import utility
 from ..corpus import corpus_index, iterate
-from ..interface import GroupingKey, SegmentLevel, TemporalKey
-from .item import DispatchItem
-from .utility import create_grouping_hashcoder
+from ..interface import TemporalKey
 
-# pylint: disable=too-many-arguments, unbalanced-tuple-unpacking
+# pylint: disable=unbalanced-tuple-unpacking
 
 
-class SegmentMerger:
-    """Merge stream of segments based on temporal and grouping keys
+def hashcoder_with_no_grouping_keys(item: iterate.ProtocolSegment, **_) -> tuple[dict, str, str]:
+    return ({}, item.name, hashlib.md5(item.name.encode('utf-8')).hexdigest())
 
-    Temporal aggregation is performed before group aggregation.
-    This reducer assumes that data is sorted by the temporal key.
 
-    The temporal key can be None, Year, Lustrum, Decade or Custom.
-    Temporal value is a tuple (from-year, to-year)
+def take(d: dict, properties: set[str]) -> dict:
+    return {k: v for k, v in (d.items() or {}) if k in properties}
 
-    NOTE! if multiprocessing, then all items belonging to same temporal category
-    must be distributed to the same process!
 
-    """
+def probe(x: Any, properties: set[str]) -> dict:
+    return {k: getattr(x, k) for k in properties if hasattr(x, k)}
 
-    def __init__(
-        self,
-        *,
-        source_index: corpus_index.CorpusSourceIndex,
-        temporal_key: TemporalKey,
-        grouping_keys: list[GroupingKey],
-    ):
-        """Setup merger.
 
-        Args:
-            source_index (corpus_index.CorpusSourceIndex): Source item index.
-            speaker_service (person.SpeakerInfoService): Parliamentary speaker helper service.
-            temporal_key (TemporalKey): Temporal key None, 'Year', 'Decade', 'Lustrum', 'Custom', 'Protocol', None
-            grouping_keys (list[GroupingKey]): Grouping within temporal key
-        """
+def create_grouping_hashcoder(
+    grouping_keys: list[str],
+) -> Callable[[iterate.ProtocolSegment, corpus_index.ICorpusSourceItem], str]:
+    """Create a hashcode function for given grouping keys"""
 
-        self.source_index: corpus_index.CorpusSourceIndex = source_index
-        self.temporal_key: TemporalKey = temporal_key
-        self.grouping_keys: list[GroupingKey] = grouping_keys or []
-        self.grouping_hashcoder = create_grouping_hashcoder(self.grouping_keys)
+    grouping_keys: set[str] = set(grouping_keys)
 
-    def merge(
-        self, iterator: list[iterate.ProtocolSegment] | iterate.ProtocolSegmentIterator
-    ) -> Iterable[dict[str, DispatchItem]]:
-        """Merges stream of protocol segments based on grouping keys. Yield merged groups continously.
-        Note: value of `item.id` depends on aggregation level, it is u_id for levels speech and utterance.
-        """
+    if not grouping_keys:
+        """No grouping apart from temporal key"""
+        return hashcoder_with_no_grouping_keys
 
-        hashcoder = self.grouping_hashcoder
+    def hashcoder(item: iterate.ProtocolSegment, source_item: corpus_index.ICorpusSourceItem) -> tuple[dict, str, str]:
+        """Compute hash for item, speaker and source item. Return values, hash string and hash code"""
+        assert issubclass(type(source_item), corpus_index.ICorpusSourceItem)
+        parts: dict[str, str | int] = {
+            # **take(item.speaker_info.asdict(), grouping_keys),
+            # **take(source_item.to_dict(), grouping_keys),
+            # **take(item.to_dict(), grouping_keys),
+            **probe(item.speaker_info.term_of_office, grouping_keys),
+            **probe(item.speaker_info, grouping_keys),
+            **probe(source_item, grouping_keys),
+            **probe(item, grouping_keys),
+        }
+        missing: set[str] = grouping_keys - set(parts.keys())
+        if len(missing) > 0:
+            raise ValueError(f"unknown keys: {', '.join(list(missing))}")
 
-        try:
-            current_temporal_value: str = None
-            current_group: dict[str, DispatchItem] = {}
-            grouping_keys: set[str] = set(self.grouping_keys)
-            source_item: corpus_index.CorpusSourceItem
+        hashcode_str = utility.slugify('_'.join(str(x).lower().replace(' ', '_') for x in parts.values()))
 
-            if grouping_keys and getattr(iterator, 'segment_level', None) == SegmentLevel.Protocol:
-                raise ValueError("cannot group by key (within protocol) when segement level is entire protocol.")
+        return (parts, hashcode_str, hashlib.md5(hashcode_str.encode('utf-8')).hexdigest())
 
-            for item in iterator:
+    return hashcoder if grouping_keys else hashcoder_with_no_grouping_keys
 
-                source_item = self.source_index[item.protocol_name]
 
-                if not bool(source_item):
-                    logger.error(f"source item not found: {item.name}")
-                    continue
+def truncate_year_to_category(year: int, temporal_key: TemporalKey) -> int:
+    """truncates year to closest lustrum or decade."""
+    if temporal_key == TemporalKey.Decade:
+        return year - year % 10
+    if temporal_key == TemporalKey.Lustrum:
+        return year - year % 5
+    return year
 
-                temporal_value: str = self.to_temporal_value(item)
 
-                if current_temporal_value != temporal_value:
-                    """Yield previous group"""
-                    if current_group:
-                        yield current_group
+def to_temporal_category(temporal_key: str | TemporalKey | dict, year: int, default_value: str) -> str:
+    if isinstance(temporal_key, (TemporalKey, str, type(None))):
+        if temporal_key == TemporalKey.Year:
+            return str(year)
 
-                    current_group, current_temporal_value = {}, temporal_value
+        if temporal_key == TemporalKey.Lustrum:
+            low_year: int = year - (year % 5)
+            return f"{low_year}-{low_year+4}"
 
-                grouping_values, hashcode_str, hashcode = hashcoder(item=item, source_item=source_item)
+        if temporal_key == TemporalKey.Decade:
+            low_year: int = year - (year % 10)
+            return f"{low_year}-{low_year+9}"
 
-                # FIXME: #14 This fix cannot work. It prevents groupings that exclude `who` added https://github.com/welfare-state-analytics/pyriksprot/commit/8479a7c03458adcc0a0f0d0750cf48e55eec4bb0
-                grouping_values['who'] = item.who
+        return default_value
 
-                if hashcode not in current_group:
+    if isinstance(temporal_key, dict):
+        """custom periods as a dict {'category-name': (from_year,to_year), ...}"""
+        for k, v in temporal_key:
+            if v[0] <= year <= v[1]:
+                return k
 
-                    current_group[hashcode] = DispatchItem(
-                        segment_level=item.segment_level,
-                        content_type=item.content_type,
-                        group_name=hashcode_str,
-                        group_hash=hashcode,
-                        group_temporal_value=temporal_value,
-                        group_values=grouping_values,
-                        year=source_item.year,
-                        protocol_segments=[],
-                        n_tokens=0,
-                    )
+    raise ValueError(f"temporal period failed for {default_value}")
 
-                current_group[hashcode].add(item)
 
-            """Yield last group"""
-            if current_group:
-                yield current_group
+def decode_protocol_segment_filename(lookups: md.Codecs, speech: iterate.ProtocolSegment, naming_keys: list[str]):
+    basename, extension = splitext(speech.filename)
 
-        except Exception as ex:
-            logger.exception(ex)
-            raise
+    suffix: str = ""
 
-    def to_year(self, source_item: corpus_index.CorpusSourceItem, temporal_key: TemporalKey) -> int:
-        """Compute a year that represents the group."""
-        if temporal_key == TemporalKey.Decade:
-            return source_item.year - source_item.year % 10
-        if temporal_key == TemporalKey.Lustrum:
-            return source_item.year - source_item.year % 5
-        return source_item.year
+    for key in naming_keys:
+        if hasattr(speech, key):
+            key_value: int = getattr(speech, key)
+        elif hasattr(speech.speaker_info, key):
+            key_value: int = getattr(speech.speaker_info, key)
+        else:
+            raise ValueError(f"attribute {key} not found")
+
+        key_value_label: str = lookups.lookup_name(key, key_value, "unknown")
+
+        suffix = f"{suffix}_{key_value_label}"
+
+    if speech.speaker_info is not None:
+        suffix += f"_{speech.speaker_info.name[:80]}_{speech.speaker_info.person_id}"
+
+    suffix = utility.slugify(suffix.lower(), True)
+
+    filename: str = f"{basename}_{suffix}{extension}"
+    return filename
+
+
+# def _split_properties_by_dataclass(properties: set[str], *cls_list: tuple[Type, ...]) -> tuple[set[str], ...]:
+
+#     properties = set(properties)
 
-    def to_temporal_value(self, item: iterate.ProtocolSegment) -> str:
+#     key_sets: list[set[str]] = []
 
-        year: int = item.year
-        if isinstance(self.temporal_key, (TemporalKey, str, type(None))):
+#     for cls in cls_list:
 
-            if self.temporal_key in [None, '', 'document', 'protocol', TemporalKey.NONE]:
-                """No temporal key gives a group per document/protocol"""
-                return item.protocol_name
+#         if not is_dataclass(cls):
+#             raise ValueError(f"{cls.__name__} is not a dataclass")
 
-            if self.temporal_key == TemporalKey.Year:
-                return str(year)
+#         key_set: set[str] = properties.intersection({f.name for f in fields(cls)})
 
-            if self.temporal_key == TemporalKey.Lustrum:
-                low_year: int = year - (year % 5)
-                return f"{low_year}-{low_year+4}"
+#         properties -= key_set
 
-            if self.temporal_key == TemporalKey.Decade:
-                low_year: int = year - (year % 10)
-                return f"{low_year}-{low_year+9}"
+#         key_sets.append(key_set)
 
-        elif isinstance(self.temporal_key, dict):
-            """custom periods as a dict {'category-name': (from_year,to_year), ...}"""
-            for k, v in self.temporal_key:
-                if v[0] <= year <= v[1]:
-                    return k
+#     if properties:
+#         raise ValueError(f"split_properties_by_dataclass: {','.join(properties)} not found.")
 
-        raise ValueError(f"temporal period failed for {item.protocol_name}")
+#     return tuple(key_sets)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv` & `pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/foss/bettertokenizer.sv.saldo-tokens` & `pyriksprot-2023.4.1/pyriksprot/foss/bettertokenizer.sv.saldo-tokens`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/foss/pos_tags.py` & `pyriksprot-2023.4.1/pyriksprot/foss/pos_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,42 +214,39 @@
 
         """Add lowercased keys to maps"""
         self.pos_to_id: dict = self.pos_to_id | {k.lower(): v for k, v in self.pos_to_id.items()}
         self.tag_to_group: dict = self.tag_to_group | {k.lower(): v for k, v in self.tag_to_group.items()}
 
     @property
     def tags(self) -> List[str]:
-
         return list(self.PD_PoS_tags.index)
 
     def unwrap(self, x: Any) -> Any:
         if isinstance(x, str):
             if x in self.groups:
                 return self.groups[x]
             if '|' in x:
                 return str_to_pos_tags(x)
             return x
         return list(x)
 
     def exclude(self, excludes: Union[str, Container[str]] = None) -> List[str]:
-
         _all_tags = list(self.PD_PoS_tags.index)
 
         if excludes is None:
             return _all_tags
 
         if isinstance(excludes, str):
             excludes = [excludes]
 
         excludes = set(collapse(map(self.unwrap, excludes)))
 
         return [x for x in _all_tags if x not in excludes]
 
     def all_types_except(self, tags: Union[str, Container[str]] = None) -> List[str]:
-
         return self.exclude([tags, self.Delimiter])
 
     @property
     def Pronoun(self) -> List[str]:
         return self.groups.get('Pronoun', [])
 
     @property
@@ -327,15 +324,14 @@
     Universal=PoS_Tag_Scheme(PD_Universal_PoS_tags),
     PennTree=PoS_Tag_Scheme(PD_PennTree_O5_PoS_tags),
 )
 
 
 @dataclass
 class PoS_Tag_Schemes:
-
     SUC: PoS_Tag_Scheme = PoS_Tag_Scheme(PD_SUC_PoS_tags)
     Universal: PoS_Tag_Scheme = PoS_Tag_Scheme(PD_Universal_PoS_tags)
     PennTree: PoS_Tag_Scheme = PoS_Tag_Scheme(PD_PennTree_O5_PoS_tags)
 
 
 PoS_TAGS_SCHEMES = PoS_Tag_Schemes()
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/foss/sparv_tokenize.py` & `pyriksprot-2023.4.1/pyriksprot/foss/sparv_tokenize.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,20 +166,18 @@
             begin += len(w)
 
 
 sparv_better_tokenizer = None
 
 
 class ModelNotFoundError(Exception):
-
     ...
 
 
 def default_tokenize(text: str) -> List[str]:
-
     global sparv_better_tokenizer
 
     sparv_better_tokenizer = sparv_better_tokenizer or BetterWordTokenizer(
         model=MODEL_FILENAME, token_list=SALDO_TOKENS_FILENAME
     )
 
     span_tokens = list(sparv_better_tokenizer.span_tokenize(text))
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/foss/stopwords.py` & `pyriksprot-2023.4.1/pyriksprot/foss/stopwords.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2022.5.2/pyriksprot/foss/untangle.py` & `pyriksprot-2023.4.1/pyriksprot/foss/untangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,27 @@
         return ''.join(self.cdatas)
 
     @cdata.setter
     def cdata(self, cdata):
         self.cdatas = [cdata]
 
     def add_child(self, element: "Element") -> None:
-        """ Store child elements. """
+        """Store child elements."""
         self.children.append(element)
 
     def add_cdata(self, cdata: str) -> None:
-        """ Store cdata """
+        """Store cdata"""
         self.cdatas.append(cdata)
 
     def get_attribute(self, key) -> Optional[str]:
-        """ Get attributes by key """
+        """Get attributes by key"""
         return self.attributes.get(key)
 
     def get_elements(self, name: str = None) -> List["Element"]:
-        """ Find a child element by name """
+        """Find a child element by name"""
         if name:
             return [e for e in self.children if e.name == name]
         return self.children
 
     def __getitem__(self, key):
         return self.get_attribute(key)
 
@@ -132,15 +132,14 @@
 
         self.root: Element = Element(None, None)
         self.root.is_root = True
         self.elements: List[Element] = []
         self.ignore_tags: Set[str] = set(ignore_tags or [])
 
     def startElement(self, name: str, attrs: Mapping[str, str]) -> None:
-
         if name in self.ignore_tags:
             return
 
         name = name.replace("-", "_").replace(".", "_").replace(":", "_")
 
         if keyword.iskeyword(name):
             name += "_"
@@ -149,15 +148,14 @@
         if len(self.elements) > 0:
             self.elements[-1].add_child(element)
         else:
             self.root.add_child(element)
         self.elements.append(element)
 
     def endElement(self, name: str) -> None:
-
         if name in self.ignore_tags:
             return
 
         self.elements.pop()
 
     def characters(self, content: str) -> None:
         # self.elements[-1].add_cdata(content)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/interface.py` & `pyriksprot-2023.4.1/pyriksprot/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import contextlib
 import csv
 import hashlib
 import re
 from dataclasses import dataclass, field
 from enum import Enum
 from io import StringIO
-from typing import Any, Callable, Mapping, Optional, Union
+from typing import Any, Callable, Literal, Mapping, Optional, Union
 
 import pandas as pd
 from pandas.io import json
 
-from pyriksprot.corpus.parlaclarin.parse import MISSING_SPEAKER_NOTE_ID
-
-from .utility import flatten, merge_tagged_csv, strip_extensions
+from .utility import flatten, merge_csv_strings, strip_extensions
 
 # pylint: disable=too-many-arguments, no-member
 
+MISSING_SPEAKER_NOTE_ID: str = "missing"
+
 
 class ParlaClarinError(ValueError):
     ...
 
 
 class TemporalKey(str, Enum):
     NONE = None
@@ -69,15 +69,15 @@
     JSON = 'json'
 
 
 PARAGRAPH_MARKER: str = '@#@'
 
 
 @dataclass
-class IDispachItem(abc.ABC):
+class IDispatchItem(abc.ABC):
     segment_level: SegmentLevel
     content_type: ContentType
     n_tokens: int
 
     @property
     def filename(self) -> str:
         ...
@@ -87,56 +87,77 @@
         ...
 
     def to_dict(self):
         ...
 
 
 class IProtocol(abc.ABC):
-    ...
+    date: str
+    name: str
+    utterances: list[Utterance]
+    speaker_notes: dict[str, str]
+
+    @abc.abstractmethod
+    def get_year(self, which: Literal["filename", "date"] = "filename") -> int:
+        ...
+
+    @abc.abstractmethod
+    def preprocess(self, preprocess: Callable[[str], str] = None) -> "Protocol":
+        ...
+
+    @abc.abstractmethod
+    def checksum(self) -> Optional[str]:
+        ...
+
+    @abc.abstractmethod
+    def get_content(self, content_type: ContentType) -> str:
+        ...
+
+    @abc.abstractmethod
+    def get_speaker_notes(self) -> dict[str, str]:
+        ...
+
+
+@dataclass
+class SpeakerNote:
+    speaker_note_id: str
+    speaker_note: str
+
+
+MISSING_SPEAKER_NOTE: SpeakerNote = SpeakerNote(MISSING_SPEAKER_NOTE_ID, "")
 
 
 class Utterance:
     """Represents an utterance in the ParlaClarin XML file"""
 
     delimiter: str = '\n'
 
     def __init__(
         self,
         *,
         u_id: str,
-        speaker_note_id: str,
         who: str,
-        n: str = "",
         prev_id: str = None,
         next_id: str = None,
         paragraphs: Union[list[str], str] = None,
         annotation: Optional[str] = None,
-        page_number: Optional[str] = '',
+        page_number: Optional[int] = 0,
+        speaker_note_id: str = MISSING_SPEAKER_NOTE.speaker_note_id,
         **_,
     ):
-
-        if not speaker_note_id:
-            speaker_note_id = MISSING_SPEAKER_NOTE_ID
-            # FIXME #15 Exists utterances in data not preceeded by a speakers's intro note
-            # logger.warning(f"utterance {u_id}: empty speaker_note_id")
-            # raise ValueError(f"utterance {u_id}: empty speaker_note_id not allowed")
-
         self.u_id: str = u_id
-        self.n: str = n
         self.who: str = who
         self.prev_id: str = prev_id if isinstance(prev_id, str) else None
         self.next_id: str = next_id if isinstance(next_id, str) else None
         self.paragraphs: list[str] = (
             [] if not paragraphs else paragraphs if isinstance(paragraphs, list) else paragraphs.split(PARAGRAPH_MARKER)
         )
         self.annotation: Optional[str] = annotation if isinstance(annotation, str) else None
-        self.page_number: Optional[str] = page_number if isinstance(page_number, str) else ''
-        self.speaker_note_id: Optional[str] = (
-            speaker_note_id if isinstance(speaker_note_id, str) else MISSING_SPEAKER_NOTE_ID
-        )
+        self.page_number: Optional[int] = page_number if isinstance(page_number, int) else None
+        self.speaker_note_id: str = speaker_note_id
 
     @property
     def is_unknown(self) -> bool:
         return self.who == "unknown"
 
     @property
     def document_name(self) -> str:
@@ -149,60 +170,78 @@
     @property
     def text(self) -> str:
         """Merge utterance paragraphs. Return text."""
         return self.delimiter.join(p for p in self.paragraphs if p != '').strip()
 
     def checksum(self) -> str:
         """Compute checksum of utterance text."""
-        return hashlib.sha1(self.text.encode('utf-8')).hexdigest()[:16]
+        return UtteranceHelper.compute_checksum(self.text)
 
     def to_str(self, what: ContentType) -> str:
         return self.tagged_text if what == ContentType.TaggedFrame else self.text
 
+    def to_dict(self) -> dict:
+        return UtteranceHelper.to_dict(self)
 
-class UtteranceHelper:
 
+class UtteranceHelper:
     CSV_OPTS = dict(
         quoting=csv.QUOTE_MINIMAL,
         escapechar="\\",
         doublequote=False,
         sep='\t',
     )
 
     @staticmethod
-    def to_dict(utterances: list[Utterance]) -> list[Mapping[str, Any]]:
+    def compute_paragraph_checksum(text: str | list[str]) -> str:
+        """Compute checksum of given text."""
+        if isinstance(text, str) and PARAGRAPH_MARKER in text:
+            text = text.split(PARAGRAPH_MARKER)
+
+        if isinstance(text, list):
+            text = Utterance.delimiter.join(p for p in text if p != '').strip()
+
+        return UtteranceHelper.compute_checksum(text or "")
+
+    @staticmethod
+    def compute_checksum(text: str) -> str:
+        """Compute checksum of given text."""
+        return hashlib.sha1(text.encode('utf-8')).hexdigest()[:16]
+
+    @staticmethod
+    def to_dict(u: Utterance) -> dict[str, Any]:
+        return {
+            'u_id': u.u_id,
+            'who': u.who,
+            'speaker_note_id': u.speaker_note_id,
+            'prev_id': u.prev_id,
+            'next_id': u.next_id,
+            'annotation': u.tagged_text,
+            'paragraphs': PARAGRAPH_MARKER.join(u.paragraphs),
+            'page_number': u.page_number,
+            'checksum': u.checksum(),
+        }
+
+    @staticmethod
+    def to_dicts(utterances: list[Utterance]) -> list[Mapping[str, Any]]:
         """Convert list of utterances to a list of dicts. Return the list."""
-        return [
-            {
-                'u_id': u.u_id,
-                'n': u.n,
-                'who': u.who,
-                'speaker_note_id': u.speaker_note_id,
-                'prev_id': u.prev_id,
-                'next_id': u.next_id,
-                'annotation': u.tagged_text,
-                'paragraphs': PARAGRAPH_MARKER.join(u.paragraphs),
-                'page_number': u.page_number or '',
-                'checksum': u.checksum(),
-            }
-            for u in utterances
-        ]
+        return [UtteranceHelper.to_dict(u) for u in utterances]
 
     @staticmethod
     def to_dataframe(utterances: Union[StringIO, str, list[Utterance]]) -> pd.DataFrame:
         """Convert list of utterances, CSV string or a CSV file to a dataframe."""
         if isinstance(utterances, (str, StringIO)):
             df: pd.DataFrame = pd.read_csv(
                 StringIO(utterances) if isinstance(utterances, str) else utterances,
                 **UtteranceHelper.CSV_OPTS,
                 index_col='u_id',
             )
             df.drop(columns='checksum')
         else:
-            df: pd.DataFrame = pd.DataFrame(UtteranceHelper.to_dict(utterances)).set_index('u_id')
+            df: pd.DataFrame = pd.DataFrame(UtteranceHelper.to_dicts(utterances)).set_index('u_id')
         return df
 
     @staticmethod
     def to_csv(utterances: list[Utterance]) -> str:
         """Convert list of utterances to a CSV string. Return CSV string."""
         return UtteranceHelper.to_dataframe(utterances=utterances).to_csv(**UtteranceHelper.CSV_OPTS, index=True)
 
@@ -224,19 +263,19 @@
         """Convert JSON string to list of utterances. Return list."""
         data: list[Utterance] = list(map(lambda x: Utterance(**x), json.loads(json_str)))
         return data
 
     @staticmethod
     def merge_tagged_texts(utterances: list[Utterance], sep: str = '\n') -> str:
         """Merge annotations into a single tagged CSV string"""
-        return merge_tagged_csv([u.tagged_text for u in (utterances or [])], sep=sep)
+        return merge_csv_strings([u.tagged_text for u in (utterances or [])], sep=sep)
 
     @staticmethod
     def merge_tagged_csv(csv_strings: list[str], sep: str = '\n') -> str:
-        return merge_tagged_csv(csv_strings, sep=sep)
+        return merge_csv_strings(csv_strings, sep=sep)
 
 
 class UtteranceMixIn:
     def to_text(self, *, sep: str = '\n', require_letter: bool = False) -> str:
         t: str = sep.join(t for t in (u.text for u in self.utterances) if t != '')
         if require_letter and not re.search('[a-zåäöA-ZÅÄÖ]', t):
             """Empty string if no letter in text"""
@@ -261,15 +300,15 @@
     @property
     def has_tagged_text(self) -> bool:
         """Check if any utterance actually has any uttered words."""
         return any(bool(u.tagged_text) for u in self.utterances)
 
     def to_dict(self) -> list[Mapping[str, Any]]:
         """Convert utterances to list of dict."""
-        return UtteranceHelper.to_dict(self.utterances)
+        return UtteranceHelper.to_dicts(self.utterances)
 
     def to_dataframe(self) -> pd.DataFrame:
         """Convert utterances to dataframe"""
         return UtteranceHelper.to_dataframe(self.utterances)
 
     def to_csv(self) -> str:
         """Convert utterances to CSV string"""
@@ -302,24 +341,23 @@
 
     protocol_name: str
     document_name: str
     speech_id: str
     who: str
     speech_date: str
     speech_index: int
-    page_number: str
+    page_number: int
 
     utterances: list[Utterance] = field(default_factory=list)
 
     num_tokens: int = 0
     num_words: int = 0
     delimiter: str = field(default='\n')
 
     def __post_init__(self):
-
         if len(self.utterances or []) == 0:
             raise ParlaClarinError("utterance list cannot be empty")
 
         if any(self.who != u.who for u in self.utterances):
             raise ParlaClarinError("multiple speakers in same speech not allowed")
 
     @property
@@ -338,39 +376,50 @@
         return MISSING_SPEAKER_NOTE_ID if not self.utterances else self.utterances[0].speaker_note_id
 
     def add(self, item: Utterance) -> "Speech":
         self.utterances.append(item)
         return self
 
 
-class Protocol(UtteranceMixIn):
+class Protocol(UtteranceMixIn, IProtocol):
     """Entity that represents a ParlaCLARIN document."""
 
     def __init__(self, date: str, name: str, utterances: list[Utterance], speaker_notes: dict[str, str], **_):
         self.date: str = date
         self.name: str = name
         self.utterances: list[Utterance] = utterances
-        self.year: int = int(self.date[:4])
         self.speaker_notes: dict[str, str] = speaker_notes or {}
 
+    def get_year(self, which: Literal["filename", "date"] = "filename") -> int:
+        """Returns protocol's year either extracted from filename or from `date` tag in XML header"""
+        if which != "filename":
+            return int(self.date[:4])
+        return int(self.name.split("-")[1][:4])
+
     def preprocess(self, preprocess: Callable[[str], str] = None) -> "Protocol":
         """Apply text transforms. Return self."""
 
         if preprocess is None:
             return self
 
-        for utterance in self.utterances:
-            utterance.paragraphs = [preprocess(p.strip()) for p in utterance.paragraphs]
+        for uttr in self.utterances:
+            uttr.paragraphs = [preprocess(p.strip()) for p in uttr.paragraphs]
 
         return self
 
     def checksum(self) -> Optional[str]:
         """Compute checksum for entire text."""
         with contextlib.suppress(Exception):
             return hashlib.sha1(''.join(u.text for u in self.utterances).encode('utf-8')).hexdigest()
         return None
 
     def get_content(self, content_type: ContentType) -> str:
         return self.text if content_type == ContentType.Text else self.tagged_text
 
     def get_speaker_notes(self) -> dict[str, str]:
         return self.speaker_notes
+
+
+class IProtocolParser(abc.ABC):
+    @staticmethod
+    def parse(filename: str, ignore_tags: set[str]) -> IProtocol:  # pylint: disable=unused-argument
+        ...
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/metadata/codecs.py` & `pyriksprot-2023.4.1/pyriksprot/metadata/codecs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from contextlib import nullcontext
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Callable, Literal, Mapping
 
 import pandas as pd
 
+from .. import utility as pu
 from . import utility as mdu
 
 CODE_TABLES: dict[str, str] = {
     'chamber': 'chamber_id',
     'gender': 'gender_id',
     'government': 'government_id',
     'office_type': 'office_type_id',
@@ -21,15 +22,15 @@
 
 
 @dataclass
 class Codec:
     type: Literal['encoder', 'decoder']
     from_column: str
     to_column: str
-    fx: Callable[[int], str]
+    get: Callable[[int], str]
     default: str = None
 
 
 null_frame: pd.DataFrame = pd.DataFrame()
 
 
 class Codecs:
@@ -39,79 +40,87 @@
         self.government: pd.DataFrame = null_frame
         self.office_type: pd.DataFrame = null_frame
         self.party: pd.DataFrame = null_frame
         self.sub_office_type: pd.DataFrame = null_frame
         self.extra_codecs: list[Codec] = []
 
     def load(self, source: str | sqlite3.Connection | dict) -> Codecs:
-        with (sqlite3.connect(database=source) if isinstance(source, str) else nullcontext(source)) as db:
+        with sqlite3.connect(database=source) if isinstance(source, str) else nullcontext(source) as db:
             tables: dict[str, pd.DataFrame] = mdu.load_tables(CODE_TABLES, db=db)
             for table_name, table in tables.items():
                 setattr(self, table_name, table)
         return self
 
     @cached_property
     def gender2name(self) -> dict:
         return self.gender['gender'].to_dict()
 
     @cached_property
     def gender2id(self) -> dict:
-        return mdu.revdict(self.gender2name)
+        return pu.revdict(self.gender2name)
 
     @cached_property
     def office_type2name(self) -> dict:
         return self.office_type['office'].to_dict()
 
     @cached_property
     def office_type2id(self) -> dict:
-        return mdu.revdict(self.office_type2name)
+        return pu.revdict(self.office_type2name)
 
     @cached_property
     def sub_office_type2name(self) -> dict:
         return self.sub_office_type['description'].to_dict()
 
     @cached_property
     def sub_office_type2id(self) -> dict:
-        return mdu.revdict(self.sub_office_type2name)
+        return pu.revdict(self.sub_office_type2name)
 
     @cached_property
     def party_abbrev2name(self) -> dict:
         return self.party['party_abbrev'].to_dict()
 
     @cached_property
     def party_abbrev2id(self) -> dict:
-        return mdu.revdict(self.party_abbrev2name)
+        return pu.revdict(self.party_abbrev2name)
 
     @property
     def codecs(self) -> list[Codec]:
         return self.extra_codecs + [
             Codec('decode', 'gender_id', 'gender', self.gender2name.get),
             Codec('decode', 'office_type_id', 'office_type', self.office_type2name.get),
             Codec('decode', 'party_id', 'party_abbrev', self.party_abbrev2name.get),
             Codec('decode', 'sub_office_type_id', 'sub_office_type', self.sub_office_type2name.get),
             Codec('encode', 'gender', 'gender_id', self.gender2id.get),
             Codec('encode', 'office_type', 'office_type_id', self.office_type2id.get),
             Codec('encode', 'party', 'party_id', self.party_abbrev2id.get),
             Codec('encode', 'sub_office_type', 'sub_office_type_id', self.sub_office_type2id.get),
         ]
 
+    def lookup_name(self, key: str, key_id: int, default_value: str = "unknown") -> str:
+        return self.decoder(key=key).get(key_id, default_value)
+
+    def decoder(self, key: str) -> Codec:
+        return next((x for x in self.decoders if x.from_column == key), {})
+
+    def encoder(self, key: str) -> Codec:
+        return next((x for x in self.encoders if x.from_column == key), lambda _: 0)
+
     @property
     def decoders(self) -> list[Codec]:
         return [c for c in self.codecs if c.type == 'decode']
 
     @property
     def encoders(self) -> list[dict]:
         return [c for c in self.codecs if c.type == 'encode']
 
     def apply_codec(self, df: pd.DataFrame, codecs: list[Codec], drop: bool = True) -> pd.DataFrame:
-
         for codec in codecs:
             if codec.from_column in df.columns:
                 if codec.to_column not in df:
-                    df[codec.to_column] = df[codec.from_column].apply(codec.fx)
+                    df[codec.to_column] = df[codec.from_column].apply(codec.get)
                 if codec.default is not None:
                     df[codec.to_column] = df[codec.to_column].fillna(codec.default)
             if drop:
                 df.drop(columns=[codec.from_column], inplace=True, errors='ignore')
         return df
 
     def decode(self, df: pd.DataFrame, drop: bool = True) -> pd.DataFrame:
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/metadata/utterance.py` & `pyriksprot-2023.4.1/pyriksprot/metadata/utterance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 from __future__ import annotations
 
-import sqlite3
-from contextlib import nullcontext
 from functools import cached_property
 
 import pandas as pd
 
-from . import utility as mdu
-
-DATA_TABLES: dict[str, str] = {
-    'protocols': 'document_id',
-    'utterances': 'u_id',
-    'unknown_utterance_gender': 'u_id',
-    'unknown_utterance_party': 'u_id',
-}
+from . import generate
 
 null_frame: pd.DataFrame = pd.DataFrame()
 
 
 class UtteranceIndex:
     def __init__(self):
-
         self.protocols: pd.DataFrame = null_frame
         self.utterances: pd.DataFrame = null_frame
         self.unknown_utterance_gender: pd.DataFrame = null_frame
         self.unknown_utterance_party: pd.DataFrame = null_frame
 
-    def load(self, source: str | sqlite3.Connection | dict) -> UtteranceIndex:
-        with (sqlite3.connect(database=source) if isinstance(source, str) else nullcontext(source)) as db:
-            tables: dict[str, pd.DataFrame] = mdu.load_tables(DATA_TABLES, db=db)
-            for table_name, table in tables.items():
-                setattr(self, table_name, table)
+        self._table_infos: dict[str, str] = {
+            'protocols': 'document_id',
+            'utterances': 'u_id',
+            'unknown_utterance_gender': 'u_id',
+            'unknown_utterance_party': 'u_id',
+        }
+
+    def load(self, database_filename: str) -> UtteranceIndex:
+        tables: dict[str, pd.DataFrame] = generate.DatabaseHelper(database_filename).load_data_tables(self._table_infos)
+        for table_name, table in tables.items():
+            setattr(self, table_name, table)
         return self
 
     @cached_property
     def unknown_party_lookup(self) -> dict[str, int]:
         """Utterance `u_id` to `party_id` mapping"""
         return self.unknown_utterance_party['party_id'].to_dict()
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/scripts/fix_speaker_notes.py` & `pyriksprot-2023.4.1/pyriksprot/scripts/fix_speaker_notes.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from pyriksprot import metadata as md
 from pyriksprot.corpus.tagged.persist import update_speaker_note_id
 
 jj = os.path.join
 relpath = os.path.relpath
 
+
 # FIXME #20 Tagging does not assign correct speaker hashes to utterances
 def temporary_update(tag: str, target_tag: str):
-
     source_folder: str = f"/data/riksdagen_corpus_data/tagged_frames_{tag}"
     target_folder: str = f"/data/riksdagen_corpus_data/tagged_frames_{target_tag}"
     database_filename: str = f"/data/riksdagen_corpus_data/metadata/riksprot_metadata.{tag}.db"
 
     service = md.SpeakerInfoService(database_filename)
     speaker_note_id_lookup = service.utterance_index.utterances['speaker_note_id'].to_dict()
     update_speaker_note_id(speaker_note_id_lookup, source_folder, target_folder)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/scripts/metadata2db.py` & `pyriksprot-2023.4.1/pyriksprot/workflows/subset_corpus.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,60 @@
-import sys
-from os.path import dirname
-
-import click
-from loguru import logger
+import os
+import shutil
+from os.path import join as jj
 
+from pyriksprot import corpus as pc
 from pyriksprot import metadata as md
 from pyriksprot.corpus.parlaclarin import ProtocolMapper
+from pyriksprot.utility import reset_folder
 
 
-@click.group(help="CLI tool to manage riksprot metadata")
-def main():
-    pass
-
-
-@click.command()
-@click.argument('tag', type=click.STRING)
-@click.argument('target_folder', type=click.STRING)
-def download_metadata(tag: str, target_folder: str):
-    md.download_to_folder(tag=tag, folder=target_folder, force=True)
-
-
-@click.command()
-@click.argument('corpus_folder', type=click.STRING)
-@click.argument('target_folder', type=click.STRING)
-def create_utterance_index(corpus_folder: str, target_folder: str):
-    md.generate_corpus_indexes(ProtocolMapper, corpus_folder=corpus_folder, target_folder=target_folder)
-
-
-@click.command()
-@click.argument('target', type=click.STRING)
-@click.option('--branch', type=click.STRING, help='Text or tags', default=None)
-@click.option('--source-folder', type=click.STRING, default=None)
-@click.option('--force', type=click.BOOL, is_flag=True, help='Force overwrite', default=False)
-@click.option('--load-index', type=click.BOOL, is_flag=True, help='Load utterance index', default=False)
-@click.option('--scripts-folder', type=click.STRING, help='If set, apply scripts in folder to DB', default=None)
-def create_database(
-    target: str,
-    branch: str = None,
-    source_folder: str = None,
-    force: bool = False,
+def subset_corpus_and_metadata(
+    documents: list[str] | str = None,
+    target_folder: str = None,
+    tag: str = None,
     scripts_folder: str = None,
-    load_index: bool = True,
-) -> None:
-
-    try:
+    force: bool = True,
+):
+    """Subset metadata to folder `target_folder`/tag"""
+
+    root_folder: str = jj(target_folder, tag)
+
+    metadata_folder: str = jj(root_folder, "tmp")
+    parlaclarin_folder: str = jj(root_folder, "parlaclarin")
+    metadata_target_folder: str = jj(parlaclarin_folder, "metadata")
+    protocols_target_folder: str = jj(parlaclarin_folder, "protocols")
+    database_name: str = jj(root_folder, "riksprot_metadata.db")
+
+    reset_folder(root_folder, force=force)
+
+    if isinstance(documents, str):
+        documents: list[str] = _load_document_filenames(documents)
+
+    md.gh_dl_metadata_extra(folder=metadata_folder, tag=tag, force=True)
+    pc.download_protocols(filenames=documents, target_folder=protocols_target_folder, create_subfolder=True, tag=tag)
+
+    md.subset_to_folder(
+        ProtocolMapper,
+        protocols_source_folder=parlaclarin_folder,
+        source_folder=jj(metadata_folder, tag),
+        target_folder=metadata_target_folder,
+    )
+    """Add generated corpus indexes (speeches, utterances)"""
+    factory: md.CorpusIndexFactory = md.CorpusIndexFactory(ProtocolMapper)
+    factory.generate(corpus_folder=parlaclarin_folder, target_folder=metadata_target_folder)
+
+    """Create metadata database with base tables"""
+    md.DatabaseHelper(database_name).create(tag=tag, folder=metadata_target_folder, force=True).load_corpus_indexes(
+        folder=metadata_target_folder
+    ).load_scripts(folder=scripts_folder)
+
+    shutil.rmtree(path=metadata_folder, ignore_errors=True)
+
+
+def _load_document_filenames(filename):
+    """Loads a list of ParlaCLARIN document names from a file"""
+    if not os.path.isfile(filename):
+        raise FileNotFoundError(filename)
 
-        md.create_database(
-            database_filename=target,
-            branch=branch,
-            folder=source_folder,
-            force=force,
-        )
-
-        if load_index:
-            logger.info("loading index...")
-            md.load_corpus_indexes(database_filename=target, source_folder=source_folder or dirname(target))
-
-        if scripts_folder:
-            logger.info("loading scripts...")
-            md.load_scripts(database_filename=target, script_folder=scripts_folder)
-
-    except Exception as ex:
-        logger.error(ex)
-        click.echo(ex)
-        sys.exit(1)
-
-
-# type: ignore
-
-if __name__ == "__main__":
-    main.add_command(create_utterance_index, "index")
-    main.add_command(create_database, "database")
-    main.add_command(download_metadata, "download")
-    main()  # pylint: disable=no-value-for-parameter
+    with open(filename, "r", encoding="utf8") as fp:
+        return [x for x in fp.read().splitlines() if x.endswith(".xml")]
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2speech.py` & `pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2speech.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import click
 
 from pyriksprot import interface, to_speech
 from pyriksprot.dispatch import dispatch
 from pyriksprot.scripts.utils import option2, update_arguments_from_options_file
+from pyriksprot.utility import strip_path_and_extension
 from pyriksprot.workflows import extract_tags
 
 # pylint: disable=too-many-arguments, unused-argument
 
 
 @click.command()
 @click.argument('source-folder', type=click.STRING)
@@ -37,15 +38,17 @@
     skip_lemma: bool = False,
     skip_text: bool = False,
     skip_puncts: bool = False,
     skip_stopwords: bool = False,
     lowercase: bool = True,
     force: bool = False,
 ):
-    arguments: dict = update_arguments_from_options_file(arguments=locals(), filename_key='options_filename')
+    arguments: dict = update_arguments_from_options_file(
+        arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
+    )
     arguments['content_type'] = interface.ContentType(arguments['content_type'])
     arguments['merge_strategy'] = to_speech.MergeStrategyType(arguments['merge_strategy'])
     arguments['compress_type'] = dispatch.CompressType(arguments['compress_type'].lower())
 
     extract_tags.extract_corpus_tags(
         **{
             **arguments,
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/scripts/riksprot2tagged.py` & `pyriksprot-2023.4.1/pyriksprot/scripts/riksprot2tagged.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Sequence
 
 import click
 
 from pyriksprot import interface
 from pyriksprot.dispatch import dispatch
 from pyriksprot.scripts.utils import option2, update_arguments_from_options_file
+from pyriksprot.utility import strip_path_and_extension
 from pyriksprot.workflows import extract_tags
 
 sys.path.insert(0, '.')
 
 
 sys.path.insert(0, '.')
 
@@ -66,30 +67,31 @@
     skip_puncts: bool = False,
     skip_stopwords: bool = False,
     multiproc_processes: int = 1,
     multiproc_keep_order: str = None,
     force: bool = False,
 ):
     try:
-        arguments: dict = update_arguments_from_options_file(arguments=locals(), filename_key='options_filename')
+        arguments: dict = update_arguments_from_options_file(
+            arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
+        )
         arguments['content_type'] = interface.ContentType(arguments['content_type'])
         arguments['compress_type'] = dispatch.CompressType(arguments['compress_type'].lower())
 
         arguments['group_keys'] = arguments['group_key']
         del arguments['group_key']
 
         extract_tags.extract_corpus_tags(**arguments)
 
     except Exception as ex:
         click.echo(ex)
         sys.exit(1)
 
 
 if __name__ == "__main__":
-
     main()
 
     # from click.testing import CliRunner
 
     # runner = CliRunner()
     # result = runner.invoke(
     #     main,
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/scripts/speech_index.py` & `pyriksprot-2023.4.1/pyriksprot/scripts/speech_index.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import sys
 
 import click
 
 from pyriksprot import interface, to_speech
 from pyriksprot.scripts.utils import option2, update_arguments_from_options_file
+from pyriksprot.utility import strip_path_and_extension
 from pyriksprot.workflows.speech_index import extract_speech_index
 
 jj = os.path.join
 relpath = os.path.relpath
 
 # pylint: disable=too-many-arguments, W0613
 
@@ -27,15 +28,17 @@
     source_folder: str = None,
     target_name: str = None,
     database_filename: str = None,
     merge_strategy: str = 'chain',
     multiproc_processes: int = 1,
 ):
     """Extracts a speech index from given speech corpus"""
-    arguments: dict = update_arguments_from_options_file(arguments=locals(), filename_key='options_filename')
+    arguments: dict = update_arguments_from_options_file(
+        arguments=locals(), filename_key='options_filename', suffix=strip_path_and_extension(target_name)
+    )
     arguments['merge_strategy'] = to_speech.MergeStrategyType(arguments['merge_strategy'])
 
     try:
         extract_speech_index(
             **arguments,
             **dict(
                 segment_skip_size=1,
@@ -50,21 +53,26 @@
         click.echo(ex)
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
 
+    # tag: str = "v0.4.6"
+    # data_folder: str = "/data/riksdagen_corpus_data"
+
     # arguments = {
-    #     'source_folder': '/data/riksdagen_corpus_data/tagged_frames_vx.x.x',
-    #     'target_name': 'speech_index.csv.gz',
-    #     'database_filename': '/data/riksdagen_corpus_data/metadata/riksprot_metadata.main.db',
+    #     'source_folder': f'{data_folder}/tagged_frames_{tag}',
+    #     'target_name': f'speech_index.{tag}.csv.gz',
+    #     'database_filename': f'{data_folder}/metadata/riksprot_metadata.{tag}.db',
     #     'merge_strategy': 'chain',
     #     'multiproc_processes': None,
     #     'segment_skip_size': 0,
     #     'years': None,
     #     'content_type': "tagged_frame",
     #     'segment_level': interface.SegmentLevel.Speech,
     #     'multiproc_keep_order': True,
     #     'multiproc_chunksize': 10,
     # }
     # extract_speech_index(**arguments)
+
+    # poetry run python pyriksprot/scripts/speech_index.py /data/riksdagen_corpus_data/tagged_frames_v0.4.6 speech_index.v0.4.6.csv.gz /data/riksdagen_corpus_data/metadata/data/v0.4.6/riksprot_metadata.v0.4.6.db
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/scripts/utils.py` & `pyriksprot-2023.4.1/pyriksprot/scripts/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,40 +21,44 @@
 
 CLI_OPTIONS = {
     '--compress-type': dict(default='lzma', type=click.Choice(COMPRESS_TYPES), help='Compress type'),
     '--content-type': dict(default='tagged_frame', type=click.Choice(CONTENT_TYPES), help='Text or tags'),
     '--dedent': dict(default=False, is_flag=True, help='Remove indentation'),
     '--dehyphen': dict(default=False, is_flag=True, help='Dehyphen text'),
     '--group-key': dict(help='Partition key(s)', multiple=True, type=click.STRING),
-    '--lowercase': dict(default=True, type=click.BOOL, is_flag=True, help='Lowercase tokem/text'),
+    '--naming-key': dict(help='Property values to be added to filename(s)', multiple=True, type=click.STRING),
+    '--lowercase': dict(default=True, type=click.BOOL, is_flag=True, help='Lowercase token/text'),
     '--merge-strategy': dict(default='chain', type=click.Choice(MERGE_STRATEGIES), help='Merge strategy'),
     '--multiproc-keep-order': dict(default=False, is_flag=True, help='Process is sort order (slower, multiproc)'),
     '--multiproc-processes': dict(default=None, type=click.IntRange(1, 40), help='Number of processes to use'),
     '--segment-level': dict(default='who', type=click.Choice(SEGMENT_LEVELS), help='Protocol iterate level'),
     '--segment-skip-size': dict(default=1, type=click.IntRange(1, 1024), help='Skip smaller than threshold'),
+    '--skip-size': dict(default=1, type=click.IntRange(1, 1024), help='Skip size less than threshold'),
     '--skip-lemma': dict(default=False, type=click.BOOL, is_flag=True, help='Skip lemma'),
     '--skip-puncts': dict(default=False, type=click.BOOL, is_flag=True, help='Skip puncts'),
     '--skip-stopwords': dict(default=False, type=click.BOOL, is_flag=True, help='Skip stopwords'),
     '--skip-text': dict(default=False, type=click.BOOL, is_flag=True, help='Skip text'),
     '--target-type': dict(
         default='single-id-tagged-frame-per-group', type=click.Choice(TARGET_TYPES), help='Target type'
     ),
     '--temporal-key': dict(default=None, help='Temporal partition key(s)', type=click.STRING),
+    '--subfolder-key': dict(default=None, help='Subfolder sort key', type=click.STRING),
     '--years': dict(default=None, help='Years to include in output', type=click.STRING),
     '--force': dict(default=False, help='Force remove of existing files', is_flag=True),
 }
 
 
 def update_arguments_from_options_file(
     *,
     arguments: dict,
     filename_key: str,
     log_args: bool = True,
     ctx: click.Context = None,
     skip_keys: str = 'ctx,options_filename',
+    suffix: str = None,
 ) -> dict:
     """Updates `arguments` based on values found in file specified by `filename_key`.
     Values specified at the command line overrides values from options file."""
 
     options_filename: Optional[str] = arguments.get(filename_key)
     del arguments[filename_key]
 
@@ -62,20 +66,22 @@
     arguments.update(passed_cli_arguments(ctx, arguments))
 
     for k in skip_keys.split(','):
         if k in arguments:
             del arguments[k]
 
     if log_args:
-        log_arguments(arguments)
+        log_arguments(arguments, suffix=suffix)
 
     return arguments
 
 
-def log_arguments(args: dict, subdir: bool = False, skip_keys: str = 'ctx,options_filename') -> None:
+def log_arguments(
+    args: dict, subdir: bool = False, skip_keys: str = 'ctx,options_filename', suffix: str = None
+) -> None:
     def fix_value(v: Any):
         if isinstance(v, tuple):
             v = list(v)
         # if isinstance(v, list):
         #     if len(v) == 1:
         #         v = v[0]
         return v
@@ -83,14 +89,18 @@
     cli_command: str = utility.strip_path_and_extension(sys.argv[0])
 
     log_dir: str = os.path.join(CLI_LOG_PATH, cli_command) if subdir else CLI_LOG_PATH
 
     os.makedirs(log_dir, exist_ok=True)
 
     log_name: str = utility.ts_data_path(log_dir, f"{cli_command}.yml")
+
+    if suffix:
+        log_name = utility.path_add_suffix(log_name, suffix=f"_{suffix.strip('_')}")
+
     log_args: dict = {k: fix_value(v) for k, v in args.items() if k not in skip_keys.split(',')}
     utility.write_yaml(log_args, log_name)
 
 
 def passed_cli_arguments(ctx: click.Context, args: dict) -> dict:
     """Return args specified in commande line"""
     ctx = ctx or click.get_current_context()
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/to_speech.py` & `pyriksprot-2023.4.1/pyriksprot/to_speech.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # pylint: disable=too-many-arguments, no-member
 
 
 class MergeStrategyType(str, Enum):
     who = 'who'
     who_sequence = 'who_sequence'
     chain = 'chain'
+    chain_consecutive_unknowns = 'chain_consecutive_unknowns'
     who_speaker_note_id_sequence = 'who_speaker_note_id_sequence'
     speaker_note_id_sequence = 'speaker_note_id_sequence'
     undefined = 'undefined'
 
 
 def to_speeches(
     *, protocol: Protocol, merge_strategy: MergeStrategyType | Type[IMergeStrategy], skip_size: int = 1
 ) -> list[Speech]:
-
     if not protocol.utterances:
         return []
 
     merger: IMergeStrategy = MergerFactory.get(merge_strategy)
 
     speeches: list[Speech] = [
         Speech(
@@ -56,57 +56,64 @@
     """Abstract strategy for merging a protocol into speeches"""
 
     def cluster(self, utterances: Protocol) -> list[list[Utterance]]:
         return [utterances]
 
 
 class MergeByWho(IMergeStrategy):
-    """Merge all uterrances for a unique `who` into a single speech """
+    """Merge all uterrances for a unique `who` into a single speech"""
 
     def cluster(self, utterances: Protocol) -> list[list[Utterance]]:
         """Create a speech for each unique `who`. Return list of Speech."""
         data = defaultdict(list)
         for u in utterances or []:
             data[u.who].append(u)
         return [data[who] for who in data]
 
 
 class MergeByWhoSequence(IMergeStrategy):
-    """Merge sequences with same `who` into a speech """
+    """Merge sequences with same `who` into a speech"""
 
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         groups: list[list[Utterance]] = [list(g) for _, g in groupby(utterances or [], key=lambda x: x.who)]
         return groups
 
 
 class MergeBySpeakerNoteIdSequence(IMergeStrategy):
-    """Merge sequences with same `speaker_note_id` into a speech """
+    """Merge sequences with same `speaker_note_id` into a speech"""
 
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         groups: list[list[Utterance]] = [list(g) for _, g in groupby(utterances or [], key=lambda x: x.speaker_note_id)]
         return groups
 
 
 class MergeByWhoSpeakerNoteIdSequence(IMergeStrategy):
-    """Merge sequences with same `who` & 'speaker_note_id' into a speech """
+    """Merge sequences with same `who` & 'speaker_note_id' into a speech"""
 
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         groups: list[list[Utterance]] = [
             list(g) for _, g in groupby(utterances or [], key=lambda x: f"{x.who}_{x.speaker_note_id}")
         ]
         return groups
 
 
 class MergeByChain(IMergeStrategy):
+    def __init__(self, merge_consecutive_unknowns: bool = False):
+        self.merge_consecutive_unknowns = merge_consecutive_unknowns
+
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
-        groups: list[list[Utterance]] = MergeByChain.group_utterances_by_chain(utterances)
+        groups: list[list[Utterance]] = MergeByChain.group_utterances_by_chain(
+            utterances, self.merge_consecutive_unknowns
+        )
         return groups
 
     @staticmethod
-    def group_utterances_by_chain(utterances: list[Utterance]) -> list[list[Utterance]]:
+    def group_utterances_by_chain(
+        utterances: list[Utterance], merge_consecutive_unknowns: bool
+    ) -> list[list[Utterance]]:
         """Split utterances based on prev/next pointers. Return list of lists."""
         speeches: list[list[Utterance]] = []
         speech: list[Utterance] = []
         start_of_speech: bool = None
 
         for _, u in enumerate(utterances or []):
             """Rules:
@@ -130,53 +137,60 @@
                 True
                 if bool(u.next_id)
                 else not is_unknown_continuation
                 if not is_part_of_chain
                 else not bool(speech) and bool(u.prev_id)
             )
 
-            if start_of_speech:
+            if not start_of_speech:
+                if is_unknown_continuation:
+                    if not merge_consecutive_unknowns:
+                        start_of_speech = True
 
+            if start_of_speech:
                 if bool(u.prev_id) and not bool(speech):
                     logger.warning(f"logic error: {u.u_id} has prev attribute but no previous utterance")
 
                 speech = [u]
                 speeches.append(speech)
 
             else:
-
                 if bool(speech):
-
                     if bool(u.prev_id) and speech[0].u_id != u.prev_id:
                         logger.warning(f"u[{u.u_id}]: current prev_id differs from first u.u_id '{speech[0].u_id}'")
 
                     if speech[0].who != u.who:
                         raise ValueError(f"u[{u.u_id}]: multiple who ids in current speech '{speech[0].who}'")
 
                 speech.append(u)
 
         return speeches
 
 
+class MergeByChainAndConsecutiveUnknowns(MergeByChain):
+    def __init__(self):
+        super().__init__(True)
+
+
 class UndefinedMerge(IMergeStrategy):
     def cluster(self, utterances: list[Utterance]) -> list[list[Utterance]]:
         raise ValueError("undefined merge strategy encountered")
 
     def merge(self, protocol: Protocol) -> list[Speech]:
         raise ValueError("undefined merge strategy encountered")
 
 
 class MergerFactory:
-
     strategies: dict[MergeStrategyType, IMergeStrategy] = {
         'who': MergeByWho(),
         'who_sequence': MergeByWhoSequence(),
         'who_speaker_note_id_sequence': MergeByWhoSpeakerNoteIdSequence(),
         'speaker_note_id_sequence': MergeBySpeakerNoteIdSequence(),
-        'chain': MergeByChain(),
+        'chain': MergeByChain(False),
+        'chain_consecutive_unknowns': MergeByChain(True),
         'undefined': UndefinedMerge(),
     }
 
     @staticmethod
     def get(strategy: str | Type[IMergeStrategy]) -> IMergeStrategy:
         return (
             strategy()
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/utility.py` & `pyriksprot-2023.4.1/pyriksprot/utility.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,35 +3,32 @@
 import base64
 import bz2
 import contextlib
 import functools
 import glob
 import gzip
 import inspect
+import json
 import lzma
 import os
 import pathlib
-import pickle
 import re
 import shutil
 import tempfile
 import time
 import unicodedata
 import warnings
 import zlib
-from collections import defaultdict
-from dataclasses import fields, is_dataclass
 from itertools import chain
 from os.path import basename, dirname, expanduser, isfile
 from os.path import join as jj
 from os.path import normpath, splitext
 from types import ModuleType
 from typing import Any, Callable, List, Literal, Sequence, Set, Type, TypeVar
-from urllib.error import URLError
-from urllib.request import urlretrieve
+from urllib.request import urlopen
 
 import requests
 import unidecode  # pylint: disable=import-error
 import yaml
 from loguru import logger
 
 
@@ -107,27 +104,18 @@
     return path_add_suffix(path, f'_{time.strftime(fmt)}')
 
 
 def ts_data_path(directory: str, filename: str):
     return jj(directory, f'{time.strftime("%Y%m%d%H%M")}_{filename}')
 
 
-def data_path_ts(directory: str, path: str):
-    name, extension = splitext(path)
-    return jj(directory, f'{name}_{time.strftime("%Y%m%d%H%M")}{extension}')
-
-
 def path_add_sequence(path: str, i: int, j: int = 0) -> str:
     return path_add_suffix(path, f"_{str(i).zfill(j)}")
 
 
-def strip_path_and_add_counter(filename: str, i: int, n_zfill: int = 3):
-    return f'{basename(strip_extensions(filename))}_{str(i).zfill(n_zfill)}.txt'
-
-
 def strip_paths(filenames: str | List[str]) -> str | List[str]:
     if isinstance(filenames, str):
         return basename(filenames)
     return [basename(filename) for filename in filenames]
 
 
 T = TypeVar("T")
@@ -146,110 +134,54 @@
         if not hasattr(data, attrib):
             return False
         data = getattr(data, attrib)
 
     return True
 
 
-def dict_get_by_path(data: dict, path: str, default=None) -> Any:
-    for attrib in path.split("."):
-        if not attrib in data:
-            return default
-        data = data[attrib]
-    return data
-
-
 def lookup(data, *keys):
     for key in keys or []:
         data = data.get(key, {})
     return data
 
 
-def load_token_set(filename: str) -> Set[str]:
-    """Load tokens from `filename`, one token per line"""
-    if isfile(filename):
-        with gzip.open(filename, 'rb') as f:
-            return set(f.read().decode().split('\n'))
-    return set()
-
-
-def store_token_set(tokens: Set[str], filename: str):
-    with gzip.open(filename, 'wb') as f:
-        f.write('\n'.join(list(tokens)).encode())
-
-
-def store_dict(data: dict, filename: str):
-    with open(filename, 'wb') as fp:
-        pickle.dump(data, fp, pickle.HIGHEST_PROTOCOL)
-
-
-def load_dict(filename: str) -> defaultdict(int):
-    # logger.info(f"loading {filename}")
-    if isfile(filename):
-        with open(filename, 'rb') as fp:
-            return pickle.load(fp)
-    return defaultdict(int)
-
-
 @contextlib.contextmanager
 def temporary_file(*, filename: str = None, content: Any = None, **mktemp):
-
     if filename is None:
         filename: str = tempfile.mktemp(**mktemp)
 
     path: pathlib.Path = pathlib.Path(filename)
 
     try:
-
         if content:
             mode: str = "wb" if isinstance(content, (bytes, bytearray)) else "w"
             with open(filename, mode) as fp:
                 fp.write(content)
 
         yield path.resolve()
 
     finally:
         path: pathlib.Path = pathlib.Path(filename)
         if path.is_file():
             path.unlink()
 
 
-def download_url(*, url: str, target_folder: str, filename: str = None) -> None:
-    """Download a file from a url and place it in `target_folder`.
-    https://stackoverflow.com/a/61003039/12383895
-    Args:
-        url (str): URL to download file from
-        target_folder (str): Directory to place downloaded file in
-        filename (str, optional): Name to save the file under. If None, use the basename of the URL
-    """
-
-    target_folder: str = expanduser(target_folder)
-    target_filename: str = jj(target_folder, filename or basename(url))
-
-    os.makedirs(target_folder, exist_ok=True)
-
-    logger.info(f'downloading: {filename}')
-    try:
-        urlretrieve(url, target_filename)
-    except (URLError, IOError):
-        if url.startswith('https:'):
-            urlretrieve(url.replace('https:', 'http:'), target_filename)
-
-
 def download_url_to_file(url: str, target_name: str, force: bool = False) -> None:
+    target_name: str = expanduser(target_name)
 
     if os.path.isfile(target_name):
         if not force:
             raise ValueError("File exists, use `force=True` to overwrite")
         os.unlink(target_name)
 
     ensure_path(target_name)
 
+    logger.info(f'downloading: {target_name}')
     with open(target_name, 'w', encoding="utf-8") as fp:
-        data: str = requests.get(url, allow_redirects=True).content.decode("utf-8")
+        data: str = requests.get(url, allow_redirects=True, timeout=10).content.decode("utf-8")
         fp.write(data)
 
 
 def deprecated(func):
     """Decorator that marks functions or classes as deprecated (emits a warning when used)."""
 
     @functools.wraps(func)
@@ -259,30 +191,47 @@
         warnings.simplefilter('default', DeprecationWarning)
         return func(*args, **kwargs)
 
     return inner
 
 
 def unlink(f: str) -> None:
-
     fo = pathlib.Path(f)
 
     if fo.is_dir():
         shutil.rmtree(f)
 
     elif fo.is_file():
         fo.unlink(missing_ok=True)
 
 
 def touch(f: str) -> None:
     pathlib.Path(f).touch()
 
 
-def ensure_path(f: str) -> None:
-    os.makedirs(dirname(f), exist_ok=True)
+def ensure_path(path: str) -> str:
+    os.makedirs(dirname(path), exist_ok=True)
+    return path
+
+
+def reset_folder(folder: str, force: bool = False) -> str:
+    if os.path.isdir(folder) and not force:
+        raise FileExistsError(folder)
+
+    shutil.rmtree(folder, ignore_errors=True)
+    os.makedirs(folder, exist_ok=True)
+
+
+def reset_file(path: str, force: bool):
+    if path is None:
+        return
+    if os.path.isfile(path):
+        if not force:
+            raise FileExistsError(path)
+        os.unlink(path)
 
 
 def get_kwargs():
     frame = inspect.currentframe().f_back
     keys, _, _, values = inspect.getargvalues(frame)
     kwargs = {}
     for key in keys:
@@ -356,21 +305,14 @@
 def compose(*fns: Sequence[Callable[[str], str]]) -> Callable[[str], str]:
     """Create a composed function from a list of function. Return function."""
     if len(fns) == 0:
         return None
     return functools.reduce(lambda f, g: lambda *args: f(g(*args)), fns)
 
 
-# def dedent(text: str) -> str:
-#     """Remove any white-space indentation from `text`."""
-#     if isinstance(text, Undefined):
-#         raise TypeError("dedent: jinja2.Undefined value string encountered")
-#     return textwrap.dedent(text) if text is not None else ""
-
-
 def dedent(text: str) -> str:
     """Remove whitespaces before and after newlines"""
     return '\n'.join(x.strip() for x in text.split('\n'))
 
 
 def is_empty(filename: str) -> bool:
     """Check if file is empty."""
@@ -383,15 +325,15 @@
         return ''
     idx: int = csv_str.find(sep)
     if idx <= 0:
         return ''
     return csv_str[idx + 1 :]
 
 
-def merge_tagged_csv(csv_strings: List[str], sep: str = '\n') -> str:
+def merge_csv_strings(csv_strings: List[str], sep: str = '\n') -> str:
     """Merge tagged CSV strings into a single tagged CSV string"""
     if len(csv_strings or []) == 0:
         return ''
     texts: List[str] = [csv_strings[0]]
     for csv_string in csv_strings[1:]:
         text = strip_csv_header(csv_string, sep=sep)
         if text:
@@ -443,65 +385,25 @@
     if yaml_file is None:
         return data
     options: dict = read_yaml(yaml_file)
     data.update(options)
     return data
 
 
-def download_protocols(*, protocols: List[str], target_folder: str, create_subfolder: bool, tag: str) -> None:
-    """Downloads protocols. Used only in tests."""
-
-    def _protocol_uri(filename: str, sub_folder: str, tag: str) -> str:
-        return f"https://github.com/welfare-state-analytics/riksdagen-corpus/raw/{tag}/corpus/protocols/{sub_folder}/{filename}"
-
-    shutil.rmtree(target_folder, ignore_errors=True)
-    os.makedirs(target_folder, exist_ok=True)
-
-    logger.info(f"downloading protocols from branch {tag}.")
-
-    for filename in protocols:
-        sub_folder: str = filename.split('-')[1]
-        filename: str = replace_extension(filename, 'xml')
-        download_url(
-            url=_protocol_uri(filename=filename, sub_folder=sub_folder, tag=tag),
-            target_folder=target_folder if not create_subfolder else jj(target_folder, sub_folder),
-            filename=filename,
-        )
+def load_json(url: str) -> list[dict]:
+    return json.loads(urlopen(url).read())
 
 
 def probe_filename(filename: list[str], exts: list[str] = None) -> str | None:
     """Probes existence of filename with any of given extensions in folder"""
     for probe_name in set([filename] + ([replace_extension(filename, ext) for ext in exts] if exts else [])):
         if isfile(probe_name):
             return probe_name
     raise FileNotFoundError(filename)
 
 
 def revdict(d: dict) -> dict:
     return {v: k for k, v in d.items()}
 
 
-def split_properties_by_dataclass(properties: set[str], *cls_list: tuple[Type, ...]) -> tuple[set[str], ...]:
-
-    properties = set(properties)
-
-    key_sets: list[set[str]] = []
-
-    for cls in cls_list:
-
-        if not is_dataclass(cls):
-            raise ValueError(f"{cls.__name__} is not a dataclass")
-
-        key_set: set[str] = properties.intersection({f.name for f in fields(cls)})
-
-        properties -= key_set
-
-        key_sets.append(key_set)
-
-    if properties:
-        raise ValueError(f"split_properties_by_dataclass: {','.join(properties)} not found.")
-
-    return tuple(key_sets)
-
-
 def props(cls: Type) -> list[str]:
     return [i for i in cls.__dict__.keys() if i[:1] != '_']
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/workflows/extract_tags.py` & `pyriksprot-2023.4.1/pyriksprot/workflows/extract_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,20 @@
                 skip_lemma=skip_lemma,
                 skip_text=skip_text,
                 skip_puncts=skip_puncts,
                 skip_stopwords=skip_stopwords,
             ),
         }
 
+    lookups: md.Codecs = md.Codecs().load(metadata_filename)
+
     source_index: corpus_index.CorpusSourceIndex = corpus_index.CorpusSourceIndex.load(
         source_folder=source_folder, source_pattern='**/prot-*.zip', years=years
     )
-    logger.info("loading parliamentary metadata...")
+    # logger.info("loading parliamentary metadata...")
 
     # FIXME: How to ensure metadata tag is the same as corpus??? Add tag to DB?
     speaker_service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename=metadata_filename)
 
     def get_speaker(item: iterate.ProtocolSegment) -> None:
         item.speaker_info = speaker_service.get_speaker_info(u_id=item.u_id, person_id=item.who, year=item.year)
 
@@ -126,21 +128,20 @@
     merger: merge.SegmentMerger = merge.SegmentMerger(
         source_index=source_index,
         temporal_key=temporal_key,
         grouping_keys=group_keys,
     )
 
     with dispatch.IDispatcher.dispatcher(target_type)(
-        target_name=target_name, compress_type=compress_type, **dispatch_opts
+        target_name=target_name, compress_type=compress_type, lookups=lookups, **dispatch_opts
     ) as dispatcher:
         data: t.Iterable[dict[str, DispatchItem]]
         n_total: int = len(source_index.source_items)
 
         for data in tqdm(merger.merge(texts), total=n_total, miniters=10, disable=not progress):
-
             if not data:
                 logger.error("merge returned empty data")
                 continue
 
             # items: list[DispatchItem] = list(data.values())
             # print(f"dispatch: group count is {len(items)}")
             # for item in items:
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/workflows/extract_text.py` & `pyriksprot-2023.4.1/pyriksprot/workflows/extract_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import os
 from typing import Sequence
 
 from loguru import logger
 
 from pyriksprot.corpus.iterate import ProtocolSegment
 from pyriksprot.corpus.parlaclarin import iterate
 
@@ -13,24 +12,14 @@
 from .. import utility
 from ..corpus import corpus_index
 from ..dispatch import dispatch, merge
 
 # pylint: disable=too-many-arguments
 
 
-def create_dehyphen(data_path: str) -> dehyphenation.SwedishDehyphenatorService:
-    opts = dict(
-        word_frequency_filename=os.path.join(data_path, 'riksdagen-corpus-term-frequencies.pkl'),
-        whitelist_filename=os.path.join(data_path, 'dehyphen_whitelist.txt.gz'),
-        whitelist_log_filename=os.path.join(data_path, 'dehyphen_whitelist_log.pkl'),
-        unresolved_filename=os.path.join(data_path, 'dehyphen_unresolved.txt.gz'),
-    )
-    return dehyphenation.SwedishDehyphenatorService.create_dehypen(*opts)
-
-
 def extract_corpus_text(
     source_folder: str = None,
     metadata_filename: str = None,
     target_name: str = None,
     target_type: str = None,
     segment_level: interface.SegmentLevel = None,
     temporal_key: interface.TemporalKey = None,
@@ -68,48 +57,52 @@
         dehyphen (bool, optional): Dehyphen text. Defaults to False.
         data_path (str, optional): Path to model data (used by dedent/dehyphen). Defaults to '.'.
     """
     source_index: corpus_index.CorpusSourceIndex = corpus_index.CorpusSourceIndex.load(
         source_folder=source_folder, source_pattern='**/prot-*.xml', years=years
     )
 
-    dehypenator = create_dehyphen(data_path) if dehyphen else None
+    lookups: md.Codecs = md.Codecs().load(source=metadata_filename)
 
-    get_speaker = None
-    if segment_level == interface.SegmentLevel.Speech:
-        speaker_service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename=metadata_filename)
-        get_speaker = speaker_service.get_speaker_info
+    dehypenator: dehyphenation.SwedishDehyphenator = (
+        dehyphenation.SwedishDehyphenator(data_folder=data_path, word_frequencies=None) if dehyphen else None
+    )
+    speaker_service: md.SpeakerInfoService = md.SpeakerInfoService(database_filename=metadata_filename)
 
     def preprocess(item: ProtocolSegment) -> None:
-
         if dedent:
             item.data = utility.dedent(item.data)
 
         if dehypenator:
             item.data = dehypenator(item.data)  # pylint: disable=not-callable
 
-        if get_speaker:
-            item.speaker_info = get_speaker(item.u_id, item.who, item.year)
+        if segment_level not in ('protocol', None):
+            item.speaker_info = speaker_service.get_speaker_info(u_id=item.u_id, person_id=item.who, year=item.year)
+
+        # If not unknown a speaker info must have been assigned
+        assert not (item.who and item.who != "unknown" and item.speaker_info is None)
 
     segments: iterate.XmlUntangleSegmentIterator = iterate.XmlUntangleSegmentIterator(
         filenames=source_index.paths,
         segment_level=segment_level,
         segment_skip_size=segment_skip_size,
-        multiproc_processes=multiproc_processes,
         multiproc_keep_order=multiproc_keep_order,
+        multiproc_processes=multiproc_processes,
         multiproc_chunksize=multiproc_chunksize,
         preprocess=preprocess,
     )
 
     merger: merge.SegmentMerger = merge.SegmentMerger(
         source_index=source_index,
         temporal_key=temporal_key,
         grouping_keys=group_keys,
     )
 
-    with dispatch.IDispatcher.dispatcher(target_type)(target_name, compress_type=compress_type) as dispatcher:
+    with dispatch.IDispatcher.dispatcher(target_type)(
+        target_name, compress_type=compress_type, lookups=lookups
+    ) as dispatcher:
         for item in merger.merge(segments):
             dispatcher.dispatch(list(item.values()))
 
     # metadata_index.store(target_name if isdir(target_name) else dirname(target_name))
 
     logger.info(f"Corpus stored in {target_name}.")
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/workflows/speech_index.py` & `pyriksprot-2023.4.1/pyriksprot/workflows/speech_index.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     multiproc_processes: int = 1,
     multiproc_chunksize: int = 100,
     merge_strategy: to_speech.MergeStrategyType = 'chain',
 ) -> None:
     """Generates a speech index for corpus in `source_folder`, and according to given parameters..
 
     Args:
-        source_folder (str): _description_
-        database_filename (str): _description_
-        target_name (str): _description_
-        content_type (interface.ContentType, optional): _description_. Defaults to interface.ContentType.TaggedFrame.
-        segment_level (interface.SegmentLevel, optional): _description_. Defaults to None.
-        segment_skip_size (int, optional): _description_. Defaults to 1.
-        years (str, optional): _description_. Defaults to None.
-        multiproc_keep_order (str, optional): _description_. Defaults to None.
-        multiproc_processes (int, optional): _description_. Defaults to 1.
-        multiproc_chunksize (int, optional): _description_. Defaults to 100.
-        merge_strategy (to_speech.MergeStrategyType, optional): _description_. Defaults to 'chain'.
+        source_folder (str): Source folder
+        database_filename (str): Metadata database filename (Sqlite3)
+        target_name (str): Target filename.
+        content_type (interface.ContentType, optional): Text or PoS-tagged. Defaults to interface.ContentType.TaggedFrame.
+        segment_level (interface.SegmentLevel, optional): Document level. Defaults to None.
+        segment_skip_size (int, optional): Size of text to include. Defaults to 1.
+        years (str, optional): Years filter. Defaults to None.
+        multiproc_keep_order (str, optional): Multiprocessing option. Defaults to None.
+        multiproc_processes (int, optional): Number of processes. Defaults to 1.
+        multiproc_chunksize (int, optional): Size of work loads assigned to each process. Defaults to 100.
+        merge_strategy (to_speech.MergeStrategyType, optional): Speech merge strategy. Defaults to 'chain'.
     """
     logger.info("extracting corpus speech index...")
 
     source_index: corpus_index.CorpusSourceIndex = corpus_index.CorpusSourceIndex.load(
         source_folder=source_folder, source_pattern='**/prot-*.zip', years=years
     )
     logger.info("loading parliamentary metadata...")
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/workflows/tag.py` & `pyriksprot-2023.4.1/pyriksprot/workflows/tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     def preprocess(self, text: str) -> str:
         """Transform `text` with preprocessors."""
         text: str = reduce(lambda res, f: f(res), self.preprocessors, text)
         return text
 
 
 def tag_protocol(tagger: ITagger, protocol: interface.Protocol, preprocess=False) -> interface.Protocol:
-
     texts = [u.text for u in protocol.utterances]
 
     documents: List[TaggedDocument] = tagger.tag(texts, preprocess=preprocess)
 
     for i, document in enumerate(documents):
         protocol.utterances[i].annotation = tagger.to_csv(document)
         protocol.utterances[i].num_tokens = document.get("num_tokens")
@@ -89,32 +88,29 @@
     return protocol
 
 
 def tag_protocol_xml(
     input_filename: str,
     output_filename: str,
     tagger: ITagger,
-    segment_skip_size: int = 5,
     force: bool = False,
     storage_format: interface.StorageFormat = interface.StorageFormat.JSON,
 ) -> None:
     """Annotate XML protocol `input_filename` to `output_filename`.
 
     Args:
         input_filename (str, optional): Defaults to None.
         output_filename (str, optional): Defaults to None.
         tagger (StanzaTagger, optional): Defaults to None.
     """
 
     try:
         ensure_path(output_filename)
 
-        protocol: interface.Protocol = parse.ProtocolMapper.to_protocol(
-            input_filename, segment_skip_size=segment_skip_size
-        )
+        protocol: interface.Protocol = parse.ProtocolMapper.parse(input_filename)
 
         if not protocol.has_text:
             unlink(output_filename)
             touch(output_filename)
             return
 
         protocol.preprocess(tagger.preprocess)
```

### Comparing `pyriksprot-2022.5.2/pyriksprot/workflows/tf.py` & `pyriksprot-2023.4.1/pyriksprot/workflows/tf.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     source: Union[str, List[str]],
     filename: str,
     segment_skip_size: int = 1,
     multiproc_processes: int = 2,
     multiproc_keep_order: bool = False,
     progress: bool = True,
 ) -> TermFrequencyCounter:
-    """Compute (corpus) term frequency for documents in `source `.
-
+    """Compute (corpus) term frequency for documents in  `source `.
+    Source is an ParlaClarin XML file so TF is never counted on lemmatized text.
     Args:
         source (Union[str, List[str]]): ParlaClarin filename(s), folder, filename patterna
         filename (str): [description]
 
     Raises:
         ValueError: Unsupported source.
```

### Comparing `pyriksprot-2022.5.2/setup.py` & `pyriksprot-2023.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,271 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyriksprot
+Version: 2023.4.1
+Summary: Python API for Riksdagens Protokoll
+Home-page: https://westac.se
+License: Apache-2.0
+Author: Roger Mähler
+Author-email: roger.mahler@hotmail.com
+Requires-Python: >=3.11.0,<3.12.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Requires-Dist: Jinja2
+Requires-Dist: click
+Requires-Dist: loguru
+Requires-Dist: lz4
+Requires-Dist: more-itertools
+Requires-Dist: pandas
+Requires-Dist: pdoc
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: pyarrow
+Requires-Dist: pygit2 (>=1.11.1,<2.0.0)
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: sqlalchemy (>=2.0.6,<3.0.0)
+Requires-Dist: tqdm
+Requires-Dist: unidecode (>=1.3.6,<2.0.0)
+Project-URL: Repository, https://github.com/welfare-state-analytics/pyriksprot
+Description-Content-Type: text/markdown
 
-packages = \
-['pyriksprot',
- 'pyriksprot.corpus',
- 'pyriksprot.corpus.parlaclarin',
- 'pyriksprot.corpus.parlaclarin.resources',
- 'pyriksprot.corpus.parlaclarin.resources.templates',
- 'pyriksprot.corpus.tagged',
- 'pyriksprot.dehyphenation',
- 'pyriksprot.dispatch',
- 'pyriksprot.foss',
- 'pyriksprot.metadata',
- 'pyriksprot.scripts',
- 'pyriksprot.workflows']
-
-package_data = \
-{'': ['*'], 'pyriksprot.corpus.parlaclarin.resources': ['xslt/*']}
-
-install_requires = \
-['Jinja2',
- 'Unidecode',
- 'click',
- 'loguru',
- 'lz4',
- 'more-itertools',
- 'pandas',
- 'pdoc',
- 'pyarrow',
- 'python-dotenv',
- 'requests',
- 'tqdm']
-
-entry_points = \
-{'console_scripts': ['riksprot2any = pyriksprot.scripts.riksprot2any:main',
-                     'riksprot2text = pyriksprot.scripts.riksprot2text:main',
-                     'riksprot2tfs = pyriksprot.scripts.riksprot2tfs:main']}
-
-setup_kwargs = {
-    'name': 'pyriksprot',
-    'version': '2022.5.2',
-    'description': 'Python API for Riksdagens Protokoll',
-    'long_description': '# Python package for reading and tagging Riksdagens Protokoll\n\nBatteries (tagger) not included.\n\n## Overview\n\nThis package is intended to cover the following use cases:\n\n### Extract "text documents" from the Parla-CLARIN XML files\n\nText can be extracted from the XML files at different granularity (paragraphs, utterance, speech, who, protocol). The text can be grouped (combined) into larger temporal blocks based on time (year, lustrum, decade or custom periods). Within each of these block the text in turn can be grouped by speaker attributes (who, party, gender).\n\nThe text extraction can done using the `riksprot2text` utility, which is a CLI interface installed with the package, or in Python code using the API that this package exposes. The Python API exposed both streaming (SAX based) methods and a domain model API (i.e. Python classes representing protocols, speeches and utterances).\n\nBoth the CLI and the API supports dehyphenation using method described in [Anföranden: Annotated and Augmented Parliamentary Debates from Sweden, Stian Rødven Eide, 2020](https://gup.ub.gu.se/publication/302449). The API also supports user defined text transformations.\n\n### Extract PoS-tagged versions of the Parla-CLARIN XML files\n\nPart-of-speech tagged versions of the protocols can be extracted with the same granularity and aggregation as described above for the raw text. The returned documents are tab-separated files with fields for text, baseform and pos-tag (UPOS, XPOS). Note that the actual part-of-speech tagging is done using tools found in the `pyriksprot_tagging` repository ([link](https://github.com/welfare-state-analytics/westac_parlaclarin_pipeline)).\n\nCurrently there are no open-source tagged versions of the corpos avaliable. The tagging is done using [Stanza](https://stanfordnlp.github.io/stanza/) with Swedish language models produced and made publically avaliable by Språkbanken Text.\n\n### Store extracted text\n\nThe extracted text can be stored as optionally compressed plain text files on disk, or in a ZIP-archive.\n\n## Pre-requisites\n\n- Python >=3.8\n- A folder containing the Riksdagen Protokoll (parliamentary protocols) Github repository.\n\n```bash\ncd some-folder \\\ngit clone --branch "tag" tags/"tag" --depth 1 https://github.com/welfare-state-analytics/riksdagen-corpus.git\ncd riksdagen-corpus\ngit config core.quotepath off\n\n```\n\n## Installation (Linux)\n\nCreate an new isolated virtual environment for pyriksprot:\n\n```bash\nmkdir /path/to/new/pyriksprot-folder\ncd /path/to/new/pyriksprot-folder\npython -m venv .venv\n```\n\nActivate the environment:\n\n```bash\ncd /path/to/new/pyriksprot-folder\nsource .venv/bin/activate\n```\n\nInstall `pyriksprot` in activated virtual environment.\n\n```bash\npip install pyriksprot\n```\n\n## CLI riksprot2text:  Extract aggregated text corpus from Parla-CLARIN XML files\n\n```bash\n\nλ riksprot2text --help\n\nUsage: riksprot2text [OPTIONS] SOURCE_FOLDER TARGET\n\nOptions:\n  -m, --mode [plain|zip|gzip|bz2|lzma]\n                                  Target type\n  -t, --temporal-key TEXT         Temporal partition key(s)\n  -y, --years TEXT                Years to include in output\n  -g, --group-key TEXT            Partition key(s)\n  -p, --processes INTEGER RANGE   Number of processes to use\n  -l, --segment-level [protocol|speech|utterance|paragraph|who]\n                                  Protocol extract segment level\n  -e, --keep-order                Keep output in filename order (slower, multiproc)\n\n  -s, --skip-size INTEGER RANGE   Skip blocks of char length less than\n  -d, --dedent                    Remove indentation\n  -k, --dehyphen                  Dehyphen text\n  --help                          Show this message and exit.\n\n```\n\n### Examples CLI\n\nAggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.\n\n```python\nriksprot2text /path/to/corpus output.zip -m zip -t year -l protocol -g who --skip-size 50\n```\n\nAggregate text per decade grouped by speaker. Store result in a single zip. Remove indentations and hyphenations.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t decade -l who -g who --dedent --dehyphen\n```\n\nAggregate text using customized temporal periods and grouped by party.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t "1920-1938,1929-1945,1946-1989,1990-2020" -l who -g party\n```\n\nAggregate text per document and group by gender and party.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t protocol -l who -g party -g gender\n```\n\nAggregate text per year grouped by gender and party and include only 1946-1989.\n\n```bash\nriksprot2text /path/to/corpus output.zip -m zip -t year -l who -g party -g gender -y 1946-1989\n```\n\n## Python API - Iterate XML protocols\n\nAggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.\n\n<!--pytest-codeblocks:skip-->\n```python\nimport pyriksprot\n\ntarget_filename: str = f\'output.zip\'\nopts = {\n    \'source_folder\': \'/path/to/corpus\',\n    \'target\': \'outout.zip\',\n    \'target_type\': \'files-in-zip\',\n    \'segment_level\': SegmentLevel.Who,\n    \'dedent\': True,\n    \'dehyphen\': False,\n    \'years\': \'1955-1965\',\n    \'temporal_key\': TemporalKey.Protocol,\n    \'group_keys\': (GroupingKey.Party, GroupingKey.Gender),\n}\n\npyriksprot.extract_corpus_text(**opts)\n\n```\n\n\nIterate over protocol and speaker:\n\n```python\n\nfrom pyriksprot import interface, iterstors\n\nitems: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(\n    filenames=filenames, segment_level=SegmentLevel.Who, segment_skip_size=0, processes=4\n)\n\nfor item in items:\n    print(item.who, len(item.text))\n\n```\n\nIterate over protocol and speech, skip empty:\n\n```python\n\nfrom pyriksprot import interface, iterstors\n\nitems: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(\n    filenames=filenames, segment_level=SegmentLevel.Who, segment_skip_size=1, processes=4\n)\n\nfor item in items:\n    print(item.who, len(item.text))\n\n```\n\nIterate over protocol and speech, apply preprocess function(s):\n\n```python\n\nfrom pyriksprot import interface, iterstors\nimport ftfy  # pip install ftfy\nimport unidecode\n\nfix_text: Callable[[str], str] = pyriksprot.compose(\n    [str.lower, pyriksprot.dedent, ftfy.fix_character_width, unidecode.unidecode ]\n)\nitems: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(\n    filenames=filenames, segment_level=SegmentLevel.Speech, segment_skip_size=1, processes=4, preprocessor=fix_text,\n)\n\nfor item in items:\n    print(item.who, len(item.text))\n\n```\n\n## Python API - Iterate protocols as domain entities\n\n## CLI riksprot2tags:  Extract aggregated part-of-speech tagged corpus\n',
-    'author': 'Roger Mähler',
-    'author_email': 'roger.mahler@hotmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://westac.se',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '==3.9.10',
+# Python package for reading and tagging Riksdagens Protokoll
+
+Batteries (tagger) not included.
+
+## Overview
+
+This package is intended to cover the following use cases:
+
+### Extract "text documents" from the Parla-CLARIN XML files
+
+Text can be extracted from the XML files at different granularity (paragraphs, utterance, speech, who, protocol). The text can be grouped (combined) into larger temporal blocks based on time (year, lustrum, decade or custom periods). Within each of these block the text in turn can be grouped by speaker attributes (who, party, gender).
+
+The text extraction can done using the `riksprot2text` utility, which is a CLI interface installed with the package, or in Python code using the API that this package exposes. The Python API exposed both streaming (SAX based) methods and a domain model API (i.e. Python classes representing protocols, speeches and utterances).
+
+Both the CLI and the API supports dehyphenation using method described in [Anföranden: Annotated and Augmented Parliamentary Debates from Sweden, Stian Rødven Eide, 2020](https://gup.ub.gu.se/publication/302449). The API also supports user defined text transformations.
+
+### Extract PoS-tagged versions of the Parla-CLARIN XML files
+
+Part-of-speech tagged versions of the protocols can be extracted with the same granularity and aggregation as described above for the raw text. The returned documents are tab-separated files with fields for text, baseform and pos-tag (UPOS, XPOS). Note that the actual part-of-speech tagging is done using tools found in the `pyriksprot_tagging` repository ([link](https://github.com/welfare-state-analytics/westac_parlaclarin_pipeline)).
+
+Currently there are no open-source tagged versions of the corpos avaliable. The tagging is done using [Stanza](https://stanfordnlp.github.io/stanza/) with Swedish language models produced and made publically avaliable by Språkbanken Text.
+
+### Store extracted text
+
+The extracted text can be stored as optionally compressed plain text files on disk, or in a ZIP-archive.
+
+## Pre-requisites
+
+- Python >=3.11
+- A folder containing the Riksdagen Protokoll (parliamentary protocols) Github repository.
+
+```bash
+cd some-folder \
+git clone --branch "tag" tags/"tag" --depth 1 https://github.com/welfare-state-analytics/riksdagen-corpus.git
+cd riksdagen-corpus
+git config core.quotepath off
+
+```
+
+## Installation (Linux)
+
+Create an new isolated virtual environment for pyriksprot:
+
+```bash
+mkdir /path/to/new/pyriksprot-folder
+cd /path/to/new/pyriksprot-folder
+python -m venv .venv
+```
+
+Activate the environment:
+
+```bash
+cd /path/to/new/pyriksprot-folder
+source .venv/bin/activate
+```
+
+Install `pyriksprot` in activated virtual environment.
+
+```bash
+pip install pyriksprot
+```
+
+## CLI riksprot2text:  Extract aggregated text corpus from Parla-CLARIN XML files
+
+```bash
+
+λ riksprot2text --help
+
+Usage: riksprot2text [OPTIONS] SOURCE_FOLDER TARGET
+
+Options:
+  -m, --mode [plain|zip|gzip|bz2|lzma]
+                                  Target type
+  -t, --temporal-key TEXT         Temporal partition key(s)
+  -y, --years TEXT                Years to include in output
+  -g, --group-key TEXT            Partition key(s)
+  -p, --processes INTEGER RANGE   Number of processes to use
+  -l, --segment-level [protocol|speech|utterance|paragraph|who]
+                                  Protocol extract segment level
+  -e, --keep-order                Keep output in filename order (slower, multiproc)
+
+  -s, --skip-size INTEGER RANGE   Skip blocks of char length less than
+  -d, --dedent                    Remove indentation
+  -k, --dehyphen                  Dehyphen text
+  --help                          Show this message and exit.
+
+  λ metadata2db --help
+Usage: metadata2db.py [OPTIONS] COMMAND [ARGS]...
+
+  CLI tool to manage riksprot metadata
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  columns
+  database
+  download
+  filenames
+  index
+
+  λ metadata2db.py database --help
+Usage: metadata2db.py database [OPTIONS] TARGET
+
+Options:
+  --tag TEXT             Metadata version
+  --source-folder TEXT
+  --force                Force overwrite
+  --load-index           Load utterance index
+  --scripts-folder TEXT  Apply scripts in specified folder to DB. If not
+                         specified the scripts are loaded from SQL-module.
+  --skip-scripts         Skip loading SQL scripts
+  --help                 Show this message and exit.
+
+
+  λ metadata2db index --help
+Usage: metadata2db.py index [OPTIONS] CORPUS_FOLDER TARGET_FOLDER
+
+Options:
+  --help  Show this message and exit.
+
+```
+
+
+### Examples CLI
+
+Aggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.
+
+```python
+riksprot2text /path/to/corpus output.zip -m zip -t year -l protocol -g who --skip-size 50
+```
+
+Aggregate text per decade grouped by speaker. Store result in a single zip. Remove indentations and hyphenations.
+
+```bash
+riksprot2text /path/to/corpus output.zip -m zip -t decade -l who -g who --dedent --dehyphen
+```
+
+Aggregate text using customized temporal periods and grouped by party.
+
+```bash
+riksprot2text /path/to/corpus output.zip -m zip -t "1920-1938,1929-1945,1946-1989,1990-2020" -l who -g party
+```
+
+Aggregate text per document and group by gender and party.
+
+```bash
+riksprot2text /path/to/corpus output.zip -m zip -t protocol -l who -g party -g gender
+```
+
+Aggregate text per year grouped by gender and party and include only 1946-1989.
+
+```bash
+riksprot2text /path/to/corpus output.zip -m zip -t year -l who -g party -g gender -y 1946-1989
+```
+
+## Python API - Iterate XML protocols
+
+Aggregate text per year grouped by speaker. Store result in a single zip. Skip documents less than 50 characters.
+
+<!--pytest-codeblocks:skip-->
+```python
+import pyriksprot
+
+target_filename: str = f'output.zip'
+opts = {
+    'source_folder': '/path/to/corpus',
+    'target': 'outout.zip',
+    'target_type': 'files-in-zip',
+    'segment_level': SegmentLevel.Who,
+    'dedent': True,
+    'dehyphen': False,
+    'years': '1955-1965',
+    'temporal_key': TemporalKey.Protocol,
+    'group_keys': (GroupingKey.Party, GroupingKey.Gender),
 }
 
+pyriksprot.extract_corpus_text(**opts)
+
+```
+
+
+Iterate over protocol and speaker:
+
+```python
+
+from pyriksprot import interface, iterstors
+
+items: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(
+    filenames=filenames, segment_level=SegmentLevel.Who, segment_skip_size=0, processes=4
+)
+
+for item in items:
+    print(item.who, len(item.text))
+
+```
+
+Iterate over protocol and speech, skip empty:
+
+```python
+
+from pyriksprot import interface, iterstors
+
+items: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(
+    filenames=filenames, segment_level=SegmentLevel.Who, segment_skip_size=1, processes=4
+)
+
+for item in items:
+    print(item.who, len(item.text))
+
+```
+
+Iterate over protocol and speech, apply preprocess function(s):
+
+```python
+
+from pyriksprot import interface, iterstors
+import ftfy  # pip install ftfy
+import unidecode
+
+fix_text: Callable[[str], str] = pyriksprot.compose(
+    [str.lower, pyriksprot.dedent, ftfy.fix_character_width, unidecode.unidecode ]
+)
+items: Iterable[interface.ProtocolSegment] = iterators.XmlProtocolTextIterator(
+    filenames=filenames, segment_level=SegmentLevel.Speech, segment_skip_size=1, processes=4, preprocessor=fix_text,
+)
+
+for item in items:
+    print(item.who, len(item.text))
+
+```
+
+## Python API - Iterate protocols as domain entities
+
+## CLI riksprot2tags:  Extract aggregated part-of-speech tagged corpus
 
-setup(**setup_kwargs)
```

