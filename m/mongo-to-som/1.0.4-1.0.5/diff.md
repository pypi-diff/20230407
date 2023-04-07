# Comparing `tmp/mongo_to_som-1.0.4.tar.gz` & `tmp/mongo_to_som-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_to_som-1.0.4.tar", last modified: Fri Apr  7 14:26:40 2023, max compression
+gzip compressed data, was "mongo_to_som-1.0.5.tar", last modified: Fri Apr  7 15:56:42 2023, max compression
```

## Comparing `mongo_to_som-1.0.4.tar` & `mongo_to_som-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 14:26:40.466751 mongo_to_som-1.0.4/
--rw-rw-rw-   0        0        0     1143 2023-04-07 14:26:40.465750 mongo_to_som-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-07 12:24:07.000000 mongo_to_som-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 14:26:40.064751 mongo_to_som-1.0.4/mongo_to_som/
--rw-rw-rw-   0        0        0       49 2023-04-07 14:06:43.000000 mongo_to_som-1.0.4/mongo_to_som/__init__.py
--rw-rw-rw-   0        0        0     7405 2023-04-07 12:10:25.000000 mongo_to_som-1.0.4/mongo_to_som/mongotosom.py
-drwxrwxrwx   0        0        0        0 2023-04-07 14:26:40.463749 mongo_to_som-1.0.4/mongo_to_som.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-04-07 14:26:39.000000 mongo_to_som-1.0.4/mongo_to_som.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-07 14:26:39.000000 mongo_to_som-1.0.4/mongo_to_som.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 14:26:39.000000 mongo_to_som-1.0.4/mongo_to_som.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-07 14:26:39.000000 mongo_to_som-1.0.4/mongo_to_som.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-07 14:26:39.000000 mongo_to_som-1.0.4/mongo_to_som.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 14:26:40.466751 mongo_to_som-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1428 2023-04-07 14:26:04.000000 mongo_to_som-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:56:42.505564 mongo_to_som-1.0.5/
+-rw-rw-rw-   0        0        0     1143 2023-04-07 15:56:42.505564 mongo_to_som-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-07 12:24:07.000000 mongo_to_som-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 15:56:42.499561 mongo_to_som-1.0.5/mongo_to_som/
+-rw-rw-rw-   0        0        0       49 2023-04-07 14:06:43.000000 mongo_to_som-1.0.5/mongo_to_som/__init__.py
+-rw-rw-rw-   0        0        0     7505 2023-04-07 15:50:16.000000 mongo_to_som-1.0.5/mongo_to_som/mongotosom.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:56:42.503561 mongo_to_som-1.0.5/mongo_to_som.egg-info/
+-rw-rw-rw-   0        0        0     1143 2023-04-07 15:56:42.000000 mongo_to_som-1.0.5/mongo_to_som.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-07 15:56:42.000000 mongo_to_som-1.0.5/mongo_to_som.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 15:56:42.000000 mongo_to_som-1.0.5/mongo_to_som.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-07 15:56:42.000000 mongo_to_som-1.0.5/mongo_to_som.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-07 15:56:42.000000 mongo_to_som-1.0.5/mongo_to_som.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 15:56:42.505564 mongo_to_som-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2023-04-07 15:56:34.000000 mongo_to_som-1.0.5/setup.py
```

### Comparing `mongo_to_som-1.0.4/PKG-INFO` & `mongo_to_som-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_to_som
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to create Self-Organizing Map from MongoDB collection
 Home-page: UNKNOWN
 Author: Tomáš Peregrín
 Author-email: djtoso@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mongo_to_som-1.0.4/mongo_to_som/mongotosom.py` & `mongo_to_som-1.0.5/mongo_to_som/mongotosom.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,50 +74,50 @@
     # main function
 
     train_x_norm = self.minmax_scaler(train_x)  # normalisation
 
     # initialising self-organising map
     num_dims = train_x_norm.shape[1]  # numnber of dimensions in the input data
     np.random.seed(40)
-    som = np.random.random_sample(size=(num_rows, num_cols, num_dims))  # map construction
+    som = np.random.random_sample(size=(self.num_rows, self.num_cols, num_dims))  # map construction
 
     # start training iterations
     for step in range(max_steps):
       if (step + 1) % 1000 == 0:
         print("Iteration: ", step + 1)  # print out the current iteration for every 1k
       learning_rate, neighbourhood_range = self.decay(step, max_steps, max_learning_rate, self.max_m_distance)
 
       t = np.random.randint(0, high=train_x_norm.shape[0])  # random index of traing data
       winner = self.winning_neuron(train_x_norm, t, som, self.num_rows, self.num_cols)
-      for row in range(num_rows):
-        for col in range(num_cols):
+      for row in range(self.num_rows):
+        for col in range(self.num_cols):
           if self.m_distance([row, col], winner) <= neighbourhood_range:
             som[row][col] += learning_rate * (train_x_norm[t] - som[row][col])  # update neighbour's weight
 
     print("SOM training completed")
 
     # collecting labels
 
     label_data = train_y
-    map = np.empty(shape=(num_rows, num_cols), dtype=object)
+    map = np.empty(shape=(self.num_rows, self.num_cols), dtype=object)
 
-    for row in range(num_rows):
-      for col in range(num_cols):
+    for row in range(self.num_rows):
+      for col in range(self.num_cols):
         map[row][col] = []  # empty list to store the label
 
     for t in range(train_x_norm.shape[0]):
       if (t + 1) % 1000 == 0:
         print("sample data: ", t + 1)
-      winner = self.winning_neuron(train_x_norm, t, som, num_rows, num_cols)
+      winner = self.winning_neuron(train_x_norm, t, som, self.num_rows, self.num_cols)
       map[winner[0]][winner[1]].append(label_data[t])  # label of winning neuron
 
     # construct label map
-    label_map = np.zeros(shape=(num_rows, num_cols), dtype=np.int64)
-    for row in range(num_rows):
-      for col in range(num_cols):
+    label_map = np.zeros(shape=(self.num_rows, self.num_cols), dtype=np.int64)
+    for row in range(self.num_rows):
+      for col in range(self.num_cols):
         label_list = map[row][col]
         if len(label_list) == 0:
           label = 2
         else:
           label = max(label_list, key=label_list.count)
         label_map[row][col] = label
 
@@ -125,15 +125,15 @@
     cmap = colors.ListedColormap(['tab:green', 'tab:red', 'tab:orange'])
     plt.imshow(label_map, cmap=cmap)
     plt.colorbar()
     plt.title(title)
     plt.show()
 
     # reshape SOM into 3D array
-    som_3d = som.reshape(num_rows * num_cols, num_dims)
+    som_3d = som.reshape(self.num_rows * self.num_cols, num_dims)
 
     # create 3D scatter plot
     fig = plt.figure()
     ax = fig.add_subplot(111, projection='3d')
     ax.scatter(som_3d[:, 0], som_3d[:, 1], som_3d[:, 2], c=label_map.flatten(), cmap='viridis')
     ax.set_xlabel('Feature 1')
     ax.set_ylabel('Feature 2')
@@ -145,21 +145,21 @@
     ax = fig.add_subplot(111, projection='3d')
     ax.scatter(som_3d[:, 0], som_3d[:, 1], som_3d[:, 2], c=label_map.flatten(), cmap='viridis')
     ax.set_xlabel('Feature 1')
     ax.set_ylabel('Feature 2')
     ax.set_zlabel('Feature 3')
 
     # add lines between neighboring nodes
-    for i in range(num_rows):
-      for j in range(num_cols):
-        if j < num_cols - 1:
+    for i in range(self.num_rows):
+      for j in range(self.num_cols):
+        if j < self.num_cols - 1:
           # add line between current node and its right neighbor
           ax.plot([som[i][j][0], som[i][j + 1][0]], [som[i][j][1], som[i][j + 1][1]], [som[i][j][2], som[i][j + 1][2]],
                   color='black', linewidth=0.5)
-        if i < num_rows - 1:
+        if i < self.num_rows - 1:
           # add line between current node and its bottom neighbor
           ax.plot([som[i][j][0], som[i + 1][j][0]], [som[i][j][1], som[i + 1][j][1]], [som[i][j][2], som[i + 1][j][2]],
                   color='black', linewidth=0.5)
 
     plt.show()
 
   # Data Normalisation
@@ -177,16 +177,16 @@
     return distance.cityblock(x, y)
 
   # Best Matching Unit search
   def winning_neuron(self, data, t, som, num_rows, num_cols):
     winner = [0, 0]
     shortest_distance = np.sqrt(data.shape[1])  # initialise with max distance
     input_data = data[t]
-    for row in range(self.num_rows):
-      for col in range(self.num_cols):
+    for row in range(num_rows):
+      for col in range(num_cols):
         distance = self.e_distance(som[row][col], data[t])
         if distance < shortest_distance:
           shortest_distance = distance
           winner = [row, col]
     return winner
 
   # Learning rate and neighbourhood range calculation
@@ -194,7 +194,8 @@
     coefficient = 1.0 - (np.float64(step) / self.max_steps)
     learning_rate = coefficient * max_learning_rate
     neighbourhood_range = ceil(coefficient * max_m_distance)
     return learning_rate, neighbourhood_range
 
 
 #mongo_to_som(10,10, int(1*10e3), 4, 0.5, 'localhost', 27017, "som_db", "sum_pms")
+print('A')
```

### Comparing `mongo_to_som-1.0.4/mongo_to_som.egg-info/PKG-INFO` & `mongo_to_som-1.0.5/mongo_to_som.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-to-som
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to create Self-Organizing Map from MongoDB collection
 Home-page: UNKNOWN
 Author: Tomáš Peregrín
 Author-email: djtoso@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mongo_to_som-1.0.4/setup.py` & `mongo_to_som-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="mongo_to_som",
     packages=["mongo_to_som"],
     include_package_data=True,
-    version='1.0.4',
+    version='1.0.5',
     description='Library to create Self-Organizing Map from MongoDB collection',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tomáš Peregrín',
     author_email="djtoso@gmail.com",
     license='MIT',
     classifiers=[
```

