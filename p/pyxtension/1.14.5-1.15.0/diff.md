# Comparing `tmp/pyxtension-1.14.5-py3-none-any.whl.zip` & `tmp/pyxtension-1.15.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 29096 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    15389 b- defN 23-Jan-15 20:29 pyxtension/Json.py
--rw-rw-rw-  2.0 fat     1885 b- defN 23-Jan-15 20:29 pyxtension/__init__.py
--rw-rw-rw-  2.0 fat    11752 b- defN 23-Jan-15 20:29 pyxtension/fileutils.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Jan-15 20:29 pyxtension/racelib.py
--rw-rw-rw-  2.0 fat    58818 b- defN 23-Jan-15 20:29 pyxtension/streams.py
--rw-rw-rw-  2.0 fat      775 b- defN 23-Jan-15 20:29 pyxtension/throttler.py
--rw-rw-rw-  2.0 fat      103 b- defN 22-Dec-15 23:05 pyxtension-1.14.5.data/data/requirements.txt
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jan-15 20:29 pyxtension-1.14.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    16499 b- defN 23-Jan-15 20:29 pyxtension-1.14.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-15 20:29 pyxtension-1.14.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jan-15 20:29 pyxtension-1.14.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      979 b- defN 23-Jan-15 20:29 pyxtension-1.14.5.dist-info/RECORD
-12 files, 109660 bytes uncompressed, 27460 bytes compressed:  75.0%
+Zip file size: 30371 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat    15389 b- defN 23-Apr-13 09:45 pyxtension/Json.py
+-rw-rw-rw-  2.0 fat     1885 b- defN 23-Apr-13 09:45 pyxtension/__init__.py
+-rw-rw-rw-  2.0 fat    11752 b- defN 23-Apr-13 09:45 pyxtension/fileutils.py
+-rw-rw-rw-  2.0 fat     2647 b- defN 23-Apr-13 09:45 pyxtension/models.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Apr-13 09:45 pyxtension/racelib.py
+-rw-rw-rw-  2.0 fat    58818 b- defN 23-Apr-13 09:45 pyxtension/streams.py
+-rw-rw-rw-  2.0 fat      775 b- defN 23-Apr-13 09:45 pyxtension/throttler.py
+-rw-rw-rw-  2.0 fat      134 b- defN 23-Apr-12 22:39 pyxtension-1.15.0.data/data/requirements.txt
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17203 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1056 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/RECORD
+13 files, 113119 bytes uncompressed, 28619 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -3,35 +3,38 @@
 
 Filename: pyxtension/__init__.py
 Comment: 
 
 Filename: pyxtension/fileutils.py
 Comment: 
 
+Filename: pyxtension/models.py
+Comment: 
+
 Filename: pyxtension/racelib.py
 Comment: 
 
 Filename: pyxtension/streams.py
 Comment: 
 
 Filename: pyxtension/throttler.py
 Comment: 
 
-Filename: pyxtension-1.14.5.data/data/requirements.txt
+Filename: pyxtension-1.15.0.data/data/requirements.txt
 Comment: 
 
-Filename: pyxtension-1.14.5.dist-info/LICENSE
+Filename: pyxtension-1.15.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyxtension-1.14.5.dist-info/METADATA
+Filename: pyxtension-1.15.0.dist-info/METADATA
 Comment: 
 
-Filename: pyxtension-1.14.5.dist-info/WHEEL
+Filename: pyxtension-1.15.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyxtension-1.14.5.dist-info/top_level.txt
+Filename: pyxtension-1.15.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyxtension-1.14.5.dist-info/RECORD
+Filename: pyxtension-1.15.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyxtension-1.14.5.dist-info/LICENSE` & `pyxtension-1.15.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyxtension-1.14.5.dist-info/METADATA` & `pyxtension-1.15.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,655 +1,656 @@
-Metadata-Version: 2.1
-Name: pyxtension
-Version: 1.14.5
-Summary: Extension library for Python
-Home-page: https://github.com/asuiu/pyxtension
-Author: Andrei Suiu
-Author-email: andrei.suiu@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tqdm (>=4.62.0) ; python_version >= "3"
-Requires-Dist: pydantic (>=1.8.2) ; python_version >= "3"
-Requires-Dist: tblib (>=1.7.0) ; python_version >= "3"
-Provides-Extra: dev
-Requires-Dist: mock ; (python_version < "3") and extra == 'dev'
-Provides-Extra: test
-Requires-Dist: mock ; (python_version < "3") and extra == 'test'
-
-pyxtension
-==========
-
-| |build Status|
-| |Coverage Status|
-
-`pyxtension <https://github.com/asuiu/pyxtension>`__ is a pure Python
-GNU-licensed library that includes Scala-like streams, Json with
-attribute access syntax, and other common-use stuff.
-
-Installation
-------------
-
-::
-
-    pip install pyxtension
-
-or from Github:
-
-::
-
-    git clone https://github.com/asuiu/pyxtension.git
-    cd pyxtension
-    python setup.py install
-
-or
-
-::
-
-    git submodule add https://github.com/asuiu/pyxtension.git
-
-Modules overview
-----------------
-
-Json.py
-~~~~~~~
-
-Json
-^^^^
-
-| A ``dict`` subclass to represent a Json object. You should be able to
-  use this
-| absolutely anywhere you can use a ``dict``. While this is probably the
-  class you
-| want to use, there are a few caveats that follow from this being a
-  ``dict`` under
-| the hood.
-
-**Never again will you have to write code like this**:
-
-.. code:: python
-
-            body = {
-                'query': {
-                    'filtered': {
-                        'query': {
-                            'match': {'description': 'addictive'}
-                        },
-                        'filter': {
-                            'term': {'created_by': 'ASU'}
-                        }
-                    }
-                }
-            }
-
-From now on, you may simply write the following three lines:
-
-.. code:: python
-
-            body = Json()
-            body.query.filtered.query.match.description = 'addictive'
-            body.query.filtered.filter.term.created_by = 'ASU'
-
-streams.py
-~~~~~~~~~~
-
-stream
-^^^^^^
-
-| ``stream`` subclasses ``collections.Iterable``. It's the same Python
-  iterable, but with more added methods, suitable for multithreading and
-  multiprocess processings.
-| Used to create stream processing pipelines, similar to those used in
-  `Scala <http://www.scala-lang.org/>`__ and
-  `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__ programming
-  model.
-| Those who used `Apache Spark <http://spark.apache.org/>`__
-  `RDD <http://spark.apache.org/docs/latest/programming-guide.html#rdd-operations>`__
-  functions will find this model of processing very easy to use.
-
-`streams <https://github.com/asuiu/pyxtension/blob/master/streams.py>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-**Never again will you have to write code like this**:
-
-.. code:: python
-
-    > lst = xrange(1,6)
-    > reduce(lambda x, y: x * y, map(lambda _: _ * _, filter(lambda _: _ % 2 == 0, lst)))
-    64
-
-From now on, you may simply write the following lines:
-
-.. code:: python
-
-    > the_stream = stream( xrange(1,6) )
-    > the_stream.\
-        filter(lambda _: _ % 2 == 0).\
-        map(lambda _: _ * _).\
-        reduce(lambda x, y: x * y)
-    64
-
-A Word Count `Map-Reduce <https://en.wikipedia.org/wiki/MapReduce>`__ naive example using multiprocessing map
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code:: python
-
-    corpus = [
-        "MapReduce is a programming model and an associated implementation for processing and generating large data sets with a parallel, distributed algorithm on a cluster.",
-        "At Google, MapReduce was used to completely regenerate Google's index of the World Wide Web",
-        "Conceptually similar approaches have been very well known since 1995 with the Message Passing Interface standard having reduce and scatter operations."]
-
-    def reduceMaps(m1, m2):
-        for k, v in m2.iteritems():
-            m1[k] = m1.get(k, 0) + v
-        return m1
-
-    word_counts = stream(corpus).\
-        mpmap(lambda line: stream(line.lower().split(' ')).countByValue()).\
-        reduce(reduceMaps)
-
-Basic methods
-^^^^^^^^^^^^^
-
-**map(f)**
-''''''''''
-
-Identic with builtin ``map`` but returns a stream
-
-**mpmap(f, poolSize=16)**
-'''''''''''''''''''''''''
-
-Parallel ordered map using ``multiprocessing.Pool.imap()``.
-
-It can replace the ``map`` when need to split computations to multiple
-cores, and order of results matters.
-
-It spawns at most ``poolSize`` processes and applies the ``f`` function.
-
-The elements in the result stream appears in the same order they appear
-in the initial iterable.
-
-::
-
-    :type f: (T) -> V
-    :rtype: `stream`
-
-**mpfastmap(f, poolSize=16)**
-'''''''''''''''''''''''''''''
-
-Parallel ordered map using ``multiprocessing.Pool.imap_unordered()``.
-
-It can replace the ``map`` when the ordered of results doesn't matter.
-
-It spawns at most ``poolSize`` processes and applies the ``f`` function.
-
-The elements in the result stream appears in the unpredicted order.
-
-::
-
-    :type f: (T) -> V
-    :rtype: `stream`
-
-**fastmap(f, poolSize=16)**
-'''''''''''''''''''''''''''
-
-| Parallel unordered map using multithreaded pool.
-| It can replace the ``map`` when the ordered of results doesn't matter.
-
-It spawns at most ``poolSize`` threads and applies the ``f`` function.
-
-The elements in the result stream appears in the unpredicted order.
-
-Because of CPython
-`GIL <https://wiki.python.org/moin/GlobalInterpreterLock>`__ it's most
-usefull for I/O or CPU intensive consuming native functions, or on
-Jython or IronPython interpreters.
-
-:type f: (T) -> V
-
-:rtype: ``stream``
-
-\*\*flatMap(predicate=\_IDENTITY\_FUNC)\*\*
-:param predicate: is a function that will receive elements of self collection and return an iterable
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-By default predicate is an identity function
-
-:type predicate: (V)-> collections.Iterable[T]
-
-:return: will return stream of objects of the same type of elements from the stream returned by predicate()
-
-Example:
-
-.. code:: python
-
-    stream([[1, 2], [3, 4], [4, 5]]).flatMap().toList() == [1, 2, 3, 4, 4, 5]
-
-**filter(predicate)**
-'''''''''''''''''''''
-
-identic with builtin filter, but returns stream
-
-**reversed()**
-''''''''''''''
-
-returns reversed stream
-
-**exists(predicate)**
-'''''''''''''''''''''
-
-Tests whether a predicate holds for some of the elements of this
-sequence.
-
-:rtype: bool
-
-Example:
-
-.. code:: python
-
-    stream([1, 2, 3]).exists(0) -> False
-    stream([1, 2, 3]).exists(1) -> True
-
-\*\*keyBy(keyfunc = \_IDENTITY\_FUNC)\*\*
-Transforms stream of values to a stream of tuples (key, value)
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-:param keyfunc: function to map values to keys
-
-:type keyfunc: (V) -> T
-
-:return: stream of Key, Value pairs
-
-:rtype: stream[( T, V )]
-
-Example:
-
-.. code:: python
-
-    stream([1, 2, 3, 4]).keyBy(lambda _:_ % 2) -> [(1, 1), (0, 2), (1, 3), (0, 4)]
-
-**groupBy()**
-'''''''''''''
-
-groupBy([keyfunc]) -> Make an iterator that returns consecutive keys and
-groups from the iterable.
-
-The iterable needs not to be sorted on the same key function, but the
-keyfunction need to return hasable objects.
-
-:param keyfunc: [Optional] The key is a function computing a key value for each element.
-
-:type keyfunc: (T) -> (V)
-
-:return: (key, sub-iterator) grouped by each value of key(value).
-
-:rtype: stream[ ( V, slist[T] ) ]
-
-Example:
-
-.. code:: python
-
-    stream([1, 2, 3, 4]).groupBy(lambda _: _ % 2) -> [(0, [2, 4]), (1, [1, 3])]
-
-**countByValue()**
-''''''''''''''''''
-
-Returns a collections.Counter of values
-
-Example
-
-.. code:: python
-
-    stream(['a', 'b', 'a', 'b', 'c', 'd']).countByValue() == {'a': 2, 'b': 2, 'c': 1, 'd': 1}
-
-**distinct()**
-''''''''''''''
-
-Returns stream of distinct values. Values must be hashable.
-
-.. code:: python
-
-    stream(['a', 'b', 'a', 'b', 'c', 'd']).distinct() == {'a', 'b', 'c', 'd'}
-
-**reduce(f, init=None)**
-''''''''''''''''''''''''
-
-same arguments with builtin reduce() function
-
-**toSet()**
-'''''''''''
-
-returns sset() instance
-
-**toList()**
-''''''''''''
-
-returns slist() instance
-
-**toMap()**
-'''''''''''
-
-returns sdict() instance
-
-**sorted(key=None, cmp=None, reverse=False)**
-'''''''''''''''''''''''''''''''''''''''''''''
-
-same arguments with builtin sorted()
-
-**size()**
-''''''''''
-
-returns length of stream. Use carefully on infinite streams.
-
-**join(f)**
-'''''''''''
-
-Returns a string joined by f. Proivides same functionality as str.join()
-builtin method.
-
-if f is basestring, uses it to join the stream, else f should be a
-callable that returns a string to be used for join
-
-**mkString(f)**
-'''''''''''''''
-
-identic with join(f)
-
-**take(n)**
-'''''''''''
-
-::
-
-    returns first n elements from stream
-
-**head()**
-''''''''''
-
-::
-
-    returns first element from stream
-
-**zip()**
-'''''''''
-
-::
-
-    the same behavior with itertools.izip()
-
-**throttle(max_req: int, interval: float)**
-'''''''''
-
-::
-
-    throttles to process at most max_req elements pe every 'interval' seconds.
-
-
-\*\*unique(predicate=\_IDENTITY\_FUNC)\*\*
-Returns a stream of unique (according to predicate) elements appearing in the same order as in original stream
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-::
-
-    The items returned by predicate should be hashable and comparable.
-
-Statistics related methods
-^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-**entropy()**
-'''''''''''''
-
-calculates the Shannon entropy of the values from stream
-
-**pstddev()**
-'''''''''''''
-
-Calculates the population standard deviation.
-
-**mean()**
-''''''''''
-
-returns the arithmetical mean of the values
-
-**sum()**
-'''''''''
-
-returns the sum of elements from stream
-
-\*\*min(key=\_IDENTITY\_FUNC)\*\*
-same functionality with builtin min() funcion
-'''''''''''''''''''''''''''''''''''''''''''''
-
-\*\*min\_default(default, key=\_IDENTITY\_FUNC)\*\*
-same functionality with min() but returns :default: when called on empty streams
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-**max()**
-'''''''''
-
-same functionality with builtin max()
-
-\*\*maxes(key=\_IDENTITY\_FUNC)\*\*
-returns a stream of max values from stream
-''''''''''''''''''''''''''''''''''''''''''
-
-\*\*mins(key=\_IDENTITY\_FUNC)\*\*
-returns a stream of min values from stream
-''''''''''''''''''''''''''''''''''''''''''
-
-Other classes
-~~~~~~~~~~~~~
-
-slist
-^^^^^
-
-Inherits ``streams.stream`` and built-in ``list`` classes, and keeps in
-memory a list allowing faster index access
-
-sset
-^^^^
-
-Inherits ``streams.stream`` and built-in ``set`` classes, and keeps in
-memory the whole set of values
-
-sdict
-^^^^^
-
-Inherits ``streams.stream`` and built-in ``dict``, and keeps in memory
-the dict object.
-
-defaultstreamdict
-^^^^^^^^^^^^^^^^^
-
-Inherits ``streams.sdict`` and adds functionality of
-``collections.defaultdict`` from stdlib
-
-`throttler <https://github.com/asuiu/pyxtension/blob/master/throttler.py>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Thread-safe time throttler that can be attached on a stream to limit the number of calls per time interval.
-Example:
-
-.. code:: python
-
-        > from pyxtension.throttler import Throttler
-        > throttler = Throttler(5, 10)
-        > stream(range(100)).map(throttler.throttle).map(print).to_list()
-
-
-it will throttle the stream to max 5 calls per every 10 seconds.
-
-`Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-`Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__ is a
-module that provides mapping objects that allow their elements to be
-accessed both as keys and as attributes:
-
-.. code:: python
-
-        > from pyxtension.Json import Json
-        > a = Json({'foo': 'bar'})
-        > a.foo
-        'bar'
-        > a['foo']
-        'bar'
-
-Attribute access makes it easy to create convenient, hierarchical
-settings objects:
-
-.. code:: python
-
-        with open('settings.yaml') as fileobj:
-            settings = Json(yaml.safe_load(fileobj))
-
-        cursor = connect(**settings.db.credentials).cursor()
-
-        cursor.execute("SELECT column FROM table;")
-
-Basic Usage
-~~~~~~~~~~~
-
-| Json comes with two different classes, ``Json``, and ``JsonList``.
-| Json is fairly similar to native ``dict`` as it extends it an is a
-  mutable mapping that allow creating, accessing, and deleting key-value
-  pairs as attributes.
-| ``JsonList`` is similar to native ``list`` as it extends it and offers
-  a way to transform the ``dict`` objects from inside also in ``Json``
-  instances.
-
-Construction
-^^^^^^^^^^^^
-
-Directly from a JSON string
-'''''''''''''''''''''''''''
-
-.. code:: python
-
-    > Json('{"key1": "val1", "lst1": [1,2] }')
-    {u'key1': u'val1', u'lst1': [1, 2]}
-
-From ``tuple``\ s:
-''''''''''''''''''
-
-.. code:: python
-
-    > Json( ('key1','val1'), ('lst1', [1,2]) )
-    {'key1': 'val1', 'lst1': [1, 2]}
-    # keep in mind that you should provide at least two tuples with key-value pairs
-
-As a built-in ``dict``
-''''''''''''''''''''''
-
-.. code:: python
-
-    > Json( [('key1','val1'), ('lst1', [1,2])] )
-    {'key1': 'val1', 'lst1': [1, 2]}
-
-    Json({'key1': 'val1', 'lst1': [1, 2]})
-    {'key1': 'val1', 'lst1': [1, 2]}
-
-Convert to a ``dict``
-^^^^^^^^^^^^^^^^^^^^^
-
-.. code:: python
-
-    > json = Json({'key1': 'val1', 'lst1': [1, 2]})
-    > json.toOrig()
-    {'key1': 'val1', 'lst1': [1, 2]}
-
-Valid Names
-^^^^^^^^^^^
-
-Any key can be used as an attribute as long as:
-
-#. The key represents a valid attribute (i.e., it is a string comprised
-   only of
-   alphanumeric characters and underscores that doesn't start with a
-   number)
-#. The key does not shadow a class attribute (e.g., get).
-
-Attributes vs. Keys
-^^^^^^^^^^^^^^^^^^^
-
-| There is a minor difference between accessing a value as an attribute
-  vs.
-| accessing it as a key, is that when a dict is accessed as an
-  attribute, it will
-| automatically be converted to a ``Json`` object. This allows you to
-  recursively
-| access keys::
-
-.. code:: python
-
-        > attr = Json({'foo': {'bar': 'baz'}})
-        > attr.foo.bar
-        'baz'
-
-| Relatedly, by default, sequence types that aren't ``bytes``, ``str``,
-  or ``unicode``
-| (e.g., ``list``\ s, ``tuple``\ s) will automatically be converted to
-  ``tuple``\ s, with any
-| mappings converted to ``Json``:
-
-.. code:: python
-
-        > attr = Json({'foo': [{'bar': 'baz'}, {'bar': 'qux'}]})
-        > for sub_attr in attr.foo:
-        >     print(sub_attr.bar)
-        'baz'
-        'qux'
-
-| To get this recursive functionality for keys that cannot be used as
-  attributes,
-| you can replicate the behavior by using dict syntax on ``Json``
-  object::
-
-
-.. code:: python
-
-        > json = Json({1: {'two': 3}})
-        > json[1].two
-        3
-
-``JsonList`` usage examples:
-
-.. code:: python
-
-    > json = Json('{"lst":[1,2,3]}')
-    > type(json.lst)
-    <class 'pyxtension.Json.JsonList'>
-
-    > json = Json('{"1":[1,2]}')
-    > json["1"][1]
-    2
-
-Assignment as keys will still work::
-
-.. code:: python
-
-        > json = Json({'foo': {'bar': 'baz'}})
-        > json['foo']['bar'] = 'baz'
-        > json.foo
-        {'bar': 'baz'}
-
-License
-~~~~~~~
-
-| pyxtension is released under a GNU Public license.
-| The idea for
-  `Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__
-  module was inspired from
-  `addict <https://github.com/mewwts/addict%3E>`__ and
-  `AttrDict <https://github.com/bcj/AttrDict>`__,
-| but it has a better performance with lower memory consumption.
-
-.. |build Status| image:: https://travis-ci.org/asuiu/pyxtension.svg?branch=master
-   :target: https://travis-ci.org/asuiu/pyxtension
-.. |Coverage Status| image:: https://coveralls.io/repos/asuiu/pyxtension/badge.svg?branch=master&service=github
-   :target: https://coveralls.io/github/asuiu/pyxtension?branch=master
+Metadata-Version: 2.1
+Name: pyxtension
+Version: 1.15.0
+Summary: Extension library for Python
+Home-page: https://github.com/asuiu/pyxtension
+Author: Andrei Suiu
+Author-email: andrei.suiu@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: json-composite-encoder (>=1.0.0)
+Requires-Dist: tqdm (>=4.62.0) ; python_version >= "3"
+Requires-Dist: pydantic (>=1.8.2) ; python_version >= "3"
+Requires-Dist: tblib (>=1.7.0) ; python_version >= "3"
+Provides-Extra: dev
+Requires-Dist: mock ; (python_version < "3") and extra == 'dev'
+Provides-Extra: test
+Requires-Dist: mock ; (python_version < "3") and extra == 'test'
+
+pyxtension
+==========
+
+| |build Status|
+| |Coverage Status|
+
+`pyxtension <https://github.com/asuiu/pyxtension>`__ is a pure Python
+MIT-licensed library that includes Scala-like streams, Json with
+attribute access syntax, and other common-use stuff.
+
+Installation
+------------
+
+::
+
+    pip install pyxtension
+
+or from Github:
+
+::
+
+    git clone https://github.com/asuiu/pyxtension.git
+    cd pyxtension
+    python setup.py install
+
+or
+
+::
+
+    git submodule add https://github.com/asuiu/pyxtension.git
+
+Modules overview
+----------------
+
+Json.py
+~~~~~~~
+
+Json
+^^^^
+
+| A ``dict`` subclass to represent a Json object. You should be able to
+  use this
+| absolutely anywhere you can use a ``dict``. While this is probably the
+  class you
+| want to use, there are a few caveats that follow from this being a
+  ``dict`` under
+| the hood.
+
+**Never again will you have to write code like this**:
+
+.. code:: python
+
+            body = {
+                'query': {
+                    'filtered': {
+                        'query': {
+                            'match': {'description': 'addictive'}
+                        },
+                        'filter': {
+                            'term': {'created_by': 'ASU'}
+                        }
+                    }
+                }
+            }
+
+From now on, you may simply write the following three lines:
+
+.. code:: python
+
+            body = Json()
+            body.query.filtered.query.match.description = 'addictive'
+            body.query.filtered.filter.term.created_by = 'ASU'
+
+streams.py
+~~~~~~~~~~
+
+stream
+^^^^^^
+
+| ``stream`` subclasses ``collections.Iterable``. It's the same Python
+  iterable, but with more added methods, suitable for multithreading and
+  multiprocess processings.
+| Used to create stream processing pipelines, similar to those used in
+  `Scala <http://www.scala-lang.org/>`__ and
+  `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__ programming
+  model.
+| Those who used `Apache Spark <http://spark.apache.org/>`__
+  `RDD <http://spark.apache.org/docs/latest/programming-guide.html#rdd-operations>`__
+  functions will find this model of processing very easy to use.
+
+`streams <https://github.com/asuiu/pyxtension/blob/master/streams.py>`__
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+**Never again will you have to write code like this**:
+
+.. code:: python
+
+    > lst = xrange(1,6)
+    > reduce(lambda x, y: x * y, map(lambda _: _ * _, filter(lambda _: _ % 2 == 0, lst)))
+    64
+
+From now on, you may simply write the following lines:
+
+.. code:: python
+
+    > the_stream = stream( xrange(1,6) )
+    > the_stream.\
+        filter(lambda _: _ % 2 == 0).\
+        map(lambda _: _ * _).\
+        reduce(lambda x, y: x * y)
+    64
+
+A Word Count `Map-Reduce <https://en.wikipedia.org/wiki/MapReduce>`__ naive example using multiprocessing map
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code:: python
+
+    corpus = [
+        "MapReduce is a programming model and an associated implementation for processing and generating large data sets with a parallel, distributed algorithm on a cluster.",
+        "At Google, MapReduce was used to completely regenerate Google's index of the World Wide Web",
+        "Conceptually similar approaches have been very well known since 1995 with the Message Passing Interface standard having reduce and scatter operations."]
+
+    def reduceMaps(m1, m2):
+        for k, v in m2.iteritems():
+            m1[k] = m1.get(k, 0) + v
+        return m1
+
+    word_counts = stream(corpus).\
+        mpmap(lambda line: stream(line.lower().split(' ')).countByValue()).\
+        reduce(reduceMaps)
+
+Basic methods
+^^^^^^^^^^^^^
+
+**map(f)**
+''''''''''
+
+Identic with builtin ``map`` but returns a stream
+
+**mpmap(f, poolSize=16)**
+'''''''''''''''''''''''''
+
+Parallel ordered map using ``multiprocessing.Pool.imap()``.
+
+It can replace the ``map`` when need to split computations to multiple
+cores, and order of results matters.
+
+It spawns at most ``poolSize`` processes and applies the ``f`` function.
+
+The elements in the result stream appears in the same order they appear
+in the initial iterable.
+
+::
+
+    :type f: (T) -> V
+    :rtype: `stream`
+
+**mpfastmap(f, poolSize=16)**
+'''''''''''''''''''''''''''''
+
+Parallel ordered map using ``multiprocessing.Pool.imap_unordered()``.
+
+It can replace the ``map`` when the ordered of results doesn't matter.
+
+It spawns at most ``poolSize`` processes and applies the ``f`` function.
+
+The elements in the result stream appears in the unpredicted order.
+
+::
+
+    :type f: (T) -> V
+    :rtype: `stream`
+
+**fastmap(f, poolSize=16)**
+'''''''''''''''''''''''''''
+
+| Parallel unordered map using multithreaded pool.
+| It can replace the ``map`` when the ordered of results doesn't matter.
+
+It spawns at most ``poolSize`` threads and applies the ``f`` function.
+
+The elements in the result stream appears in the unpredicted order.
+
+Because of CPython
+`GIL <https://wiki.python.org/moin/GlobalInterpreterLock>`__ it's most
+usefull for I/O or CPU intensive consuming native functions, or on
+Jython or IronPython interpreters.
+
+:type f: (T) -> V
+
+:rtype: ``stream``
+
+\*\*flatMap(predicate=\_IDENTITY\_FUNC)\*\*
+:param predicate: is a function that will receive elements of self collection and return an iterable
+''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
+
+By default predicate is an identity function
+
+:type predicate: (V)-> collections.Iterable[T]
+
+:return: will return stream of objects of the same type of elements from the stream returned by predicate()
+
+Example:
+
+.. code:: python
+
+    stream([[1, 2], [3, 4], [4, 5]]).flatMap().toList() == [1, 2, 3, 4, 4, 5]
+
+**filter(predicate)**
+'''''''''''''''''''''
+
+identic with builtin filter, but returns stream
+
+**reversed()**
+''''''''''''''
+
+returns reversed stream
+
+**exists(predicate)**
+'''''''''''''''''''''
+
+Tests whether a predicate holds for some of the elements of this
+sequence.
+
+:rtype: bool
+
+Example:
+
+.. code:: python
+
+    stream([1, 2, 3]).exists(0) -> False
+    stream([1, 2, 3]).exists(1) -> True
+
+\*\*keyBy(keyfunc = \_IDENTITY\_FUNC)\*\*
+Transforms stream of values to a stream of tuples (key, value)
+''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
+
+:param keyfunc: function to map values to keys
+
+:type keyfunc: (V) -> T
+
+:return: stream of Key, Value pairs
+
+:rtype: stream[( T, V )]
+
+Example:
+
+.. code:: python
+
+    stream([1, 2, 3, 4]).keyBy(lambda _:_ % 2) -> [(1, 1), (0, 2), (1, 3), (0, 4)]
+
+**groupBy()**
+'''''''''''''
+
+groupBy([keyfunc]) -> Make an iterator that returns consecutive keys and
+groups from the iterable.
+
+The iterable needs not to be sorted on the same key function, but the
+keyfunction need to return hasable objects.
+
+:param keyfunc: [Optional] The key is a function computing a key value for each element.
+
+:type keyfunc: (T) -> (V)
+
+:return: (key, sub-iterator) grouped by each value of key(value).
+
+:rtype: stream[ ( V, slist[T] ) ]
+
+Example:
+
+.. code:: python
+
+    stream([1, 2, 3, 4]).groupBy(lambda _: _ % 2) -> [(0, [2, 4]), (1, [1, 3])]
+
+**countByValue()**
+''''''''''''''''''
+
+Returns a collections.Counter of values
+
+Example
+
+.. code:: python
+
+    stream(['a', 'b', 'a', 'b', 'c', 'd']).countByValue() == {'a': 2, 'b': 2, 'c': 1, 'd': 1}
+
+**distinct()**
+''''''''''''''
+
+Returns stream of distinct values. Values must be hashable.
+
+.. code:: python
+
+    stream(['a', 'b', 'a', 'b', 'c', 'd']).distinct() == {'a', 'b', 'c', 'd'}
+
+**reduce(f, init=None)**
+''''''''''''''''''''''''
+
+same arguments with builtin reduce() function
+
+**toSet()**
+'''''''''''
+
+returns sset() instance
+
+**toList()**
+''''''''''''
+
+returns slist() instance
+
+**toMap()**
+'''''''''''
+
+returns sdict() instance
+
+**sorted(key=None, cmp=None, reverse=False)**
+'''''''''''''''''''''''''''''''''''''''''''''
+
+same arguments with builtin sorted()
+
+**size()**
+''''''''''
+
+returns length of stream. Use carefully on infinite streams.
+
+**join(f)**
+'''''''''''
+
+Returns a string joined by f. Proivides same functionality as str.join()
+builtin method.
+
+if f is basestring, uses it to join the stream, else f should be a
+callable that returns a string to be used for join
+
+**mkString(f)**
+'''''''''''''''
+
+identic with join(f)
+
+**take(n)**
+'''''''''''
+
+::
+
+    returns first n elements from stream
+
+**head()**
+''''''''''
+
+::
+
+    returns first element from stream
+
+**zip()**
+'''''''''
+
+::
+
+    the same behavior with itertools.izip()
+
+**throttle(max_req: int, interval: float)**
+'''''''''
+
+::
+
+    throttles to process at most max_req elements pe every 'interval' seconds.
+
+
+\*\*unique(predicate=\_IDENTITY\_FUNC)\*\*
+Returns a stream of unique (according to predicate) elements appearing in the same order as in original stream
+''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
+
+::
+
+    The items returned by predicate should be hashable and comparable.
+
+Statistics related methods
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+**entropy()**
+'''''''''''''
+
+calculates the Shannon entropy of the values from stream
+
+**pstddev()**
+'''''''''''''
+
+Calculates the population standard deviation.
+
+**mean()**
+''''''''''
+
+returns the arithmetical mean of the values
+
+**sum()**
+'''''''''
+
+returns the sum of elements from stream
+
+\*\*min(key=\_IDENTITY\_FUNC)\*\*
+same functionality with builtin min() funcion
+'''''''''''''''''''''''''''''''''''''''''''''
+
+\*\*min\_default(default, key=\_IDENTITY\_FUNC)\*\*
+same functionality with min() but returns :default: when called on empty streams
+''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
+
+**max()**
+'''''''''
+
+same functionality with builtin max()
+
+\*\*maxes(key=\_IDENTITY\_FUNC)\*\*
+returns a stream of max values from stream
+''''''''''''''''''''''''''''''''''''''''''
+
+\*\*mins(key=\_IDENTITY\_FUNC)\*\*
+returns a stream of min values from stream
+''''''''''''''''''''''''''''''''''''''''''
+
+Other classes
+~~~~~~~~~~~~~
+
+slist
+^^^^^
+
+Inherits ``streams.stream`` and built-in ``list`` classes, and keeps in
+memory a list allowing faster index access
+
+sset
+^^^^
+
+Inherits ``streams.stream`` and built-in ``set`` classes, and keeps in
+memory the whole set of values
+
+sdict
+^^^^^
+
+Inherits ``streams.stream`` and built-in ``dict``, and keeps in memory
+the dict object.
+
+defaultstreamdict
+^^^^^^^^^^^^^^^^^
+
+Inherits ``streams.sdict`` and adds functionality of
+``collections.defaultdict`` from stdlib
+
+`throttler <https://github.com/asuiu/pyxtension/blob/master/throttler.py>`__
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Thread-safe time throttler that can be attached on a stream to limit the number of calls per time interval.
+Example:
+
+.. code:: python
+
+        > from pyxtension.throttler import Throttler
+        > throttler = Throttler(5, 10)
+        > stream(range(100)).map(throttler.throttle).map(print).to_list()
+
+
+it will throttle the stream to max 5 calls per every 10 seconds.
+
+`Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+`Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__ is a
+module that provides mapping objects that allow their elements to be
+accessed both as keys and as attributes:
+
+.. code:: python
+
+        > from pyxtension.Json import Json
+        > a = Json({'foo': 'bar'})
+        > a.foo
+        'bar'
+        > a['foo']
+        'bar'
+
+Attribute access makes it easy to create convenient, hierarchical
+settings objects:
+
+.. code:: python
+
+        with open('settings.yaml') as fileobj:
+            settings = Json(yaml.safe_load(fileobj))
+
+        cursor = connect(**settings.db.credentials).cursor()
+
+        cursor.execute("SELECT column FROM table;")
+
+Basic Usage
+~~~~~~~~~~~
+
+| Json comes with two different classes, ``Json``, and ``JsonList``.
+| Json is fairly similar to native ``dict`` as it extends it an is a
+  mutable mapping that allow creating, accessing, and deleting key-value
+  pairs as attributes.
+| ``JsonList`` is similar to native ``list`` as it extends it and offers
+  a way to transform the ``dict`` objects from inside also in ``Json``
+  instances.
+
+Construction
+^^^^^^^^^^^^
+
+Directly from a JSON string
+'''''''''''''''''''''''''''
+
+.. code:: python
+
+    > Json('{"key1": "val1", "lst1": [1,2] }')
+    {u'key1': u'val1', u'lst1': [1, 2]}
+
+From ``tuple``\ s:
+''''''''''''''''''
+
+.. code:: python
+
+    > Json( ('key1','val1'), ('lst1', [1,2]) )
+    {'key1': 'val1', 'lst1': [1, 2]}
+    # keep in mind that you should provide at least two tuples with key-value pairs
+
+As a built-in ``dict``
+''''''''''''''''''''''
+
+.. code:: python
+
+    > Json( [('key1','val1'), ('lst1', [1,2])] )
+    {'key1': 'val1', 'lst1': [1, 2]}
+
+    Json({'key1': 'val1', 'lst1': [1, 2]})
+    {'key1': 'val1', 'lst1': [1, 2]}
+
+Convert to a ``dict``
+^^^^^^^^^^^^^^^^^^^^^
+
+.. code:: python
+
+    > json = Json({'key1': 'val1', 'lst1': [1, 2]})
+    > json.toOrig()
+    {'key1': 'val1', 'lst1': [1, 2]}
+
+Valid Names
+^^^^^^^^^^^
+
+Any key can be used as an attribute as long as:
+
+#. The key represents a valid attribute (i.e., it is a string comprised
+   only of
+   alphanumeric characters and underscores that doesn't start with a
+   number)
+#. The key does not shadow a class attribute (e.g., get).
+
+Attributes vs. Keys
+^^^^^^^^^^^^^^^^^^^
+
+| There is a minor difference between accessing a value as an attribute
+  vs.
+| accessing it as a key, is that when a dict is accessed as an
+  attribute, it will
+| automatically be converted to a ``Json`` object. This allows you to
+  recursively
+| access keys::
+
+.. code:: python
+
+        > attr = Json({'foo': {'bar': 'baz'}})
+        > attr.foo.bar
+        'baz'
+
+| Relatedly, by default, sequence types that aren't ``bytes``, ``str``,
+  or ``unicode``
+| (e.g., ``list``\ s, ``tuple``\ s) will automatically be converted to
+  ``tuple``\ s, with any
+| mappings converted to ``Json``:
+
+.. code:: python
+
+        > attr = Json({'foo': [{'bar': 'baz'}, {'bar': 'qux'}]})
+        > for sub_attr in attr.foo:
+        >     print(sub_attr.bar)
+        'baz'
+        'qux'
+
+| To get this recursive functionality for keys that cannot be used as
+  attributes,
+| you can replicate the behavior by using dict syntax on ``Json``
+  object::
+
+
+.. code:: python
+
+        > json = Json({1: {'two': 3}})
+        > json[1].two
+        3
+
+``JsonList`` usage examples:
+
+.. code:: python
+
+    > json = Json('{"lst":[1,2,3]}')
+    > type(json.lst)
+    <class 'pyxtension.Json.JsonList'>
+
+    > json = Json('{"1":[1,2]}')
+    > json["1"][1]
+    2
+
+Assignment as keys will still work::
+
+.. code:: python
+
+        > json = Json({'foo': {'bar': 'baz'}})
+        > json['foo']['bar'] = 'baz'
+        > json.foo
+        {'bar': 'baz'}
+
+License
+~~~~~~~
+
+| pyxtension is released under a GNU Public license.
+| The idea for
+  `Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__
+  module was inspired from
+  `addict <https://github.com/mewwts/addict%3E>`__ and
+  `AttrDict <https://github.com/bcj/AttrDict>`__,
+| but it has a better performance with lower memory consumption.
+
+.. |build Status| image:: https://travis-ci.org/asuiu/pyxtension.svg?branch=master
+   :target: https://travis-ci.org/asuiu/pyxtension
+.. |Coverage Status| image:: https://coveralls.io/repos/asuiu/pyxtension/badge.svg?branch=master&service=github
+   :target: https://coveralls.io/github/asuiu/pyxtension?branch=master
```

## Comparing `pyxtension-1.14.5.dist-info/RECORD` & `pyxtension-1.15.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pyxtension/Json.py,sha256=uiafIjQIrsyzbhbBp48HHzEDBbuPfO6uQXtB4PsRqpI,15389
 pyxtension/__init__.py,sha256=PCbm4P4-Tr-Kyr10YxCYaER9gJE-_BsBrdGIRqlKqBw,1885
 pyxtension/fileutils.py,sha256=splDsyuOI_-t3TChrD4Py3VabhCcs87bdGynJ-PQd1E,11752
+pyxtension/models.py,sha256=Ptn8hsIgrVHM9EhoAJNIHdwLqZWfdf3zafsl1bwBH80,2647
 pyxtension/racelib.py,sha256=mAMO_pZGgT8mnDXCWWQRx_v17jaCowWnuBqnA4qBiyg,2268
 pyxtension/streams.py,sha256=BmzEtjFIe0c6VsmDSMD0h2vE8irNQYsiAKCehcNSRik,58818
 pyxtension/throttler.py,sha256=LDJgG5TAhwmwUWzuvPpwoNpEruMCqZz_Bfnzpu2WNoo,775
-pyxtension-1.14.5.data/data/requirements.txt,sha256=QQ3zXz7b-pPEaMeU6AHmwYusahlcdhXR5e06fo7mZfU,103
-pyxtension-1.14.5.dist-info/LICENSE,sha256=FCxjh5qaSQZB3aa6B14YcS1sc01c6nwy1snNJsDlUXc,1089
-pyxtension-1.14.5.dist-info/METADATA,sha256=c3fGnWROgTdKloO_NA90EaUUIJ9LEWSTmhaL2KsbXjA,16499
-pyxtension-1.14.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyxtension-1.14.5.dist-info/top_level.txt,sha256=wEW423Tnz4ikjYol7udkFtAXi7Kmns-TPB74OJ0m6gY,11
-pyxtension-1.14.5.dist-info/RECORD,,
+pyxtension-1.15.0.data/data/requirements.txt,sha256=rxumPsxCB5AXMESWsnpEl6bsVdw4BlQ3yrfi_6h5pvg,134
+pyxtension-1.15.0.dist-info/LICENSE,sha256=FCxjh5qaSQZB3aa6B14YcS1sc01c6nwy1snNJsDlUXc,1089
+pyxtension-1.15.0.dist-info/METADATA,sha256=g6gLpeJNUH4DeWj1I34jBuIqvJNF4Pl9SgIgQdgcVZ4,17203
+pyxtension-1.15.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pyxtension-1.15.0.dist-info/top_level.txt,sha256=wEW423Tnz4ikjYol7udkFtAXi7Kmns-TPB74OJ0m6gY,11
+pyxtension-1.15.0.dist-info/RECORD,,
```

