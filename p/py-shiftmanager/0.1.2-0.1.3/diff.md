# Comparing `tmp/py_shiftmanager-0.1.2.tar.gz` & `tmp/py_shiftmanager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_shiftmanager-0.1.2.tar", last modified: Tue Apr 11 13:06:53 2023, max compression
+gzip compressed data, was "py_shiftmanager-0.1.3.tar", last modified: Thu Apr 13 12:13:58 2023, max compression
```

## Comparing `py_shiftmanager-0.1.2.tar` & `py_shiftmanager-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-11 13:06:53.229206 py_shiftmanager-0.1.2/
--rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/MANIFEST.in
--rw-r--r--   0 amitnakash   (501) staff       (20)     6976 2023-04-11 13:06:53.229054 py_shiftmanager-0.1.2/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)     6657 2023-04-11 12:49:14.000000 py_shiftmanager-0.1.2/Readme.md
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-11 13:06:53.227995 py_shiftmanager-0.1.2/py_shiftmanager/
--rw-r--r--   0 amitnakash   (501) staff       (20)      370 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/py_shiftmanager/__init__.py
--rw-r--r--   0 amitnakash   (501) staff       (20)       42 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.2/py_shiftmanager/exceptions.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.2/py_shiftmanager/logger.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     4794 2023-04-11 13:05:25.000000 py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_compute.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     5100 2023-04-11 13:05:35.000000 py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_io.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/py_shiftmanager/timeout.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     3273 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/py_shiftmanager/worker.py
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-11 13:06:53.228842 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/
--rw-r--r--   0 amitnakash   (501) staff       (20)     6976 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)      436 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/SOURCES.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/dependency_links.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/requires.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/top_level.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-11 13:06:53.229251 py_shiftmanager-0.1.2/setup.cfg
--rw-r--r--   0 amitnakash   (501) staff       (20)      591 2023-04-11 12:49:38.000000 py_shiftmanager-0.1.2/setup.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-13 12:13:58.550831 py_shiftmanager-0.1.3/
+-rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.3/MANIFEST.in
+-rw-r--r--   0 amitnakash   (501) staff       (20)     8033 2023-04-13 12:13:58.550680 py_shiftmanager-0.1.3/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)     7714 2023-04-13 12:08:22.000000 py_shiftmanager-0.1.3/Readme.md
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-13 12:13:58.549677 py_shiftmanager-0.1.3/py_shiftmanager/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      289 2023-04-13 06:10:21.000000 py_shiftmanager-0.1.3/py_shiftmanager/__init__.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.3/py_shiftmanager/logger.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     4794 2023-04-13 12:06:40.000000 py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_compute.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5025 2023-04-13 12:06:42.000000 py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_io.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      782 2023-04-13 05:47:37.000000 py_shiftmanager-0.1.3/py_shiftmanager/timeout.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     3272 2023-04-13 11:21:29.000000 py_shiftmanager-0.1.3/py_shiftmanager/worker.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-13 12:13:58.550434 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/
+-rw-r--r--   0 amitnakash   (501) staff       (20)     8033 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)      406 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/requires.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-13 12:13:58.000000 py_shiftmanager-0.1.3/py_shiftmanager.egg-info/top_level.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-13 12:13:58.550879 py_shiftmanager-0.1.3/setup.cfg
+-rw-r--r--   0 amitnakash   (501) staff       (20)      591 2023-04-13 12:06:46.000000 py_shiftmanager-0.1.3/setup.py
```

### Comparing `py_shiftmanager-0.1.2/PKG-INFO` & `py_shiftmanager-0.1.3/Readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: py_shiftmanager
-Version: 0.1.2
-Summary: A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-
 # Py-ShiftManager
-#### v0.1.2
+#### v0.1.3
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
-## What's new in v0.1.1
+## What's new in v0.1.3
 This small update is dedicated to my friend Ram Manor :).
-* Introducing new timeout wrapper: *timeout_timer* - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
-* Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
-* *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
-* *ShiftManager_IO* now initializes the number of workers to 2, instead of 1, by default.  
-### New for v0.1.2
-* New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
+#### added in v0.1.1
+* ⏲️ Introducing new timeout wrapper: `@timeout_timer()` - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
+* 🔒 Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
+* 🛠️ *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
+* 🛠️ *ShiftManager_IO* now initializes the number of workers to `2`, instead of `1`, by default.  
+#### added in v0.1.2
+* ▶️ New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
 `with ShiftManager_Compute() as manager:`  
 `   manager.new_task(lambda x: x**2, 4)`  
 `   manager.new_task(lambda x: x**4, 13)`  
 then get the results:  
 `results = manager.get_results()`  
 It's that simple.  
+#### added in v0.1.3
+* 🛠️ Improved handling of queue exceptions - a better managing solution for large incoming amount of tasks.  
+* 🛠️ Improved task submission logic.
+* 🔒 Improved encapsulation.
+* 🛠️ New method added - `configure()`; read more under *'API'* section.   
+* 🛠️ Improved concurrency and parallelism in the IO module.
+* ⌫ Deprecated methods - `queue_in_size()`, `queue_out_size()` 
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py-shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py-shiftmanager.timeout import timeout_timer`
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_IO(num_of_workers=4)`  
-
-**Note**: by default *ShiftManager* objects init with these values for its attributes:
+By default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
-* queue size = `10`    
+* input_q_size = `10`
+* output_q_size = `15`
+ 
+**Note**: Once initialized, queue size cannot be changed.  
 
-Also, by default the output queue is set to 1.5 times the input queue size.
-  
 # Add some tasks to the input queue
-Assume we have created a function and applied the *timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
+Assume we have created a function called 'get_status()' that uses *requests* and applied the *@timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
 `manager.new_batch(tasks)`  
   
-**Note**: you can also pass *lambda* functions.
+**Note**: you can also pass in *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -77,21 +77,23 @@
 And here's an example of how to use Py-ShiftManager to handle computational tasks:
 
 `from py-shiftmanager import ShiftManager_Compute`  
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_Compute(num_of_workers=4)`  
 But this time we'll increase the number to 5 using simple addition:  
-`manager + 1` - now *manager* is set to run 5 workers.
+`manager + 1` - now *manager* is set to run 5 workers.   
 
-**Note**: by default *ShiftManager_Compute* init with these default values for its attributes:  
-* num_of_workers = *number of CPU's in the system.*
+By default *ShiftManager_Compute* initializes with these default values for its attributes:  
+* num_of_workers = *number of CPU's in the system.* 
 * daemon = `False`
-* queue size = `10`
+* input_q_size = `10`
+* output_q_size = `15`  
 
+**Note**: Once initialized, queue size cannot be changed.  
 # Add some tasks to the input queue
 We can assign single tasks, like so:  
 `manager.new_task(lambda x: x**2, 3)`  
 `manager.new_task(lambda x: x**3, 4)`  
 `manager.new_task(lambda x, y: x**4 + y, 5, 9)`  
 or submit a batch by passing a list of tuples:  
 `tasks = [(lambda x: x**2, 3),(lambda x: x**3, 4)]`
@@ -112,59 +114,59 @@
 # Wait for the tasks to complete
 `manager.end_shift()`  
 This method sends a shut-down signal to all workers, they will stop gracefully.
 
 ## API
 
 **ShiftManager_IO**  
-`ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> None`  
-Creates a new ShiftManager instance with the specified number of workers, daemon status, and queue size.
-
-`new_task(func: Callable, task: Any) -> None`  
-Adds a new task to the input queue.
-
-`new_batch(tasks: List[tuple]) -> None`  
-Adds a list of tasks to the input queue.
+`ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
+Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
-`queue_in_size() -> int`  
-Returns the current size of the input queue, if implemented, else, exists gracefully.
+`new_task(func: Callable, task: Any, force: bool = False) -> None`  
+Adds a new task to the input queue; you could force it if you want.
 
-`queue_out_size() -> int`  
-Returns the current size of the output queue, if implemented, else, exists gracefully.
+`new_batch(tasks: List[tuple], force: bool = False) -> None`  
+Adds a list of tasks to the input queue; you could force it if you want.
 
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
-Ends the shift and waits for all tasks to complete.
+Ends the shift and waits for all tasks to complete.  
+
+`configure(**kwargs) -> None`  
+Allows the user to configure the following attributes by passing keyword arguments:  
+* `daemon: bool` - reconfigure workers daemon status. 
+* `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
+* `num_of_workers: int` - reconfigure number of workers.  
 
 **ShiftManager_Compute**  
-`ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> None`  
-Creates a new ShiftManager instance with the specified number of workers, daemon status, and queue size.
+`ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
+Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
 `new_task(func: Callable, task: Any) -> None`  
 Adds a new task to the input queue.
 
 `new_batch(tasks: List[tuple]) -> None`  
 Adds a list of tasks to the input queue.
 
-`queue_in_size() -> int`  
-Returns the current size of the input queue, if implemented, else, exists gracefully.
-
-`queue_out_size() -> int`  
-Returns the current size of the output queue, if implemented, else, exists gracefully.
-
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
 Ends the shift and waits for all tasks to complete.  
 
+`configure(**kwargs) -> None`  
+Allows the user to configure the following attributes by passing keyword arguments:  
+* `daemon: bool` - reconfigure workers daemon status. 
+* `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
+* `num_of_workers: int` - reconfigure number of workers.  
+
 **timeout_timer**  
 `@timeout_timer(seconds: int = 5)`  
-A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; 5 seconds by default.
+A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `5` seconds by default.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py_shiftmanager-0.1.2/Readme.md` & `py_shiftmanager-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,78 @@
+Metadata-Version: 2.1
+Name: py_shiftmanager
+Version: 0.1.3
+Summary: A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+
 # Py-ShiftManager
-#### v0.1.2
+#### v0.1.3
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
-## What's new in v0.1.1
+## What's new in v0.1.3
 This small update is dedicated to my friend Ram Manor :).
-* Introducing new timeout wrapper: *timeout_timer* - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
-* Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
-* *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
-* *ShiftManager_IO* now initializes the number of workers to 2, instead of 1, by default.  
-### New for v0.1.2
-* New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
+#### added in v0.1.1
+* ⏲️ Introducing new timeout wrapper: `@timeout_timer()` - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
+* 🔒 Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
+* 🛠️ *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
+* 🛠️ *ShiftManager_IO* now initializes the number of workers to `2`, instead of `1`, by default.  
+#### added in v0.1.2
+* ▶️ New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
 `with ShiftManager_Compute() as manager:`  
 `   manager.new_task(lambda x: x**2, 4)`  
 `   manager.new_task(lambda x: x**4, 13)`  
 then get the results:  
 `results = manager.get_results()`  
 It's that simple.  
+#### added in v0.1.3
+* 🛠️ Improved handling of queue exceptions - a better managing solution for large incoming amount of tasks.  
+* 🛠️ Improved task submission logic.
+* 🔒 Improved encapsulation.
+* 🛠️ New method added - `configure()`; read more under *'API'* section.   
+* 🛠️ Improved concurrency and parallelism in the IO module.
+* ⌫ Deprecated methods - `queue_in_size()`, `queue_out_size()` 
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py-shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py-shiftmanager.timeout import timeout_timer`
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_IO(num_of_workers=4)`  
-
-**Note**: by default *ShiftManager* objects init with these values for its attributes:
+By default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
-* queue size = `10`    
+* input_q_size = `10`
+* output_q_size = `15`
+ 
+**Note**: Once initialized, queue size cannot be changed.  
 
-Also, by default the output queue is set to 1.5 times the input queue size.
-  
 # Add some tasks to the input queue
-Assume we have created a function and applied the *timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
+Assume we have created a function called 'get_status()' that uses *requests* and applied the *@timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
 `manager.new_batch(tasks)`  
   
-**Note**: you can also pass *lambda* functions.
+**Note**: you can also pass in *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -69,21 +85,23 @@
 And here's an example of how to use Py-ShiftManager to handle computational tasks:
 
 `from py-shiftmanager import ShiftManager_Compute`  
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_Compute(num_of_workers=4)`  
 But this time we'll increase the number to 5 using simple addition:  
-`manager + 1` - now *manager* is set to run 5 workers.
+`manager + 1` - now *manager* is set to run 5 workers.   
 
-**Note**: by default *ShiftManager_Compute* init with these default values for its attributes:  
-* num_of_workers = *number of CPU's in the system.*
+By default *ShiftManager_Compute* initializes with these default values for its attributes:  
+* num_of_workers = *number of CPU's in the system.* 
 * daemon = `False`
-* queue size = `10`
+* input_q_size = `10`
+* output_q_size = `15`  
 
+**Note**: Once initialized, queue size cannot be changed.  
 # Add some tasks to the input queue
 We can assign single tasks, like so:  
 `manager.new_task(lambda x: x**2, 3)`  
 `manager.new_task(lambda x: x**3, 4)`  
 `manager.new_task(lambda x, y: x**4 + y, 5, 9)`  
 or submit a batch by passing a list of tuples:  
 `tasks = [(lambda x: x**2, 3),(lambda x: x**3, 4)]`
@@ -104,59 +122,59 @@
 # Wait for the tasks to complete
 `manager.end_shift()`  
 This method sends a shut-down signal to all workers, they will stop gracefully.
 
 ## API
 
 **ShiftManager_IO**  
-`ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> None`  
-Creates a new ShiftManager instance with the specified number of workers, daemon status, and queue size.
-
-`new_task(func: Callable, task: Any) -> None`  
-Adds a new task to the input queue.
-
-`new_batch(tasks: List[tuple]) -> None`  
-Adds a list of tasks to the input queue.
+`ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
+Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
-`queue_in_size() -> int`  
-Returns the current size of the input queue, if implemented, else, exists gracefully.
+`new_task(func: Callable, task: Any, force: bool = False) -> None`  
+Adds a new task to the input queue; you could force it if you want.
 
-`queue_out_size() -> int`  
-Returns the current size of the output queue, if implemented, else, exists gracefully.
+`new_batch(tasks: List[tuple], force: bool = False) -> None`  
+Adds a list of tasks to the input queue; you could force it if you want.
 
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
-Ends the shift and waits for all tasks to complete.
+Ends the shift and waits for all tasks to complete.  
+
+`configure(**kwargs) -> None`  
+Allows the user to configure the following attributes by passing keyword arguments:  
+* `daemon: bool` - reconfigure workers daemon status. 
+* `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
+* `num_of_workers: int` - reconfigure number of workers.  
 
 **ShiftManager_Compute**  
-`ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> None`  
-Creates a new ShiftManager instance with the specified number of workers, daemon status, and queue size.
+`ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
+Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
 `new_task(func: Callable, task: Any) -> None`  
 Adds a new task to the input queue.
 
 `new_batch(tasks: List[tuple]) -> None`  
 Adds a list of tasks to the input queue.
 
-`queue_in_size() -> int`  
-Returns the current size of the input queue, if implemented, else, exists gracefully.
-
-`queue_out_size() -> int`  
-Returns the current size of the output queue, if implemented, else, exists gracefully.
-
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
 Ends the shift and waits for all tasks to complete.  
 
+`configure(**kwargs) -> None`  
+Allows the user to configure the following attributes by passing keyword arguments:  
+* `daemon: bool` - reconfigure workers daemon status. 
+* `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
+* `num_of_workers: int` - reconfigure number of workers.  
+
 **timeout_timer**  
 `@timeout_timer(seconds: int = 5)`  
-A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; 5 seconds by default.
+A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `5` seconds by default.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_compute.py` & `py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,147 @@
+import datetime
+import queue
 import multiprocessing
+import threading
+import dill
 from typing import *
 
-from .worker import Worker_COM, PoisonPill
-from .shiftmanager_io import ShiftManager_IO
+from .worker import Worker_IO
 from .logger import Logger
 
 """
-ShiftManager_Compute:
-This module is part of the Py-ShiftManager module for handling IO/Computational tasks -
+ShiftManager_IO:
+This module is part of the Py_ShiftManager module for handling IO/Computational tasks -
 in managed queued environment.
 
-Handle all your computational tasks without bothering with concurrency, multiprocessing -
+Handle all your I/O tasks without bothering with concurrency, multithreading -
 or any other higher concept; simply use ShiftManager and enjoy the benefits of fast runtime speeds.
 
 Read the 'Readme.md' file for more documentation and information.
 """
 
 logger = Logger()
 
 
-class ShiftManager_Compute(ShiftManager_IO):
-    pool: multiprocessing.Pool
-
-    def __init__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, queue_size: int = 10) -> NoReturn:
-        super().__init__(num_of_workers, daemon)
-        self._q_in = multiprocessing.JoinableQueue(maxsize=queue_size)
-        self._q_out = multiprocessing.Queue(maxsize=int(queue_size * 1.5))
-        self.worker = Worker_COM()
-        self.workers = []
-        self._lock = multiprocessing.Lock()
+class ShiftManager_IO:
+    def __init__(self, num_of_workers: int = 2, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> NoReturn:
+        self.__num_of_workers = num_of_workers
+        self.__daemon = daemon
+        self.__q_in = queue.Queue(maxsize=input_q_size)
+        self.__q_out = multiprocessing.Queue(maxsize=output_q_size)
+        self.__worker = Worker_IO()
+        self.__workers = []
+        self.__lock = threading.Lock()
+        self.__put_timeout = 1
         
-    def __enter__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, queue_size: int = 10):
-        self.manager = ShiftManager_Compute(num_of_workers, daemon, queue_size)
+    def __enter__(self, num_of_workers: int = 2, daemon: bool = False, queue_size: int = 10):
+        self.manager = ShiftManager_IO(num_of_workers, daemon, queue_size)
         return self.manager
     
     def __exit__(self, exc_type, exc_val, exc_tb) -> NoReturn:
         if exc_type is not None:
             logger.logger.error(f"An exception of type {exc_type} occurred: {exc_val}")
         self.manager.handle_work()
         self.manager.end_shift()
 
     def __repr__(self):
-        return f"""ShiftManagerCOM;daemonized={self.daemon};workers={self._num_of_workers}"""
+        return f"""ShiftManagerIO;daemonized={self.__daemon};workers={self.__num_of_workers}"""
 
     """ Manual scaling of workers """
     def __add__(self, x: int) -> NoReturn:
-        super().__add__(x)
+        self.__num_of_workers += x
 
     def __sub__(self, x: int) -> NoReturn:
-        super().__sub__(x)
+        self.__num_of_workers -= x
 
     def __mul__(self, x: int) -> NoReturn:
-        super().__mul__(x)
+        self.__num_of_workers *= x
 
     def __divmod__(self, x: int) -> NoReturn:
-        super().__divmod__(x)
-
-    """ Task and queue management """
-    def new_task(self, func: Callable, *args) -> NoReturn:
-        super().new_task(func, *args)
-
-    def new_batch(self, tasks: List[tuple]) -> NoReturn:
-        super().new_batch(tasks)
+        self.__num_of_workers /= x
 
-    def queue_in_size(self) -> int or str:
-        return super().queue_in_size()
+    def __submit_task(self, new_task, force: bool = False) -> NoReturn:
+        try:
+            if force:
+                self.__lock.acquire()
+                self.__q_in.put_nowait(new_task)
+            else:
+                self.__lock.acquire()
+                self.__q_in.put(new_task, timeout=self.__put_timeout)
+        except queue.Full:
+            logger.logger.error("INPUT-QUEUE IS FULL.")
+        finally:
+            self.__lock.release()
+            
+    def configure(self, **kwargs) -> NoReturn:
+        if kwargs['put_timeout']:
+            self.__put_timeout = kwargs['put_timeout']
+        if kwargs['num_of_workers']:
+            self.__num_of_workers = kwargs['num_of_workers']
+        if kwargs['daemon']:
+            self.__daemon = kwargs['daemon']
 
-    def queue_out_size(self) -> int or str:
-        return super().queue_out_size()
+    """ Task and queue management """
+    def new_task(self, func: Callable, *args, force: bool = False) -> NoReturn:
+        new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args}
+        self.__submit_task(new_task, force)
+
+    def new_batch(self, tasks: List[tuple], force: bool = False) -> NoReturn:
+        for task in tasks:
+            self.new_task(*task, force=force)
+
+    # def queue_in_size(self) -> int or NoReturn:
+    #     try:
+    #         return self.__q_in.qsize()
+    #     except NotImplementedError:
+    #         logger.logger.error("Input-queue .qsize() not implemented; exited gracefully.")
 
     def handle_work(self) -> NoReturn:
-        """ start pool without close() to enable continuous acceptance of new submitted tasks """
-        self.pool = multiprocessing.Pool(processes=self._num_of_workers, initializer=self.worker.work,
-                                    initargs=(self._q_in, self._q_out))
+        for _ in range(self.__num_of_workers):
+            worker = threading.Thread(target=self.__worker.work, args=(self.__q_in, self.__q_out))
+            worker.daemon = self.__daemon
+            worker.start()
+            self.__workers.append(worker)
+
+        # if self.__q_in.qsize() > 0:
+        #     self.__q_in.join()
 
     def get_results(self) -> List:
-        results = super().get_results()
+        results = []
+        with self.__lock:
+            while not self.__q_out.empty():
+                results.append(self.__q_out.get())
         return results
 
+    def __join_all_workers(self) -> NoReturn:
+        for worker in self.__workers:
+            worker.join()
+
     def end_shift(self) -> NoReturn:
-        """ inject PoisonPill to input-queue and close() pool """
-        for _ in range(self._num_of_workers):
-            self._q_in.put(PoisonPill())
-        self.pool.close()
-        self.pool.join()
-
-    # def terminate(self) -> NoReturn:
-    #     """ send SIGTERM to pool workers """
-    #     self.pool.terminate()
-    #     self.flush_queue()
-
-    # def del_task(self, task: Any) -> NoReturn:
-    #     """
-    #     using .task_done() on completed_tasks to sync-up with main process.
-    #      """
-    #     with self._lock:
-    #         # Keep track of completed tasks
-    #         completed_tasks = multiprocessing.JoinableQueue()
-    #         i = 0  # using i since qsize() not implemented for multiprocessing.Queue()
-    #         while not self._q_in.empty():
-    #             current_item = self._q_in.get()
-    #             if current_item['task'] == task:
-    #                 continue
-    #             completed_tasks.put(current_item)
-    #             i += 1
-    #         # Mark all completed tasks as done
-    #         for _ in range(i):
-    #             completed_tasks.task_done()
-    #
-    #         while not completed_tasks.empty():
-    #             self._q_in.put(completed_tasks.get())
-
-    def flush_queue(self) -> NoReturn:
-        while not self._q_in.empty():
-            self._q_in.get_nowait()
+        self.__q_in.join()
+        with self.__lock:
+            for _ in range(self.__num_of_workers):
+                self.__q_in.put(None)
+        self.__join_all_workers()
+        self.__workers.clear()
+        self.__flush_queue()
+
+    def __flush_queue(self) -> NoReturn:
+        with self.__lock:
+            self.__q_in.queue.clear()
 
-    def autoscale(self, arrival_rate: float, avg_queue_time: float, avg_service_time: float) -> NoReturn:
+    def __autoscale(self, arrival_rate: float, avg_queue_time: float, avg_service_time: float) -> NoReturn:
         """
         [!] Currently unavailable.
 
         This method auto-calculates the number of workers/processes needed for the kind of tasks provided -
         and auto-scales them each time it's called.
 
         Params:
         :param arrival_rate: float
         :param avg_queue_time: float
         :param avg_service_time: float
 
         :return:
             No return.
         """
-        super().autoscale(arrival_rate, avg_queue_time, avg_service_time)
+        pass
```

### Comparing `py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_io.py` & `py_shiftmanager-0.1.3/py_shiftmanager/shiftmanager_compute.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,155 +1,129 @@
-import datetime
-import queue
 import multiprocessing
-import threading
+import datetime
 import dill
 from typing import *
-
-from .worker import Worker_IO
-from .exceptions import QueueFullError
+import queue
+from .worker import Worker_COM, PoisonPill
 from .logger import Logger
 
 """
-ShiftManager_IO:
-This module is part of the Py_ShiftManager module for handling IO/Computational tasks -
+ShiftManager_Compute:
+This module is part of the Py-ShiftManager module for handling IO/Computational tasks -
 in managed queued environment.
 
-Handle all your I/O tasks without bothering with concurrency, multithreading -
+Handle all your computational tasks without bothering with concurrency, multiprocessing -
 or any other higher concept; simply use ShiftManager and enjoy the benefits of fast runtime speeds.
 
 Read the 'Readme.md' file for more documentation and information.
 """
 
 logger = Logger()
 
 
-class ShiftManager_IO:
-    _num_of_workers: int
-    _q_in: queue.Queue
-    _q_out: multiprocessing.Queue
-
-    def __init__(self, num_of_workers: int = 2, daemon: bool = False, queue_size: int = 10) -> NoReturn:
-        self._num_of_workers = num_of_workers
-        self.daemon = daemon
-        self.queue_size = queue_size
-        self._q_in = queue.Queue(maxsize=self.queue_size)
-        self._q_out = multiprocessing.Queue(maxsize=int(self.queue_size * 1.5))
-        self.worker = Worker_IO()
-        self.workers = []
-        self._lock = threading.Lock()
+class ShiftManager_Compute():
+    __pool: multiprocessing.Pool
+
+    def __init__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> NoReturn:
+        self.__num_of_workers = num_of_workers
+        self.__daemon = daemon
+        self.__q_in = multiprocessing.JoinableQueue(maxsize=input_q_size)
+        self.__q_out = multiprocessing.Queue(maxsize=output_q_size)
+        self.__worker = Worker_COM()
+        self.__lock = multiprocessing.Lock()
+        self.__put_timeout = 1
         
-    def __enter__(self, num_of_workers: int = 2, daemon: bool = False, queue_size: int = 10):
-        self.manager = ShiftManager_IO(num_of_workers, daemon, queue_size)
+    def __enter__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, queue_size: int = 10):
+        self.manager = ShiftManager_Compute(num_of_workers, daemon, queue_size)
         return self.manager
     
     def __exit__(self, exc_type, exc_val, exc_tb) -> NoReturn:
         if exc_type is not None:
             logger.logger.error(f"An exception of type {exc_type} occurred: {exc_val}")
         self.manager.handle_work()
         self.manager.end_shift()
 
     def __repr__(self):
-        return f"""ShiftManagerIO;daemonized={self.daemon};workers={self._num_of_workers}"""
+        return f"""ShiftManagerCOM;daemonized={self.__daemon};workers={self.__num_of_workers}"""
 
     """ Manual scaling of workers """
     def __add__(self, x: int) -> NoReturn:
-        self._num_of_workers += x
+        self.__num_of_workers += x
 
     def __sub__(self, x: int) -> NoReturn:
-        self._num_of_workers -= x
+        self.__num_of_workers -= x
 
     def __mul__(self, x: int) -> NoReturn:
-        self._num_of_workers *= x
+        self.__num_of_workers *= x
 
     def __divmod__(self, x: int) -> NoReturn:
-        self._num_of_workers /= x
+        self.__num_of_workers /= x
 
+    def __submit_task(self, new_task, force: bool = False) -> NoReturn:
+        try:
+            if force:
+                self.__lock.acquire()
+                self.__q_in.put_nowait(new_task)
+            else:
+                self.__lock.acquire()
+                self.__q_in.put(new_task, timeout=self.__put_timeout)
+        except queue.Full:
+            logger.logger.error("INPUT-QUEUE IS FULL.")
+        finally:
+            self.__lock.release()
+            
+    def configure(self, **kwargs) -> NoReturn:
+        if kwargs['put_timeout']:
+            self.__put_timeout = kwargs['put_timeout']
+        if kwargs['num_of_workers']:
+            self.__num_of_workers = kwargs['num_of_workers']
+        if kwargs['daemon']:
+            self.__daemon = kwargs['daemon']
+            
     """ Task and queue management """
-    def new_task(self, func: Callable, *args) -> NoReturn:
+    def new_task(self, func: Callable, *args, force: bool = False) -> NoReturn:
         new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args}
-        try:
-            with self._lock:
-                self._q_in.put(new_task)
-        except QueueFullError:
-            logger.logger.warn("INPUT-QUEUE IS FULL.")
+        self.__submit_task(new_task, force)
 
-    def new_batch(self, tasks: List[tuple]) -> NoReturn:
+    def new_batch(self, tasks: List[tuple], force: bool = False) -> NoReturn:
         for task in tasks:
-            self.new_task(*task)
-
-    def queue_in_size(self) -> int or NoReturn:
-        try:
-            return self._q_in.qsize()
-        except NotImplementedError:
-            logger.logger.error("Input-queue .qsize() not implemented; exited gracefully.")
-
-    def queue_out_size(self) -> int or NoReturn:
-        try:
-            return self._q_out.qsize()
-        except NotImplementedError:
-            logger.logger.error("Output-queue .qsize() not implemented; exited gracefully.")
+            self.new_task(*task, force=force)
 
     def handle_work(self) -> NoReturn:
-        for i in range(self._num_of_workers):
-            worker = threading.Thread(target=self.worker.work, args=(self._q_in, self._q_out))
-            worker.daemon = self.daemon
-            worker.start()
-            self.workers.append(worker)
-
-        if self._q_in.qsize() > 0:
-            self._q_in.join()
+        """ start pool without close() to enable continuous acceptance of new submitted tasks """
+        self.__pool = multiprocessing.Pool(processes=self.__num_of_workers, initializer=self.__worker.work,
+                                    initargs=(self.__q_in, self.__q_out))
 
     def get_results(self) -> List:
-        # self._q_in.join()
         results = []
-        with self._lock:
-            while not self._q_out.empty():
-                results.append(self._q_out.get())
+        with self.__lock:
+            while not self.__q_out.empty():
+                results.append(self.__q_out.get())
         return results
 
-    def join_all_workers(self) -> NoReturn:
-        for worker in self.workers:
-            worker.join()
-
     def end_shift(self) -> NoReturn:
-        self._q_in.join()
-        with self._lock:
-            for _ in range(self._num_of_workers):
-                self._q_in.put(None)
-        self.join_all_workers()
-        self.workers.clear()
-        self.flush_queue()
-
-    # def del_task(self, task: Any) -> NoReturn:
-    #     temp_queue = queue.Queue()
-    #     with self._lock:
-    #         while not self._q_in.empty():
-    #             current_item = self._q_in.get()
-    #             self._q_in.task_done()
-    #             if current_item == task:
-    #                 continue
-    #             temp_queue.put(current_item)
-    #
-    #         while not temp_queue.empty():
-    #             self._q_in.put(temp_queue.get())
-
-    def flush_queue(self) -> NoReturn:
-        with self._lock:
-            self._q_in.queue.clear()
+        """ inject PoisonPill to input-queue and close() pool """
+        for _ in range(self.__num_of_workers):
+            self.__q_in.put(PoisonPill())
+        self.__pool.close()
+        self.__pool.join()
+
+    def __flush_queue(self) -> NoReturn:
+        while not self.__q_in.empty():
+            self.__q_in.get_nowait()
 
-    def autoscale(self, arrival_rate: float, avg_queue_time: float, avg_service_time: float) -> NoReturn:
+    def __autoscale(self, arrival_rate: float, avg_queue_time: float, avg_service_time: float) -> NoReturn:
         """
         [!] Currently unavailable.
 
         This method auto-calculates the number of workers/processes needed for the kind of tasks provided -
         and auto-scales them each time it's called.
 
         Params:
         :param arrival_rate: float
         :param avg_queue_time: float
         :param avg_service_time: float
 
         :return:
             No return.
         """
-        pass
+        super().__autoscale(arrival_rate, avg_queue_time, avg_service_time)
```

### Comparing `py_shiftmanager-0.1.2/py_shiftmanager/timeout.py` & `py_shiftmanager-0.1.3/py_shiftmanager/timeout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import threading
 
 def timeout_timer(func=None, seconds=5, error_message='Task timed out.'):
-    """ Timeout wrapper, sets a seconds timer on a separate running thread with the join().
-        The main key here is setting the daemon flag, so it shuts the thread down when the time passes-
-        even though it didnt finish it's task.
+    """ Timeout wrapper, sets a seconds countdown on a separate running thread with using join().
+        Setting the thread daemon flag to True, so that it exits when the time runs out and program ended.
     """
     if func is None:
         return lambda f: timeout_timer(f, seconds, error_message)
 
     def wrapper(*args):
         result = {"task": func.__name__, "args": args}
         def target():
```

### Comparing `py_shiftmanager-0.1.2/py_shiftmanager/worker.py` & `py_shiftmanager-0.1.3/py_shiftmanager/worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,98 +11,93 @@
     pass
 
 
 logger = Logger()
 """ using thread locks to make queue interaction thread safe. 1 for in 1 for out. """
 lock1 = threading.Lock()
 lock2 = threading.Lock()
-lock3 = threading.Lock()
-lock4 = threading.Lock()
+lock3 = multiprocessing.Lock()
+lock4 = multiprocessing.Lock()
 
 
 class Worker_IO:
-    is_hired: bool
-    is_working: bool
-    role: str
-
     def __init__(self):
-        self.is_hired = True
-        self.is_working = False
-        self.role = "IO"
+        self.__is_hired = True
+        self.__is_working = False
+        self.__role = "IO"
 
     def __repr__(self):
-        return f"Worker;role={self.role};is_working={self.is_working};is_hired={self.is_hired}"
+        return f"Worker;role={self.__role};is_working={self.__is_working};is_hired={self.__is_hired}"
     
     def work(self, qu_in: queue.Queue, qu_out: multiprocessing.Queue) -> NoReturn:
-        self.is_hired = True
-        while self.is_hired:
+        self.__is_hired = True
+        while self.__is_hired:
             try:
                 lock1.acquire()
-                task = qu_in.get()
+                task = qu_in.get(timeout=1)
             except queue.Empty:
                 if lock1.locked():
                     lock1.release()
                 continue
             else:
                 lock1.release()
                 if task is None:
                     qu_in.task_done()
-                    self.is_hired = False
+                    self.__is_hired = False
                     break
-                self.is_working = True
+                self.__is_working = True
                 func = dill.loads(task['func'])
                 args = task['args']
                 try:
                     result = func(*args)
                 except Exception as err:
                     result = {"error": err, "task": func.__name__, "args": args}
                 qu_in.task_done()
                 try:
                     lock2.acquire()
-                    qu_out.put(result)
+                    qu_out.put(result, timeout=1)
                 except queue.Full:
                     logger.logger.error("OUTPUT-QUEUE IS FULL.")
                 finally:
                     if lock2.locked():
                         lock2.release()
-                    self.is_working = False
+                    self.__is_working = False
 
 
-class Worker_COM(Worker_IO):
+class Worker_COM():
+    __is_working: bool
+    
     def __init__(self):
-        super().__init__()
-        self.role = "COM"
+        self.__is_hired = True
+        self.__role = "COM"
 
     def __repr__(self):
-        super().__repr__()
+        return f"Worker;role={self.__role};is_working={self.__is_working};is_hired={self.__is_hired}"
 
     def work(self, qu_in: queue.Queue, qu_out: multiprocessing.Queue) -> NoReturn:
-        self.is_hired = True
-        while self.is_hired:
+        self.__is_hired = True
+        while self.__is_hired:
             try:
                 lock3.acquire()
-                task = qu_in.get(timeout=0.1)
+                task = qu_in.get(timeout=1)
             except queue.Empty:
-                if lock3.locked():
-                    lock3.release()
+                lock3.release()
                 continue
             else:
                 lock3.release()
                 if isinstance(task, PoisonPill):
-                    self.is_hired = False
+                    self.__is_hired = False
                     qu_in.task_done()
                     break
-                self.is_working = True
+                self.__is_working = True
                 func = dill.loads(task['func'])
                 args = task['args']
-                # insert timeout func here <<<<
                 result = func(*args)
                 qu_in.task_done()
                 try:
                     lock4.acquire()
-                    qu_out.put(result)
+                    qu_out.put(result, timeout=1)
+                    lock4.release()
                 except queue.Full:
+                    lock4.release()
                     logger.logger.error("OUTPUT-QUEUE IS FULL.")
-                finally:
-                    if lock4.locked():
-                        lock4.release()
-                self.is_working = False
+                self.__is_working = False
```

### Comparing `py_shiftmanager-0.1.2/py_shiftmanager.egg-info/PKG-INFO` & `py_shiftmanager-0.1.3/py_shiftmanager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 Metadata-Version: 2.1
 Name: py-shiftmanager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 
 # Py-ShiftManager
-#### v0.1.2
+#### v0.1.3
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
-## What's new in v0.1.1
+## What's new in v0.1.3
 This small update is dedicated to my friend Ram Manor :).
-* Introducing new timeout wrapper: *timeout_timer* - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
-* Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
-* *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
-* *ShiftManager_IO* now initializes the number of workers to 2, instead of 1, by default.  
-### New for v0.1.2
-* New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
+#### added in v0.1.1
+* ⏲️ Introducing new timeout wrapper: `@timeout_timer()` - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
+* 🔒 Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
+* 🛠️ *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
+* 🛠️ *ShiftManager_IO* now initializes the number of workers to `2`, instead of `1`, by default.  
+#### added in v0.1.2
+* ▶️ New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
 `with ShiftManager_Compute() as manager:`  
 `   manager.new_task(lambda x: x**2, 4)`  
 `   manager.new_task(lambda x: x**4, 13)`  
 then get the results:  
 `results = manager.get_results()`  
 It's that simple.  
+#### added in v0.1.3
+* 🛠️ Improved handling of queue exceptions - a better managing solution for large incoming amount of tasks.  
+* 🛠️ Improved task submission logic.
+* 🔒 Improved encapsulation.
+* 🛠️ New method added - `configure()`; read more under *'API'* section.   
+* 🛠️ Improved concurrency and parallelism in the IO module.
+* ⌫ Deprecated methods - `queue_in_size()`, `queue_out_size()` 
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py-shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py-shiftmanager.timeout import timeout_timer`
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_IO(num_of_workers=4)`  
-
-**Note**: by default *ShiftManager* objects init with these values for its attributes:
+By default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
-* queue size = `10`    
+* input_q_size = `10`
+* output_q_size = `15`
+ 
+**Note**: Once initialized, queue size cannot be changed.  
 
-Also, by default the output queue is set to 1.5 times the input queue size.
-  
 # Add some tasks to the input queue
-Assume we have created a function and applied the *timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
+Assume we have created a function called 'get_status()' that uses *requests* and applied the *@timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
 `manager.new_batch(tasks)`  
   
-**Note**: you can also pass *lambda* functions.
+**Note**: you can also pass in *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -77,21 +85,23 @@
 And here's an example of how to use Py-ShiftManager to handle computational tasks:
 
 `from py-shiftmanager import ShiftManager_Compute`  
 
 # Create a new ShiftManager instance with 4 workers
 `manager = ShiftManager_Compute(num_of_workers=4)`  
 But this time we'll increase the number to 5 using simple addition:  
-`manager + 1` - now *manager* is set to run 5 workers.
+`manager + 1` - now *manager* is set to run 5 workers.   
 
-**Note**: by default *ShiftManager_Compute* init with these default values for its attributes:  
-* num_of_workers = *number of CPU's in the system.*
+By default *ShiftManager_Compute* initializes with these default values for its attributes:  
+* num_of_workers = *number of CPU's in the system.* 
 * daemon = `False`
-* queue size = `10`
+* input_q_size = `10`
+* output_q_size = `15`  
 
+**Note**: Once initialized, queue size cannot be changed.  
 # Add some tasks to the input queue
 We can assign single tasks, like so:  
 `manager.new_task(lambda x: x**2, 3)`  
 `manager.new_task(lambda x: x**3, 4)`  
 `manager.new_task(lambda x, y: x**4 + y, 5, 9)`  
 or submit a batch by passing a list of tuples:  
 `tasks = [(lambda x: x**2, 3),(lambda x: x**3, 4)]`
@@ -112,59 +122,59 @@
 # Wait for the tasks to complete
 `manager.end_shift()`  
 This method sends a shut-down signal to all workers, they will stop gracefully.
 
 ## API
 
 **ShiftManager_IO**  
-`ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> None`  
-Creates a new ShiftManager instance with the specified number of workers, daemon status, and queue size.
+`ShiftManager_IO(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
+Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
-`new_task(func: Callable, task: Any) -> None`  
-Adds a new task to the input queue.
-
-`new_batch(tasks: List[tuple]) -> None`  
-Adds a list of tasks to the input queue.
+`new_task(func: Callable, task: Any, force: bool = False) -> None`  
+Adds a new task to the input queue; you could force it if you want.
 
-`queue_in_size() -> int`  
-Returns the current size of the input queue, if implemented, else, exists gracefully.
-
-`queue_out_size() -> int`  
-Returns the current size of the output queue, if implemented, else, exists gracefully.
+`new_batch(tasks: List[tuple], force: bool = False) -> None`  
+Adds a list of tasks to the input queue; you could force it if you want.
 
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
-Ends the shift and waits for all tasks to complete.
+Ends the shift and waits for all tasks to complete.  
+
+`configure(**kwargs) -> None`  
+Allows the user to configure the following attributes by passing keyword arguments:  
+* `daemon: bool` - reconfigure workers daemon status. 
+* `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
+* `num_of_workers: int` - reconfigure number of workers.  
 
 **ShiftManager_Compute**  
-`ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> None`  
-Creates a new ShiftManager instance with the specified number of workers, daemon status, and queue size.
+`ShiftManager_Compute(num_of_workers: int = 1, daemon: bool = False, input_q_size: int = 10, output_q_size: int = 15) -> None`  
+Creates a new ShiftManager instance with the specified number of workers, daemon status, input queue size and output queue size.
 
 `new_task(func: Callable, task: Any) -> None`  
 Adds a new task to the input queue.
 
 `new_batch(tasks: List[tuple]) -> None`  
 Adds a list of tasks to the input queue.
 
-`queue_in_size() -> int`  
-Returns the current size of the input queue, if implemented, else, exists gracefully.
-
-`queue_out_size() -> int`  
-Returns the current size of the output queue, if implemented, else, exists gracefully.
-
 `handle_work() -> None`  
 Handles the tasks in the input queue.
 
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
 Ends the shift and waits for all tasks to complete.  
 
+`configure(**kwargs) -> None`  
+Allows the user to configure the following attributes by passing keyword arguments:  
+* `daemon: bool` - reconfigure workers daemon status. 
+* `put_timeout: int` - reconfigure timeout (in seconds) for input queue task submission (default is `1` second).
+* `num_of_workers: int` - reconfigure number of workers.  
+
 **timeout_timer**  
 `@timeout_timer(seconds: int = 5)`  
-A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; 5 seconds by default.
+A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; `5` seconds by default.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py_shiftmanager-0.1.2/setup.py` & `py_shiftmanager-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 long_description = Path('Readme.md').read_text()
 
 setup(
     name='py_shiftmanager',
-    version='0.1.2',
+    version='0.1.3',
     description='A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.',
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'dill==0.3.6',
     ],
     classifiers=[
```

