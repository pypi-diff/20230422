# Comparing `tmp/syncdsgen-0.0.7.tar.gz` & `tmp/syncdsgen-0.0.8.tar.gz`

## Comparing `syncdsgen-0.0.7.tar` & `syncdsgen-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/requirements.txt
--rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/syncdsgen_demo.ipynb
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/.vscode/settings.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/SynCDsGen/__init__.py
--rwxr-xr-x   0        0        0    13261 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/SynCDsGen/syncdsgen.py
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/LICENCE
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/README.md
--rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/requirements.txt
+-rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/syncdsgen_demo.ipynb
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/.vscode/settings.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/SynCDsGen/__init__.py
+-rwxr-xr-x   0        0        0    16514 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/SynCDsGen/syncdsgen.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/LICENCE
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/README.md
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/PKG-INFO
```

### Comparing `syncdsgen-0.0.7/requirements.txt` & `syncdsgen-0.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.7/syncdsgen_demo.ipynb` & `syncdsgen-0.0.8/syncdsgen_demo.ipynb`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.7/SynCDsGen/syncdsgen.py` & `syncdsgen-0.0.8/SynCDsGen/syncdsgen.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,70 @@
         Initialize a new instance of SyncCDsGeneratorConf
 
         Args:
             bases (list): list of bases
             codons (list): list of codons
             start_codons (list): list of start codons
             stop_codons (list): list of stop codons
+            AAs (list): list of amino acids
+
+            translation_dict (dict): dictionary containing the rules of translation of the codons into amino acids
+                key: amino aicd
+                value: codons encoding the amino acid
+
+            transition_prob_t (squared 2D tensor of the same shape as the AAs list): transition probability table between the different amino acids
+                transition_prob_t[i][j] represents the probability that the amino acid at index i in
+                AAs is followed by the amino acid at index j in AAs
+
+            emission_prob_t (squared 2D tensor of shape(len(AAs), L), where L is the maximum length of values in the translation_dict): emission probability table
+                emission_prob_t[i][j] is the probability that the amino acid at index i in AAs is
+                encoded by the codon j in the list of values corresponding to that amino acid in the 
+                translation dict
+            
+            AAs_initial_prob_dist (1D numpy array): array containing the initial probability
+            distribution of the different amino acids
+                AAs_initial_prob_dist[i] is the probability that a sequence starts with the amino acid
+                at the index i in AAs
+            
+            codon_length (int): length of a codon
+            constraints_dict (dict): dictionary containing the constraints of emission of codons
+            based on the previously translated sequence
+                key: a regex pattern representing the form of the previously translated sequence
+                value: a dictionary giving the emission contraints for the concerned amino acids
+                    key: an amino acid (an element of AAs)
+                    value: a 1D array of length L giving the emission probability table of the key amino acid when the previously translated sequence matches the regex. 
+            
+            AAs_stop_prob_dist (1D numpy array): array containing the end probability distribution of 
+            the different amino acids.
+                AAs_stop_prob_dist[i] is the probability that a sequence ends with the amino acid at
+                the index i in AAs.
+
+            Example:
+                conf = SynCDsGen.SyncCDsGeneratorConf()
+
+                conf.bases = ['a', 'b', 'c']
+                conf.codons = ['aa', 'ab', 'ac', 'ba', 'ca', 'bb', 'bc', 'cb']
+                conf.start_codons = ['aa', 'ab']
+                conf.stop_codons = ['ac']
+                conf.AAs = ['A', 'B', 'C', 'D']
+                conf.translation_dict = {
+                    'A':  ['aa', 'ab'],
+                    'B': ['ac'],
+                    'C': ['ba', 'bc', 'cb'],
+                    'D': ['ca', 'bb']
+                }
+                conf.transition_prob_t = torch.Tensor([[0,  0, 1/2, 1/2],
+                                            [0, 0, 1/2, 1/2],
+                                            [0, 0, 1/2, 1/2],
+                                            [0, 0, 1/2, 1/2]])
+
+                conf.emission_prob_t = torch.Tensor([[1/2, 1/2, 0.0],
+                                        [1, 0.0, 0.0],
+                                        [0.6, 0.2, 0.2],
+                                        [0.7, 0.3, 0.0]])
         """
         self.bases = bases
         self.codons = codons
         self.start_codons = start_codons
         self.stop_codons = stop_codons
         self.AAs = AAs
         self.translation_dict = translation_dict
@@ -189,15 +245,15 @@
             observations = []
 
             #generate the first AA of the AA sequence from the start codons
             state, observation = self.generate_token(Position.START)
             hidden_states.append(state)
             observations.append(observation)
 
-            for k in torch.arange(1, length-2):
+            for k in torch.arange(1, length-1):
                 transition_p_t = self.generatorConf.transition_prob_t[state]
                 state = pyro.sample("x_{}_{}".format(j, k),
                                     pyro.distributions.Categorical(transition_p_t))
                 emission_p_t = self.generatorConf.emission_prob_t[state]
 
                 observation = pyro.sample("y_{}_{}".format(j, k),
                                           pyro.distributions.Categorical(emission_p_t))
@@ -247,15 +303,15 @@
             observations = []
 
             #generate the first AA of the AA sequence from the start codons
             state, observation = self.generate_token(Position.START)
             hidden_states.append(state)
             observations.append(observation)
 
-            for k in torch.arange(1, length-2):
+            for k in torch.arange(1, length-1):
                 transition_p_t = self.generatorConf.transition_prob_t[state]
                 state = pyro.sample("x_{}_{}".format(j, k),
                                     pyro.distributions.Categorical(transition_p_t))
                 
                 hidden_AAs_sequence = self.AA_indices_sequence_to_AA_sequence(hidden_states)
 
                 emission_p_t = self.generatorConf.emission_prob_t[state]
```

### Comparing `syncdsgen-0.0.7/LICENCE` & `syncdsgen-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.7/pyproject.toml` & `syncdsgen-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "syncdsgen"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Ramses TANANKEM", email="tanankemr@gmail.com" },
 ]
 description = "A package to generate synthetic coding sequences data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `syncdsgen-0.0.7/PKG-INFO` & `syncdsgen-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncdsgen
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to generate synthetic coding sequences data
 Project-URL: Homepage, https://github.com/wl-research/syncdsgen
 Author-email: Ramses TANANKEM <tanankemr@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

