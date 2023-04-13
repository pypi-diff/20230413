# Comparing `tmp/dama-0.4.6.tar.gz` & `tmp/dama-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dama-0.4.6.tar", last modified: Fri May  7 14:24:12 2021, max compression
+gzip compressed data, was "dist/dama-0.4.7.tar", last modified: Thu Apr 13 09:36:56 2023, max compression
```

## Comparing `dama-0.4.6.tar` & `dama-0.4.7.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:12.387010 dama-0.4.6/
--rw-r--r--   0 peller    (1000) peller    (1000)    15816 2021-05-07 14:24:12.388009 dama-0.4.6/PKG-INFO
--rw-r--r--   0 peller    (1000) peller    (1000)    12219 2021-03-26 16:34:04.000000 dama-0.4.6/README.md
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:11.794912 dama-0.4.6/dama/
--rw-r--r--   0 peller    (1000) peller    (1000)      355 2021-05-05 10:41:59.000000 dama-0.4.6/dama/__init__.py
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:11.887815 dama-0.4.6/dama/cm/
--rw-r--r--   0 peller    (1000) peller    (1000)      398 2021-03-23 10:50:22.000000 dama-0.4.6/dama/cm/__init__.py
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:12.061798 dama-0.4.6/dama/core/
--rw-r--r--   0 peller    (1000) peller    (1000)        0 2021-03-11 16:55:33.000000 dama-0.4.6/dama/core/__init__.py
--rw-r--r--   0 peller    (1000) peller    (1000)     7576 2021-05-05 10:41:59.000000 dama-0.4.6/dama/core/axis.py
--rw-r--r--   0 peller    (1000) peller    (1000)    11894 2021-03-22 18:20:09.000000 dama-0.4.6/dama/core/binneddata.py
--rw-r--r--   0 peller    (1000) peller    (1000)     9095 2021-03-25 14:45:48.000000 dama-0.4.6/dama/core/edges.py
--rw-r--r--   0 peller    (1000) peller    (1000)    11421 2021-03-26 14:53:41.000000 dama-0.4.6/dama/core/grid.py
--rw-r--r--   0 peller    (1000) peller    (1000)    16769 2021-05-05 10:41:59.000000 dama-0.4.6/dama/core/gridarray.py
--rw-r--r--   0 peller    (1000) peller    (1000)    13909 2021-05-05 10:41:59.000000 dama-0.4.6/dama/core/griddata.py
--rw-r--r--   0 peller    (1000) peller    (1000)     1504 2021-03-11 16:55:33.000000 dama-0.4.6/dama/core/pointarray.py
--rw-r--r--   0 peller    (1000) peller    (1000)     7211 2021-05-05 10:41:59.000000 dama-0.4.6/dama/core/pointdata.py
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:12.100423 dama-0.4.6/dama/plotting/
--rw-r--r--   0 peller    (1000) peller    (1000)       25 2021-03-11 16:55:33.000000 dama-0.4.6/dama/plotting/__init__.py
--rw-r--r--   0 peller    (1000) peller    (1000)    15442 2021-03-25 11:07:13.000000 dama-0.4.6/dama/plotting/stat_plot.py
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:12.273997 dama-0.4.6/dama/translations/
--rw-r--r--   0 peller    (1000) peller    (1000)      213 2021-03-26 08:42:03.000000 dama-0.4.6/dama/translations/__init__.py
--rw-r--r--   0 peller    (1000) peller    (1000)     2509 2021-03-11 16:55:33.000000 dama-0.4.6/dama/translations/histogram.py
--rw-r--r--   0 peller    (1000) peller    (1000)     4483 2021-03-12 15:54:04.000000 dama-0.4.6/dama/translations/interpolation.py
--rw-r--r--   0 peller    (1000) peller    (1000)     5422 2021-03-11 16:55:33.000000 dama-0.4.6/dama/translations/kde.py
--rw-r--r--   0 peller    (1000) peller    (1000)     1790 2021-03-11 16:55:33.000000 dama-0.4.6/dama/translations/lookup.py
--rw-r--r--   0 peller    (1000) peller    (1000)    10899 2021-03-26 08:38:03.000000 dama-0.4.6/dama/translations/ndimage.py
--rw-r--r--   0 peller    (1000) peller    (1000)     2492 2021-03-11 16:55:33.000000 dama-0.4.6/dama/translations/resample.py
--rw-r--r--   0 peller    (1000) peller    (1000)     6902 2021-03-11 16:55:33.000000 dama-0.4.6/dama/translations/translation.py
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:12.369011 dama-0.4.6/dama/utils/
--rw-r--r--   0 peller    (1000) peller    (1000)        0 2021-03-11 16:55:33.000000 dama-0.4.6/dama/utils/__init__.py
--rw-r--r--   0 peller    (1000) peller    (1000)      560 2021-03-11 16:55:33.000000 dama-0.4.6/dama/utils/bind.py
--rw-r--r--   0 peller    (1000) peller    (1000)      794 2021-05-05 10:41:59.000000 dama-0.4.6/dama/utils/fileio.py
--rw-r--r--   0 peller    (1000) peller    (1000)     7576 2021-03-25 11:06:59.000000 dama-0.4.6/dama/utils/formatter.py
--rw-r--r--   0 peller    (1000) peller    (1000)     7287 2021-03-11 16:55:33.000000 dama-0.4.6/dama/utils/stats.py
-drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2021-05-07 14:24:11.870260 dama-0.4.6/dama.egg-info/
--rw-r--r--   0 peller    (1000) peller    (1000)    15816 2021-05-07 14:24:11.000000 dama-0.4.6/dama.egg-info/PKG-INFO
--rw-r--r--   0 peller    (1000) peller    (1000)      798 2021-05-07 14:24:11.000000 dama-0.4.6/dama.egg-info/SOURCES.txt
--rw-r--r--   0 peller    (1000) peller    (1000)        1 2021-05-07 14:24:11.000000 dama-0.4.6/dama.egg-info/dependency_links.txt
--rw-r--r--   0 peller    (1000) peller    (1000)       69 2021-05-07 14:24:11.000000 dama-0.4.6/dama.egg-info/requires.txt
--rw-r--r--   0 peller    (1000) peller    (1000)        5 2021-05-07 14:24:11.000000 dama-0.4.6/dama.egg-info/top_level.txt
--rw-r--r--   0 peller    (1000) peller    (1000)      112 2021-05-07 14:24:12.392011 dama-0.4.6/setup.cfg
--rw-r--r--   0 peller    (1000) peller    (1000)      787 2021-05-07 14:24:09.000000 dama-0.4.6/setup.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:56.231747 dama-0.4.7/
+-rw-r--r--   0 peller    (1000) peller    (1000)    11357 2021-03-11 16:55:33.000000 dama-0.4.7/LICENSE
+-rw-r--r--   0 peller    (1000) peller    (1000)    12730 2023-04-13 09:36:56.235746 dama-0.4.7/PKG-INFO
+-rw-r--r--   0 peller    (1000) peller    (1000)    12410 2021-05-20 15:44:32.000000 dama-0.4.7/README.md
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:51.729580 dama-0.4.7/dama/
+-rw-r--r--   0 peller    (1000) peller    (1000)      355 2021-05-05 10:41:59.000000 dama-0.4.7/dama/__init__.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:52.368403 dama-0.4.7/dama/cm/
+-rw-r--r--   0 peller    (1000) peller    (1000)      398 2021-03-23 10:50:22.000000 dama-0.4.7/dama/cm/__init__.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:53.826485 dama-0.4.7/dama/core/
+-rw-r--r--   0 peller    (1000) peller    (1000)        0 2021-03-11 16:55:33.000000 dama-0.4.7/dama/core/__init__.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     7576 2021-05-05 10:41:59.000000 dama-0.4.7/dama/core/axis.py
+-rw-r--r--   0 peller    (1000) peller    (1000)    12464 2021-05-14 13:11:54.000000 dama-0.4.7/dama/core/binneddata.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     9095 2021-03-25 14:45:48.000000 dama-0.4.7/dama/core/edges.py
+-rw-r--r--   0 peller    (1000) peller    (1000)    11884 2021-05-25 14:04:58.000000 dama-0.4.7/dama/core/grid.py
+-rw-r--r--   0 peller    (1000) peller    (1000)    16769 2021-05-05 10:41:59.000000 dama-0.4.7/dama/core/gridarray.py
+-rw-r--r--   0 peller    (1000) peller    (1000)    13909 2021-05-05 10:41:59.000000 dama-0.4.7/dama/core/griddata.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     1504 2021-03-11 16:55:33.000000 dama-0.4.7/dama/core/pointarray.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     7211 2021-05-05 10:41:59.000000 dama-0.4.7/dama/core/pointdata.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:54.149036 dama-0.4.7/dama/plotting/
+-rw-r--r--   0 peller    (1000) peller    (1000)       25 2021-03-11 16:55:33.000000 dama-0.4.7/dama/plotting/__init__.py
+-rw-r--r--   0 peller    (1000) peller    (1000)    15442 2021-03-25 11:07:13.000000 dama-0.4.7/dama/plotting/stat_plot.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:55.382568 dama-0.4.7/dama/translations/
+-rw-r--r--   0 peller    (1000) peller    (1000)      213 2021-03-26 08:42:03.000000 dama-0.4.7/dama/translations/__init__.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     2509 2021-03-11 16:55:33.000000 dama-0.4.7/dama/translations/histogram.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     4483 2021-03-12 15:54:04.000000 dama-0.4.7/dama/translations/interpolation.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     5422 2021-03-11 16:55:33.000000 dama-0.4.7/dama/translations/kde.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     1790 2021-03-11 16:55:33.000000 dama-0.4.7/dama/translations/lookup.py
+-rw-r--r--   0 peller    (1000) peller    (1000)    10899 2021-03-26 08:38:03.000000 dama-0.4.7/dama/translations/ndimage.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     2492 2021-03-11 16:55:33.000000 dama-0.4.7/dama/translations/resample.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     6902 2021-03-11 16:55:33.000000 dama-0.4.7/dama/translations/translation.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:56.115188 dama-0.4.7/dama/utils/
+-rw-r--r--   0 peller    (1000) peller    (1000)        0 2021-03-11 16:55:33.000000 dama-0.4.7/dama/utils/__init__.py
+-rw-r--r--   0 peller    (1000) peller    (1000)      560 2021-03-11 16:55:33.000000 dama-0.4.7/dama/utils/bind.py
+-rw-r--r--   0 peller    (1000) peller    (1000)      794 2021-05-05 10:41:59.000000 dama-0.4.7/dama/utils/fileio.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     7576 2021-03-25 11:06:59.000000 dama-0.4.7/dama/utils/formatter.py
+-rw-r--r--   0 peller    (1000) peller    (1000)     7287 2021-03-11 16:55:33.000000 dama-0.4.7/dama/utils/stats.py
+drwxr-xr-x   0 peller    (1000) peller    (1000)        0 2023-04-13 09:36:52.236397 dama-0.4.7/dama.egg-info/
+-rw-r--r--   0 peller    (1000) peller    (1000)    12730 2023-04-13 09:36:49.000000 dama-0.4.7/dama.egg-info/PKG-INFO
+-rw-r--r--   0 peller    (1000) peller    (1000)      806 2023-04-13 09:36:50.000000 dama-0.4.7/dama.egg-info/SOURCES.txt
+-rw-r--r--   0 peller    (1000) peller    (1000)        1 2023-04-13 09:36:49.000000 dama-0.4.7/dama.egg-info/dependency_links.txt
+-rw-r--r--   0 peller    (1000) peller    (1000)       69 2023-04-13 09:36:49.000000 dama-0.4.7/dama.egg-info/requires.txt
+-rw-r--r--   0 peller    (1000) peller    (1000)        5 2023-04-13 09:36:49.000000 dama-0.4.7/dama.egg-info/top_level.txt
+-rw-r--r--   0 peller    (1000) peller    (1000)      112 2023-04-13 09:36:56.261103 dama-0.4.7/setup.cfg
+-rw-r--r--   0 peller    (1000) peller    (1000)      787 2023-04-13 09:36:29.000000 dama-0.4.7/setup.py
```

### Comparing `dama-0.4.6/README.md` & `dama-0.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -156,31 +156,31 @@
 > y_pixel_boundaries = np.concatenate([[y[0] - 0.5*y_widths[0]], y[:-1] + 0.5*y_widths, [y[-1] + 0.5*y_widths[-1]]])
 > 
 > pc = plt.pcolormesh(x_pixel_boundaries, y_pixel_boundaries, a)
 > plt.gca().set_xlabel('x')
 > plt.gca().set_ylabel('y')
 > cb = plt.colorbar(pc)
 > cb.set_label('a')
-```
+> ```
 
 and for doing the interpolation:
 
 > ```
 > from scipy.interpolate import griddata
 > 
 > interp_x = np.linspace(0,3*np.pi, 200)
 > interp_y = np.linspace(0,2*np.pi, 200) 
 > 
 > grid_x, grid_y = np.meshgrid(interp_x, interp_y)
 > 
 > points = np.vstack([xx.flatten(), yy.flatten()]).T
 > values = a.flatten()
 > 
->interp_a = griddata(points, values, (grid_x, grid_y), method='cubic')
-```
+> interp_a = griddata(points, values, (grid_x, grid_y), method='cubic')
+> ```
 
 ### PointData
 
 Another representation of data is `PointData`, which is not any different of a dictionary holding same-length nd-arrays or a pandas `DataFrame` (And can actually be instantiated with those).
 
 
 ```python
@@ -195,16 +195,16 @@
 ```
 
 
 
 
 <table>
 <tbody>
-<tr><td><b>x</b></td><td style="text-align: right;">1.73</td><td style="text-align: right;">-0.484</td><td style="text-align: right;">0.0993 </td><td>...</td><td style="text-align: right;">0.226 </td><td style="text-align: right;">-0.0637 </td><td style="text-align: right;">0.378  </td></tr>
-<tr><td><b>a</b></td><td style="text-align: right;">0.14</td><td style="text-align: right;"> 0.105</td><td style="text-align: right;">0.00459</td><td>...</td><td style="text-align: right;">0.0174</td><td style="text-align: right;"> 0.00351</td><td style="text-align: right;">0.00574</td></tr>
+<tr><td><b>x</b></td><td style="text-align: right;">0.0341 </td><td style="text-align: right;">0.212</td><td style="text-align: right;">0.517</td><td>...</td><td style="text-align: right;">1.27</td><td style="text-align: right;">0.827</td><td style="text-align: right;">1.57 </td></tr>
+<tr><td><b>a</b></td><td style="text-align: right;">0.00106</td><td style="text-align: right;">0.035</td><td style="text-align: right;">0.18 </td><td>...</td><td style="text-align: right;">1.59</td><td style="text-align: right;">0.246</td><td style="text-align: right;">0.201</td></tr>
 </tbody>
 </table>
 
 
 
 
 ```python
@@ -238,16 +238,16 @@
 ```
 
 
 
 
 <table>
 <tbody>
-<tr><td><b>x</b></td><td><b>[-4.377 -3.93 ]</b></td><td><b>[-3.93  -3.483]</b></td><td><b>[-3.483 -3.036]</b></td><td>...</td><td><b>[3.225 3.672]</b></td><td><b>[3.672 4.12 ]</b></td><td><b>[4.12  4.567]</b></td></tr>
-<tr><td><b>a</b></td><td>30.8                  </td><td>119                   </td><td>686                   </td><td>...</td><td>357                 </td><td>75.6                </td><td>20.6                </td></tr>
+<tr><td><b>x</b></td><td><b>[-4.392 -3.962]</b></td><td><b>[-3.962 -3.532]</b></td><td><b>[-3.532 -3.102]</b></td><td>...</td><td><b>[2.916 3.346]</b></td><td><b>[3.346 3.776]</b></td><td><b>[3.776 4.206]</b></td></tr>
+<tr><td><b>a</b></td><td>29                    </td><td>131                   </td><td>456                   </td><td>...</td><td>631                 </td><td>163                 </td><td>77.7                </td></tr>
 </tbody>
 </table>
 
 
 
 
 ```python
@@ -268,16 +268,16 @@
 ```
 
 
 
 
 <table>
 <tbody>
-<tr><td><b>x</b></td><td><b>[-4.377 -3.93 ]</b></td><td><b>[-3.93  -3.483]</b></td><td><b>[-3.483 -3.036]</b></td><td>...</td><td><b>[3.225 3.672]</b></td><td><b>[3.672 4.12 ]</b></td><td><b>[4.12  4.567]</b></td></tr>
-<tr><td><b></b> </td><td>30.8                  </td><td>119                   </td><td>686                   </td><td>...</td><td>357                 </td><td>75.6                </td><td>20.6                </td></tr>
+<tr><td><b>x</b></td><td><b>[-4.392 -3.962]</b></td><td><b>[-3.962 -3.532]</b></td><td><b>[-3.532 -3.102]</b></td><td>...</td><td><b>[2.916 3.346]</b></td><td><b>[3.346 3.776]</b></td><td><b>[3.776 4.206]</b></td></tr>
+<tr><td><b></b> </td><td>29                    </td><td>131                   </td><td>456                   </td><td>...</td><td>631                 </td><td>163                 </td><td>77.7                </td></tr>
 </tbody>
 </table>
 
 
 
 
 ```python
@@ -339,14 +339,26 @@
 
 
     
 ![png](https://raw.githubusercontent.com/philippeller/dama/master/README_files/README_39_0.png)
     
 
 
+### Saving and loading
+
+Dama supports the pickle protocol, and objects can be stored like:
+```python
+dm.save("filename.pkl", obj)
+```
+
+And read back like:
+```python
+obj = dm.read("filename.pkl")
+```
+
 # Example gallery
 
 This is just to illustrate some different, seemingly random applications, resulting in various plots. All starting from some random data points
 
 
 ```python
 from matplotlib import pyplot as plt
@@ -378,34 +390,34 @@
 p.histogram(x=100, y=100).counts.median_filter(10).plot(ax=ax[7])
 
 # Third row
 p.binwise(x=100).quantile(q=[0.1, 0.3, 0.5, 0.7, 0.9]).y.plot_bands(ax=ax[8])
 p.binwise(x=100).quantile(q=[0.1, 0.3, 0.5, 0.7, 0.9]).y.gaussian_filter((2.5,0)).interp(x=500).plot_bands(filled=False, lines=True, linestyles=[':', '--', '-'],ax=ax[9])
 p.binwise(a=100).mean().y.plot(ax=ax[10])
 p.binwise(a=100).std().y.plot(ax=ax[10])
+p.histogram(x=100, y=100).counts.std(axis='x').plot(ax=ax[11])
 
 # Fourth row
-p.histogram(x=100, y=100).counts.std(axis='x').plot(ax=ax[11])
 np.log(p.histogram(x=100, y=100).counts + 1).gaussian_filter(0.5).plot_contour(cmap=dm.cm.passion_r, ax=ax[12])
 p.histogram(x=30, y=30).gaussian_filter(1).lookup(p).plot_scatter('x', 'y', 'a', 1, cmap='Spectral', ax=ax[13])
 h = p.histogram(y=100, x=np.logspace(-1,0,100)).a.T
 h[h>0].plot(ax=ax[14])
 h[1/3:2/3].plot(ax=ax[15])
 ```
 
 
 
 
-    <matplotlib.collections.QuadMesh at 0x7efbe96989a0>
+    <matplotlib.collections.QuadMesh at 0x7f8a0315d1f0>
 
 
 
 
     
-![png](https://raw.githubusercontent.com/philippeller/dama/master/README_files/README_43_1.png)
+![png](https://raw.githubusercontent.com/philippeller/dama/master/README_files/README_44_1.png)
     
 
 
 
 ```python
 
 ```
```

#### html2text {}

```diff
@@ -52,44 +52,44 @@
 (0,3*np.pi, 30) > y = np.linspace(0,2*np.pi, 20) > > xx, yy = np.meshgrid(x, y)
 > a = np.sin(xx) * np.cos(yy) > > import matplotlib.pyplot as plt > > x_widths
 = np.diff(x) > x_pixel_boundaries = np.concatenate([[x[0] - 0.5*x_widths[0]], x
 [:-1] + 0.5*x_widths, [x[-1] + 0.5*x_widths[-1]]]) > y_widths = np.diff(y) >
 y_pixel_boundaries = np.concatenate([[y[0] - 0.5*y_widths[0]], y[:-1] +
 0.5*y_widths, [y[-1] + 0.5*y_widths[-1]]]) > > pc = plt.pcolormesh
 (x_pixel_boundaries, y_pixel_boundaries, a) > plt.gca().set_xlabel('x') >
-plt.gca().set_ylabel('y') > cb = plt.colorbar(pc) > cb.set_label('a') ``` and
+plt.gca().set_ylabel('y') > cb = plt.colorbar(pc) > cb.set_label('a') > ``` and
 for doing the interpolation: > ``` > from scipy.interpolate import griddata > >
 interp_x = np.linspace(0,3*np.pi, 200) > interp_y = np.linspace(0,2*np.pi, 200)
 > > grid_x, grid_y = np.meshgrid(interp_x, interp_y) > > points = np.vstack(
-[xx.flatten(), yy.flatten()]).T > values = a.flatten() > >interp_a = griddata
-(points, values, (grid_x, grid_y), method='cubic') ``` ### PointData Another
+[xx.flatten(), yy.flatten()]).T > values = a.flatten() > > interp_a = griddata
+(points, values, (grid_x, grid_y), method='cubic') > ``` ### PointData Another
 representation of data is `PointData`, which is not any different of a
 dictionary holding same-length nd-arrays or a pandas `DataFrame` (And can
 actually be instantiated with those). ```python p = dm.PointData() p.x =
 np.random.randn(100_000) p.a = np.random.rand(p.size) * p.x**2 ``` ```python p
 ```
-x 1.73 -0.484 0.0993  ... 0.226  -0.0637 0.378
-a 0.14 0.105  0.00459 ... 0.0174 0.00351 0.00574
+x 0.0341  0.212 0.517 ... 1.27 0.827 1.57
+a 0.00106 0.035 0.18  ... 1.59 0.246 0.201
 ```python p.plot() ``` ![png](https://raw.githubusercontent.com/philippeller/
 dama/master/README_files/README_23_0.png) Maybe a correlation plot would be
 more insightful: ```python p.plot('x', 'a', '.'); ``` ![png](https://
 raw.githubusercontent.com/philippeller/dama/master/README_files/
 README_25_0.png) This can now seamlessly be translated into `Griddata`, for
 example taking the data binwise in `x` in 20 bins, and in each bin summing up
 points: ```python p.binwise(x=20).sum() ```
-x [-4.377 -3.93 [-3.93 - [-3.483 - ... [3.225 3.672] [3.672 4.12 ] [4.12 4.567]
-  ]             3.483]   3.036]
-a 30.8          119      686       ... 357           75.6          20.6
+x [-4.392 - [-3.962 - [-3.532 - ... [2.916 3.346] [3.346 3.776] [3.776 4.206]
+  3.962]    3.532]    3.102]
+a 29        131       456       ... 631           163           77.7
 ```python p.binwise(x=20).sum().plot(); ``` ![png](https://
 raw.githubusercontent.com/philippeller/dama/master/README_files/
 README_28_0.png) This is equivalent of making a weighted histogram, while the
 latter is faster. ```python p.histogram(x=20).a ```
-x [-4.377 -3.93 [-3.93 - [-3.483 - ... [3.225 3.672] [3.672 4.12 ] [4.12 4.567]
-  ]             3.483]   3.036]
-  30.8          119      686       ... 357           75.6          20.6
+x [-4.392 - [-3.962 - [-3.532 - ... [2.916 3.346] [3.346 3.776] [3.776 4.206]
+  3.962]    3.532]    3.102]
+  29        131       456       ... 631           163           77.7
 ```python np.allclose(p.histogram(x=10).a, p.binwise(x=10).sum().a) ``` True
 There is also KDE in n-dimensions available, for example: ```python p.kde
 (x=1000).a.plot(); ``` ![png](https://raw.githubusercontent.com/philippeller/
 dama/master/README_files/README_33_0.png) `GridArrays` can also hold multi-
 dimensional values, like RGB images or here 5 values from the percentile
 function. Let's plot those as bands: ```python p.binwise(x=20).quantile(q=[0.1,
 0.3, 0.5, 0.7, 0.9]).plot_bands() ``` ![png](https://raw.githubusercontent.com/
@@ -100,33 +100,35 @@
 filled=True, linestyles=[':', '--', '-'], lw=1) ``` ![png](https://
 raw.githubusercontent.com/philippeller/dama/master/README_files/
 README_37_0.png) This is not the same as using edges as in the example below,
 hence also the plots look different. ```python p.binwise(x=dm.Edges(np.linspace
 (-3,3,10))).quantile(q=[0.1, 0.3, 0.5, 0.7, 0.9]).plot_bands(lines=True,
 filled=True, linestyles=[':', '--', '-'], lw=1) ``` ![png](https://
 raw.githubusercontent.com/philippeller/dama/master/README_files/
-README_39_0.png) # Example gallery This is just to illustrate some different,
-seemingly random applications, resulting in various plots. All starting from
-some random data points ```python from matplotlib import pyplot as plt ```
-```python p = dm.PointData() p.x = np.random.rand(10_000) p.y = np.random.randn
-(p.size) * np.sin(p.x*3*np.pi) * p.x p.a = p.y/p.x ``` ```python fig, ax =
-plt.subplots(4,4,figsize=(20,20)) ax = ax.flatten() # First row p.y.plot(ax=ax
-[0]) p.plot('x', 'y', '.', ax=ax[1]) p.plot_scatter('x', 'y', c='a', s=1,
-cmap=dm.cm.spectrum, ax=ax[2]) p.interp(x=100, y=100, method="nearest").a.plot
-(ax=ax[3]) # Second row np.log(1 + p.histogram(x=100, y=100).counts).plot(ax=ax
-[4]) p.kde(x=100, y=100, bw=(0.02, 0.05)).density.plot
-(cmap=dm.cm.afterburner_r, ax=ax[5]) p.histogram(x=10, y=10).interp
-(x=100,y=100).a.plot(cmap="RdBu", ax=ax[6]) p.histogram(x=100,
+README_39_0.png) ### Saving and loading Dama supports the pickle protocol, and
+objects can be stored like: ```python dm.save("filename.pkl", obj) ``` And read
+back like: ```python obj = dm.read("filename.pkl") ``` # Example gallery This
+is just to illustrate some different, seemingly random applications, resulting
+in various plots. All starting from some random data points ```python from
+matplotlib import pyplot as plt ``` ```python p = dm.PointData() p.x =
+np.random.rand(10_000) p.y = np.random.randn(p.size) * np.sin(p.x*3*np.pi) *
+p.x p.a = p.y/p.x ``` ```python fig, ax = plt.subplots(4,4,figsize=(20,20)) ax
+= ax.flatten() # First row p.y.plot(ax=ax[0]) p.plot('x', 'y', '.', ax=ax[1])
+p.plot_scatter('x', 'y', c='a', s=1, cmap=dm.cm.spectrum, ax=ax[2]) p.interp
+(x=100, y=100, method="nearest").a.plot(ax=ax[3]) # Second row np.log(1 +
+p.histogram(x=100, y=100).counts).plot(ax=ax[4]) p.kde(x=100, y=100, bw=(0.02,
+0.05)).density.plot(cmap=dm.cm.afterburner_r, ax=ax[5]) p.histogram(x=10,
+y=10).interp(x=100,y=100).a.plot(cmap="RdBu", ax=ax[6]) p.histogram(x=100,
 y=100).counts.median_filter(10).plot(ax=ax[7]) # Third row p.binwise
 (x=100).quantile(q=[0.1, 0.3, 0.5, 0.7, 0.9]).y.plot_bands(ax=ax[8]) p.binwise
 (x=100).quantile(q=[0.1, 0.3, 0.5, 0.7, 0.9]).y.gaussian_filter((2.5,0)).interp
 (x=500).plot_bands(filled=False, lines=True, linestyles=[':', '--', '-'],ax=ax
 [9]) p.binwise(a=100).mean().y.plot(ax=ax[10]) p.binwise(a=100).std().y.plot
-(ax=ax[10]) # Fourth row p.histogram(x=100, y=100).counts.std(axis='x').plot
-(ax=ax[11]) np.log(p.histogram(x=100, y=100).counts + 1).gaussian_filter
+(ax=ax[10]) p.histogram(x=100, y=100).counts.std(axis='x').plot(ax=ax[11]) #
+Fourth row np.log(p.histogram(x=100, y=100).counts + 1).gaussian_filter
 (0.5).plot_contour(cmap=dm.cm.passion_r, ax=ax[12]) p.histogram(x=30,
 y=30).gaussian_filter(1).lookup(p).plot_scatter('x', 'y', 'a', 1,
 cmap='Spectral', ax=ax[13]) h = p.histogram(y=100, x=np.logspace(-1,0,100)).a.T
 h[h>0].plot(ax=ax[14]) h[1/3:2/3].plot(ax=ax[15]) ```
-collections.QuadMesh at 0x7efbe96989a0> ![png](https://
+collections.QuadMesh at 0x7f8a0315d1f0> ![png](https://
 raw.githubusercontent.com/philippeller/dama/master/README_files/
-README_43_1.png) ```python ```
+README_44_1.png) ```python ```
```

### Comparing `dama-0.4.6/dama/core/axis.py` & `dama-0.4.7/dama/core/axis.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/core/binneddata.py` & `dama-0.4.7/dama/core/binneddata.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,15 +194,23 @@
                 out_data[var] = output_map
 
         return out_data
 
     def apply_function(
         self, function, *args, fill_value=np.nan, return_len=None, **kwargs
         ):
-        '''apply function per bin'''
+        '''apply function per bin
+
+        function : callable
+        return_len : int (optional)
+            the shape (array length) of the `function` output. If None is passed, 
+            `return_len` is (tried to be) determined on the fly
+
+        if weights are passed as kwarg, they are interpreted as being a variable in the dataset
+        '''
 
         if self.indices is None:
             self.compute_indices()
 
         outputs = {}
         output_maps = {}
 
@@ -211,19 +219,23 @@
         for var in self.data.vars:
             source_data = self.data[var]
 
             if return_len is None:
                 # try to figure out return length of function
 
                 if source_data.ndim > 1:
+                    if weights is not None:
+                        kwargs['weights'] = self.data[weights][:3, [0] * (source_data.ndim - 1)]
                     test_value = function(
                         source_data[:3, [0] * (source_data.ndim - 1)], *args,
                         **kwargs
                         )
                 else:
+                    if weights is not None:
+                        kwargs['weights'] = self.data[weights][:3]
                     test_value = function(source_data[:3], *args, **kwargs)
                 if np.isscalar(test_value):
                     return_len = 1
                 else:
                     return_len = len(test_value)
 
             if source_data.ndim > 1:
```

### Comparing `dama-0.4.6/dama/core/edges.py` & `dama-0.4.7/dama/core/edges.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/core/grid.py` & `dama-0.4.7/dama/core/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import
 from numbers import Number
 from collections import OrderedDict
 from collections.abc import Iterable
+import copy
 
 import dama as dm
 
 import numpy as np
 
 __license__ = '''Copyright 2019 Philipp Eller
 
@@ -22,14 +23,17 @@
 limitations under the License.'''
 
 
 class Grid(object):
     '''
     Class to hold a number of axes
     '''
+
+    __slots__ = ['axes',]
+
     def __init__(self, *args, **kwargs):
         '''
         Paramters:
         ----------
         args : Axis or Grid object, or list thereof
 
         an axis can also be given by kwargs
@@ -40,14 +44,37 @@
 
         for d in args:
             self.add_axis(d)
 
         for k, v in kwargs.items():
             self[k] = v
 
+
+    def __getattr__(self, item):
+        try:
+            return self[item]
+        except Exception as e:
+            raise AttributeError from e
+
+    def __setattr__(self, item, value):
+        if item in self.__slots__:
+            object.__setattr__(self, item, value)
+        else:
+            self[item] = value
+
+    def __getstate__(self):
+        return self.axes
+
+    def __setstate__(self, state):
+        self.axes = state
+
+    def __deepcopy__(self, memo=None):
+        return dm.Grid(*copy.deepcopy(self.axes, memo=memo))
+
+
     def initialize(self, source=None):
         '''Method to initialize the grid if grid is not fully set up
         it derive information from source
         
         Parameters
         ----------
         source : dm.GridData, dm.PointData
@@ -251,17 +278,15 @@
     def __getitem__(self, item):
         '''
         item : int, str, slice, ierable
         '''
         if isinstance(item, str):
             # by name
             if not item in self.vars:
-                # if it does not exist, add empty axis: ToDo: really?
-                print('needs to be checked, is weird behaviour')
-                self.add_axis(item)
+                raise IndexError('Variable %s not present'%item)
             idx = self.vars.index(item)
             return self.axes[idx]
 
         elif isinstance(item, Number):
             return self[(item, )]
         elif isinstance(item, slice):
             return self[(item, )]
@@ -351,16 +376,16 @@
         return raveled_indices
 
 
 def test():
     a = Grid(var='a', edges=np.linspace(0, 1, 2))
     print(a)
     print(a.vars)
-    a['x'].edges = np.linspace(0, 10, 11)
-    a['y'].points = np.logspace(-1, 1, 20)
+    a.x = dm.Edges(np.linspace(0, 10, 11))
+    a.y = np.logspace(-1, 1, 20)
     print(a['x'].points)
     print(a['x'].edges)
     print(a['x', 'y'])
 
 
 if __name__ == '__main__':
     test()
```

### Comparing `dama-0.4.6/dama/core/gridarray.py` & `dama-0.4.7/dama/core/gridarray.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/core/griddata.py` & `dama-0.4.7/dama/core/griddata.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/core/pointarray.py` & `dama-0.4.7/dama/core/pointarray.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/core/pointdata.py` & `dama-0.4.7/dama/core/pointdata.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/plotting/stat_plot.py` & `dama-0.4.7/dama/plotting/stat_plot.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/histogram.py` & `dama-0.4.7/dama/translations/histogram.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/interpolation.py` & `dama-0.4.7/dama/translations/interpolation.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/kde.py` & `dama-0.4.7/dama/translations/kde.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/lookup.py` & `dama-0.4.7/dama/translations/lookup.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/ndimage.py` & `dama-0.4.7/dama/translations/ndimage.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/resample.py` & `dama-0.4.7/dama/translations/resample.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/translations/translation.py` & `dama-0.4.7/dama/translations/translation.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/utils/bind.py` & `dama-0.4.7/dama/utils/bind.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/utils/fileio.py` & `dama-0.4.7/dama/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/utils/formatter.py` & `dama-0.4.7/dama/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama/utils/stats.py` & `dama-0.4.7/dama/utils/stats.py`

 * *Files identical despite different names*

### Comparing `dama-0.4.6/dama.egg-info/SOURCES.txt` & `dama-0.4.7/dama.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 dama/__init__.py
 dama.egg-info/PKG-INFO
 dama.egg-info/SOURCES.txt
 dama.egg-info/dependency_links.txt
```

### Comparing `dama-0.4.6/setup.py` & `dama-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='dama',
-    version='0.4.6',
+    version='0.4.7',
     packages=find_packages(),
     license='Apache 2.0',
     author='Philipp Eller',
     author_email='peller.phys@gmail.com',
     url='https://github.com/philippeller/dama',
     description='Look at data in different ways',
     long_description=long_description,
```

