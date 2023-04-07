# Comparing `tmp/ga_vqc-0.0.48.tar.gz` & `tmp/ga_vqc-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga_vqc-0.0.48.tar", last modified: Wed Apr  5 00:22:59 2023, max compression
+gzip compressed data, was "ga_vqc-0.0.49.tar", last modified: Fri Apr  7 19:37:41 2023, max compression
```

## Comparing `ga_vqc-0.0.48.tar` & `ga_vqc-0.0.49.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-05 00:22:59.795414 ga_vqc-0.0.48/
--rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.48/LICENSE
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-05 00:22:59.795096 ga_vqc-0.0.48/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.48/README.md
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-05 00:22:59.793157 ga_vqc-0.0.48/ga_vqc/
--rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.48/ga_vqc/GA_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)      490 2023-03-23 02:52:56.000000 ga_vqc-0.0.48/ga_vqc/GA_Manager.py
--rw-r--r--   0 tsievert   (502) staff       (20)     1019 2023-03-23 02:52:56.000000 ga_vqc-0.0.48/ga_vqc/GA_Support.py
--rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.48/ga_vqc/VQC_ABC.py
--rw-r--r--   0 tsievert   (502) staff       (20)       41 2023-03-23 02:52:56.000000 ga_vqc-0.0.48/ga_vqc/__init__.py
--rw-r--r--   0 tsievert   (502) staff       (20)    22808 2023-04-05 00:19:53.000000 ga_vqc-0.0.48/ga_vqc/simple_ga.py
-drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-05 00:22:59.794731 ga_vqc-0.0.48/ga_vqc.egg-info/
--rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-05 00:22:59.000000 ga_vqc-0.0.48/ga_vqc.egg-info/PKG-INFO
--rw-r--r--   0 tsievert   (502) staff       (20)      291 2023-04-05 00:22:59.000000 ga_vqc-0.0.48/ga_vqc.egg-info/SOURCES.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-05 00:22:59.000000 ga_vqc-0.0.48/ga_vqc.egg-info/dependency_links.txt
--rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-05 00:22:59.000000 ga_vqc-0.0.48/ga_vqc.egg-info/requires.txt
--rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-05 00:22:59.000000 ga_vqc-0.0.48/ga_vqc.egg-info/top_level.txt
--rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-05 00:22:59.795506 ga_vqc-0.0.48/setup.cfg
--rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-05 00:22:33.000000 ga_vqc-0.0.48/setup.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-07 19:37:41.732835 ga_vqc-0.0.49/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1076 2023-02-08 00:23:26.000000 ga_vqc-0.0.49/LICENSE
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-07 19:37:41.732509 ga_vqc-0.0.49/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      791 2023-04-01 20:47:43.000000 ga_vqc-0.0.49/README.md
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-07 19:37:41.729937 ga_vqc-0.0.49/ga_vqc/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1743 2023-04-07 18:51:17.000000 ga_vqc-0.0.49/ga_vqc/Distance.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      495 2023-03-23 02:52:56.000000 ga_vqc-0.0.49/ga_vqc/GA_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      565 2023-04-07 18:02:50.000000 ga_vqc-0.0.49/ga_vqc/GA_Manager.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     1019 2023-03-23 02:52:56.000000 ga_vqc-0.0.49/ga_vqc/GA_Support.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     2598 2023-04-07 17:34:26.000000 ga_vqc-0.0.49/ga_vqc/Genes.py
+-rw-r--r--   0 tsievert   (502) staff       (20)      430 2023-03-23 02:52:56.000000 ga_vqc-0.0.49/ga_vqc/VQC_ABC.py
+-rw-r--r--   0 tsievert   (502) staff       (20)       69 2023-04-07 16:50:57.000000 ga_vqc-0.0.49/ga_vqc/__init__.py
+-rw-r--r--   0 tsievert   (502) staff       (20)     9420 2023-04-07 17:36:08.000000 ga_vqc-0.0.49/ga_vqc/simple_Individual.py
+-rw-r--r--   0 tsievert   (502) staff       (20)    16189 2023-04-07 19:37:03.000000 ga_vqc-0.0.49/ga_vqc/simple_Model.py
+drwxr-xr-x   0 tsievert   (502) staff       (20)        0 2023-04-07 19:37:41.732092 ga_vqc-0.0.49/ga_vqc.egg-info/
+-rw-r--r--   0 tsievert   (502) staff       (20)     1260 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/PKG-INFO
+-rw-r--r--   0 tsievert   (502) staff       (20)      357 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/SOURCES.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        1 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/dependency_links.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)      132 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/requires.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)        7 2023-04-07 19:37:41.000000 ga_vqc-0.0.49/ga_vqc.egg-info/top_level.txt
+-rw-r--r--   0 tsievert   (502) staff       (20)       38 2023-04-07 19:37:41.732931 ga_vqc-0.0.49/setup.cfg
+-rw-r--r--   0 tsievert   (502) staff       (20)     1067 2023-04-06 18:50:32.000000 ga_vqc-0.0.49/setup.py
```

### Comparing `ga_vqc-0.0.48/LICENSE` & `ga_vqc-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.48/PKG-INFO` & `ga_vqc-0.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga_vqc
-Version: 0.0.48
+Version: 0.0.49
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.48/README.md` & `ga_vqc-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.48/ga_vqc/GA_Support.py` & `ga_vqc-0.0.49/ga_vqc/GA_Support.py`

 * *Files identical despite different names*

### Comparing `ga_vqc-0.0.48/ga_vqc/simple_ga.py` & `ga_vqc-0.0.49/ga_vqc/simple_Model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,22 @@
 import copy
 import datetime
 import difflib
 import multiprocessing as mp
+import os
 import time
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pennylane as qml
 
-from .GA_ABC import GA_Individual, GA_Model
+from .Distance import euclidian_distances, tsne
+from .GA_ABC import GA_Model
 from .GA_Support import make_results_json
-
-
-class Individual(GA_Individual):
-    """
-    Data structure for the ansatz.
-    """
-
-    def __init__(self, n_qubits, n_moments, gates_arr, gates_probs, rng_seed):
-        """
-        Initializes the inidivual object, all individuals (ansatz) are members of this class.
-            - n_qubits: Number of qubits in the ansatz.
-            - n_moments: Number of moments in the ansatz.
-            - gates_arr: Number of possible states on a qubit.
-                Defined as 1 + n_undirected_gates + 2n_directed_gates.
-
-        TODO: change params to allow for multi-param gates
-        """
-        self.n_qubits = n_qubits
-        self.n_moments = n_moments
-        self.gates_arr = gates_arr
-        self.gates_probs = gates_probs
-        self.rng = np.random.default_rng(seed=rng_seed)
-
-        self.ansatz_dicts = []
-        self.ansatz_qml = []
-        self.ansatz_draw = []
-        self.params = []
-
-        self.generate()  # Should this be done automatically?
-        self.convert_to_qml()
-        self.draw_ansatz()
-
-    def __len__(self):
-        return len(self.ansatz_dicts[0])
-
-    def __getitem__(self, key):
-        if type(key) is tuple:
-            return self.ansatz_dicts[int(key[0])][int(key[1])]
-        else:
-            return self.ansatz_dicts[int(key)]
-
-    def __setitem__(self, key, value):
-        """
-        TODO: fix implementation (need to set whole moments?)
-        """
-        if type(key) is tuple:
-            self.ansatz_dicts[int(key[0])][int(key[1])] = value
-        else:
-            self.ansatz_dicts[int(key)] = value
-
-    def __str__(self):
-        return str(self.ansatz_dicts)
-
-    def __repr__(self):
-        return self.__str__()
-
-    def generate(self):
-        """
-        Generates the ansatz stochastically based on the other member variables.
-        """
-        for j in range(self.n_moments):
-            self.ansatz_dicts.append(dict.fromkeys(range(self.n_qubits), 0))
-            ix = self.rng.permutation(self.n_qubits)  # which qubit to pick first
-            for i in ix:
-                if self.ansatz_dicts[j][i] != 0:
-                    continue
-                k = self.rng.choice(self.gates_arr, p=self.gates_probs)
-
-                # if k.find('_') < 0:
-                if k[0] != "C":
-                    self.ansatz_dicts[j][i] = k
-                    continue
-
-                q_p_arr = self.rng.permutation(
-                    self.n_qubits
-                )  # qubit_pair_array for 2-qubit gates
-                for q_p in q_p_arr:
-                    if self.ansatz_dicts[j][q_p] != 0 or q_p == i:
-                        continue
-
-                    direction = self.rng.permutation(["_C", "_T"])
-                    self.ansatz_dicts[j][i] = k + direction[0] + f"-{q_p}"
-                    self.ansatz_dicts[j][q_p] = k + direction[1] + f"-{i}"
-                    break
-
-                if self.ansatz_dicts[j][i] == 0:
-                    self.ansatz_dicts[j][i] = self.rng.choice(self.gates_arr[:-1])
-
-    def convert_to_qml(self):
-        """
-        Converts the ansatz into a general format for the QML.
-
-            moment_dict example: **_C (_T) means current qubit is control (target) qubit of 2-qubit gate**
-                {'I': [],
-                 'RX': [],
-                 'RY': [],
-                 'RZ': [],
-                 'CNOT': []}
-        """
-        self.ansatz_qml = []
-        self.params = []
-        for j in range(len(self.ansatz_dicts)):
-            moment_dict = {i: list() for i in self.gates_arr}
-            stored_i = []
-            for i in range(self.n_qubits):
-                _ix = self.ansatz_dicts[j][i].find("_")
-                if _ix < 0:
-                    moment_dict[self.ansatz_dicts[j][i]].append(i)
-                else:
-                    if i in stored_i:
-                        continue
-                    _1ix = self.ansatz_dicts[j][i][_ix + 1]
-                    q_p = int(self.ansatz_dicts[j][i][-1])
-                    stored_i.append(q_p)
-                    if _1ix == "C":
-                        moment_dict[self.ansatz_dicts[j][i][:_ix]].append([i, int(q_p)])
-                    else:
-                        moment_dict[self.ansatz_dicts[j][i][:_ix]].append([int(q_p), i])
-
-            for k in moment_dict.keys():
-                if len(moment_dict[k]) == 0 or k == "I":  # add in identity gates?
-                    continue
-                if len(k) <= 2:
-                    self.ansatz_qml.append(
-                        f"qml.broadcast(qml.{k}, wires={moment_dict[k]}, pattern='single', parameters=params[{len(self.params)}:{len(self.params)+len(moment_dict[k])}])"
-                    )
-                    # change to allow for one-qubit gates with 0 or 2+ params
-                    for i in range(len(moment_dict[k])):
-                        self.params.append(0.0)
-                elif (
-                    len(k) > 2
-                ):  # Assumes the 2-qubit gates have no parameters, which is not generally true
-                    self.ansatz_qml.append(
-                        f"qml.broadcast(qml.{k}, wires={np.array(moment_dict[k]).flatten(order='C').tolist()}, pattern={moment_dict[k]})"
-                    )
-                    # change to allow for two-qubit gates with 1+ params
-
-    def ansatz_circuit(self, params, event=None):
-        for m in self.ansatz_qml:
-            # exec(m)
-            try:
-                exec(m)
-            except:
-                print(m)
-                raise Exception("oopsies there's a problem")
-        return qml.expval(qml.PauliZ(wires=[self.n_qubits - 1]))
-
-    def draw_ansatz(self):
-        self.ansatz_draw = []
-        full_ansatz_draw = qml.draw(
-            qml.QNode(
-                self.ansatz_circuit,
-                qml.device("default.qubit", wires=self.n_qubits, shots=1),
-            ),
-            decimals=None,
-            expansion_strategy="device",
-            show_all_wires=True,
-        )(self.params, event=[i for i in range(self.n_qubits)])[:-3]
-        indices = [i for i, c in enumerate(full_ansatz_draw) if c == ":"]
-        for _ in range(self.n_qubits):
-            self.ansatz_draw.append(full_ansatz_draw[: indices[1] - 2][3:-2])
-            full_ansatz_draw = full_ansatz_draw[indices[1] - 1 :]
-
-    def add_moment(self):
-        """
-        TODO: change to randomly generate new moment?
-        """
-        j = self.rng.integers(self.n_moments)
-        self.ansatz_dicts.append(copy.deepcopy(self.ansatz_dicts[j]))
-        self.n_moments += 1
+from .simple_Individual import Individual
 
 
 class Model(GA_Model):
     """
     Container for all the logic of the GA Model.
 
     TODO: change the I assignment to a random assignment. check for back-to-back CNOTs bc compile to I
@@ -196,16 +30,15 @@
         self.backend_type = config["backend_type"]
         self.vqc = config["vqc"]
         self.max_concurrent = config["max_concurrent"]
 
         self.n_qubits = config["n_qubits"]
         self.max_moments = config["max_moments"]
         self.add_moment_prob = config["add_moment_prob"]
-        self.gates_arr = config["gates_arr"]
-        self.gates_probs = config["gates_probs"]
+        self.genepool = config["genepool"]
         self.pop_size = config["pop_size"]
         self.init_pop_size = config["init_pop_size"]
         self.n_new_individuals = config["n_new_individuals"]
         self.n_winners = config["n_winners"]
         self.n_mutations = config["n_mutations"]
         self.n_mate_swaps = config["n_mate_swaps"]
         self.n_steps_patience = config["n_steps_patience"]
@@ -241,35 +74,35 @@
         """
         start_time = time.time()
         init_pop = []
         for _ in range(self.init_pop_size):
             init_pop.append(
                 Individual(
                     self.n_qubits,
-                    self.rng.integers(1, self.max_moments + 1),
-                    self.gates_arr,
-                    self.gates_probs,
+                    # self.rng.integers(1, self.max_moments + 1),
+                    self.max_moments,
+                    self.genepool,
                     self.rng_seed,
                 )
             )
 
         seq_mat = difflib.SequenceMatcher(isjunk=lambda x: x in " -")
-        compare_arr = ["" for i in range(self.n_qubits)]
+        compare_arr = ["" for qubit in range(self.n_qubits)]
         distances_arr = []
         selected_ixs = set()
         for _ in range(self.pop_size):
             distances = []
             for j, individual in enumerate(init_pop):
                 if j in selected_ixs:
                     distances.append(0)
                     continue
                 dist = 0.0
-                for i in range(self.n_qubits):
-                    seq_mat.set_seq2(compare_arr[i])
-                    seq_mat.set_seq1(individual.ansatz_draw[i])
+                for qubit in range(self.n_qubits):
+                    seq_mat.set_seq2(compare_arr[qubit])
+                    seq_mat.set_seq1(individual.ansatz_draw[qubit])
                     dist += 1 - seq_mat.ratio()
                 distances.append(dist / self.n_qubits)
 
             distances_arr.append(np.array(distances))
             selected_ix = np.argmax(np.mean(distances_arr, axis=0))
             selected_ixs.add(selected_ix)
             self.population.append(init_pop[selected_ix])
@@ -292,15 +125,17 @@
 
             parents = self.select()
             self.mate(parents)
             self.immigrate()
             self.check_max_moments()
 
             print(
-                f"Best Fitness: {self.best_perf['fitness']}, Best ansatz: {self.best_perf['ansatz_dicts']}"
+                f"Best fitness: {self.best_perf['fitness']}, " + 
+                f"Best metrics: {self.best_perf['eval_metrics']}, " +
+                f"Best ansatz: {self.best_perf['ansatz_dicts']}"
             )
 
             if step > 20:
                 if (step - self.best_perf["generation"]) > self.n_steps_patience:
                     break
             make_results_json(results, self.start_time, self.ga_output_path, step)
             step += 1
@@ -322,15 +157,15 @@
         args_arr = []
         for ansatz in self.population:
             ansatz.convert_to_qml()
             ansatz.draw_ansatz()
             vqc_config_ansatz = {key: value for key, value in self.vqc_config.items()}
             vqc_config_ansatz["ansatz_dicts"] = ansatz.ansatz_dicts
             vqc_config_ansatz["ansatz_qml"] = ansatz.ansatz_qml
-            vqc_config_ansatz["params"] = ansatz.params
+            vqc_config_ansatz["n_params"] = ansatz.n_params
             vqc_config_ansatz["ix"] = ix
             vqc_config_ansatz["gen"] = gen
             args_arr.append(copy.deepcopy(vqc_config_ansatz))
             ix += 1
 
         start_time = time.time()
         output_arr = []
@@ -342,15 +177,15 @@
                         args_arr[
                             i * self.max_concurrent : (i + 1) * self.max_concurrent
                         ],
                     )
                 )
         for i in range(len(output_arr)):
             # Both the fitness metrics and eval_metrics must be JSON serializable -> (ie. 
-            # default python classes or have custom serialization)
+            #  default python classes or have custom serialization)
             self.fitness_arr[i] = output_arr[i]["fitness_metric"]
             self.metrics_arr[i] = output_arr[i]["eval_metrics"]
         end_time = time.time()
         exec_time = end_time - start_time
         print(f"QML Optimization in {exec_time:.2f} seconds")
 
         if self.best_perf["fitness"] < np.amax(self.fitness_arr):
@@ -365,25 +200,56 @@
             self.best_perf["ansatz_draw"] = copy.deepcopy(
                 self.population[np.argmax(self.fitness_arr)].ansatz_draw
             )
             self.best_perf["generation"] = gen
             self.best_perf["index"] = np.argmax(self.fitness_arr).item()
 
     def make_results(self):
+
+        distances_from_best = euclidian_distances(self.best_perf["ansatz_dicts"], self.population)
+        destdir_curves = os.path.join(self.ga_output_path, "ga_curves")
+        if not os.path.exists(destdir_curves):
+            os.makedirs(destdir_curves)
+        filepath_euclid = os.path.join(
+            destdir_curves,
+            "%03deuclid_distance-%d_data.png"
+            % (self.best_perf["generation"], self.start_time),
+        )
+        plt.figure(0)
+        plt.style.use("seaborn")
+        plt.scatter(distances_from_best, self.fitness_arr, marker=".", color="g")
+        plt.ylabel("Fitness")
+        plt.xlabel("Euclidian distance from best ansatz")
+        plt.savefig(filepath_euclid, format="png")
+        # data_tsne = tsne(self.population)
+        # filepath_tsne = os.path.join(
+        #     destdir_curves,
+        #     "%03dtsne_distance-%d_data.png"
+        #     % (self.best_perf["generation"], self.start_time),
+        # )
+        # plt.figure(0)
+        # plt.style.use("seaborn")
+        # plt.scatter([i[0] for i in data_tsne.T], [i[1] for i in data_tsne.T], marker=".", cmap=)
+        # plt.ylabel("a.u.")
+        # plt.xlabel("a.u.")
+        # plt.savefig(filepath_tsne, format="png")
+
         results = {
             "full_population": [i.ansatz_dicts for i in self.population],
             "full_drawn_population": [i.ansatz_draw for i in self.population],
             "full_fitness": self.fitness_arr,
             "fitness_stats": f"Avg fitness: {np.mean(self.fitness_arr)}, Std. Dev: {np.std(self.fitness_arr)}",
             "full_eval_metrics": self.metrics_arr,
             "eval_metrics_stats": [
                 f"Avg {k}: {np.mean([i[k] for i in self.metrics_arr])}, "
                 + f"Std. Dev: {np.std([i[k] for i in self.metrics_arr])}"
                 for k in self.metrics_arr[0].keys()
             ],
+            "full_distances": distances_from_best,
+            "distances_stats": f"Avg distance: {np.mean(distances_from_best)}, Std. Dev: {np.std(distances_from_best)}",
             "best_ansatz": self.best_perf["ansatz_dicts"],
             "best_drawn_ansatz": self.best_perf["ansatz_draw"],
             "best_fitness": self.best_perf["fitness"],
             "best_eval_metrics": self.best_perf["eval_metrics"],
             "best_fitness_gen": self.best_perf["generation"],
             "best_fitness_ix": self.best_perf["index"],
         }
@@ -476,17 +342,17 @@
             #             break
             #         swap_set.add(i0_new)
             #     qubit_A, qubit_B = i0_new, i1_new
 
             #     if qubit_A < 0 or qubit_B < 0:
             #         break
 
-            # for i in swap_set:
-            #     children[0][moment_A, i] = parents[swap_ix[1]][moment_B, i]
-            #     children[1][moment_B, i] = parents[swap_ix[0]][moment_A, i]
+            # for qubit in swap_set:
+            #     children[0][moment_A, qubit] = parents[swap_ix[1]][moment_B, qubit]
+            #     children[1][moment_B, qubit] = parents[swap_ix[0]][moment_A, qubit]
 
             # print(f"Post-mateswap ansatz: {children}")
             # ADDED IN FOR MOMENT SWAP
             # children["child_A"][moment_A] = parents[swap_ix[1]][moment_B]
             # children["child_B"][moment_B] = parents[swap_ix[0]][moment_A]
             children[0][moment_A] = parents[swap_ix[1]][moment_B]
             children[1][moment_B] = parents[swap_ix[0]][moment_A]
@@ -511,75 +377,37 @@
         TODO: add in functionality to add or remove moments from an ansatz
 
         Variables
             j: selected moment
             i: selected qubit
             k: selected gate
         """
-        # print(f"Pre-mutate ansatz: {ansatz}")
         for _ in range(self.n_mutations):
-            double_swap_flag = 0
             if (
                 ansatz.n_moments < self.max_moments
                 and self.rng.random() < self.add_moment_prob
             ):
-                ansatz.add_moment()
-            j = self.rng.integers(ansatz.n_moments)
-            i = self.rng.integers(self.n_qubits)
-            k = self.rng.choice(self.gates_arr, p=self.gates_probs)
-
-            if ansatz[j][i].find("_") > 0:
-                double_swap_flag += 1
-                k_p = self.rng.choice(self.gates_arr[:-1])
-                ansatz[j][int(ansatz[j][i][-1])] = k_p
-
-            # if k.find('_') < 0:
-            if k[0] != "C":
-                ansatz[j][i] = k
-            else:
-                q_p_arr = self.rng.permutation(self.n_qubits)
-                for q_p in q_p_arr:
-                    if q_p == i:
-                        continue
-                    if ansatz[j][q_p].find("_") > 0:
-                        double_swap_flag += 1
-                        k_pp = self.rng.choice(self.gates_arr, p=self.gates_probs)
-                        if double_swap_flag == 2 and k_pp[0] == "C":
-                            direction = self.rng.permutation(["_C", "_T"])
-                            ansatz[j][int(ansatz[j][i][-1])] = (
-                                k + direction[0] + f"-{int(ansatz[j][q_p][-1])}"
-                            )
-                            ansatz[j][int(ansatz[j][q_p][-1])] = (
-                                k + direction[1] + f"-{int(ansatz[j][i][-1])}"
-                            )
-                        else:
-                            ansatz[j][int(ansatz[j][q_p][-1])] = self.rng.choice(
-                                self.gates_arr[:-1]
-                            )
-
-                    direction = self.rng.permutation(["_C", "_T"])
-                    ansatz[j][i] = k + direction[0] + f"-{q_p}"
-                    ansatz[j][q_p] = k + direction[1] + f"-{i}"
-                    break
-
-        # print(f"Post-mutate ansatz: {ansatz}")
+                ansatz.add_moment(method='duplicate')
+            
+            moment = self.rng.integers(ansatz.n_moments)
+            qubit = self.rng.integers(self.n_qubits)
+            ansatz.mutate(moment, qubit)
 
         self.population.append(ansatz)
 
     def immigrate(self):
         """
         Adds in new individuals with every generation, in order to keep up the overall population diversity.
         """
         for _ in range(self.n_new_individuals):
             self.population.append(
                 Individual(
                     self.n_qubits,
                     self.rng.integers(1, self.max_moments + 1),
-                    self.gates_arr,
-                    self.gates_probs,
+                    self.genepool,
                     self.rng_seed,
                 )
             )
 
     def check_max_moments(self):
         """
         Checks if many of the ansatz are 'full' with respect to max_moments, and if so it raises the ceiling
```

### Comparing `ga_vqc-0.0.48/ga_vqc.egg-info/PKG-INFO` & `ga_vqc-0.0.49/ga_vqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-vqc
-Version: 0.0.48
+Version: 0.0.49
 Summary: Genetic Algorithm for VQC ansatz search.
 Home-page: https://github.com/tcoulvert/GA_Ansatz_Search
 Author: Thomas Sievert
 Author-email: 63161166+tcoulvert@users.noreply.github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ga_vqc-0.0.48/setup.py` & `ga_vqc-0.0.49/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ga_vqc",
-    version="0.0.48",
+    version="0.0.49",
     description="Genetic Algorithm for VQC ansatz search.",
     packages=find_packages(include=["ga_vqc"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

