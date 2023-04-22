# Comparing `tmp/scatterd-1.2.7.tar.gz` & `tmp/scatterd-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.2.7.tar", last modified: Fri Apr 21 15:58:34 2023, max compression
+gzip compressed data, was "scatterd-1.3.0.tar", last modified: Sat Apr 22 16:13:46 2023, max compression
```

## Comparing `scatterd-1.2.7.tar` & `scatterd-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:58:34.065308 scatterd-1.2.7/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.2.7/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4994 2023-04-21 15:58:34.066305 scatterd-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 15:58:34.060322 scatterd-1.2.7/scatterd/
--rw-rw-rw-   0        0        0     1570 2023-04-21 10:55:12.000000 scatterd-1.2.7/scatterd/__init__.py
--rw-rw-rw-   0        0        0     5627 2023-04-21 14:47:41.000000 scatterd-1.2.7/scatterd/examples.py
--rw-rw-rw-   0        0        0    19524 2023-04-21 15:49:04.000000 scatterd-1.2.7/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:58:34.065308 scatterd-1.2.7/scatterd.egg-info/
--rw-rw-rw-   0        0        0     4994 2023-04-21 15:58:33.000000 scatterd-1.2.7/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-21 15:58:33.000000 scatterd-1.2.7/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:58:33.000000 scatterd-1.2.7/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-21 15:58:33.000000 scatterd-1.2.7/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 15:58:33.000000 scatterd-1.2.7/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-04-21 15:58:34.067140 scatterd-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:13:46.905522 scatterd-1.3.0/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-04-22 16:13:46.905522 scatterd-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 16:13:46.896527 scatterd-1.3.0/scatterd/
+-rw-rw-rw-   0        0        0     1570 2023-04-22 16:12:59.000000 scatterd-1.3.0/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     6836 2023-04-22 15:54:10.000000 scatterd-1.3.0/scatterd/examples.py
+-rw-rw-rw-   0        0        0    20055 2023-04-22 16:09:15.000000 scatterd-1.3.0/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:13:46.904505 scatterd-1.3.0/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 16:13:46.000000 scatterd-1.3.0/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-04-22 16:13:46.911486 scatterd-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-04-21 11:44:02.000000 scatterd-1.3.0/setup.py
```

### Comparing `scatterd-1.2.7/LICENSE` & `scatterd-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.2.7/PKG-INFO` & `scatterd-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.2.7
+Version: 1.3.0
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.2.7.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.2.7 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.0 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.2.7.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.0.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.2.7/README.md` & `scatterd-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.2.7/scatterd/__init__.py` & `scatterd-1.3.0/scatterd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing, gradient_on_density_color
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.2.7'
+__version__ = '1.3.0'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
 Description
```

### Comparing `scatterd-1.2.7/scatterd/examples.py` & `scatterd-1.3.0/scatterd/examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 from scatterd import scatterd, import_example
 import numpy as np
 
 # %%
 
-# df = import_example()
-# scatterd(df['tsneX'], df['tsneY'], z=df['PC2'], labels=df['labx'], gradient='#FFFFFF', cmap='Set1')
-# scatterd(df['tsneX'], df['tsneY'], cmap='Set1')
-# scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], cmap='Set1')
+df = import_example()
+fig, ax = scatterd(df['tsneX'],
+                   df['tsneY'],
+                   labels=df['labx'],
+                   density=True,
+                   density_on_top=True,
+                   args_density={'alpha': 0.3},
+                   gradient='#FFFFFF',
+                   edgecolor='#FFFFFF',
+                   grid=True,
+                   fontweight='bold',
+                   fontsize=26,
+                   )
+
+# %%
+# Import example iris dataet
+from sklearn import datasets
+iris = datasets.load_iris()
+X = iris.data[:, :2]
+labels = iris.target
+
+# Load library
+from scatterd import scatterd
+
+# Scatter the results
+fig, ax = scatterd(X[:,0], X[:,1], s=250, grid=True)
+
 
 # %%import some data to play with
 from sklearn import datasets
 iris = datasets.load_iris()
 X = iris.data[:, :2]  # we only take the first two features.
 labels = iris.target
 
@@ -19,41 +42,61 @@
 c[0]=[0,0,0]
 c[1]=[0,0,0]
 s = (labels+1) * 200
 random_integers = np.random.randint(0, len(s), size=X.shape[0])
 alpha = np.random.rand(1, X.shape[0])[0][random_integers]
 
 # %%
+from scatterd import scatterd
+import matplotlib as mpl
+custom_cmap = mpl.colors.ListedColormap(['green', 'black', 'blue'])
 
+s = (labels+1) * 200
+random_integers = np.random.randint(0, len(s), size=X.shape[0])
+alpha = np.random.rand(1, X.shape[0])[0][random_integers]
+
+fig, ax = scatterd(X[:,0], X[:,1], labels=labels, marker=labels, gradient='#ffffff', edgecolor='#ffffff', s=s, density=True, alpha=1, cmap=custom_cmap, density_on_top=False)
+
+# %%
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, s=alpha*1000, alpha=alpha)
 
 # %%
 # s=np.random.randint(10, 500,len(labels))
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, marker=labels.astype(str), s=s, cmap='Set2', xlabel='xlabel', ylabel='ylabel', title='Title', fontsize=25, density=True, fontcolor=[0,0,0])
 fig, ax = scatterd(X[:,0], X[:,1], labels=labels, marker=labels, s=s, cmap='Set2', xlabel='xlabel', ylabel='ylabel', title='Title', fontsize=25, density=True, fontcolor=[0,0,0])
 
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, marker=np.repeat('X', X.shape[0]))
-fig, ax = scatterd(X[:,0], X[:,1], labels=labels, marker=labels, s=300)
+fig, ax = scatterd(X[:,0], X[:,1], labels=labels, marker=labels, s=300, grid=True)
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, marker=labels, s=300)
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, marker='s', visible=True)
 
 
 marker=labels.astype(str)
 marker[labels==0]='s'
 marker[labels==1]='o'
 marker[labels==2]='d'
 
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, marker=marker, visible=True)
 
+# %% Density 3d
+fig, ax = scatterd(X[:,0], X[:,1], z=X[:,1], c=[0,0,0], labels=labels, density=True)
+
 # %% Scatter
 
+# Dots foreground
+fig, ax = scatterd(X[:,0], X[:,1], c=[0,0,0], labels=None, verbose=4, visible=True,density=True)
+
+# Dots background
 fig, ax = scatterd(X[:,0], X[:,1], c=[0,0,0], labels=None, verbose=4, visible=False)
 scatterd(X[:,0], X[:,1], c=None, density=True, ax=ax)
 fig.set_visible(True)
 
+
+# %% Scatter
+
 fig, ax = scatterd(X[:,0], X[:,1], c=[1,0,0], labels=None, verbose=4)
 
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, c=[0,0,0], density=True)
 fig, ax = scatterd(X[:,0], X[:,1], labels=labels, c=[0,0,0], density=True, fontsize=28, legend=False, fontcolor='#000000')
 fig, ax = scatterd(X[:,0], X[:,1], labels=labels, c=[0,0,0], density=True, fontsize=28, legend=True, fontcolor='#000000')
 
 fig, ax = scatterd(X[:,0], X[:,1], labels=None, c=None, density=True)
```

### Comparing `scatterd-1.2.7/scatterd/scatterd.py` & `scatterd-1.3.0/scatterd/scatterd.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,29 @@
              y,
              z=None,
              s=150,
              c=[0,0.1,0.4],
              labels=None,
              marker='o',
              alpha=0.8,
-             edgecolor='#FFFFFF',
+             edgecolor='#000000',
              gradient=None,
              density=False,
+             density_on_top=False,
              norm=False,
              cmap='tab20c',
              figsize=(25, 15),
              dpi=100,
              legend=True,
-             ax=None,
              jitter=None,
              xlabel='x-axis', ylabel='y-axis', title='', fontsize=24, fontcolor=None, grid=False, fontweight='normal',
              args_density = {'cmap': 'Reds', 'fill': True, 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False},
              visible=True,
+             fig=None,
+             ax=None,
              verbose=3):
     """Make scaterplot.
 
     Parameters
     ----------
     x : numpy array
         1D Coordinates x-axis.
@@ -69,14 +71,17 @@
             * 'none': No patch boundary will be drawn.
             * '#FFFFFF' : A color or sequence of colors.
     gradient : String, (default: None)
         Hex color to make a lineair gradient for the scatterplot.
         '#FFFFFF'
     density : Bool (default: False)
         Include the kernel density in the scatter plot.
+    density_on_top : bool, (default: False)
+        True : The density is the highest layer.
+        False : The density is the lowest layer.
     xlabel : String, optional
         Xlabel. The default is None.
     ylabel : String, optional
         Ylabel. The default is None.
     title : String, optional
         Title of the figure. The default is None.
     fontsize : String, optional
@@ -125,48 +130,52 @@
     >>> # Import library
     >>> from scatterd import scatterd, import_example
     >>>
     >>> # Import example
     >>> df = import_example()
     >>>
     >>> # Simple scatter
-    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'])
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], edgecolor='#FFFFFF')
+    >>>
+    >>> # Scatter with labels
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'])
     >>>
     >>> # Scatter with labels
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'])
     >>>
     >>> # Scatter with gradient
-    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], gradient='#FFFFFF')
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], z=df['tsneY'], labels=df['labx'], gradient='#FFFFFF')
     >>>
     >>> # Change cmap
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], gradient='#FFFFFF', cmap='Set2')
     >>>
     >>> # Scatter with density
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True)
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=False, gradient='#FFFFFF', edgecolor='#FFFFFF')
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF', edgecolor='#FFFFFF')
+    >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF', c=None)
     >>>
     >>> # Scatter with density and gradient
     >>> fig, ax = scatterd(df['tsneX'], df['tsneY'], labels=df['labx'], density=True, gradient='#FFFFFF')
     >>>
 
     References
     -------
     * github: https://github.com/erdogant/scatterd
     * Documentation: https://erdogant.github.io/scatterd/
     * Colormap: https://matplotlib.org/examples/color/colormaps_reference.html
 
     """
-    fig = None
     if len(x)!=len(y): raise Exception('[scatterd] >Error: input parameter x should be the same size of y.')
-    # if s is None: raise Exception('[scatterd] >Error: input parameter s(ize) should have value >0.')
-    # if c is None: raise Exception('[scatterd] >Error: input parameter c(olors) can not be None.')
     if isinstance(c, str): raise Exception('[scatterd] >Error: input parameter c(olors) should be RGB of type tuple [0,0,0] .')
     if not isinstance(s, int) and len(s)!=len(x): raise Exception('[scatterd] >Error: input parameter s(ize) should be of same size of X.')
     if (z is not None) and len(x)!=len(z): raise Exception('[scatterd] >Error: input parameter z should be the same size of x and y.')
     if s is None: s=0
     if c is None: s, c = 0, [0, 0, 0]
+    zorder = None if density_on_top else 10
 
     # Defaults
     defaults_density = {'cmap': 'Reds', 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False, 'fill': True}
     args_density = {**defaults_density, **args_density}
 
     # Preprocessing
     X, labels = _preprocessing(x, y, z, labels, jitter, norm)
@@ -177,23 +186,21 @@
     # Set size
     s = set_size(X, s)
     # Set size
     alpha = set_alpha(X, alpha)
     # Set marker
     marker = set_marker(X, marker)
     # Bootup figure
-    fig, ax = init_figure(ax, z, dpi, figsize, visible)
-
+    fig, ax = init_figure(ax, z, dpi, figsize, visible, fig)
     # Set figure properties
     ax = _set_figure_properties(X, labels, fontcolor, fontsize, xlabel, ylabel, title, grid, fontweight, ax)
 
     # Add density as bottom layer to the scatterplot
     if density:
         ax = sns.kdeplot(x=X[:, 0], y=X[:, 1], ax=ax, **args_density)
-        # ax = sns.kdeplot(x=X[:, 0], y=X[:, 1], ax=ax, hue=labels, **args_density)
 
     # Scatter all at once
     if (labels is None) and isinstance(marker, str):
         if z is None:
             ax.scatter(X[:, 0], X[:, 1], c=c_rgb, s=s, edgecolor=edgecolor, marker=marker, alpha=alpha)
         else:
             ax.scatter(X[:, 0], X[:, 1], X[:, 2], s=s, c=c_rgb, edgecolor=edgecolor, marker=marker, alpha=alpha)
@@ -201,15 +208,15 @@
         uilabels = np.unique(labels)
         for label in uilabels:
             Iloc1 = label==labels
             # Extract the unique markers
             for m in np.unique(marker[Iloc1]):
                 Iloc2 = np.logical_and(Iloc1, m==marker)
                 if z is None:
-                    ax.scatter(X[Iloc2, 0], X[Iloc2, 1], c=c_rgb[Iloc2], s=s[Iloc2], edgecolor=edgecolor, marker=m, label=label, alpha=alpha[Iloc2])
+                    ax.scatter(X[Iloc2, 0], X[Iloc2, 1], c=c_rgb[Iloc2], s=s[Iloc2], edgecolor=edgecolor, marker=m, label=label, alpha=alpha[Iloc2], zorder=zorder)
                 else:
                     # Let op: alpha[Iloc2] geeft een foutmelding
                     ax.scatter(X[Iloc2, 0], X[Iloc2, 1], X[Iloc2, 2], s=s[Iloc2], c=c_rgb[Iloc2], edgecolor=edgecolor, marker=m, label=label, alpha=0.8)
 
     # Show legend (only if labels are present)
     if legend and labels is not None: ax.legend()
 
@@ -227,15 +234,15 @@
 
     # Plot labels
     if (labels is not None) and (fontcolor is not None):
         for uilabel in fontcolor.keys():
             # Compute median for better center compared to mean
             XYmean = np.median(X[labels==uilabel, :], axis=0)
             if X.shape[1]==2:
-                ax.text(XYmean[0], XYmean[1], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize})
+                ax.text(XYmean[0], XYmean[1], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize}, zorder=15)
             else:
                 ax.text(XYmean[0], XYmean[1], XYmean[2], str(uilabel), color=fontcolor.get(uilabel), fontdict={'weight': fontweight, 'size': fontsize})
 
     # Labels on axis
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     if title is not None: ax.set_title(title)
@@ -382,29 +389,32 @@
     else:
         raise Exception('[scatterd] >ERROR : fontcolor input is not correct.')
 
     return fontcolor
 
 
 def set_size(X, s):
+    """Set size."""
     if isinstance(s, (int, float)): s = np.repeat(s, X.shape[0])
     # Minimum size should be 0 (dots will not be showed)
     s = np.maximum(s, 0)
     return s
 
 
 def set_alpha(X, alpha):
+    """Set alpha."""
     if alpha is None: alpha=0.8
     if isinstance(alpha, (int, float)): alpha = np.repeat(alpha, X.shape[0])
     # Minimum size should be 0 (dots will not be showed)
     alpha = np.maximum(alpha, 0)
     return alpha
 
 
 def set_marker(X, marker):
+    """Set markers."""
     markers = np.array(['o', 'v', 's', 'p', '*', 'h', 'H', 'D', 'd', 'P', 'X', '.', '^', '>', '<', '8'])
     # markers_list = dict(zip(markers, np.arange(0,len(markers))))
     # In case single str
     if isinstance(marker, str) and np.isin(marker, markers):
         return np.repeat(marker, X.shape[0])
     # In case array of markers.
     if np.all(np.isin(marker, markers)) and len(marker)==X.shape[0]:
@@ -413,18 +423,18 @@
     if len(marker)==X.shape[0]:
         d = dict(zip(set(marker), range(len(set(marker)))))
         marker_num = [d[i] for i in marker]
         return markers[np.mod(marker_num, len(markers))]
     # Return
     return np.repeat('o', X.shape[0])
 
-def init_figure(ax, z, dpi, figsize, visible):
-    fig = None
+
+def init_figure(ax, z, dpi, figsize, visible, fig):
+    """Initialize figure."""
     if ax is None:
-        # fig, ax = plt.subplots(figsize=figsize)
         fig = plt.figure(figsize=figsize, dpi=dpi)
         if z is None:
             ax = fig.add_subplot()
         else:
             ax = fig.add_subplot(projection='3d')
 
     if fig is not None:
```

### Comparing `scatterd-1.2.7/scatterd.egg-info/PKG-INFO` & `scatterd-1.3.0/scatterd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.2.7
+Version: 1.3.0
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.2.7.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.3.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.2.7 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.3.0 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.2.7.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+archive/1.3.0.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
 (https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
 img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
 (https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
```

### Comparing `scatterd-1.2.7/setup.py` & `scatterd-1.3.0/setup.py`

 * *Files identical despite different names*

