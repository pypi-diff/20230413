# Comparing `tmp/ultimodel-1.0.0.tar.gz` & `tmp/ultimodel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultimodel-1.0.0.tar", last modified: Tue Apr 11 13:58:16 2023, max compression
+gzip compressed data, was "ultimodel-1.0.1.tar", last modified: Thu Apr 13 16:29:39 2023, max compression
```

## Comparing `ultimodel-1.0.0.tar` & `ultimodel-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:58:16.333174 ultimodel-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-04-11 13:57:46.000000 ultimodel-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3450 2023-04-11 13:58:16.324100 ultimodel-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2936 2023-04-11 13:57:46.000000 ultimodel-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 13:58:16.333174 ultimodel-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1357 2023-04-11 13:57:46.000000 ultimodel-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:58:16.315097 ultimodel-1.0.0/ultimodel/
--rw-rw-rw-   0        0        0    18570 2023-04-11 13:57:46.000000 ultimodel-1.0.0/ultimodel/AttractionFactors.py
--rw-rw-rw-   0        0        0    57136 2023-04-11 13:57:46.000000 ultimodel-1.0.0/ultimodel/CreateNetwork.py
--rw-rw-rw-   0        0        0    36613 2023-04-11 13:57:46.000000 ultimodel-1.0.0/ultimodel/DistributeTraffic.py
--rw-rw-rw-   0        0        0     7110 2023-04-11 13:57:46.000000 ultimodel-1.0.0/ultimodel/Matrices.py
--rw-rw-rw-   0        0        0      990 2023-04-11 13:57:46.000000 ultimodel-1.0.0/ultimodel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:58:16.323115 ultimodel-1.0.0/ultimodel.egg-info/
--rw-rw-rw-   0        0        0     3450 2023-04-11 13:58:16.000000 ultimodel-1.0.0/ultimodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-11 13:58:16.000000 ultimodel-1.0.0/ultimodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:58:16.000000 ultimodel-1.0.0/ultimodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-11 13:58:16.000000 ultimodel-1.0.0/ultimodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 13:58:16.000000 ultimodel-1.0.0/ultimodel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 16:29:39.204896 ultimodel-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-11 13:57:46.000000 ultimodel-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3450 2023-04-13 16:29:39.204896 ultimodel-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2936 2023-04-11 13:57:46.000000 ultimodel-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 16:29:39.204896 ultimodel-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-04-13 15:35:49.000000 ultimodel-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:29:39.204896 ultimodel-1.0.1/ultimodel/
+-rw-rw-rw-   0        0        0    18655 2023-04-13 15:33:40.000000 ultimodel-1.0.1/ultimodel/AttractionFactors.py
+-rw-rw-rw-   0        0        0    57606 2023-04-13 16:27:57.000000 ultimodel-1.0.1/ultimodel/CreateNetwork.py
+-rw-rw-rw-   0        0        0    36771 2023-04-13 15:33:40.000000 ultimodel-1.0.1/ultimodel/DistributeTraffic.py
+-rw-rw-rw-   0        0        0     7149 2023-04-13 15:33:40.000000 ultimodel-1.0.1/ultimodel/Matrices.py
+-rw-rw-rw-   0        0        0      990 2023-04-11 13:57:46.000000 ultimodel-1.0.1/ultimodel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:29:39.204896 ultimodel-1.0.1/ultimodel.egg-info/
+-rw-rw-rw-   0        0        0     3450 2023-04-13 16:29:39.000000 ultimodel-1.0.1/ultimodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-13 16:29:39.000000 ultimodel-1.0.1/ultimodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:29:39.000000 ultimodel-1.0.1/ultimodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-13 16:29:39.000000 ultimodel-1.0.1/ultimodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 16:29:39.000000 ultimodel-1.0.1/ultimodel.egg-info/top_level.txt
```

### Comparing `ultimodel-1.0.0/LICENSE` & `ultimodel-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ultimodel-1.0.0/PKG-INFO` & `ultimodel-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultimodel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Universal transport distribution model
 Home-page: https://github.com/DLR-VF/ULTImodel
 Author: German Aerospace Center - DLR (Nina Thomsen)
 Author-email: nina.thomsen@dlr.de
 License: MIT
 Project-URL: Documentation, https://ultimodel.readthedocs.io/
 Project-URL: Source, https://github.com/DLR-VF/ULTImodel
```

### Comparing `ultimodel-1.0.0/README.md` & `ultimodel-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ultimodel-1.0.0/setup.py` & `ultimodel-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 '''
 import required packages from requirements file
 with open("requirements.txt") as f:
     INSTALL_REQUIRES = [line.strip() for line in f.readlines()]'''
 
 setuptools.setup(
     name='ultimodel',
-    version='1.0.0',
+    version='1.0.1',
     author='German Aerospace Center - DLR (Nina Thomsen)',
     author_email='nina.thomsen@dlr.de',
     description='Universal transport distribution model',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DLR-VF/ULTImodel',
     project_urls = {
         "Documentation": 'https://ultimodel.readthedocs.io/',
         "Source": 'https://github.com/DLR-VF/ULTImodel',
         "Bug Tracker": "https://github.com/DLR-VF/ULTImodel/issues "
     },
     license='MIT',
     packages=['ultimodel'],
     install_requires=['pandas', 'numpy', 'geopandas', 'shapely', 'osmnx', 'networkx', 'tqdm', 'requests', 'scikit-learn', 'scipy']
-)
+)
```

### Comparing `ultimodel-1.0.0/ultimodel/AttractionFactors.py` & `ultimodel-1.0.1/ultimodel/AttractionFactors.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,15 @@
         # find borders for each country
         gdf_borderbuffer = gpd.GeoDataFrame()
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
             warnings.filterwarnings("ignore", category=FutureWarning, append=True)
             warnings.filterwarnings("ignore", category=UserWarning, append=True)
+            warnings.filterwarnings("ignore", category=RuntimeWarning, append=True)
 
             for country in self.countries:
 
                 country_ = border[border[self.taz_cn] == country]
                 country_ = country_[self.taz_geo].buffer(1)
 
                 for index, row in border.iterrows():
```

### Comparing `ultimodel-1.0.0/ultimodel/CreateNetwork.py` & `ultimodel-1.0.1/ultimodel/CreateNetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     """Create network edges from OSM"""
 
     def __init__(self, country, taz, taz_cn="country", taz_geo="geometry"):
         """
 
         :param country: code or name of country
         :param taz: GeoDataFrame including the TAZ
-        :param taz_geo: Name of geometry column in TAZ layer, default "geometry
+        :param taz_geo: Name of geometry column in TAZ layer
         :param taz_cn: Name of column in TAZ layer that defines the country of the TAZ
         :type taz_geo: str
         :type taz_cn: str
         :type taz: gpd.GeoDataFrame
         :type country: str
         """
         self.country = country
@@ -313,15 +313,15 @@
             # 2 get end nodes per graph
             end_nodes = {}
             for sg in S:
                 sg_id = sg[0]
                 sg_g = sg[1]
                 # get all nodes in sg
                 n_sg = [e[:-1] for e in sg_g.edges]
-                # get end nodes: all nodes with two or less edges (or minimum number of edges if min>2)
+                # get end nodes: all nodes with two or fewer edges (or minimum number of edges if min>2)
                 n_sg = np.unique(n_sg, return_counts=True)
                 end_sg = n_sg[0][n_sg[1] <= max(2, min(n_sg[1]))]
                 end_nodes.update({sg_id: end_sg})
 
             # 3 calculate distances between end nodes
             for i in range(len(end_nodes))[:-1]:
                 nodes_sg = nodes[nodes[node_id].isin(end_nodes[i])]
@@ -376,14 +376,15 @@
 
                 # connect if True
                 if connect:
                     # add s1, s2 to container and create line between nodes
                     container.extend([s1, s2])
                     with warnings.catch_warnings():
                         warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
+                        warnings.filterwarnings("ignore", category=FutureWarning, append=True)
                         # create lines in both directions
                         node_from = nodes.loc[nodes[node_id] == row[node_id], node_geo]
                         node_to = nodes.loc[nodes[node_id] == row['{}_near'.format(node_id)], node_geo]
                         line = LineString([[node_from.x, node_from.y], [node_to.x, node_to.y]])
                         # add to road network
                         id_ = roads_final[edge_id].max()
                         roads_final.loc[len(roads_final) + 1] = [id_ + 1, row[node_id], row['{}_near'.format(node_id)], 9, '{}000'.format(self.country), 0,
@@ -394,16 +395,16 @@
             # 5 remove single edges and small subgraphs
             S_del = [_graph_u.subgraph(c).copy() for c in nx.connected_components(_graph_u) if len(c) <= 5]
             # get nodes and edges from RU_del
             nodes_del = []
             edges_del = []
             for sg in S_del:
                 # get all nodes and edges in sg
-                n_sg = np.unique([e[:-1] for e in (sg.edges)])
-                e_sg = np.unique([e[2] for e in (sg.edges)])
+                n_sg = np.unique([e[:-1] for e in sg.edges])
+                e_sg = np.unique([e[2] for e in sg.edges])
                 nodes_del.extend(n_sg)
                 edges_del.extend(e_sg)
             roads_final = roads_final.loc[~roads_final[edge_id].isin(edges_del)]
             nodes_final = nodes.loc[~nodes[node_id].isin(nodes_del)]
 
         else:
             roads_final, nodes_final = edges, nodes
@@ -546,15 +547,15 @@
         # overlay pop and taz
         taz = taz.to_crs(epsg=epsg_pop)
         pop_taz = gpd.overlay(pop, taz[[taz_id, taz_geom]])
 
         for t in taz[taz_id].unique():
             pop_t = pop_taz[pop_taz[taz_id] == t]
             if len(pop_t) > 0:
-                n_c = int(taz.loc[taz[taz_id] == t, "numcon"])
+                n_c = int(taz.loc[taz[taz_id] == t, "numcon"].iloc[0])
                 with warnings.catch_warnings():
                     warnings.filterwarnings("ignore", category=UserWarning)
                     kmeans = KMeans(init="random", n_clusters=n_c, n_init=10, max_iter=300, random_state=42)
                     kmeans.fit(list(zip(pop_t.geometry.x, pop_t.geometry.y)))
                 # assign pop to cluster
                 pop_t = pd.concat([pop_t.reset_index(), pd.Series(kmeans.labels_, name="c_n")], axis=1)
                 # create GeoDataFrame with weights and coordinates of centers (connectors)
@@ -571,25 +572,27 @@
 
     def identify_connector_nodes(self, nodes, node_no="node_id", node_geom="geometry", zone="nuts_id",
                                  weight="weight", country_check=False):
         """
         Move connector locations to network nodes
 
         :param nodes: GeoDataFrame Points; network nodes
-        :param node_no: column name with node identifyer
+        :param node_no: column name with node identifier
         :param node_geom: name of geometry column in nodes GDF
-        :param zone: column name with zone identifyer
+        :param zone: column name with zone identifier
         :param weight: column name with weight of connector
+        :param country_check: ensure that connectors are moved to nodes within the same country
         :return: GeoDataFrame with connector nodes
 
         :type nodes: gpd.GeoDataFrame
         :type node_no: str
         :type node_geom: str
         :type zone: str
         :type weight: str
+        :type country_check: bool
         :rtype: gpd.GeoDataFrame
         """
         con = self.connectors.copy()
 
         # find one node per connector location
         distances = ckdnearest(con, nodes, 'c_n', node_no, 1)
         output = con[[zone, 'c_n', weight]].merge(distances, on='c_n')
@@ -731,15 +734,15 @@
             warnings.filterwarnings("ignore", category=UserWarning, append=True)
             # find nodes in border area
             self.region.to_crs(self.nodes.crs, inplace=True)
             reg_buf = self.region.copy()
             reg_buf[self.taz_geo] = reg_buf[self.taz_geo].buffer(ferry_buffer)
             border_ferry = gpd.overlay(self.nodes, reg_buf[[region_id, self.taz_geo]])
             # find end nodes within two different cells
-            n_g = border_ferry.groupby('LinkID')['order', region_id].nunique().reset_index()
+            n_g = border_ferry.groupby('LinkID')[['order', region_id]].nunique().reset_index()
             filter_ferry = list(n_g.loc[(n_g['order'] > 1) & (n_g[region_id] > 1), 'LinkID'])
             # final result
             ferry_routes = self.ferry[self.ferry['id'].isin(filter_ferry)].copy()
             ferry_nodes = self.nodes[self.nodes['LinkID'].isin(filter_ferry)].copy()
 
         return ferry_routes, ferry_nodes
 
@@ -759,15 +762,15 @@
             warnings.filterwarnings("ignore", category=UserWarning, append=True)
             # find nodes in border area
             self.region.to_crs(self.nodes.crs, inplace=True)
             reg_buf = self.region.copy()
             reg_buf[self.taz_geo] = reg_buf[self.taz_geo].buffer(ferry_buffer)
             border_ferry = gpd.overlay(self.nodes, reg_buf[[self.taz_cn, self.taz_geo]])
             # find end nodes within two different countries
-            n_g = border_ferry.groupby('LinkID')['order', self.taz_cn].nunique().reset_index()
+            n_g = border_ferry.groupby('LinkID')[['order', self.taz_cn]].nunique().reset_index()
             filter_ferry = list(n_g.loc[(n_g['order'] > 1) & (n_g[self.taz_cn] > 1), 'LinkID'])
             # final result
             ferry_routes = self.ferry[self.ferry['id'].isin(filter_ferry)].copy()
             ferry_nodes = self.nodes[self.nodes['LinkID'].isin(filter_ferry)].copy()
 
         return ferry_routes, ferry_nodes
 
@@ -884,15 +887,15 @@
                             line = LineString([[node_from.x, node_from.y], [node_to.x, node_to.y]])
                             # add to Lines GDF
                             lines.loc[len(lines) + 1] = [id_st, l[0][node_id], l[1][node_id], type_ferry, 'FERRY',
                                                          len_ferry, speed, (len_ferry / speed) * 60 ** 2, line]
                             id_st += 1
                     else:
                         print('no start / end connection for ferry route {}'.format(ferry))
-
+        lines.crs = network_roads.crs
         network_roads = pd.concat([network_roads, lines])
 
         return network_roads
 
 
 class CombineNetworks:
     """
@@ -940,14 +943,15 @@
         # find borders for each country
         gdf_borderbuffer = gpd.GeoDataFrame()
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
             warnings.filterwarnings("ignore", category=FutureWarning, append=True)
             warnings.filterwarnings("ignore", category=UserWarning, append=True)
+            warnings.filterwarnings("ignore", category=RuntimeWarning, append=True)
 
             for country in self.countries:
 
                 country_ = taz_dis[taz_dis[self.taz_cn] == country]
                 country_ = country_[taz_geo].buffer(1)
 
                 for index, row in taz_dis.iterrows():
@@ -1093,14 +1097,15 @@
                 pairs_b = pairs_b.sort_values(by='distance_x')
                 pairs_b = pairs_b.drop_duplicates(subset='node_from')
                 pairs_b = pairs_b.drop_duplicates(subset='node_to')
                 pairs_b = [[row['node_from'], row['node_to']] for i, row in pairs_b.iterrows()]
 
                 with warnings.catch_warnings():
                     warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
+                    warnings.filterwarnings("ignore", category=FutureWarning, append=True)
                     # create lines between node pairs
                     for l in pairs_b:
                         # get coordinates and create LineString
                         node_from = nodes_int.loc[nodes_int[node_id] == l[0], 'geometry']
                         node_to = nodes_int.loc[nodes_int[node_id] == l[1], 'geometry']
                         line = LineString([[node_from.x, node_from.y], [node_to.x, node_to.y]])
                         # add to Lines GDF
@@ -1108,11 +1113,12 @@
                         id_st += 1
                 self.dict_borders.update({b: len(pairs_b)})
             else:
                 print('No border connection for {}'.format(b))
                 self.dict_borders.update({b: 0})
 
         # concat border crossings and rest of the network
+        lines.crs = self.network.crs
         self.network_int = pd.concat([self.network, lines])
         # ensure that IDs are integer
         self.network_int[roads_id] = self.network_int[roads_id].astype(int)
         print("Finished connecting border roads at {}".format(datetime.now()))
```

### Comparing `ultimodel-1.0.0/ultimodel/DistributeTraffic.py` & `ultimodel-1.0.1/ultimodel/DistributeTraffic.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :type taz: gpd.GeoDataFrame or pd.DataFrame
     :type goal_col: str
     :rtype: np.array
     """
     # choice probabilities and trips
     mx_trips = np.zeros(mx_grav.shape)
     for t in taz[taz_id]:
-        goal = float(taz.loc[taz[taz_id] == t, goal_col])
+        goal = float(taz.loc[taz[taz_id] == t, goal_col].iloc[0])
         # get probabilities for trips starting at t
         prob_a = mx_grav[t, :] / mx_grav[t, :].sum()
         prob_b = mx_grav[:, t] / mx_grav[:, t].sum()
         mx_trips[t, :] += prob_a * (goal / 2)
         mx_trips[:, t] += prob_b * (goal / 2)
     # fill NA
     mx_trips[np.isnan(mx_trips)] = 0
@@ -209,17 +209,17 @@
         :return: vkt per segment
 
         :type cn: str
         :type target_col: str
         :type unit: float
         :rtype: dict
         """
-        target = float(self.country_layer.loc[self.country_layer[self.cn_col]==cn, target_col])
-        shares_int = pt_shares_int(a=float(self.country_layer.loc[self.country_layer[self.cn_col]==cn, 'area']),
-                                   b=float(self.country_layer.loc[self.country_layer[self.cn_col]==cn, 'border_share']))
+        target = float(self.country_layer.loc[self.country_layer[self.cn_col]==cn, target_col].iloc[0])
+        shares_int = pt_shares_int(a=float(self.country_layer.loc[self.country_layer[self.cn_col]==cn, 'area'].iloc[0]),
+                                   b=float(self.country_layer.loc[self.country_layer[self.cn_col]==cn, 'border_share'].iloc[0]))
 
         f_in_c = target * shares_int['pt_share_foreign']
         int1 = target * shares_int['pt_share_foreign'] * shares_int['pt_ratio_int']
         inner = target - f_in_c - int1
 
         short_ = 0.65 * (inner + int1)
         long_ = 0.35 * (inner + int1) - int1
@@ -264,25 +264,25 @@
             seg_split = 'hft'
         if segments is None:
             segments = shares_tkm.keys()
 
         # check if segments, loads and shares match
         if (sorted(segments) == sorted(shares_tkm.keys())) & (sorted(segments) == sorted(loads_t.keys())) & (seg_split in segments):
 
-            target = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, target_col])
+            target = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, target_col].iloc[0])
 
             cat_dict = {0: {'int_imex': 0.03, 'int_transit': 0.00, 'nat': 0.97},
                         1: {'int_imex': 0.15, 'int_transit': 0.02, 'nat': 0.83},
                         2: {'int_imex': 0.15, 'int_transit': 0.05, 'nat': 0.80},
                         3: {'int_imex': 0.20, 'int_transit': 0.10, 'nat': 0.70},
                         4: {'int_imex': 0.00, 'int_transit': 0.00, 'nat': 1.00}}
 
-            border_share = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'border_share'])
-            neighbors = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'neighbors'])
-            border_crossings = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'border_crossings_count'])
+            border_share = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'border_share'].iloc[0])
+            neighbors = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'neighbors'].iloc[0])
+            border_crossings = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'border_crossings_count'].iloc[0])
 
             # find category for country
             cat_country = 2
             if (border_share < 0.1) & (neighbors <= 1):
                 cat_country = 0
             elif neighbors <= 5:
                 if (border_crossings < 4) | (border_share < 0.5):
@@ -294,15 +294,15 @@
                     cat_country = 2
                 else:
                     cat_country = 3
             elif border_share == 0:
                 cat_country = 4
 
             # distances
-            area = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'area'])
+            area = float(self.country_layer.loc[self.country_layer[self.cn_col] == cn, 'area'].iloc[0])
             dis_long = 0.365 * area**(1/2) + 61.488
             dis_short = 1.183 * area**(1/4) + 22.361
             dis_transit = 0.928 * area**(1/2) + 38.998
 
             # transform input tkm to t:
             share_national = cat_dict[cat_country]['nat']
             share_international = cat_dict[cat_country]['int_imex']
@@ -455,17 +455,17 @@
         # trip generation
         taz['pt_goal'] = taz[taz_pop] * mob_rate
 
         # trip distribution
         # gravity model: gravity values
         mx_grav = np.zeros((len(taz), len(taz)))
         for o in taz['id']:
-            pop_o = float(taz.loc[taz['id'] == o, taz_pop])
+            pop_o = float(taz.loc[taz['id'] == o, taz_pop].iloc[0])
             for d in taz['id']:
-                pop_d = float(taz.loc[taz['id'] == d, taz_pop])
+                pop_d = float(taz.loc[taz['id'] == d, taz_pop].iloc[0])
                 mx_grav[o, d] = (pop_o*pop_d)**alpha * mtx[o, d, 0]**gamma
         # fill diagonal (no trips) and NaN
         np.fill_diagonal(mx_grav, 0)
         mx_grav[np.isnan(mx_grav)] = 0
         # choice probabilities and trips
         mx_trips = get_trip_matrix(mx_grav, taz, 'pt_goal', taz_id='id')
         # scaling to match target
@@ -528,17 +528,17 @@
                 if c in target_trips.keys():
                     taz.loc[taz[self.taz_cn]==c, 'ft_goal'] = taz.loc[taz[self.taz_cn]==c, index_col]/taz.loc[taz[self.taz_cn]==c, index_col].sum() * target_trips[c][trips_key]
 
         # trip distribution
         # gravity model: gravity values
         mx_grav = np.zeros((len(taz), len(taz)))
         for o in taz['id']:
-            ind_o = float(taz.loc[taz['id'] == o, index_col])
+            ind_o = float(taz.loc[taz['id'] == o, index_col].iloc[0])
             for d in taz['id']:
-                ind_d = float(taz.loc[taz['id'] == d, index_col])
+                ind_d = float(taz.loc[taz['id'] == d, index_col].iloc[0])
                 mx_grav[o, d] = ind_o * ind_d * np.exp(-beta*mtx[o, d, 1])
         # fill diagonal (no trips) and NaN
         np.fill_diagonal(mx_grav, 0)
         mx_grav[np.isnan(mx_grav)] = 0
 
         # get trips
         mx_trips = get_trip_matrix(mx_grav, taz, 'ft_goal', taz_id='id')
@@ -606,15 +606,15 @@
         if veh_types is None:
             veh_types = ['car']
 
         # subordinate network length from TAZ
         sub = self.taz[[taz_id, sub_len]].copy()
         sub.rename(columns={sub_len: 'length'}, inplace=True)
         sub[net_type] = 0
-        sub['weighted_length'] = sub['length']*float(weights.loc[weights[net_type]==0, 'weight'])
+        sub['weighted_length'] = sub['length']*float(weights.loc[weights[net_type]==0, 'weight'].iloc[0])
         # concat with network length per taz from net
         len_per_type = self.net.groupby([taz_id, net_type])['length'].sum().reset_index()
         len_per_type = pd.concat([len_per_type, sub[[taz_id, net_type, 'length']]])
 
         # weighted length per net type and taz
         net = self.net.merge(weights, on=net_type, how='left')
         net.loc[net['weight'].isna(), 'weight'] = 0
@@ -718,48 +718,48 @@
             net['{}_short'.format(veh_type)] = 0
             taz_2['{}_sub'.format(veh_type)] = 0
 
         # weighted length per net type and taz
         net = net.merge(weights, on=net_type, how='left')
         net.loc[net['weight'].isna(), 'weight'] = 0
         net['weighted_length'] = net['length'] * net['weight']
-        taz_2['weighted_sub'] = taz_2[sub_len]*float(weights.loc[weights[net_type]==0, 'weight'])
+        taz_2['weighted_sub'] = taz_2[sub_len]*float(weights.loc[weights[net_type]==0, 'weight'].iloc[0])
 
         # iterate over taz
         for t in taz_2[taz_id]:
             # adjust link weight for roads within taz
             net['weighted_length2'] = net['weighted_length']
             net['weight2'] = net['weight']
             taz_2['weighted_sub2'] = taz_2['weighted_sub']
-            taz_2['weight2'] = float(weights.loc[weights[net_type]==0, 'weight'])
+            taz_2['weight2'] = float(weights.loc[weights[net_type]==0, 'weight'].iloc[0])
             net.loc[net[taz_id] == t, 'weighted_length2'] = net.loc[net[taz_id] == t, 'weighted_length2'] * fac_cell
             net.loc[net[taz_id] == t, 'weight2'] = net.loc[net[taz_id] == t, 'weight2'] *fac_cell
             taz_2.loc[taz_2[taz_id] == t, 'weighted_sub2'] = taz_2.loc[taz_2[taz_id] == t, 'weighted_sub2'] * fac_cell
             taz_2.loc[taz_2[taz_id] == t, 'weight2'] = taz_2.loc[taz_2[taz_id] == t, 'weight2'] * fac_cell
 
             # list of taz within distance
-            t_id = int(taz_2.loc[taz_2[taz_id] == t, taz_mx_id])
+            t_id = int(taz_2.loc[taz_2[taz_id] == t, taz_mx_id].iloc[0])
             matrix_t = matrix_dis[t_id, :]
             sur_ids = np.where(matrix_t <= distance)[0].tolist()
 
             # for small taz: add surrounding TAZ within higher distances if no sur found for distance
-            if (len(sur_ids)==0) & (float(taz_2.loc[taz_2[taz_id]==t, 'area'])<cell_size):
+            if (len(sur_ids) == 0) & (float(taz_2.loc[taz_2[taz_id] == t, 'area'].iloc[0]) < cell_size):
                 sur_ids = np.where(matrix_t == matrix_t.min())[0].tolist()
 
             # add id of t to sur ids (all relevant cells) and get taz_ids
             sur_ids.append(t_id)
             sur_ids_taz = taz_2.loc[taz_2[taz_mx_id].isin(sur_ids), taz_id].tolist()
 
             # aggregate weighted network length in sur_ids
             agg_w_len = net.loc[net[taz_id].isin(sur_ids_taz), 'weighted_length2'].sum()
             agg_w_len += taz_2.loc[taz_2[taz_mx_id].isin(sur_ids), 'weighted_sub2'].sum()
 
             # calculate trips per km for veh_types
             for veh_type in veh_types:
-                taz_vkt = float(taz_2.loc[taz_2[taz_id] == t, veh_type])
+                taz_vkt = float(taz_2.loc[taz_2[taz_id] == t, veh_type].iloc[0])
                 taz_veh = taz_vkt / agg_w_len
                 net.loc[net[taz_id].isin(sur_ids_taz), '{}_short'.format(veh_type)] = net.loc[net[taz_id].isin(sur_ids_taz), '{}_short'.format(veh_type)] + net.loc[net[taz_id].isin(sur_ids_taz), 'weight2'] * taz_veh
                 taz_2.loc[taz_2[taz_id].isin(sur_ids_taz), '{}_sub'.format(veh_type)] += taz_2.loc[taz_2[taz_id].isin(sur_ids_taz), 'weight2'] * taz_veh * taz_2.loc[taz_2[taz_id].isin(sur_ids_taz), sub_len]
 
         net.drop(columns=['weight', 'weight2', 'weighted_length', 'weighted_length2'], inplace=True)
 
         cols_keep = ['{}_sub'.format(veh_type) for veh_type in veh_types]
```

### Comparing `ultimodel-1.0.0/ultimodel/Matrices.py` & `ultimodel-1.0.1/ultimodel/Matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         :type zone_col: str
         :type id_col: str
         :type weight_col: str
         :type x_: str
         :type y_: str
         :type conn_geo: str
         """
-        self.conn = conn
+        self.conn = conn.copy()
         if type(self.conn) == gpd.GeoDataFrame:
             self.conn.to_crs(epsg=4326, inplace=True)
             # transform to data frame with x and y coordinates
             self.conn[x_] = self.conn[conn_geo].x
             self.conn[y_] = self.conn[conn_geo].y
             self.conn = self.conn[[id_col, zone_col, weight_col, x_, y_]]
 
@@ -131,29 +131,29 @@
 
         # weight matrix
         w = np.zeros((len(self.conn), len(self.conn)))
 
         for a in tqdm(range(len(self.conn))):
             for b in range(len(self.conn)):
                 # calc od weight
-                w[a, b] = float(self.conn.loc[self.conn[self.id_col] == a, self.weight_col]) * float(self.conn.loc[self.conn[self.id_col] == b, self.weight_col])
+                w[a, b] = float(self.conn.loc[self.conn[self.id_col] == a, self.weight_col].iloc[0]) * float(self.conn.loc[self.conn[self.id_col] == b, self.weight_col].iloc[0])
 
         # container for final values
         mx_z = np.zeros((len(zones), len(zones), 2))
 
         # fill matrix container with weighted mean for zone relations
         time1 = time.time()
         print('start aggregating zone matrix:', datetime.now())
         for o in tqdm(zones):
-            id_o = int(zones_df.loc[zones_df['zone'] == o, 'id'])
+            id_o = int(zones_df.loc[zones_df['zone'] == o, 'id'].iloc[0])
             id_conn_o = list(self.conn.loc[self.conn[self.zone_col] == o, self.id_col])
             mtx_o = self.all_mtx[id_conn_o, :]
             w_o = w[id_conn_o, :]
             for d in zones:
-                id_d = int(zones_df.loc[zones_df['zone'] == d, 'id'])
+                id_d = int(zones_df.loc[zones_df['zone'] == d, 'id'].iloc[0])
                 id_conn_d = list(self.conn.loc[self.conn[self.zone_col] == d, self.id_col])
                 mtx_od = mtx_o[:, id_conn_d]
                 w_od = w_o[:, id_conn_d]
                 # weighted mean
                 mtx_od[:, :, 0] *= w_od
                 mtx_od[:, :, 1] *= w_od
                 mx_z[id_o, id_d, :] = np.nansum(mtx_od, axis=0).sum(axis=0)  # should be shape (2,)
```

### Comparing `ultimodel-1.0.0/ultimodel/__init__.py` & `ultimodel-1.0.1/ultimodel/__init__.py`

 * *Files identical despite different names*

### Comparing `ultimodel-1.0.0/ultimodel.egg-info/PKG-INFO` & `ultimodel-1.0.1/ultimodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultimodel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Universal transport distribution model
 Home-page: https://github.com/DLR-VF/ULTImodel
 Author: German Aerospace Center - DLR (Nina Thomsen)
 Author-email: nina.thomsen@dlr.de
 License: MIT
 Project-URL: Documentation, https://ultimodel.readthedocs.io/
 Project-URL: Source, https://github.com/DLR-VF/ULTImodel
```

