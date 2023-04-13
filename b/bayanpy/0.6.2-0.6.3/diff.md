# Comparing `tmp/bayanpy-0.6.2.tar.gz` & `tmp/bayanpy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.2.tar", last modified: Thu Apr 13 14:40:21 2023, max compression
+gzip compressed data, was "bayanpy-0.6.3.tar", last modified: Thu Apr 13 15:36:04 2023, max compression
```

## Comparing `bayanpy-0.6.2.tar` & `bayanpy-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:40:21.572419 bayanpy-0.6.2/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.2/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:40:21.572419 bayanpy-0.6.2/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.2/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:40:21.572419 bayanpy-0.6.2/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    51873 2023-04-13 14:28:36.000000 bayanpy-0.6.2/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.2/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:40:21.572419 bayanpy-0.6.2/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-13 14:40:21.000000 bayanpy-0.6.2/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-13 14:40:21.572419 bayanpy-0.6.2/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      561 2023-04-13 14:39:10.000000 bayanpy-0.6.2/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 15:36:04.421276 bayanpy-0.6.3/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.3/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 15:36:04.421276 bayanpy-0.6.3/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.3/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 15:36:04.421276 bayanpy-0.6.3/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    52486 2023-04-13 15:23:37.000000 bayanpy-0.6.3/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.3/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 15:36:04.421276 bayanpy-0.6.3/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 15:36:04.000000 bayanpy-0.6.3/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-13 15:36:04.000000 bayanpy-0.6.3/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-13 15:36:04.000000 bayanpy-0.6.3/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-13 15:36:04.000000 bayanpy-0.6.3/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-13 15:36:04.000000 bayanpy-0.6.3/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-13 15:36:04.421276 bayanpy-0.6.3/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      561 2023-04-13 15:33:18.000000 bayanpy-0.6.3/setup.py
```

### Comparing `bayanpy-0.6.2/LICENSE` & `bayanpy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.2/README.md` & `bayanpy-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.2/bayanpy/BayanImplied.py` & `bayanpy-0.6.3/bayanpy/BayanImplied.py`

 * *Files 1% similar despite different names*

```diff
@@ -914,78 +914,68 @@
     for x in Graph.nodes():
         if Graph.degree[x] == 0:
             isolated.append(x)
     for x in isolated:
         Graph.remove_node(x)
     Graph = nx.convert_node_labels_to_integers(Graph)
     return Graph, isolated
-    
-
-
-# In[17]:
-
-
-def create_int_node_names(Graph):
-    G = Graph.copy()
-    count = 0
-    mapping = {}
-    for n in G.nodes():
-        mapping[n] = count
-        count += 1
-    G = nx.relabel_nodes(G, mapping)
-    return G
-
-
-# In[18]:
-
 
 def get_modularity_matrix(Graph, resolution):
     AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
     ModularityMatrix = np.empty(AdjacencyMatrix.shape)
     for i in Graph.nodes():
         for j in Graph.nodes():
             deg_i = Graph.degree(i, weight="actual_weight") - AdjacencyMatrix[i, i]
             deg_j = Graph.degree(j, weight="actual_weight") - AdjacencyMatrix[j, j]
             mod = AdjacencyMatrix[i, j] - (((deg_i*deg_j)/(np.sum(AdjacencyMatrix)))*resolution)
             ModularityMatrix[i, j] = mod
     return ModularityMatrix
 
 
-# In[46]:
+def output(mapping, develop, state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time):
+    communities = [[mapping[i] for i in com] for com in communities]
+    if develop:
+        out = state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time
+    else:
+        gap = (upper_bound - lower_bound) / upper_bound
+        out = lower_bound, gap, communities, preprocessing_time+formulation_time, solve_time
+    return out
 
 
-def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4):
+def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
     """
     Run bayan on input Graph while MIP gap > threshold and runtime < time_allowed (default is 60 seconds)
     """
     run_start = time.time()
     preprocessing_time_start = time.time()
-    G = create_int_node_names(G)
+    G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
+    mapping = nx.get_node_attributes(G, 'original_label')
+
     G1 = G.copy()
     orig_graph = create_bayan_edge_attributes(G1, resolution)
     G2 = orig_graph.copy()
     Graph, isolated_nodes = handle_isolated_nodes(G2)
     Graph = clique_filtering(Graph, resolution)
     AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
     size = int(Graph.size(weight='actual_weight'))
     order = len(AdjacencyMatrix)
     preprocessing_time = time.time() - preprocessing_time_start
     mod_lp, var_vals, model, list_of_cut_triads, formulation_time, root_lp_time = \
         lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method)
     if is_integer_solution(Graph, var_vals):
-        return 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time
+        return output(mapping, develop_mode, 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time)
     root_combo_time_start = time.time()
     partition_combo = algorithms.pycombo(Graph, weight="actual_weight", modularity_resolution=resolution)
     communities_combo = list(partition_combo.communities)
     communities_combo_declustered = decluster_communities(communities_combo, Graph, isolated_nodes)
     mod_combo = calculate_modularity(communities_combo_declustered, orig_graph, resolution)
     root_combo_time = time.time() - root_combo_time_start
     if mod_lp - mod_combo < threshold:
-        return 2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time
+        return output(mapping, develop_mode,2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time)
     best_bound = mod_lp
     incumbent = mod_combo
     root = Node([], var_vals, Graph, communities_combo_declustered)
     root.set_level(0)
     root.set_bounds(mod_combo, mod_lp)
     var_fixed_ones, var_fixed_zeros = reduced_cost_variable_fixing(model, var_vals, mod_lp, incumbent, Graph, resolution)
     root.set_fixed_ones(var_fixed_ones)
@@ -1001,19 +991,19 @@
         nodes_current_level = []
         lower_bounds = []
         upper_bounds = []
         for node in nodes_previous_level:
             if time.time() - solve_start - root_time >= time_allowed:
                 if best_combo.is_integer:
                     if best_combo.lower_bound <= best_combo.upper_bound:
-                        return 3, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time
+                        return output(mapping, develop_mode,3, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time)
                     else:
-                        return 4, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
+                        return output(mapping, develop_mode,4, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
                 else:
-                    return 5, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
+                    return output(mapping, develop_mode,5, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
             current_node = node
             left_node, right_node = perform_branch(node, model, incumbent, best_bound, Graph, orig_graph, isolated_nodes, list_of_cut_triads, delta, resolution)
             if left_node.close:
                 print("Left node is closed")
                 if left_node.is_integer and incumbent <= left_node.upper_bound:
                     incumbent = left_node.upper_bound
                     best_combo = left_node
@@ -1078,19 +1068,19 @@
                 nodes_p_level.append(a)
         nodes_previous_level = nodes_p_level
         
 #     print(best_combo.lower_bound, best_combo.upper_bound)
 #     print(best_lp.lower_bound, best_lp.upper_bound)
     if best_combo.is_integer:
         if best_combo.lower_bound <= best_combo.upper_bound:
-            return 6, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time
+            return output(mapping, develop_mode,6, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time)
         else:
-            return 7, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
+            return output(mapping, develop_mode,7, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
     else:
-        return 8, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
+        return output(mapping, develop_mode,8, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
 
 def left_implied(left_fix_ones, left_fix_zeros, branch_triple):
     ones = left_fix_ones.copy()
     zeros = left_fix_zeros.copy()
     i = branch_triple[0]
     j = branch_triple[1]
     k = branch_triple[2]
```

### Comparing `bayanpy-0.6.2/setup.py` & `bayanpy-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.2", 
+    version="0.6.3", 
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

