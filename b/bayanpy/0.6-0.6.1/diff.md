# Comparing `tmp/bayanpy-0.6.tar.gz` & `tmp/bayanpy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.tar", last modified: Tue Apr 11 16:04:35 2023, max compression
+gzip compressed data, was "bayanpy-0.6.1.tar", last modified: Thu Apr 13 14:32:37 2023, max compression
```

## Comparing `bayanpy-0.6.tar` & `bayanpy-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-11 16:04:35.713202 bayanpy-0.6/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-11 16:04:35.713202 bayanpy-0.6/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     4917 2023-04-11 15:57:56.000000 bayanpy-0.6/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-11 16:04:35.713202 bayanpy-0.6/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-08 16:13:17.000000 bayanpy-0.6/bayanpy/__init__.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    51005 2023-04-11 16:03:12.000000 bayanpy-0.6/bayanpy/bayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    44347 2023-04-08 03:05:45.000000 bayanpy-0.6/bayanpy/bayanpy.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-11 16:04:35.713202 bayanpy-0.6/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      243 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-11 16:04:35.713202 bayanpy-0.6/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      559 2023-04-11 16:04:27.000000 bayanpy-0.6/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:32:37.059519 bayanpy-0.6.1/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.1/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:32:37.059519 bayanpy-0.6.1/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.1/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:32:37.059519 bayanpy-0.6.1/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    51873 2023-04-13 14:28:36.000000 bayanpy-0.6.1/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:28:56.000000 bayanpy-0.6.1/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-13 14:32:37.059519 bayanpy-0.6.1/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-13 14:32:37.000000 bayanpy-0.6.1/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-13 14:32:36.000000 bayanpy-0.6.1/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-13 14:32:37.059519 bayanpy-0.6.1/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      561 2023-04-13 14:29:14.000000 bayanpy-0.6.1/setup.py
```

### Comparing `bayanpy-0.6/LICENSE` & `bayanpy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6/README.md` & `bayanpy-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Bayanpy: Bayan Algorithm for Community Detection
 
 Bayanpy is a Python package implementing the Bayan algorithm, a community detection method capable of providing a globally optimal solution to the modularity maximization problem. Bayan can also be implemented such that it provides an approximation of the maximum modularity with a guarantee of proximity. This algorithm is theoretically grounded by the Integer Programming (IP) formulation of the modularity maximization problem and relies on an exact branch-and-cut scheme for solving the NP-complete optimization problem to global optimality.
 
 For more information, visit the [Bayan project website](https://bayanproject.github.io/).
+For a few examples of different ways you can use Bayan see this Google Colab address: [bayanpy Examples](https://tinyurl.com/bayancolab).
+
 
 ## Installation
 
 To install Bayanpy, use pip:
 
 ```
 pip install bayanpy
```

### Comparing `bayanpy-0.6/bayanpy/bayanImplied.py` & `bayanpy-0.6.1/bayanpy/BayanImplied.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from gurobipy import *
 from cdlib import algorithms
 from networkx.algorithms.connectivity import minimum_st_node_cut
 from joblib import Parallel, delayed, parallel_backend
 from itertools import chain
 
 
-# Load Graph from network name
 def get_graph_from_network_name(network_name, sub_name=None):
     """
     Method to create a networkx Graph from network names listed at https://networks.skewed.de/
     """
     #Defining the network information url
     info_url = "https://networks.skewed.de/api/net/%s" % network_name
     req = requests.get(info_url)
@@ -114,14 +113,19 @@
     
     # If G is a multigraph then the edge attributes correspond to the attributes of the last seen edge as in the data
     if is_multigraph:
         print("%s is a multigraph but has been loaded as a simple graph" % network_name)
     
     shutil.rmtree(network_name + "_files")
     return G
+
+
+# In[4]:
+
+
 def get_local_clustering_coefficient(G, node: int):
     """
     Returns the clustering coefficient for the input node in the input graph
     """
     neighbours = nx.adjacency_matrix(G)[node].indices
     if neighbours.shape[0] <= 1:
         return 0.0
@@ -189,20 +193,28 @@
     G_prime = nx.convert_node_labels_to_integers(G_prime)
 #     ModularityMatrix = nx.modularity_matrix(G_prime, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(G_prime, resolution)
     for edge in G_prime.edges():
         G_prime.edges[edge[0], edge[1]]["weight"] = ModularityMatrix[edge[0], edge[1]]
     return G_prime
 
+
+# In[5]:
+
+
 def find_in_list_of_list(mylist, char):
     for sub_list in mylist:
         if char in sub_list:
             return (mylist.index(sub_list))
     raise ValueError("'{char}' is not in list".format(char = char))
 
+
+# In[6]:
+
+
 def model_to_communities(var_vals, Graph):
     """
     Method that outputs communities with input model variable values and the Graph
     """
     clustered = []
     
     for v in var_vals:
@@ -245,14 +257,18 @@
 
     for c in range(len(group)):
         group[c].sort()
     group.sort()
     
     return group
 
+
+# In[7]:
+
+
 def decluster_communities(group, Graph, isolated_nodes):
     """
     Method to get communities based on the original graph. Note, input Graph is the reduced graph.
     """
     group_declustered = []
     for comm in group:
         new_comm = []
@@ -297,21 +313,32 @@
     communities=[]
 
     #This code lists all sorted triples of nodes (open and closed)
 #     list_of_tuples=list(combinations(np.sort(list((Graph).nodes())),3))
 #     list_of_triads=[list(elem) for elem in list_of_tuples]
     formulation_time_start = time.time()
     list_of_cut_triads=[]
+    
+#     pairs_with_edges = []
+#     pairs_without_edges = []
+#     for i in (Graph).nodes():
+#         for j in range(i+1, len((Graph).nodes())):
+#             if Graph.has_edge(i, j):
+#                 pairs_with_edges.append((i, j))
+#             else:
+#                 pairs_without_edges.append((i, j))
+
     pairs = set(combinations(np.sort(list((Graph).nodes())),2))
     self_edges =set([(i, i) for i in (Graph).nodes()])
     pairs_with_edges = set((Graph).edges()) - self_edges
     pairs_without_edges = pairs - pairs_with_edges
     pairs_without_edges = list(pairs_without_edges)
     pairs_with_edges = list(pairs_with_edges)
         
+# JOBLIB
     with parallel_backend(backend='loky', n_jobs=-1):
         res = Parallel()(delayed(separating_set_parallel)(pair[0], pair[1], Graph) for pair in pairs_without_edges)
     
     list_of_cut_triads = list(chain(*res))
 
     for pair in pairs_with_edges:
         i = pair[0]
@@ -323,35 +350,56 @@
             Graph.remove_edge(i, j)
         minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
         for k in minimum_vertex_cut:
             list_of_cut_triads.append(list(np.sort([i,j,k])))
         if removed_edge:
             Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"], actual_weight=attr_dict["actual_weight"])
 
-    x = {}
+            
+#     list_of_cut_triads = []
+#     for i in (Graph).nodes():
+#         for j in range(i+1, len((Graph).nodes())):
+#             removed_edge = False
+#             if Graph.has_edge(i, j):
+#                 removed_edge = True
+#                 attr_dict = Graph.edges[i, j]
+#                 Graph.remove_edge(i, j)
+#             minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
+#             for k in minimum_vertex_cut:
+#                 list_of_cut_triads.append(list(np.sort([i,j,k])))
+#             if removed_edge:
+#                 Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"], actual_weight=attr_dict["actual_weight"])
+#     return list_of_cut_triads
+    
+    x={}
 
     model = Model("Modularity maximization")
     model.setParam(GRB.param.OutputFlag, 0) 
     model.setParam(GRB.param.Method, lp_method)
     model.setParam(GRB.Param.Crossover, 0)
     model.setParam(GRB.Param.Threads, min(64,multiprocessing.cpu_count()))
 
+
+
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             x[(i,j)] = model.addVar(lb=0, ub=1, vtype=GRB.CONTINUOUS, name=str(i)+','+str(j))
 
     model.update()
 
     OFV = 0 
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             OFV += ModularityMatrix[i, j] * (1 - x[(i, j)])
 
     model.setObjective(OFV, GRB.MAXIMIZE)
 
+#    print('Adding constraints...')
+#     for [i,j,k] in list_of_triads:
+#     base_constraints = []
     for [i,j,k] in list_of_cut_triads:
         model.addConstr(x[(i,k)] <= x[(i, j)] + x[(j, k)], 'triangle1'+','+str(i)+','+str(j)+','+str(k))
         model.addConstr(x[(i,j)] <= x[(i, k)] + x[(j, k)], 'triangle2'+','+str(i)+','+str(j)+','+str(k))
         model.addConstr(x[(j,k)] <= x[(i, j)] + x[(i, k)], 'triangle3'+','+str(i)+','+str(j)+','+str(k))
 #         base_constraints.append('triangle1'+','+str(i)+','+str(j)+','+str(k))
     formulation_time = time.time() - formulation_time_start
 
@@ -739,28 +787,22 @@
             else:
                 Graph.add_edge(i, j)
                 Graph.edges[(i, j)]['weight'] = ModularityMatrix[i, j]
                 Graph.edges[(i, j)]['constrained_modularity'] = False
                 edges_added.append((i, j))
     return Graph, edges_added
 
+
 def remove_extra_edges(Graph, edge_list):
     """
     Removes the additional edges added for running pycombo
     """
     for edge in edge_list:
         Graph.remove_edge(edge[0], edge[1])
     return Graph
-            
-    
-    
-        
-
-
-# In[13]:
 
 
 def reduced_cost_variable_fixing(model, var_vals, obj_value, lower_bound, Graph, resolution):
     AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
 #     ModularityMatrix = nx.modularity_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
 #     new_obj_val = ((obj_value*np.sum(AdjacencyMatrix)) - ModularityMatrix.trace()[0, 0])/2
@@ -775,21 +817,14 @@
             if new_obj_val - var.getAttr(GRB.Attr.RC) < new_lower_bound:
                 vars_one.append(key)
         elif var_vals[key] == 0:
             if new_obj_val + var.getAttr(GRB.Attr.RC) < new_lower_bound:
                 vars_zero.append(key)
     return vars_one, vars_zero
 
-#Change set of triples based on fixed nodes for branching
-
-#Assign Priority to triple with two previously fixed variables in get_best_triple
-
-
-# In[14]:
-
 
 class Node:
     """
     Represents one node in the bayan tree
     """
     def __init__(self, constraint_list, var_vals, g, combo_comms):
         self.constraints = constraint_list
@@ -842,21 +877,15 @@
     def get_fixed_ones(self):
         return self.fixed_ones
     
     def get_fixed_zeros(self):
         return self.fixed_zeros
 
 
-# In[15]:
-
-
 def create_bayan_edge_attributes(G, resolution):
-    #actual_weight is the attribute that stores the edge weight
-    
-#     ModularityMatrix = nx.modularity_matrix(G, weight="weight")
 
     for edge in G.edges():
         G.edges[edge]['constrained_modularity'] = False
         if 'weight' in G.edges[edge]:
             G.edges[edge]['actual_weight'] = G.edges[edge]['weight']
         else:
             G.edges[edge]['actual_weight'] = 1
@@ -933,48 +962,43 @@
     G = create_int_node_names(G)
     G1 = G.copy()
     orig_graph = create_bayan_edge_attributes(G1, resolution)
     G2 = orig_graph.copy()
     Graph, isolated_nodes = handle_isolated_nodes(G2)
     Graph = clique_filtering(Graph, resolution)
     AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
-#     ModularityMatrix = nx.modularity_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
     size = int(Graph.size(weight='actual_weight'))
     order = len(AdjacencyMatrix)
     preprocessing_time = time.time() - preprocessing_time_start
-    mod_lp, var_vals, model, list_of_cut_triads, formulation_time, root_lp_time = lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method)
-#     return var_vals
+    mod_lp, var_vals, model, list_of_cut_triads, formulation_time, root_lp_time = \
+        lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method)
     if is_integer_solution(Graph, var_vals):
         return 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time
     root_combo_time_start = time.time()
     partition_combo = algorithms.pycombo(Graph, weight="actual_weight", modularity_resolution=resolution)
     communities_combo = list(partition_combo.communities)
-#     return communities_combo
     communities_combo_declustered = decluster_communities(communities_combo, Graph, isolated_nodes)
     mod_combo = calculate_modularity(communities_combo_declustered, orig_graph, resolution)
     root_combo_time = time.time() - root_combo_time_start
-#    print(mod_combo)
     if mod_lp - mod_combo < threshold:
         return 2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time
     best_bound = mod_lp
     incumbent = mod_combo
     root = Node([], var_vals, Graph, communities_combo_declustered)
     root.set_level(0)
     root.set_bounds(mod_combo, mod_lp)
     var_fixed_ones, var_fixed_zeros = reduced_cost_variable_fixing(model, var_vals, mod_lp, incumbent, Graph, resolution)
     root.set_fixed_ones(var_fixed_ones)
     root.set_fixed_zeros(var_fixed_zeros)
-#     return root
     current_node = root
     current_level = 1
     nodes_previous_level = [root]
     best_combo = root
     best_lp = root
-#     program_start = time.time()
     root_time = root_lp_time + root_combo_time
     solve_start = time.time()
     while (best_bound - incumbent > threshold and nodes_previous_level != [] and time.time() - solve_start - root_time <= time_allowed): #add time_limit as a user parameter
         nodes_current_level = []
         lower_bounds = []
         upper_bounds = []
         for node in nodes_previous_level:
@@ -983,20 +1007,18 @@
                     if best_combo.lower_bound <= best_combo.upper_bound:
                         return 3, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time
                     else:
                         return 4, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
                 else:
                     return 5, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
             current_node = node
-#             model.reset()
             left_node, right_node = perform_branch(node, model, incumbent, best_bound, Graph, orig_graph, isolated_nodes, list_of_cut_triads, delta, resolution)
             if left_node.close:
                 print("Left node is closed")
                 if left_node.is_integer and incumbent <= left_node.upper_bound:
-#                     p_inc = incumbent
                     incumbent = left_node.upper_bound
                     best_combo = left_node
                     nodes_current_level.append(left_node)
                     lower_bounds.append(left_node.lower_bound)
                     upper_bounds.append(left_node.upper_bound)
                     current_node.left = left_node
                     left_node.parent = current_node
@@ -1062,18 +1084,14 @@
         if best_combo.lower_bound <= best_combo.upper_bound:
             return 6, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time
         else:
             return 7, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
     else:
         return 8, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
 
-
-# In[47]:
-
-
 def left_implied(left_fix_ones, left_fix_zeros, branch_triple):
     ones = left_fix_ones.copy()
     zeros = left_fix_zeros.copy()
     i = branch_triple[0]
     j = branch_triple[1]
     k = branch_triple[2]
     for var in left_fix_zeros:
@@ -1251,7 +1269,30 @@
             print("LP solution is integer")
             right_node.set_is_integer()
             right_node.close_node()
         if right_upper_bound <= incumbent:
             right_node.close_node()
     return left_node, right_node
     
+    
+    
+
+
+# In[230]:
+
+
+# import BayanPost as bayanpostpy
+
+
+# In[229]:
+
+
+# graph = get_graph_from_network_name("football")
+# post_ans = bayanpostpy.bayan(graph, threshold = 0, time_allowed=60)
+
+
+# In[228]:
+
+
+# G = get_graph_from_network_name("football")
+# ans = bayan(G, threshold=0, time_allowed=60)
+
```

### Comparing `bayanpy-0.6/setup.py` & `bayanpy-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6", 
+    version="0.6.1", 
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

