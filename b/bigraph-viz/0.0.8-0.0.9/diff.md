# Comparing `tmp/bigraph-viz-0.0.8.tar.gz` & `tmp/bigraph-viz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-viz-0.0.8.tar", last modified: Wed Mar 29 21:27:04 2023, max compression
+gzip compressed data, was "bigraph-viz-0.0.9.tar", last modified: Thu Mar 30 17:54:53 2023, max compression
```

## Comparing `bigraph-viz-0.0.8.tar` & `bigraph-viz-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-03-29 21:27:04.729787 bigraph-viz-0.0.8/
--rw-r--r--   0 eranagmon   (502) staff       (20)     1057 2023-03-29 14:52:00.000000 bigraph-viz-0.0.8/LICENSE.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)     1429 2023-03-29 21:27:04.729670 bigraph-viz-0.0.8/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)      468 2023-03-29 21:24:47.000000 bigraph-viz-0.0.8/README.md
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-03-29 21:27:04.728954 bigraph-viz-0.0.8/bigraph_viz.egg-info/
--rw-r--r--   0 eranagmon   (502) staff       (20)     1429 2023-03-29 21:27:04.000000 bigraph-viz-0.0.8/bigraph_viz.egg-info/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)      271 2023-03-29 21:27:04.000000 bigraph-viz-0.0.8/bigraph_viz.egg-info/SOURCES.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-03-29 21:27:04.000000 bigraph-viz-0.0.8/bigraph_viz.egg-info/dependency_links.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        9 2023-03-29 21:27:04.000000 bigraph-viz-0.0.8/bigraph_viz.egg-info/requires.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)       11 2023-03-29 21:27:04.000000 bigraph-viz-0.0.8/bigraph_viz.egg-info/top_level.txt
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-03-29 21:27:04.729371 bigraph-viz-0.0.8/bigraphviz/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2023-03-29 14:52:00.000000 bigraph-viz-0.0.8/bigraphviz/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1632 2023-03-29 14:52:00.000000 bigraph-viz-0.0.8/bigraphviz/dict_utils.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    10901 2023-03-29 21:13:13.000000 bigraph-viz-0.0.8/bigraphviz/plot.py
--rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-03-29 21:27:04.729830 bigraph-viz-0.0.8/setup.cfg
--rw-r--r--   0 eranagmon   (502) staff       (20)     1563 2023-03-29 21:26:39.000000 bigraph-viz-0.0.8/setup.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-03-30 17:54:53.255249 bigraph-viz-0.0.9/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1057 2023-03-29 14:52:00.000000 bigraph-viz-0.0.9/LICENSE.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1639 2023-03-30 17:54:53.255120 bigraph-viz-0.0.9/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)      614 2023-03-30 15:24:11.000000 bigraph-viz-0.0.9/README.md
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-03-30 17:54:53.254319 bigraph-viz-0.0.9/bigraph_viz.egg-info/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1639 2023-03-30 17:54:53.000000 bigraph-viz-0.0.9/bigraph_viz.egg-info/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)      271 2023-03-30 17:54:53.000000 bigraph-viz-0.0.9/bigraph_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-03-30 17:54:53.000000 bigraph-viz-0.0.9/bigraph_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        9 2023-03-30 17:54:53.000000 bigraph-viz-0.0.9/bigraph_viz.egg-info/requires.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)       11 2023-03-30 17:54:53.000000 bigraph-viz-0.0.9/bigraph_viz.egg-info/top_level.txt
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-03-30 17:54:53.254805 bigraph-viz-0.0.9/bigraphviz/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2023-03-29 14:52:00.000000 bigraph-viz-0.0.9/bigraphviz/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1632 2023-03-30 13:45:04.000000 bigraph-viz-0.0.9/bigraphviz/dict_utils.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    13519 2023-03-30 14:32:38.000000 bigraph-viz-0.0.9/bigraphviz/plot.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-03-30 17:54:53.255292 bigraph-viz-0.0.9/setup.cfg
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1540 2023-03-30 17:54:37.000000 bigraph-viz-0.0.9/setup.py
```

### Comparing `bigraph-viz-0.0.8/LICENSE.txt` & `bigraph-viz-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigraph-viz-0.0.8/bigraphviz/dict_utils.py` & `bigraph-viz-0.0.9/bigraphviz/dict_utils.py`

 * *Files identical despite different names*

### Comparing `bigraph-viz-0.0.8/bigraphviz/plot.py` & `bigraph-viz-0.0.9/bigraphviz/plot.py`

 * *Files 27% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             # what kind of node?
             if '_wires' in child or '_ports' in child:
                 # this is a hyperedge/process
                 if path_here not in bigraph['hyper_edges']:
                     bigraph['hyper_edges'][path_here] = {}
                 if '_wires' in child:
                     for port, state_path in child['_wires'].items():
+                        if isinstance(state_path, str):
+                            state_path = [state_path]
+                        state_path.insert(0, '..')  # go up one to the same level as the process
                         bigraph['hyper_edges'][path_here][port] = state_path
 
                 # check for mismatch, there might be disconnected wires or mismatch with declared wires
                 wire_ports = []
                 if '_wires' in child:
                     wire_ports = child['_wires'].keys()
                 if '_ports' in child:
@@ -106,37 +109,17 @@
         plot_schema=False,
         port_labels=True,
         port_label_size='10pt',
         engine='dot',
         rankdir='TB',
         node_groups=None,
         invisible_edges=None,
+        remove_process_place_edges=False,
 ):
-    """
-    Args:
-        bigraph_network (bigraph schema):
-        graph_name:
-        size (str): the size of the output figure (example: '16,10')
-        plot_schema (bool): turn on schema text in nodes
-        port_labels (bool): turn on port labels
-        port_label_size (str): the font size of the port labels (example: '10pt')
-        engine (str): graphviz graphing engine. Try 'dot' or 'neato'
-        rankdir (str): sets direction of graph layout. 'TB'=top-to-bottom, 'LR'=left-to-right
-        node_groups (list): a list of lists of nodes.
-            Each sub-list is a grouping of nodes that will be aligned at the same rank.
-            For example: [[('path to', 'group1 node1',), ('path to', 'group1 node2',)], [another group]]
-        invisible_edges (list): a list of edge tuples. The edge tuples have the (source, target) node
-            according to the nodes's paths. For example: [(('top',), ('top', 'inner1')), (another edge)]
-    Returns:
-        A graphviz digraph
-
-    Notes:
-        You can adjust node labels using HTML syntax for fonts, colors, sizes, subscript, superscript. For example:
-            H<sub><font point-size="8">2</font></sub>O will print H2O with 2 as a subscript with smaller font
-    """
+    """make a graphviz figure from a bigraph_network"""
     node_groups = node_groups or []
     invisible_edges = invisible_edges or []
     node_names = []
 
     # initialize graph
     graph = graphviz.Digraph(graph_name, engine=engine)
     graph.attr(size=size, overlap='false')
@@ -179,17 +162,19 @@
         if len(node_path) == 1 and multilayer:
             # the top node gets a double circle
             graph.node(node_name, label=label, peripheries='2')
         else:
             graph.node(node_name, label=label)
 
     # process nodes
+    process_paths = []
     graph.attr('node', shape='box', penwidth='2', constraint='false')
     for node in bigraph_network['process_nodes']:
         node_path = node['path']
+        process_paths.append(node_path)
         node_name = str(node_path)
         node_names.append(node_name)
 
         # make the label
         label = node_path[-1]
         label = label.replace(' ', '<br/>')  # replace spaces with new lines
         label = f'<{label}>'
@@ -204,18 +189,26 @@
             graph.node(node_name, label=label, peripheries='2')
         else:
             graph.node(node_name, label=label)
 
     # place edges
     graph.attr('edge', arrowhead='none', penwidth='2')
     for edge in bigraph_network['place_edges']:
+
+        # show edge or not
+        show_edge = True
+        if remove_process_place_edges and edge[1] in process_paths:
+            show_edge = False
         if edge in invisible_edges:
-            graph.attr('edge', style='invis')
-        else:
+            show_edge = False
+        if show_edge:
             graph.attr('edge', style='filled')
+        else:
+            graph.attr('edge', style='invis')
+
         node_name1 = str(edge[0])
         node_name2 = str(edge[1])
         graph.edge(node_name1, node_name2)
 
     # hyper edges
     graph.attr('edge', style='dashed', penwidth='1', arrowhead='dot', arrowsize='0.5')
     for node_path, wires in bigraph_network['hyper_edges'].items():
@@ -268,35 +261,133 @@
                     print(f'node {node_name} not in graph')
 
     return graph
 
 
 def plot_bigraph(
         bigraph_schema,
-        settings=None,
-        filename=None
+        graph_name='bigraph',
+        size='16,10',
+        node_label_size='12pt',
+        plot_schema=False,
+        port_labels=True,
+        port_label_size='10pt',
+        engine='dot',
+        rankdir='TB',
+        node_groups=None,
+        invisible_edges=None,
+        remove_process_place_edges=False,
+        view=None,
+        print_source=None,
+        file_format='png',
+        out_dir=None,
+        filename=None,
 ):
-    """ plot a bigraph from bigraph schema
+    """ Plot a bigraph from bigraph schema
+
+    Args:
+        graph_name:
+        size (str): the size of the output figure (example: '16,10')
+        plot_schema (bool): turn on schema text in nodes
+        port_labels (bool): turn on port labels
+        port_label_size (str): the font size of the port labels (example: '10pt')
+        engine (str): graphviz graphing engine. Try 'dot' or 'neato'
+        rankdir (str): sets direction of graph layout. 'TB'=top-to-bottom, 'LR'=left-to-right
+        node_groups (list): a list of lists of nodes.
+            Each sub-list is a grouping of nodes that will be aligned at the same rank.
+            For example: [[('path to', 'group1 node1',), ('path to', 'group1 node2',)], [another group]]
+        invisible_edges (list): a list of edge tuples. The edge tuples have the (source, target) node
+            according to the nodes' paths. For example: [(('top',), ('top', 'inner1')), (another edge)]
+        remove_process_place_edges (bool): turn off process place edges from plotting
 
+    Notes:
+        You can adjust node labels using HTML syntax for fonts, colors, sizes, subscript, superscript. For example:
+            H<sub><font point-size="8">2</font></sub>O will print H2O with 2 as a subscript with smaller font
     """
-    settings = copy.deepcopy(settings) or {}
-    view = settings.pop('view', None)
-    print_source = settings.pop('print_source', None)
-    file_format = settings.pop('file_format', 'png')
-    out_dir = settings.pop('out_dir', None)
-    filename = filename or settings.pop('filename', None)
+
+    # get kwargs dict and remove plotting-specific kwargs
+    kwargs = locals()
+    bigraph_schema = kwargs.pop('bigraph_schema')
+    view = kwargs.pop('view')
+    print_source = kwargs.pop('print_source')
+    file_format = kwargs.pop('file_format')
+    out_dir = kwargs.pop('out_dir')
+    filename = kwargs.pop('filename')
 
     # get the nodes and edges from the composite
     bigraph_network = get_bigraph_network(bigraph_schema)
 
     # make graphviz network
-    graph = get_graphviz_graph(bigraph_network, **settings)
+    graph = get_graphviz_graph(bigraph_network, **kwargs)
+
+    # display or save results
     if view:
         graph.view()
     if print_source:
         print(graph.source)
     if out_dir is not None:
         os.makedirs(out_dir, exist_ok=True)
         fig_path = os.path.join(out_dir, filename)
         print(f"Writing {fig_path}")
         graph.render(filename=fig_path, format=file_format)
     return graph
+
+
+def test_bigraphviz():
+    plot_settings = {'plot_schema': True, 'out_dir': 'out'}
+
+    # simple store
+    simple_store_spec = {
+        'store1': {
+            '_value': 1.0,
+            '_type': 'float',
+        },
+    }
+    plot_bigraph(simple_store_spec, **plot_settings, filename='simple_store')
+
+    # composite
+    composite_spec = {
+        'store1': {
+            'store1.1': {
+                '_value': 1.1,
+                '_type': 'float'
+            },
+            'store1.2': {
+                '_value': 2,
+                '_type': 'int'
+            },
+            'process1': {
+                '_ports': {
+                    'port1': {'_type': 'type'},
+                    'port2': {'_type': 'type'},
+                },
+                '_wires': {
+                    'port1': 'store1.1',
+                    'port2': 'store1.2',
+                }
+            },
+        },
+        'process3': {
+            '_wires': {
+                'port1': 'store1'
+            }
+        }  # TODO -- wires without ports should not work.
+    }
+    plot_bigraph(composite_spec, **plot_settings, filename='nested_composite', remove_process_place_edges=True)
+
+    # disconnected processes
+    process_schema = {
+        '_ports': {
+            'port1': {'_type': 'type'},
+            'port2': {'_type': 'type'}
+        }
+    }
+    process_spec = {
+        'process1': process_schema,
+        'process2': process_schema,
+        'process3': process_schema,
+    }
+    plot_bigraph(process_spec, **plot_settings, rankdir='BT', filename='disconnected_processes')
+
+
+if __name__ == '__main__':
+    test_bigraphviz()
```

### Comparing `bigraph-viz-0.0.8/setup.py` & `bigraph-viz-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 
 with open("README.md", "r") as readme:
-    long_description = readme.read()
-    # # Patch the relative links to absolute URLs that will work on PyPI.
-    # description2 = re.sub(
-    #     r']\(([\w/.-]+\.png)\)',
-    #     r'](https://github.com/vivarium-collective/bigraph-viz/raw/main/\1)',
-    #     description)
-    # long_description = re.sub(
-    #     r']\(([\w/.-]+)\)',
-    #     r'](https://github.com/vivarium-collective/bigraph-viz/blob/main/\1)',
-    #     description2)
+    description = readme.read()
+    # Patch the relative links to absolute URLs that will work on PyPI.
+    description2 = re.sub(
+        r']\(([\w/.-]+\.png)\)',
+        r'](https://github.com/vivarium-collective/bigraph-viz/raw/main/\1)',
+        description)
+    long_description = re.sub(
+        r']\(([\w/.-]+)\)',
+        r'](https://github.com/vivarium-collective/bigraph-viz/blob/main/\1)',
+        description2)
 
 setup(
     name="bigraph-viz",
     version=VERSION,
     author="Eran Agmon",
     author_email="agmon.eran@gmail.com",
     description="A graphviz-based plotting tool for compositional bigraph schema",
```

