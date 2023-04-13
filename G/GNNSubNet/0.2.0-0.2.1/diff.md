# Comparing `tmp/GNNSubNet-0.2.0.tar.gz` & `tmp/GNNSubNet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GNNSubNet-0.2.0.tar", last modified: Mon Feb 27 13:31:10 2023, max compression
+gzip compressed data, was "GNNSubNet-0.2.1.tar", last modified: Thu Apr 13 09:09:49 2023, max compression
```

## Comparing `GNNSubNet-0.2.0.tar` & `GNNSubNet-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:31:10.263910 GNNSubNet-0.2.0/
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:31:10.263910 GNNSubNet-0.2.0/GNNSubNet/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    47029 2023-02-27 13:19:15.000000 GNNSubNet-0.2.0/GNNSubNet/GNNSubNet.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     4596 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/GNN_paper.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    11060 2022-05-09 13:01:59.000000 GNNSubNet-0.2.0/GNNSubNet/OMICS_workflow.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    10065 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/PGExplainer.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      121 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     2072 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/community_detection.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    23565 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/dataset.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:31:10.259910 GNNSubNet-0.2.0/GNNSubNet/datasets/
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:31:10.263910 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)   578238 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/FEATURES_synthetic.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      661 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/NETWORK_synthetic.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     8897 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/TARGET_synthetic.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       80 2023-02-27 12:37:31.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/communities.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       24 2023-02-27 12:37:31.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/communities_scores.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      141 2023-02-27 12:37:21.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/edge_index.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      232 2023-02-27 12:37:31.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/edge_masks.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      111 2023-02-27 12:37:31.000000 GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/gene_names.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      206 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/edge_importance.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     9671 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/features_computation.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    32621 2023-02-27 08:32:31.000000 GNNSubNet-0.2.0/GNNSubNet/gnn_explainer.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1519 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/gnn_training_utils.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     5172 2022-06-17 11:43:48.000000 GNNSubNet-0.2.0/GNNSubNet/gnnexplainer_sim.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     5189 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/gnnexplainer_vanilla_sim.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      410 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/graph_dataset.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     3203 2023-02-27 08:14:10.000000 GNNSubNet-0.2.0/GNNSubNet/graphcheb.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     9454 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/graphcnn.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1819 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/mlp.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      809 2022-05-09 12:01:42.000000 GNNSubNet-0.2.0/GNNSubNet/s2vgraph.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:31:10.263910 GNNSubNet-0.2.0/GNNSubNet.egg-info/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1115 2023-02-27 13:31:10.000000 GNNSubNet-0.2.0/GNNSubNet.egg-info/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1058 2023-02-27 13:31:10.000000 GNNSubNet-0.2.0/GNNSubNet.egg-info/SOURCES.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2023-02-27 13:31:10.000000 GNNSubNet-0.2.0/GNNSubNet.egg-info/dependency_links.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      144 2023-02-27 13:31:10.000000 GNNSubNet-0.2.0/GNNSubNet.egg-info/requires.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       10 2023-02-27 13:31:10.000000 GNNSubNet-0.2.0/GNNSubNet.egg-info/top_level.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    35149 2022-04-26 11:18:15.000000 GNNSubNet-0.2.0/LICENSE
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1115 2023-02-27 13:31:10.263910 GNNSubNet-0.2.0/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     4713 2023-02-27 08:14:10.000000 GNNSubNet-0.2.0/README.md
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      103 2023-02-27 13:31:10.263910 GNNSubNet-0.2.0/setup.cfg
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1683 2023-02-27 13:30:27.000000 GNNSubNet-0.2.0/setup.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:09:49.318190 GNNSubNet-0.2.1/
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:09:49.314190 GNNSubNet-0.2.1/GNNSubNet/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    57026 2023-04-11 10:47:28.000000 GNNSubNet-0.2.1/GNNSubNet/GNNSubNet.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     4596 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/GNN_paper.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    11060 2022-05-09 13:01:59.000000 GNNSubNet-0.2.1/GNNSubNet/OMICS_workflow.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    10065 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/PGExplainer.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      121 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     2072 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/community_detection.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    23565 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/dataset.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:09:49.302190 GNNSubNet-0.2.1/GNNSubNet/datasets/
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:09:49.318190 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)   578238 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/FEATURES_synthetic.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      661 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/NETWORK_synthetic.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     8897 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/TARGET_synthetic.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       80 2023-04-11 10:48:27.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/communities.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       24 2023-04-11 10:48:27.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/communities_scores.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      141 2023-04-11 10:48:18.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/edge_index.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      232 2023-04-11 10:48:27.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/edge_masks.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      111 2023-04-11 10:48:27.000000 GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/gene_names.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      206 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/edge_importance.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     9671 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/features_computation.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    37857 2023-04-11 10:18:49.000000 GNNSubNet-0.2.1/GNNSubNet/gnn_explainer.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1519 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/gnn_training_utils.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     5172 2022-06-17 11:43:48.000000 GNNSubNet-0.2.1/GNNSubNet/gnnexplainer_sim.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     5189 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/gnnexplainer_vanilla_sim.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      410 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/graph_dataset.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     6380 2023-04-11 10:16:19.000000 GNNSubNet-0.2.1/GNNSubNet/graphcheb.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     9454 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/graphcnn.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1819 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/mlp.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      809 2022-05-09 12:01:42.000000 GNNSubNet-0.2.1/GNNSubNet/s2vgraph.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:09:49.314190 GNNSubNet-0.2.1/GNNSubNet.egg-info/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1115 2023-04-13 09:09:49.000000 GNNSubNet-0.2.1/GNNSubNet.egg-info/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1058 2023-04-13 09:09:49.000000 GNNSubNet-0.2.1/GNNSubNet.egg-info/SOURCES.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2023-04-13 09:09:49.000000 GNNSubNet-0.2.1/GNNSubNet.egg-info/dependency_links.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      144 2023-04-13 09:09:49.000000 GNNSubNet-0.2.1/GNNSubNet.egg-info/requires.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       10 2023-04-13 09:09:49.000000 GNNSubNet-0.2.1/GNNSubNet.egg-info/top_level.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    35149 2022-04-26 11:18:15.000000 GNNSubNet-0.2.1/LICENSE
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1115 2023-04-13 09:09:49.318190 GNNSubNet-0.2.1/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     4713 2023-02-27 08:14:10.000000 GNNSubNet-0.2.1/README.md
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      103 2023-04-13 09:09:49.318190 GNNSubNet-0.2.1/setup.cfg
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1683 2023-04-13 09:08:54.000000 GNNSubNet-0.2.1/setup.py
```

### Comparing `GNNSubNet-0.2.0/GNNSubNet/GNNSubNet.py` & `GNNSubNet-0.2.1/GNNSubNet/GNNSubNet.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 from torch_geometric.data.data import Data
 from torch_geometric.loader import DataLoader
 
 from .gnn_training_utils import check_if_graph_is_connected, pass_data_iteratively
 from .dataset import generate, load_OMICS_dataset, convert_to_s2vgraph
 from .gnn_explainer import GNNExplainer
 from .graphcnn  import GraphCNN
-from .graphcheb import GraphCheb
-
+from .graphcheb import GraphCheb, ChebConvNet, test_model_acc, test_model
 
 from .community_detection import find_communities
 from .edge_importance import calc_edge_importance
 
 from torch_geometric.nn.conv.cheb_conv import ChebConv
 
 class GNNSubNet(object):
@@ -99,64 +98,292 @@
         Print a summary for the GNNSubSet object's current state.
         """
         print("")
         print("Number of nodes:", len(self.dataset[0].x))
         print("Number of edges:", self.edges.shape[0])
         print("Number of modalities:",self.dataset[0].x.shape[1])
 
-    def train(self, epoch_nr = 20, method="chebconv"):
+    def train(self, epoch_nr = 20, method="graphcnn", learning_rate=0.01):
 
         if method=="chebconv":
             print("chebconv for training ...")
             self.train_chebconv(epoch_nr = epoch_nr)
             self.classifier="chebconv"
 
         if method=="graphcnn":
             print("graphcnn for training ...")
-            self.train_graphcnn(epoch_nr = epoch_nr)
+            self.train_graphcnn(epoch_nr = epoch_nr, learning_rate=learning_rate)
             self.classifier="graphcnn"
 
         if method=="graphcheb":
             print("graphcheb for training ...")
             self.train_graphcheb(epoch_nr = epoch_nr)
             self.classifier="graphcheb"
 
+        if method=="chebnet":
+            print("chebnet for training ...")
+            self.train_chebnet(epoch_nr = epoch_nr)
+            self.classifier="chebnet"
+
 
-    def explain(self, n_runs=1, classifier="chebconv"):
+    def explain(self, n_runs=1, classifier="graphcnn"):
 
         if self.classifier=="chebconv":
             self.explain_chebconv(n_runs=n_runs)
 
         if self.classifier=="graphcnn":
             self.explain_graphcnn(n_runs=n_runs)      
     
         if self.classifier=="graphcheb":
             self.explain_graphcheb(n_runs=n_runs)
 
+        if self.classifier=="chebnet":
+            self.explain_graphcheb(n_runs=n_runs)
+
 
-    def predict(self, gnnsubnet_test, classifier="chebconv"):
+
+    def predict(self, gnnsubnet_test, classifier="graphcnn"):
     
         if self.classifier=="chebconv":
             pred = self.predict_chebconv(gnnsubnet_test=gnnsubnet_test)
 
         if self.classifier=="graphcnn":
             pred = self.predict_graphcnn(gnnsubnet_test=gnnsubnet_test)      
         
         if self.classifier=="graphcheb":
             pred = self.predict_graphcheb(gnnsubnet_test=gnnsubnet_test)
                
+        if self.classifier=="chebnet":
+            pred = self.predict_graphcheb(gnnsubnet_test=gnnsubnet_test)
+               
         pred = np.array(pred)
         pred = pred.reshape(1, pred.size)
 
         return pred
 
+    def train_chebnet(self, epoch_nr=25, shuffle=True, weights=False,
+                        hidden_channels=10,
+                        K=10,
+                        layers_nr=1,
+                        num_classes=2):
+        """
+        ---
+        """
+        use_weights = False
+
+        dataset = self.dataset
+        gene_names = self.gene_names
+
+        graphs_class_0_list = []
+        graphs_class_1_list = []
+        for graph in dataset:
+            if graph.y.detach().cpu().numpy() == 0:
+                graphs_class_0_list.append(graph)
+            else:
+                graphs_class_1_list.append(graph)
+
+        graphs_class_0_len = len(graphs_class_0_list)
+        graphs_class_1_len = len(graphs_class_1_list)
+
+        print(f"Graphs class 0: {graphs_class_0_len}, Graphs class 1: {graphs_class_1_len}")
+
+        ########################################################################################################################
+        # Downsampling of the class that contains more elements ===========================================================
+        # ########################################################################################################################
+
+        if graphs_class_0_len >= graphs_class_1_len:
+            random_graphs_class_0_list = random.sample(graphs_class_0_list, graphs_class_1_len)
+            balanced_dataset_list = graphs_class_1_list + random_graphs_class_0_list
+
+        if graphs_class_0_len < graphs_class_1_len:
+            random_graphs_class_1_list = random.sample(graphs_class_1_list, graphs_class_0_len)
+            balanced_dataset_list = graphs_class_0_list + random_graphs_class_1_list
+
+        # print(len(random_graphs_class_0_list))
+        # print(len(random_graphs_class_1_list))
+
+        random.shuffle(balanced_dataset_list)
+        print(f"Length of balanced dataset list: {len(balanced_dataset_list)}")
+
+        list_len = len(balanced_dataset_list)
+        # print(list_len)
+        train_set_len = int(list_len * 4 / 5)
+        train_dataset_list = balanced_dataset_list[:train_set_len]
+        test_dataset_list = balanced_dataset_list[train_set_len:]
+
+        train_graph_class_0_nr = 0
+        train_graph_class_1_nr = 0
+        for graph in train_dataset_list:
+            if graph.y.detach().cpu().numpy() == 0:
+                train_graph_class_0_nr += 1
+            else:
+                train_graph_class_1_nr += 1
+        print(f"Train graph class 0: {train_graph_class_0_nr}, train graph class 1: {train_graph_class_1_nr}")
+
+        test_graph_class_0_nr = 0
+        test_graph_class_1_nr = 0
+        for graph in test_dataset_list:
+            if graph.y.detach().cpu().numpy() == 0:
+                test_graph_class_0_nr += 1
+            else:
+                test_graph_class_1_nr += 1
+        print(f"Validation graph class 0: {test_graph_class_0_nr}, validation graph class 1: {test_graph_class_1_nr}")
+
+        # s2v_train_dataset = convert_to_s2vgraph(train_dataset_list)
+        # s2v_test_dataset  = convert_to_s2vgraph(test_dataset_list)
+        s2v_train_dataset = train_dataset_list
+        s2v_test_dataset = test_dataset_list
+
+        model_path = 'omics_model.pth'
+        no_of_features = dataset[0].x.shape[1]
+        nodes_per_graph_nr = dataset[0].x.shape[0]
+        print("\tnodes_per_graph_nr", nodes_per_graph_nr)
+
+        input_dim = no_of_features
+        n_classes = 2
+
+        #device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        model = ChebConvNet(input_channels=1, n_features=nodes_per_graph_nr, n_channels=2, n_classes=2, K=8, n_layers=1)
+        #print(model)
+        #model.to(device)
+        optimizer = torch.optim.Adam(model.parameters(), lr=0.001, weight_decay=1e-6)
+        # lr_scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer=optimizer, gamma=0.9,
+        #                                                       last_epoch=-1)
+        criterion = torch.nn.CrossEntropyLoss()
+
+        model.train()
+        min_loss = 50
+
+        best_model = ChebConvNet(input_channels=1, n_features=nodes_per_graph_nr, n_channels=2, n_classes=2, K=8, n_layers=1)
+        #best_model.to(device)
+        # best_model = ChebConv(in_channels=1, out_channels=2, K=10)
+
+        min_val_loss = 1000000.0
+        n_epochs_stop = 25
+        epochs_no_improve = 0
+        batch_size = 100
+
+        train_loader = DataLoader(s2v_train_dataset, batch_size=batch_size, shuffle=True)
+        test_loader = DataLoader(s2v_test_dataset, batch_size=batch_size, shuffle=False)
+
+        for epoch in range(epoch_nr):
+            running_loss = 0.0
+            steps = 0
+            model.train()
+            # data_pbar_loader = tqdm(train_loader, unit='batch')
+            for data in train_loader:
+                out = model(x=data.x, edge_index=data.edge_index, batch=data.batch)
+                loss = criterion(out, data.y)  # Compute the loss.
+                loss.backward()  # Derive gradients.
+                optimizer.step()  # Update parameters based on gradients.
+                optimizer.zero_grad()  # Clear gradients.
+                running_loss += loss.item()
+                steps += 1
+
+            epoch_loss = running_loss / steps
+            model.eval()
+            acc_train = test_model_acc(train_loader, model)
+            val_loss, val_acc, _ , _ = test_model(test_loader, model, criterion)
+
+            print()
+            print(f'Epoch: {epoch:03d}, Train Loss: {epoch_loss:.4f}, Train Acc: {acc_train:.4f}, Val Loss: {val_loss:.4f}, Val Acc: {val_acc:.4f}', end='\t')
+            # print('Epoch {}, loss {:.4f}'.format(epoch, epoch_loss))
+            # print(f"Train Acc {acc_train:.4f}")
+
+            # data_pbar_loader.set_description('epoch: %d' % (epoch))
+            # val_loss = 0
+            #
+            # tr = DataLoader(s2v_test_dataset, batch_size=len(s2v_test_dataset), shuffle=False)
+            # for vv in tr:
+            #     # print("\toutput test")
+            #     output = model(vv.x, vv.edge_index, vv.batch)
+            #     # print("\toutput", output)
+            #
+            # # output = pass_data_iteratively(model, s2v_test_dataset)
+            #
+            # pred = output.max(1, keepdim=True)[1]
+            # labels = torch.LongTensor([graph.y for graph in s2v_test_dataset])
+            # if use_weights:
+            #     loss = nn.CrossEntropyLoss(weight=weight)(output, labels)
+            # else:
+            #     loss = nn.CrossEntropyLoss()(output, labels)
+            # val_loss += loss
+
+            # print('Epoch {}, val_loss {:.4f}'.format(epoch, val_loss))
+            if val_loss < min_val_loss and epoch > 2: # to go through at least 2 epochs
+                print(f"Saving best model with validation loss {val_loss:.4f}", end="")
+                best_model = copy.deepcopy(model)
+                epochs_no_improve = 0
+                min_val_loss = val_loss
+            else:
+                epochs_no_improve += 1
+                # Check early stopping condition
+                if epochs_no_improve == n_epochs_stop:
+                    print('Early stopping!')
+                    # model.load_state_dict(best_model.state_dict())
+                    break
+        #
+        # confusion_array = []
+        # true_class_array = []
+        # predicted_class_array = []
+        # model.eval()
+        # correct = 0
+        # true_class_array = []
+        # predicted_class_array = []
+
+        # loading the parameters of the best model
+        model.load_state_dict(best_model.state_dict())
+
+        _, _, true_labels, predicted_labels = test_model(test_loader, model, criterion)
+
+
+        # test_loss = 0
+        #
+        # model.load_state_dict(best_model.state_dict())
+        #
+        # tr = DataLoader(s2v_test_dataset, batch_size=len(s2v_test_dataset), shuffle=False)
+        # for vv in tr:
+        #     output = model(vv.x, vv.edge_index, vv.batch)
+        #
+        # # output = pass_data_iteratively(model, s2v_test_dataset)
+        # output = np.array(output.detach())
+        # predicted_class = output.argmax(1, keepdims=True)
+        #
+        # predicted_class = list(predicted_class)
+        #
+        # labels = torch.LongTensor([graph.y for graph in s2v_test_dataset])
+        # correct = torch.tensor(np.array(predicted_class)).eq(
+        #     labels.view_as(torch.tensor(np.array(predicted_class)))).sum().item()
+
+
+
+        confusion_matrix_gnn = confusion_matrix(true_labels, predicted_labels)
+        print("\nConfusion matrix (Validation set):\n")
+        print(confusion_matrix_gnn)
+
+        from sklearn.metrics import balanced_accuracy_score
+        acc_bal = balanced_accuracy_score(true_labels, predicted_labels)
+
+        print("Validation balanced accuracy: {}".format(acc_bal))
+
+        model.train()
+
+        self.model_status = 'Trained'
+        self.model = copy.deepcopy(model)
+        self.accuracy = acc_bal
+        self.confusion_matrix = confusion_matrix_gnn
+        # self.test_loss = test_loss
+        self.s2v_test_dataset = s2v_test_dataset
+        self.predictions = predicted_labels
+        self.true_class = true_labels
     
-    def train_graphcheb(self, epoch_nr = 10, shuffle=True, weights=False,
-                    hidden_channels=10,
-                    K=10,
+    
+    def train_graphcheb(self, epoch_nr = 20, shuffle=True, weights=False,
+                    hidden_channels=7,
+                    K=5,
                     layers_nr=2,
                     num_classes=2):
         """
         ---
         """
         use_weights = False
 
@@ -228,39 +455,39 @@
         nodes_per_graph_nr = dataset[0].x.shape[0]
 
         input_dim = no_of_features
         n_classes = 2
 
         model = GraphCheb(
                     num_node_features=input_dim,
-                    hidden_channels=2,
-                    K=10,
-                    layers_nr=1,
+                    hidden_channels=hidden_channels,
+                    K=K,
+                    layers_nr=layers_nr,
                     num_classes=2)
 
-        opt = torch.optim.Adam(model.parameters(), lr = 0.01)
+        opt = torch.optim.Adam(model.parameters(), lr = 0.1)
 
         load_model = False
         if load_model:
             checkpoint = torch.load(model_path)
             model.load_state_dict(checkpoint['state_dict'])
             opt = checkpoint['optimizer']
 
         model.train()
         min_loss = 50
 
         best_model = GraphCheb(
                     num_node_features=input_dim,
-                    hidden_channels=2,
-                    K=10,
+                    hidden_channels=hidden_channels,
+                    K=K,
                     layers_nr=1,
                     num_classes=2)
 
         min_val_loss = 1000000
-        n_epochs_stop = 7
+        n_epochs_stop = 10
         epochs_no_improve = 0
         steps_per_epoch = 35
 
         for epoch in range(epoch_nr):
             model.train()
             pbar = tqdm(range(steps_per_epoch), unit='batch')
             epoch_loss = 0
@@ -321,14 +548,19 @@
 
             print('Epoch {}, val_loss {:.4f}'.format(epoch, val_loss))
             if val_loss < min_val_loss:
                 print(f"Saving best model with validation loss {val_loss}")
                 best_model = copy.deepcopy(model)
                 epochs_no_improve = 0
                 min_val_loss = val_loss
+                #if acc_train > 0.75:
+                #    opt = torch.optim.Adam(model.parameters(), lr = 0.01)
+                #if acc_train > 0.85:
+                #    opt = torch.optim.Adam(model.parameters(), lr = 0.001)
+
 
             else:
                 epochs_no_improve += 1
                 # Check early stopping condition
                 if epochs_no_improve == n_epochs_stop:
                     print('Early stopping!')
                     model.load_state_dict(best_model.state_dict())
@@ -377,15 +609,15 @@
         #self.test_loss = test_loss
         self.s2v_test_dataset = s2v_test_dataset
         self.predictions = predicted_class_array
         self.true_class  = labels
 
 
 
-    def train_chebconv(self, epoch_nr = 10, shuffle=True, weights=False):
+    def train_chebconv(self, epoch_nr = 20, shuffle=True, weights=False):
         """
         Train the GNN model on the data provided during initialisation.
         """
         use_weights = False
 
         dataset = self.dataset
         gene_names = self.gene_names
@@ -450,29 +682,29 @@
         no_of_features = dataset[0].x.shape[1]
         nodes_per_graph_nr = dataset[0].x.shape[0]
 
         input_dim = no_of_features
         n_classes = 2
 
         #model = GraphCNN(num_layers, num_mlp_layers, input_dim, 32, n_classes, 0.5, True, graph_pooling_type, neighbor_pooling_type, 0)
-        model = ChebConv(input_dim,n_classes,10)
+        model = ChebConv(input_dim, n_classes, 10)
 
-        opt = torch.optim.Adam(model.parameters(), lr = 0.01)
+        opt = torch.optim.Adam(model.parameters(), lr = 0.1)
 
         load_model = False
         if load_model:
             checkpoint = torch.load(model_path)
             model.load_state_dict(checkpoint['state_dict'])
             opt = checkpoint['optimizer']
 
         model.train()
 
         #min_loss = 50000
         #best_model = GraphCNN(num_layers, num_mlp_layers, input_dim, 32, n_classes, 0.5, True, graph_pooling_type, neighbor_pooling_type, 0)
-        best_model = ChebConv(input_dim,n_classes,10)
+        best_model = ChebConv(input_dim, n_classes, 10)
 
         min_val_loss = 1000000
         n_epochs_stop = 7
         epochs_no_improve = 0
         steps_per_epoch = 35
         
         for epoch in range(epoch_nr):
@@ -513,15 +745,17 @@
             for graphs in s2v_train_dataset: 
                 output.append(model(x=graphs.x, edge_index=graphs.edge_index).max(0)[0])
                 #output.append(model(x=graphs.x, edge_index=graphs.edge_index).mean(0))
                      
             output = torch.reshape(torch.cat(output,0),(len(output),2))
             
             output = np.array(output.detach())
+            
             predicted_class = output.argmax(1, keepdims=True)          
+            
             predicted_class = list(predicted_class)
 
             labels = torch.LongTensor([graph.y for graph in s2v_train_dataset])
             
             correct = torch.tensor(np.array(predicted_class)).eq(labels.view_as(torch.tensor(np.array(predicted_class)))).sum().item()
 
             acc_train = correct / len(s2v_train_dataset)
@@ -606,22 +840,22 @@
         self.accuracy = acc_bal
         self.confusion_matrix = confusion_matrix_gnn
         #self.test_loss = test_loss
         self.s2v_test_dataset = s2v_test_dataset
         self.predictions = predicted_class_array
         self.true_class  = labels
 
-
-    def train_graphcnn(self, num_layers=5, num_mlp_layers=2, epoch_nr = 10, shuffle=True, weights=False, graph_pooling_type='sum1', neighbor_pooling_type ='sum'):
+    #model = GraphCNN(5, 2, input_dim, 32, n_classes, 0.5, True, 'sum1', 'sum', 0)
+    def train_graphcnn(self, num_layers=2, num_mlp_layers=2, epoch_nr = 20, shuffle=True, weights=False, graph_pooling_type='sum1', neighbor_pooling_type ='sum', learning_rate=0.1):
         """
         Train the GNN model on the data provided during initialisation.
         num_layers: number of layers in the neural networks (INCLUDING the input layer)
         num_mlp_layers: number of layers in mlps (EXCLUDING the input layer)
         graph_pooling_type: how to aggregate entire nodes in a graph (mean, average)
-        neighbor_pooling_type: how to aggregate neighbors (mean, average, or max)
+        neighbor_pooling_type: *sum*! how to aggregate neighbors (mean, average, or max)
         """
         use_weights = False
 
         dataset = self.dataset
         gene_names = self.gene_names
 
         graphs_class_0_list = []
@@ -702,27 +936,27 @@
         #s2v_test_dataset = convert_to_s2vgraph(test_dataset)
         #s2v_train_dataset, s2v_test_dataset = train_test_split(s2v_dataset, test_size=0.2, random_state=123)
 
         input_dim = no_of_features
         n_classes = 2
 
         model = GraphCNN(num_layers, num_mlp_layers, input_dim, 32, n_classes, 0.5, True, graph_pooling_type, neighbor_pooling_type, 0)
-        opt = torch.optim.Adam(model.parameters(), lr = 0.01)
+        opt = torch.optim.Adam(model.parameters(), lr = learning_rate)
 
         load_model = False
         if load_model:
             checkpoint = torch.load(model_path)
             model.load_state_dict(checkpoint['state_dict'])
             opt = checkpoint['optimizer']
 
         model.train()
         min_loss = 50
         best_model = GraphCNN(num_layers, num_mlp_layers, input_dim, 32, n_classes, 0.5, True, graph_pooling_type, neighbor_pooling_type, 0)
         min_val_loss = 1000000
-        n_epochs_stop = 5
+        n_epochs_stop = 10
         epochs_no_improve = 0
         steps_per_epoch = 35
 
         for epoch in range(epoch_nr):
             model.train()
             pbar = tqdm(range(steps_per_epoch), unit='batch')
             epoch_loss = 0
```

### Comparing `GNNSubNet-0.2.0/GNNSubNet/GNN_paper.py` & `GNNSubNet-0.2.1/GNNSubNet/GNN_paper.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/OMICS_workflow.py` & `GNNSubNet-0.2.1/GNNSubNet/OMICS_workflow.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/PGExplainer.py` & `GNNSubNet-0.2.1/GNNSubNet/PGExplainer.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/community_detection.py` & `GNNSubNet-0.2.1/GNNSubNet/community_detection.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/dataset.py` & `GNNSubNet-0.2.1/GNNSubNet/dataset.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/FEATURES_synthetic.txt` & `GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/FEATURES_synthetic.txt`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/NETWORK_synthetic.txt` & `GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/NETWORK_synthetic.txt`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/datasets/synthetic/TARGET_synthetic.txt` & `GNNSubNet-0.2.1/GNNSubNet/datasets/synthetic/TARGET_synthetic.txt`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/features_computation.py` & `GNNSubNet-0.2.1/GNNSubNet/features_computation.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/gnn_explainer.py` & `GNNSubNet-0.2.1/GNNSubNet/gnn_explainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -596,15 +596,142 @@
                 #print(out)
                 loss_xx = loss_xx + loss_hit 
             loss_xx.backward()
             optimizer.step()
          
         return self.node_feat_mask.view(-1,1).detach() #self.edge_mask.detach().sigmoid()
             
+    def explain_graph_modified_chebnet(self, dataset, param):
 
+        self.model.eval()
+        self.__clear_masks__()    
+
+        PRED = []
+        LOGITS = []
+        LOGITS2 =[]
+        # Get the initial prediction.
+        with torch.no_grad():
+            for yy in range(len(dataset)):
+                #x, edge_index = dataset[yy].node_features, dataset[yy].edge_mat
+                x, edge_index = dataset[yy].x, dataset[yy].edge_index   
+                out = self.model(x=x, edge_index=edge_index).max(0)[0]
+                #print(out)
+                log_logits = self.__to_log_prob__(out)
+                log_logits = torch.reshape(log_logits,(1,2))
+                pp = log_logits.argmax(dim=-1)
+                PRED.append(pp)
+                LOGITS.append(-log_logits[0,pp])
+                LOGITS2.append(-log_logits[0,:])    
+
+        self.__set_masks__(dataset[0].x,dataset[0].edge_index)
+        self.to(x.device)
+
+        n_nodes = dataset[0].x.size()[0]
+
+        optimizer = torch.optim.Adam([self.edge_mask, self.node_feat_mask], lr=self.lr)
+
+        #optimizer = torch.optim.Adam([self.edge_mask],
+        #                             lr=self.lr)                                  
+
+        # all nodes belong to same graph
+        batch = torch.zeros(x.shape[0], dtype=int, device=x.device)
+
+        for epoch in range(1, self.epochs + 1):
+            loss_xx  = 0 
+            sampSize = 10
+            if epoch%50==1: 
+                ids  = np.random.randint(len(dataset), size=sampSize)
+
+            optimizer.zero_grad()
+            for dd in ids: 
+                data = dataset[dd]
+                data_copy = copy(data)
+                h = data.x * self.node_feat_mask.sigmoid()
+                data_copy.x = h
+                out = self.model(x=data_copy.x, edge_index=data_copy.edge_index).max(0)[0]
+                log_logits = self.__to_log_prob__(out)
+                log_logits = torch.reshape(log_logits,(1,2))
+                loss_hit  = self.__loss__(-1, log_logits, PRED[dd])
+                loss_fail = self.__loss__(-1, log_logits, abs(PRED[dd]-1))
+                #print(LOGITS2[dd])
+                #print(log_logits)
+                #print(out)
+                loss_xx = loss_xx + loss_hit 
+            loss_xx.backward()
+            optimizer.step()
+
+        return self.node_feat_mask.view(-1,1).detach() #self.edge_mask.detach().sigmoid()
+
+    def explain_graph_modified_chebnet2(self, dataset, param):
+
+        self.model.eval()
+        self.__clear_masks__()    
+        n_nodes = dataset[0].x.size()[0]
+        PRED = []
+        LOGITS = []
+        LOGITS2 =[]
+        # Get the initial prediction.
+        with torch.no_grad():
+            for yy in range(len(dataset)):
+                #x, edge_index = dataset[yy].node_features, dataset[yy].edge_mat
+                x, edge_index = dataset[yy].x, dataset[yy].edge_index   
+                #tr = DataLoader(dataset[yy], batch_size=None, shuffle=False)
+                #for vv in tr:
+                out = self.model(x, edge_index, batch=torch.LongTensor(np.zeros(n_nodes)))
+                #out = self.model(x=x, edge_index=edge_index)
+                #print(out)
+                log_logits = self.__to_log_prob__(out)
+                log_logits = torch.reshape(log_logits,(1,2))
+                pp = log_logits.argmax(dim=-1)
+                PRED.append(pp)
+                LOGITS.append(-log_logits[0,pp])
+                LOGITS2.append(-log_logits[0,:])    
+
+        self.__set_masks__(dataset[0].x,dataset[0].edge_index)
+        self.to(x.device)
+
+        n_nodes = dataset[0].x.size()[0]
+
+        optimizer = torch.optim.Adam([self.edge_mask, self.node_feat_mask], lr=self.lr)
+
+        #optimizer = torch.optim.Adam([self.edge_mask],
+        #                             lr=self.lr)                                  
+
+        # all nodes belong to same graph
+        batch = torch.zeros(x.shape[0], dtype=int, device=x.device)
+
+        for epoch in range(1, self.epochs + 1):
+            loss_xx  = 0 
+            sampSize = 10
+            if epoch%50==1: 
+                ids  = np.random.randint(len(dataset), size=sampSize)
+
+            optimizer.zero_grad()
+            for dd in ids: 
+                data = dataset[dd]
+                data_copy = copy(data)
+                h = data.x * self.node_feat_mask.sigmoid()
+                data_copy.x = h
+                #tr = DataLoader(data_copy, batch_size=None, shuffle=False)
+                #for vv in tr:
+                out = self.model(data_copy.x, data_copy.edge_index, batch=torch.LongTensor(np.zeros(n_nodes)))
+                #out = self.model(x=data_copy.x, edge_index=data_copy.edge_index).max(0)[0]
+                log_logits = self.__to_log_prob__(out)
+                log_logits = torch.reshape(log_logits,(1,2))
+                loss_hit  = self.__loss__(-1, log_logits, PRED[dd])
+                loss_fail = self.__loss__(-1, log_logits, abs(PRED[dd]-1))
+                #print(LOGITS2[dd])
+                #print(log_logits)
+                #print(out)
+                loss_xx = loss_xx + loss_hit 
+            loss_xx.backward()
+            optimizer.step()
+
+        return self.node_feat_mask.view(-1,1).detach() #self.edge_mask.detach().sigmoid()
+    
     def explain_graph_modified_s2v(self, dataset, param):
         self.model.eval()
         self.__clear_masks__()    
 
         PRED = []
         LOGITS = []
         LOGITS2 =[]
```

### Comparing `GNNSubNet-0.2.0/GNNSubNet/gnn_training_utils.py` & `GNNSubNet-0.2.1/GNNSubNet/gnn_training_utils.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/gnnexplainer_sim.py` & `GNNSubNet-0.2.1/GNNSubNet/gnnexplainer_sim.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/gnnexplainer_vanilla_sim.py` & `GNNSubNet-0.2.1/GNNSubNet/gnnexplainer_vanilla_sim.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/graphcnn.py` & `GNNSubNet-0.2.1/GNNSubNet/graphcnn.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/mlp.py` & `GNNSubNet-0.2.1/GNNSubNet/mlp.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet/s2vgraph.py` & `GNNSubNet-0.2.1/GNNSubNet/s2vgraph.py`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/GNNSubNet.egg-info/PKG-INFO` & `GNNSubNet-0.2.1/GNNSubNet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GNNSubNet
-Version: 0.2.0
+Version: 0.2.1
 Summary: Disease Subnetwork Detection with Explainable Graph Neural Networks
 Home-page: https://github.com/pievos101/GNN-SubNet
 Author: Bastian Pfeifer
 Author-email: bastian.pfeifer@medunigraz.at
 License: MIT
 Keywords: graph-neural-networks,disease-networks,explainable-ai
 Platform: UNKNOWN
```

### Comparing `GNNSubNet-0.2.0/GNNSubNet.egg-info/SOURCES.txt` & `GNNSubNet-0.2.1/GNNSubNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/LICENSE` & `GNNSubNet-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/PKG-INFO` & `GNNSubNet-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GNNSubNet
-Version: 0.2.0
+Version: 0.2.1
 Summary: Disease Subnetwork Detection with Explainable Graph Neural Networks
 Home-page: https://github.com/pievos101/GNN-SubNet
 Author: Bastian Pfeifer
 Author-email: bastian.pfeifer@medunigraz.at
 License: MIT
 Keywords: graph-neural-networks,disease-networks,explainable-ai
 Platform: UNKNOWN
```

### Comparing `GNNSubNet-0.2.0/README.md` & `GNNSubNet-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `GNNSubNet-0.2.0/setup.py` & `GNNSubNet-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='GNNSubNet',
     packages=['GNNSubNet'],
-    version='0.2.0',
+    version='0.2.1',
     author="Bastian Pfeifer",
     author_email="bastian.pfeifer@medunigraz.at",
     description='Disease Subnetwork Detection with Explainable Graph Neural Networks',
     long_description='Disease Subnetwork Detection with Explainable Graph Neural Networks',
     license='MIT',
     url='https://github.com/pievos101/GNN-SubNet',
     keywords=['graph-neural-networks', 'disease-networks', 'explainable-ai'],
```

