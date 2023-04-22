# Comparing `tmp/featurewiz-0.2.7.tar.gz` & `tmp/featurewiz-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurewiz-0.2.7.tar", last modified: Thu Apr 20 12:58:59 2023, max compression
+gzip compressed data, was "featurewiz-0.2.8.tar", last modified: Sat Apr 22 13:35:20 2023, max compression
```

## Comparing `featurewiz-0.2.7.tar` & `featurewiz-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-20 12:58:59.866839 featurewiz-0.2.7/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    21535 2023-04-20 12:58:59.851224 featurewiz-0.2.7/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    19371 2023-04-20 12:49:35.000000 featurewiz-0.2.7/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-20 12:58:59.704046 featurewiz-0.2.7/featurewiz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)     3507 2022-11-01 12:53:37.000000 featurewiz-0.2.7/featurewiz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      387 2023-04-20 11:45:08.000000 featurewiz-0.2.7/featurewiz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18411 2022-08-20 11:53:32.000000 featurewiz-0.2.7/featurewiz/classify_method.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    32382 2022-02-22 01:41:19.000000 featurewiz-0.2.7/featurewiz/databunch.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     4414 2021-07-03 17:15:33.000000 featurewiz-0.2.7/featurewiz/encoders.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   166744 2023-04-20 12:23:33.000000 featurewiz-0.2.7/featurewiz/featurewiz.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    87877 2023-04-20 12:09:44.000000 featurewiz-0.2.7/featurewiz/ml_models.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   109387 2022-11-01 12:59:18.000000 featurewiz-0.2.7/featurewiz/my_encoders.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2584 2021-07-03 17:15:33.000000 featurewiz-0.2.7/featurewiz/settings.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    22089 2022-06-16 14:29:37.000000 featurewiz-0.2.7/featurewiz/stacking_models.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14954 2022-12-30 16:23:17.000000 featurewiz-0.2.7/featurewiz/sulov_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-20 12:58:59.835617 featurewiz-0.2.7/featurewiz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    21535 2023-04-20 12:58:58.000000 featurewiz-0.2.7/featurewiz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      468 2023-04-20 12:58:58.000000 featurewiz-0.2.7/featurewiz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-20 12:58:58.000000 featurewiz-0.2.7/featurewiz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      289 2023-04-20 12:58:58.000000 featurewiz-0.2.7/featurewiz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       11 2023-04-20 12:58:58.000000 featurewiz-0.2.7/featurewiz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-20 12:58:59.866839 featurewiz-0.2.7/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1274 2023-04-20 12:09:08.000000 featurewiz-0.2.7/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-22 13:35:20.364428 featurewiz-0.2.8/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    23066 2023-04-22 13:35:20.360425 featurewiz-0.2.8/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    20916 2023-04-22 13:32:42.000000 featurewiz-0.2.8/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-22 13:35:20.196425 featurewiz-0.2.8/featurewiz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     3507 2022-11-01 12:53:37.000000 featurewiz-0.2.8/featurewiz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      387 2023-04-22 12:50:23.000000 featurewiz-0.2.8/featurewiz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18411 2022-08-20 11:53:32.000000 featurewiz-0.2.8/featurewiz/classify_method.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    32382 2022-02-22 01:41:19.000000 featurewiz-0.2.8/featurewiz/databunch.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     4414 2021-07-03 17:15:33.000000 featurewiz-0.2.8/featurewiz/encoders.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   166794 2023-04-22 12:46:40.000000 featurewiz-0.2.8/featurewiz/featurewiz.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    87877 2023-04-20 12:09:44.000000 featurewiz-0.2.8/featurewiz/ml_models.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   109387 2022-11-01 12:59:18.000000 featurewiz-0.2.8/featurewiz/my_encoders.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     2584 2021-07-03 17:15:33.000000 featurewiz-0.2.8/featurewiz/settings.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    22089 2022-06-16 14:29:37.000000 featurewiz-0.2.8/featurewiz/stacking_models.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14954 2022-12-30 16:23:17.000000 featurewiz-0.2.8/featurewiz/sulov_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-22 13:35:20.331426 featurewiz-0.2.8/featurewiz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    23066 2023-04-22 13:35:19.000000 featurewiz-0.2.8/featurewiz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      468 2023-04-22 13:35:19.000000 featurewiz-0.2.8/featurewiz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-22 13:35:19.000000 featurewiz-0.2.8/featurewiz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      289 2023-04-22 13:35:19.000000 featurewiz-0.2.8/featurewiz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       11 2023-04-22 13:35:19.000000 featurewiz-0.2.8/featurewiz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-22 13:35:20.366429 featurewiz-0.2.8/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1274 2023-04-22 12:49:51.000000 featurewiz-0.2.8/setup.py
```

### Comparing `featurewiz-0.2.7/PKG-INFO` & `featurewiz-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,190 +1,165 @@
 Metadata-Version: 2.1
 Name: featurewiz
-Version: 0.2.7
+Version: 0.2.8
 Summary: Select Best Features from your data set - any size - now with XGBoost!
 Home-page: https://github.com/AutoViML/featurewiz
 Author: Ram Seshadri
 Author-email: rsesha2001@yahoo.com
 License: Apache License 2.0
 Description: # featurewiz
+        `featurewiz` is a powerful feature selection library that has a number of features that make it stand out from the competition, including:
+        <ol>
+        <li>It provides one of the best automatic feature selection algorithms (Minimum Redundancy Maximum Relevance (MRMR)) described by wikipedia as: <a href="https://en.wikipedia.org/wiki/Minimum_redundancy_feature_selection">"The MRMR selection has been found to be more powerful than the maximum relevance feature selection"</a> such as Boruta.</li>
+        <li>It selects the best number of un-correlated features that have maximum mutual information about the target without having to specify the number of features</li>
+        <li>It is fast and easy to use, and comes with a number of helpful features, such as a built-in categorical-to-numeric encoder and a powerful feature engineering module</li>
+        <li>It is well-documented, and it comes with a number of <a href="https://github.com/AutoViML/featurewiz/tree/main/examples">examples</a>.</li>
+        <li>It is actively maintained, and it is regularly updated with new features and bug fixes.</li>
+        </ol>
+        If you are looking for a single feature selection library, we would definitely recommend checking out featurewiz. It is a powerful tool that can help you to improve the performance of your machine learning models.
         
-        ![banner](featurewiz_logos.png)
-        
-        ##  Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
-        <a href="updates.md">Check out more latest updates from this page</a><br>
-        As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo), featurewiz is now available on conda-forge. You can try:<br>
-        
-        ```
-         conda install -c conda-forge featurewiz
-        ```
-        
-        ### If the above conda install fails, you can try installing featurewiz this way:
-        ##Step 1: Install featurewiz first<br>
-        
-        ```
-         !pip install featurewiz --ignore-installed --no-deps
-         !pip install xlrd --ignore-installed --no-deps 
-        ```
-        
-        ##Step 2: Next, install Pillow since Kaggle has an incompatible version. <br>
+        # Table of Contents
+        <ul>
+        <li><a href="#introduction">What is featurewiz</a></li>
+        <li><a href="#working">How it works</a></li>
+        <li><a href="#tips">Tips for using featurewiz</a></li>
+        <li><a href="#install">How to install featurewiz</a></li>
+        <li><a href="#usage">Usage</a></li>
+        <li><a href="#api">API</a></li>
+        <li><a href="#additional">Additional Tips</a></li>
+        <li><a href="#maintainers">Maintainers</a></li>
+        <li><a href="#contributing">Contributing</a></li>
+        <li><a href="#license">License</a></li>
+        <li><a href="#disclaimer">Disclaimer</a></li>
+        </ul>
+        <p>
         
-        ```
-         !pip install Pillow==9.0.0
-        ```
+        ![banner](featurewiz_logos.png)
         
-        ## What is featurewiz?
+        ## Introduction
         `featurewiz` a new python library for creating and selecting the best features in your data set fast!
         `featurewiz` can be used in one or two ways. Both are explained below.
         
-        ## 1.  Feature Engineering
+        ### 1.  Feature Engineering
         <p>The first step is not absolutely necessary but it can be used to create new features that may or may not be helpful (be careful with automated feature engineering tools!).<p>
         1. <b>Performing Feature Engineering</b>: One of the gaps in open source AutoML tools and especially Auto_ViML has been the lack of feature engineering capabilities that high powered competitions such as Kaggle required. The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables was difficult and sifting through those hundreds of new features to find best features was difficult and left only to "experts" or "professionals". featurewiz was created to help you in this endeavor.<br>
         <p>featurewiz now enables you to add hundreds of such features with a single line of code. Set the "feature_engg" flag to "interactions", "groupby" or "target" and featurewiz will select the best encoders for each of those options and create hundreds (perhaps thousands) of features in one go. Not only that, using the next step, featurewiz will sift through numerous such variables and find only the least correlated and most relevant features to your model. All in one step!.<br>
         
-        You must use this syntax for feature engg. Otherwise, featurewiz will give an error:
-        
-        ```
-        import featurewiz as FW
-        outputs = FW.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
-        		header=0, test_data='',feature_engg='', category_encoders='',
-        		dask_xgboost_flag=False, nrows=None)
-        ```
-        
         ![feature_engg](feature_engg.jpg)
         
-        ## 2.  Feature Selection
+        ### 2.  Feature Selection
         <p>The second step is Feature Selection. `featurewiz` uses the MRMR (Minimum Redundancy Maximum Relevance) algorithm as the basis for its feature selection. <br>
         <b> Why do Feature Selection</b>? Once you have created 100's of new features, you still have three questions left to answer:
         1. How do we interpret those newly created features?
         2. Which of these features is important and which are useless? How many of them are highly correlated to each other causing redundancy?
         3. Does the model overfit now on these new features and perform better or worse than before?
         <br>
         All are very important questions and featurewiz answers them by using the SULOV method and Recursive XGBoost to reduce features in your dataset to the best "minimum optimal" features for the model.<br>
         <p><b>SULOV</b>: SULOV stands for `Searching for Uncorrelated List of Variables`. The SULOV algorithm is based on the Minimum-Redundancy-Maximum-Relevance (MRMR) <a href="https://towardsdatascience.com/mrmr-explained-exactly-how-you-wished-someone-explained-to-you-9cf4ed27458b">algorithm explained in this article</a> as one of the best feature selection methods. To understand how MRMR works and how it is different from `Boruta` and other feature selection methods, see the chart below. Here "Minimal Optimal" refers to the MRMR and featurewiz kind of algorithms while "all-relevant" refers to Boruta kind of algorithms.<br>
         
         ![MRMR_chart](MRMR.png)
-        <br>
-        The working of the SULOV algorithm is as follows:
+        
+        ## Working
+        `featurewiz` performs feature selection in 2 steps. Each step is explained below.
+        <b>The working of the `SULOV` algorithm</b> is as follows:
         <ol>
-        <li>Find all the pairs of highly correlated variables exceeding a correlation threshold (say absolute(0.7)).
-        <li>Then find their MIS score (Mutual Information Score) to the target variable. MIS is a non-parametric scoring method. So its suitable for all kinds of variables and target.
-        <li>Now take each pair of correlated variables, then knock off the one with the lower MIS score.
-        <li>What’s left is the ones with the highest Information scores and least correlation with each other.
+        <li>Find all the pairs of highly correlated variables exceeding a correlation threshold (say absolute(0.7)).</li>
+        <li>Then find their MIS score (Mutual Information Score) to the target variable. MIS is a non-parametric scoring method. So its suitable for all kinds of variables and target.</li>
+        <li>Now take each pair of correlated variables, then knock off the one with the lower MIS score.</li>
+        <li>What’s left is the ones with the highest Information scores and least correlation with each other.</li>
         </ol>
         
         ![sulov](SULOV.jpg)
         
-        <b>Recursive XGBoost</b>: Once SULOV has selected variables that have high mutual information scores with least less correlation amongst them, we use XGBoost to repeatedly find best features among the remaining variables after SULOV. The Recursive XGBoost method is explained in this chart below.
-        Here is how it works:
+        <b>The working of the Recursive XGBoost</b> is as follows: 
+        Once SULOV has selected variables that have high mutual information scores with least less correlation amongst them, featurewiz uses XGBoost to repeatedly find the best features among the remaining variables after SULOV. 
         <ol>
-        <li>Select all variables in data set and the full data split into train and valid sets.
-        <li>Find top X features (could be 10) on train using valid for early stopping (to prevent over-fitting)
-        <li>Then take next set of vars and find top X
-        <li>Do this 5 times. Combine all selected features and de-duplicate them.
+        <li>Select all variables in data set and the full data split into train and valid sets.</li>
+        <li>Find top X features (could be 10) on train using valid for early stopping (to prevent over-fitting)</li>
+        <li>Then take next set of vars and find top X</li>
+        <li>Do this 5 times. Combine all selected features and de-duplicate them.</li>
         </ol>
         
         ![xgboost](xgboost.jpg)
         
-        <b>Building the simplest and most "interpretable" model</b>: featurewiz represents the "next best" step you must perform after doing feature engineering  since you might have added some highly correlated or even useless features when you use automated feature engineering. featurewiz ensures you have the least number of features needed to build a high performing or equivalent model.
-        
-        <b>A WORD OF CAUTION:</b> Just because you can engineer new features, doesn't mean you should always create tons of new features. You must make sure you understand what the new features stand for before you attempt to build a model with these (sometimes useless) features. featurewiz displays the SULOV chart which can show you how the 100's of newly created variables added to your dataset are highly correlated to each other and were removed. This will help you understand how feature selection works in featurewiz.
-        
-        ## Table of Contents
-        <ul>
-        <li><a href="#background">Background</a></li>
-        <li><a href="#install">Install</a></li>
-        <li><a href="#usage">Usage</a></li>
-        <li><a href="#api">API</a></li>
-        <li><a href="#maintainers">Maintainers</a></li>
-        <li><a href="#contributing">Contributing</a></li>
-        <li><a href="#license">License</a></li>
-        </ul>
-        
-        ## Background
-        
-        ![background](featurewiz_background.jpg)
-        
-        To learn more about how featurewiz works under the hood, watch this [video](https://www.youtube.com/embed/ZiNutwPcAU0)<br>
-        
-        <p>featurewiz was designed for selecting High Performance variables with the fewest steps.
-        
-        In most cases, featurewiz builds models with 20%-99% fewer features than your original data set with nearly the same or slightly lower performance (this is based on my trials. Your experience may vary).<br>
-        <p>
-        featurewiz is every Data Scientist's feature wizard that will:<ol>
-        <li><b>Automatically pre-process data</b>: you can send in your entire dataframe "as is" and featurewiz will classify and change/label encode categorical variables changes to help XGBoost processing. It classifies variables as numeric or categorical or NLP or date-time variables automatically so it can use them correctly to model.<br>
-        <li><b>Perform feature engineering automatically</b>: The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables is difficult and sifting through those hundreds of new features is painstaking and left only to "experts". Now, with featurewiz you can create hundreds or even thousands of new features with the click of a mouse. This is very helpful when you have a small number of features to start with. However, be careful with this option. You can very easily create a monster with this option.
-        <li><b>Perform feature reduction automatically</b>. When you have small data sets and you know your domain well, it is easy to perhaps do EDA and identify which variables are important. But when you have a very large data set with hundreds if not thousands of variables, selecting the best features from your model can mean the difference between a bloated and highly complex model or a simple model with the fewest and most information-rich features. featurewiz uses XGBoost repeatedly to perform feature selection. You must try it on your large data sets and compare!<br>
-        <li><b>Explain SULOV method graphically </b> using networkx library so you can see which variables are highly correlated to which ones and which of those have high or low mutual information scores automatically. Just set verbose = 2 to see the graph. <br>
-        <li><b>Build a fast LightGBM model </b> using the features selected by featurewiz. There is a function called "simple_lightgbm_model" which you can use to build a fast model. It is a new module, so check it out.<br>
-        </ol>
-        
-        <b>***  Notes of Gratitude ***</b>:<br>
+        ## Tips
+        Here are some additional tips for ML engineers and data scientists when using featurewiz:
         <ol>
-        <li><b>Alex Lekov</b> (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/automl_alex) for his DataBunch and encoders modules which are used by the tool (although with some modifications).</li>
-        <li><b>Category Encoders</b> library in Python : This is an amazing library. Make sure you read all about the encoders that featurewiz uses here: https://contrib.scikit-learn.org/category_encoders/index.html </li>
+        <li><b>Always cross-validate your results</b>: When you use a feature selection tool, it is important to cross-validate your results. This means that you should split your data into a training set and a test set. Use the training set to select features, and then evaluate your model on the test set. This will help you to ensure that your model is not overfitting to the training data.</li>
+        <li><b>Use multiple feature selection tools</b>: It is a good idea to use multiple feature selection tools and compare the results. This will help you to get a better understanding of which features are most important for your data.</li>
+        <li><b>Don't forget to engineer new features</b>: Feature selection is only one part of the process of building a good machine learning model. You should also spend time engineering your features to make them as informative as possible. This can involve things like creating new features, transforming existing features, and removing irrelevant features.</li>
+        <li><b>Don't overfit your model</b>: It is important to avoid overfitting your model to the training data. Overfitting occurs when your model learns the noise in the training data, rather than the underlying signal. To avoid overfitting, you can use regularization techniques, such as lasso or elasticnet.</li>
+        <li><b>Start with a small number of features</b>: When you are first starting out, it is a good idea to start with a small number of features. This will help you to avoid overfitting your model. As you become more experienced, you can experiment with adding more features.</li>
         </ol>
         
         ## Install
         
         **Prerequsites:**
         <ol>
         <li><b>featurewiz is built using xgboost, dask, numpy, pandas and matplotlib</b>. It should run on most Python 3 Anaconda installations. You won't have to import any special libraries other than "dask", "XGBoost" and "networkx" library. Optionally, it uses LightGBM for fast modeling, which it installs automatically. </li>
         <li><b>We use "networkx" library for charts and interpretability</b>. <br>But if you don't have these libraries, featurewiz will install those for you automatically.</li>
         </ol>
-        - [Anaconda](https://docs.anaconda.com/anaconda/install/)
-        
-        To clone featurewiz, it is better to create a new environment, and install the required dependencies:
-        
-        To install from PyPi:
-        
-        ```
-        conda create -n <your_env_name> python=3.7 anaconda
-        conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
-        pip install featurewiz --ignore-installed --no-deps
-        pip install lazytransform
-        or
-        pip install git+https://github.com/AutoViML/featurewiz.git
-        ```
-        
         To install from source:
         
         ```
         cd <featurewiz_Destination>
         git clone git@github.com:AutoViML/featurewiz.git
         # or download and unzip https://github.com/AutoViML/featurewiz/archive/master.zip
         conda create -n <your_env_name> python=3.7 anaconda
         conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
         cd featurewiz
         pip install -r requirements.txt
         ```
         
+        ##  Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
+        <a href="updates.md">Check out more latest updates from this page</a><br>
+        As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo), featurewiz is now available on conda-forge. You can try:<br>
+        
+        ```
+         conda install -c conda-forge featurewiz
+        ```
+        
+        ### If the above conda install fails, you can try installing featurewiz this way:
+        ##Step 1: Install featurewiz first<br>
+        
+        ```
+         !pip install featurewiz --ignore-installed --no-deps
+         !pip install xlrd --ignore-installed --no-deps 
+        ```
+        
+        ##Step 2: Next, install Pillow since Kaggle has an incompatible version. <br>
+        
+        ```
+         !pip install Pillow==9.0.0
+        ```
+        
         ## Usage
         
-        As of Jan 2022, you now invoke featurewiz in two ways for two different goals. For feature selection, you must use the scikit-learn compatible fit and predict transformer syntax such as below.
+        For feature selection, you must use the newer syntax which is similar to the scikit-learn fit and predict transformer syntax below.
         
         ```
         from featurewiz import FeatureWiz
-        features = FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='', dask_xgboost_flag=False, nrows=None, verbose=2)
-        X_train_selected = features.fit_transform(X_train, y_train)
-        X_test_selected = features.transform(X_test)
-        features.features  ### provides the list of selected features ###
+        fwiz = FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='', dask_xgboost_flag=False, nrows=None, verbose=2)
+        X_train_selected = fwiz.fit_transform(X_train, y_train)
+        X_test_selected = fwiz.transform(X_test)
+        ### get list of selected features ###
+        fwiz.features  
         ```
         
         Alternatively, you can use featurewiz for feature engineering using this older syntax. Otherwise, it will give an error. If you want to combine feature engg and then feature selection, you must use this older syntax:
         
         ```
-        import featurewiz as FW
-        outputs = FW.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
+        import featurewiz as fwiz
+        outputs = fwiz.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
         		header=0, test_data='',feature_engg='', category_encoders='',
         		dask_xgboost_flag=False, nrows=None)
         ```
         
         `outputs`: There will always be multiple objects in output. The objects in that tuple can vary:
-        1. "features" and "train": It be a list (of selected features) and one dataframe (if you sent in train only)
+        1. "features" and "trainm": It be a list (of selected features) and one dataframe (if you sent in train only)
         2. "trainm" and "testm": It can be two dataframes when you send in both test and train but with selected features.
         <ol>
         <li>Both the selected features and dataframes are ready for you to now to do further modeling.
         <li>Featurewiz works on any multi-class, multi-label data Set. So you can have as many target labels as you want.
         <li>You don't have to tell Featurewiz whether it is a Regression or Classification problem. It will decide that automatically.
         </ol>
         
@@ -224,23 +199,46 @@
             - `WOEEncoder`: WOEEncoder uses the Weight of Evidence technique for categorical features. It supports only one kind of target: binary. For polynomial target support, it uses a PolynomialWrapper. It cannot be used for Regression.
             - `JamesSteinEncoder`: JamesSteinEncoder uses the James-Stein estimator. It supports 2 kinds of targets: binary and continuous. For polynomial target support, it uses PolynomialWrapper.
             For feature value i, James-Stein estimator returns a weighted average of:
             The mean target value for the observed feature value i.
             The mean target value (regardless of the feature value).
             - `dask_xgboost_flag`: Default is False. Set to True to use dask_xgboost estimator. You can turn it off if it gives an error. Then it will use pandas and regular xgboost to do the job.
             - `nrows`: default `None`. You can set the number of rows to read from your datafile if it is too large to fit into either dask or pandas. But you won't have to if you use dask. 
-        **Return values**
+        
+        **Output values**
         -   `outputs`: Output is always a tuple. We can call our outputs in that tuple: out1 and out2.
             -   `out1` and `out2`: If you sent in just one dataframe or filename as input, you will get:
                 - 1. `features`: It will be a list (of selected features) and
                 - 2. `trainm`: It will be a dataframe (if you sent in a file or dataname as input)
             -   `out1` and `out2`: If you sent in two files or dataframes (train and test), you will get:
                 - 1. `trainm`: a modified train dataframe with engineered and selected features from dataname and
                 - 2. `testm`: a modified test dataframe with engineered and selected features from test_data.
         
+        ## Additional
+        
+        ![background](featurewiz_background.jpg)
+        
+        To learn more about how featurewiz works under the hood, watch this [video](https://www.youtube.com/embed/ZiNutwPcAU0)<br>
+        <p>featurewiz was designed for selecting High Performance variables with the fewest steps.
+        In most cases, featurewiz builds models with 20%-99% fewer features than your original data set with nearly the same or slightly lower performance (this is based on my trials. Your experience may vary).<br>
+        <p>
+        featurewiz is every Data Scientist's feature wizard that will:<ol>
+        <li><b>Automatically pre-process data</b>: you can send in your entire dataframe "as is" and featurewiz will classify and change/label encode categorical variables changes to help XGBoost processing. It classifies variables as numeric or categorical or NLP or date-time variables automatically so it can use them correctly to model.<br>
+        <li><b>Perform feature engineering automatically</b>: The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables is difficult and sifting through those hundreds of new features is painstaking and left only to "experts". Now, with featurewiz you can create hundreds or even thousands of new features with the click of a mouse. This is very helpful when you have a small number of features to start with. However, be careful with this option. You can very easily create a monster with this option.
+        <li><b>Perform feature reduction automatically</b>. When you have small data sets and you know your domain well, it is easy to perhaps do EDA and identify which variables are important. But when you have a very large data set with hundreds if not thousands of variables, selecting the best features from your model can mean the difference between a bloated and highly complex model or a simple model with the fewest and most information-rich features. featurewiz uses XGBoost repeatedly to perform feature selection. You must try it on your large data sets and compare!<br>
+        <li><b>Explain SULOV method graphically </b> using networkx library so you can see which variables are highly correlated to which ones and which of those have high or low mutual information scores automatically. Just set verbose = 2 to see the graph. <br>
+        <li><b>Build a fast XGBoost or LightGBM model using the features selected by featurewiz</b>. There is a function called "simple_lightgbm_model" which you can use to build a fast model. It is a new module, so check it out.<br>
+        </ol>
+        
+        <b>*** A Note of Gratitude ***</b>:<br>
+        <ol>
+        <li><b>Alex Lekov</b> (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/automl_alex) for his DataBunch and encoders modules which are used by the tool (although with some modifications).</li>
+        <li><b>Category Encoders</b> library in Python : This is an amazing library. Make sure you read all about the encoders that featurewiz uses here: https://contrib.scikit-learn.org/category_encoders/index.html </li>
+        </ol>
+        
         ## Maintainers
         
         * [@AutoViML](https://github.com/AutoViML)
         
         ## Contributing
         
         See [the contributing file](CONTRIBUTING.md)!
```

#### html2text {}

```diff
@@ -1,26 +1,44 @@
-Metadata-Version: 2.1 Name: featurewiz Version: 0.2.7 Summary: Select Best
+Metadata-Version: 2.1 Name: featurewiz Version: 0.2.8 Summary: Select Best
 Features from your data set - any size - now with XGBoost! Home-page: https://
 github.com/AutoViML/featurewiz Author: Ram Seshadri Author-email:
-rsesha2001@yahoo.com License: Apache License 2.0 Description: # featurewiz !
-[banner](featurewiz_logos.png) ## Good News: You can install featurewiz on
-Colab and Kaggle easily in 2 steps! Check_out_more_latest_updates_from_this
-page
-As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo),
-featurewiz is now available on conda-forge. You can try:
-``` conda install -c conda-forge featurewiz ``` ### If the above conda install
-fails, you can try installing featurewiz this way: ##Step 1: Install featurewiz
-first
-``` !pip install featurewiz --ignore-installed --no-deps !pip install xlrd --
-ignore-installed --no-deps ``` ##Step 2: Next, install Pillow since Kaggle has
-an incompatible version.
-``` !pip install Pillow==9.0.0 ``` ## What is featurewiz? `featurewiz` a new
-python library for creating and selecting the best features in your data set
-fast! `featurewiz` can be used in one or two ways. Both are explained below. ##
-1. Feature Engineering
+rsesha2001@yahoo.com License: Apache License 2.0 Description: # featurewiz
+`featurewiz` is a powerful feature selection library that has a number of
+features that make it stand out from the competition, including:
+   1. It provides one of the best automatic feature selection algorithms
+      (Minimum Redundancy Maximum Relevance (MRMR)) described by wikipedia as:
+      "The_MRMR_selection_has_been_found_to_be_more_powerful_than_the_maximum
+      relevance_feature_selection" such as Boruta.
+   2. It selects the best number of un-correlated features that have maximum
+      mutual information about the target without having to specify the number
+      of features
+   3. It is fast and easy to use, and comes with a number of helpful features,
+      such as a built-in categorical-to-numeric encoder and a powerful feature
+      engineering module
+   4. It is well-documented, and it comes with a number of examples.
+   5. It is actively maintained, and it is regularly updated with new features
+      and bug fixes.
+If you are looking for a single feature selection library, we would definitely
+recommend checking out featurewiz. It is a powerful tool that can help you to
+improve the performance of your machine learning models. # Table of Contents
+    * What_is_featurewiz
+    * How_it_works
+    * Tips_for_using_featurewiz
+    * How_to_install_featurewiz
+    * Usage
+    * API
+    * Additional_Tips
+    * Maintainers
+    * Contributing
+    * License
+    * Disclaimer
+![banner](featurewiz_logos.png) ## Introduction `featurewiz` a new python
+library for creating and selecting the best features in your data set fast!
+`featurewiz` can be used in one or two ways. Both are explained below. ### 1.
+Feature Engineering
 The first step is not absolutely necessary but it can be used to create new
 features that may or may not be helpful (be careful with automated feature
 engineering tools!).
 1. Performing Feature Engineering: One of the gaps in open source AutoML tools
 and especially Auto_ViML has been the lack of feature engineering capabilities
 that high powered competitions such as Kaggle required. The ability to create
 "interaction" variables or adding "group-by" features or "target-encoding"
@@ -30,19 +48,15 @@
 featurewiz now enables you to add hundreds of such features with a single line
 of code. Set the "feature_engg" flag to "interactions", "groupby" or "target"
 and featurewiz will select the best encoders for each of those options and
 create hundreds (perhaps thousands) of features in one go. Not only that, using
 the next step, featurewiz will sift through numerous such variables and find
 only the least correlated and most relevant features to your model. All in one
 step!.
-You must use this syntax for feature engg. Otherwise, featurewiz will give an
-error: ``` import featurewiz as FW outputs = FW.featurewiz(dataname=train,
-target=target, corr_limit=0.70, verbose=2, sep=',', header=0,
-test_data='',feature_engg='', category_encoders='', dask_xgboost_flag=False,
-nrows=None) ``` ![feature_engg](feature_engg.jpg) ## 2. Feature Selection
+![feature_engg](feature_engg.jpg) ### 2. Feature Selection
 The second step is Feature Selection. `featurewiz` uses the MRMR (Minimum
 Redundancy Maximum Relevance) algorithm as the basis for its feature selection.
 
 Why do Feature Selection? Once you have created 100's of new features, you
 still have three questions left to answer: 1. How do we interpret those newly
 created features? 2. Which of these features is important and which are
 useless? How many of them are highly correlated to each other causing
@@ -54,133 +68,100 @@
 SULOV: SULOV stands for `Searching for Uncorrelated List of Variables`. The
 SULOV algorithm is based on the Minimum-Redundancy-Maximum-Relevance (MRMR)
 algorithm_explained_in_this_article as one of the best feature selection
 methods. To understand how MRMR works and how it is different from `Boruta` and
 other feature selection methods, see the chart below. Here "Minimal Optimal"
 refers to the MRMR and featurewiz kind of algorithms while "all-relevant"
 refers to Boruta kind of algorithms.
-![MRMR_chart](MRMR.png)
-The working of the SULOV algorithm is as follows:
+![MRMR_chart](MRMR.png) ## Working `featurewiz` performs feature selection in 2
+steps. Each step is explained below. The working of the `SULOV` algorithm is as
+follows:
    1. Find all the pairs of highly correlated variables exceeding a correlation
       threshold (say absolute(0.7)).
    2. Then find their MIS score (Mutual Information Score) to the target
       variable. MIS is a non-parametric scoring method. So its suitable for all
       kinds of variables and target.
    3. Now take each pair of correlated variables, then knock off the one with
       the lower MIS score.
    4. Whatâs left is the ones with the highest Information scores and least
       correlation with each other.
-![sulov](SULOV.jpg) Recursive XGBoost: Once SULOV has selected variables that
-have high mutual information scores with least less correlation amongst them,
-we use XGBoost to repeatedly find best features among the remaining variables
-after SULOV. The Recursive XGBoost method is explained in this chart below.
-Here is how it works:
+![sulov](SULOV.jpg) The working of the Recursive XGBoost is as follows: Once
+SULOV has selected variables that have high mutual information scores with
+least less correlation amongst them, featurewiz uses XGBoost to repeatedly find
+the best features among the remaining variables after SULOV.
    1. Select all variables in data set and the full data split into train and
       valid sets.
    2. Find top X features (could be 10) on train using valid for early stopping
       (to prevent over-fitting)
    3. Then take next set of vars and find top X
    4. Do this 5 times. Combine all selected features and de-duplicate them.
-![xgboost](xgboost.jpg) Building the simplest and most "interpretable" model:
-featurewiz represents the "next best" step you must perform after doing feature
-engineering since you might have added some highly correlated or even useless
-features when you use automated feature engineering. featurewiz ensures you
-have the least number of features needed to build a high performing or
-equivalent model. A WORD OF CAUTION: Just because you can engineer new
-features, doesn't mean you should always create tons of new features. You must
-make sure you understand what the new features stand for before you attempt to
-build a model with these (sometimes useless) features. featurewiz displays the
-SULOV chart which can show you how the 100's of newly created variables added
-to your dataset are highly correlated to each other and were removed. This will
-help you understand how feature selection works in featurewiz. ## Table of
-Contents
-    * Background
-    * Install
-    * Usage
-    * API
-    * Maintainers
-    * Contributing
-    * License
-## Background ![background](featurewiz_background.jpg) To learn more about how
-featurewiz works under the hood, watch this [video](https://www.youtube.com/
-embed/ZiNutwPcAU0)
-featurewiz was designed for selecting High Performance variables with the
-fewest steps. In most cases, featurewiz builds models with 20%-99% fewer
-features than your original data set with nearly the same or slightly lower
-performance (this is based on my trials. Your experience may vary).
-featurewiz is every Data Scientist's feature wizard that will:
-   1. Automatically pre-process data: you can send in your entire dataframe "as
-      is" and featurewiz will classify and change/label encode categorical
-      variables changes to help XGBoost processing. It classifies variables as
-      numeric or categorical or NLP or date-time variables automatically so it
-      can use them correctly to model.
-   2. Perform feature engineering automatically: The ability to create
-      "interaction" variables or adding "group-by" features or "target-
-      encoding" categorical variables is difficult and sifting through those
-      hundreds of new features is painstaking and left only to "experts". Now,
-      with featurewiz you can create hundreds or even thousands of new features
-      with the click of a mouse. This is very helpful when you have a small
-      number of features to start with. However, be careful with this option.
-      You can very easily create a monster with this option.
-   3. Perform feature reduction automatically. When you have small data sets
-      and you know your domain well, it is easy to perhaps do EDA and identify
-      which variables are important. But when you have a very large data set
-      with hundreds if not thousands of variables, selecting the best features
-      from your model can mean the difference between a bloated and highly
-      complex model or a simple model with the fewest and most information-rich
-      features. featurewiz uses XGBoost repeatedly to perform feature
-      selection. You must try it on your large data sets and compare!
-   4. Explain SULOV method graphically using networkx library so you can see
-      which variables are highly correlated to which ones and which of those
-      have high or low mutual information scores automatically. Just set
-      verbose = 2 to see the graph.
-   5. Build a fast LightGBM model using the features selected by featurewiz.
-      There is a function called "simple_lightgbm_model" which you can use to
-      build a fast model. It is a new module, so check it out.
-*** Notes of Gratitude ***:
-   1. Alex Lekov (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/
-      automl_alex) for his DataBunch and encoders modules which are used by the
-      tool (although with some modifications).
-   2. Category Encoders library in Python : This is an amazing library. Make
-      sure you read all about the encoders that featurewiz uses here: https://
-      contrib.scikit-learn.org/category_encoders/index.html
+![xgboost](xgboost.jpg) ## Tips Here are some additional tips for ML engineers
+and data scientists when using featurewiz:
+   1. Always cross-validate your results: When you use a feature selection
+      tool, it is important to cross-validate your results. This means that you
+      should split your data into a training set and a test set. Use the
+      training set to select features, and then evaluate your model on the test
+      set. This will help you to ensure that your model is not overfitting to
+      the training data.
+   2. Use multiple feature selection tools: It is a good idea to use multiple
+      feature selection tools and compare the results. This will help you to
+      get a better understanding of which features are most important for your
+      data.
+   3. Don't forget to engineer new features: Feature selection is only one part
+      of the process of building a good machine learning model. You should also
+      spend time engineering your features to make them as informative as
+      possible. This can involve things like creating new features,
+      transforming existing features, and removing irrelevant features.
+   4. Don't overfit your model: It is important to avoid overfitting your model
+      to the training data. Overfitting occurs when your model learns the noise
+      in the training data, rather than the underlying signal. To avoid
+      overfitting, you can use regularization techniques, such as lasso or
+      elasticnet.
+   5. Start with a small number of features: When you are first starting out,
+      it is a good idea to start with a small number of features. This will
+      help you to avoid overfitting your model. As you become more experienced,
+      you can experiment with adding more features.
 ## Install **Prerequsites:**
    1. featurewiz is built using xgboost, dask, numpy, pandas and matplotlib. It
       should run on most Python 3 Anaconda installations. You won't have to
       import any special libraries other than "dask", "XGBoost" and "networkx"
       library. Optionally, it uses LightGBM for fast modeling, which it
       installs automatically.
    2. We use "networkx" library for charts and interpretability.
       But if you don't have these libraries, featurewiz will install those for
       you automatically.
-- [Anaconda](https://docs.anaconda.com/anaconda/install/) To clone featurewiz,
-it is better to create a new environment, and install the required
-dependencies: To install from PyPi: ``` conda create -n  python=3.7 anaconda
-conda activate  # ON WINDOWS: `source activate ` pip install featurewiz --
-ignore-installed --no-deps pip install lazytransform or pip install git+https:/
-/github.com/AutoViML/featurewiz.git ``` To install from source: ``` cd  git
-clone git@github.com:AutoViML/featurewiz.git # or download and unzip https://
-github.com/AutoViML/featurewiz/archive/master.zip conda create -n  python=3.7
-anaconda conda activate  # ON WINDOWS: `source activate ` cd featurewiz pip
-install -r requirements.txt ``` ## Usage As of Jan 2022, you now invoke
-featurewiz in two ways for two different goals. For feature selection, you must
-use the scikit-learn compatible fit and predict transformer syntax such as
-below. ``` from featurewiz import FeatureWiz features = FeatureWiz
-(corr_limit=0.70, feature_engg='', category_encoders='',
+To install from source: ``` cd  git clone git@github.com:AutoViML/
+featurewiz.git # or download and unzip https://github.com/AutoViML/featurewiz/
+archive/master.zip conda create -n  python=3.7 anaconda conda activate  # ON
+WINDOWS: `source activate ` cd featurewiz pip install -r requirements.txt ```
+## Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
+Check_out_more_latest_updates_from_this_page
+As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo),
+featurewiz is now available on conda-forge. You can try:
+``` conda install -c conda-forge featurewiz ``` ### If the above conda install
+fails, you can try installing featurewiz this way: ##Step 1: Install featurewiz
+first
+``` !pip install featurewiz --ignore-installed --no-deps !pip install xlrd --
+ignore-installed --no-deps ``` ##Step 2: Next, install Pillow since Kaggle has
+an incompatible version.
+``` !pip install Pillow==9.0.0 ``` ## Usage For feature selection, you must use
+the newer syntax which is similar to the scikit-learn fit and predict
+transformer syntax below. ``` from featurewiz import FeatureWiz fwiz =
+FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='',
 dask_xgboost_flag=False, nrows=None, verbose=2) X_train_selected =
-features.fit_transform(X_train, y_train) X_test_selected = features.transform
-(X_test) features.features ### provides the list of selected features ### ```
-Alternatively, you can use featurewiz for feature engineering using this older
-syntax. Otherwise, it will give an error. If you want to combine feature engg
-and then feature selection, you must use this older syntax: ``` import
-featurewiz as FW outputs = FW.featurewiz(dataname=train, target=target,
-corr_limit=0.70, verbose=2, sep=',', header=0, test_data='',feature_engg='',
+fwiz.fit_transform(X_train, y_train) X_test_selected = fwiz.transform(X_test)
+### get list of selected features ### fwiz.features ``` Alternatively, you can
+use featurewiz for feature engineering using this older syntax. Otherwise, it
+will give an error. If you want to combine feature engg and then feature
+selection, you must use this older syntax: ``` import featurewiz as fwiz
+outputs = fwiz.featurewiz(dataname=train, target=target, corr_limit=0.70,
+verbose=2, sep=',', header=0, test_data='',feature_engg='',
 category_encoders='', dask_xgboost_flag=False, nrows=None) ``` `outputs`: There
 will always be multiple objects in output. The objects in that tuple can vary:
-1. "features" and "train": It be a list (of selected features) and one
+1. "features" and "trainm": It be a list (of selected features) and one
 dataframe (if you sent in train only) 2. "trainm" and "testm": It can be two
 dataframes when you send in both test and train but with selected features.
    1. Both the selected features and dataframes are ready for you to now to do
       further modeling.
    2. Featurewiz works on any multi-class, multi-label data Set. So you can
       have as many target labels as you want.
    3. You don't have to tell Featurewiz whether it is a Regression or
@@ -252,23 +233,66 @@
 support, it uses PolynomialWrapper. For feature value i, James-Stein estimator
 returns a weighted average of: The mean target value for the observed feature
 value i. The mean target value (regardless of the feature value). -
 `dask_xgboost_flag`: Default is False. Set to True to use dask_xgboost
 estimator. You can turn it off if it gives an error. Then it will use pandas
 and regular xgboost to do the job. - `nrows`: default `None`. You can set the
 number of rows to read from your datafile if it is too large to fit into either
-dask or pandas. But you won't have to if you use dask. **Return values** -
+dask or pandas. But you won't have to if you use dask. **Output values** -
 `outputs`: Output is always a tuple. We can call our outputs in that tuple:
 out1 and out2. - `out1` and `out2`: If you sent in just one dataframe or
 filename as input, you will get: - 1. `features`: It will be a list (of
 selected features) and - 2. `trainm`: It will be a dataframe (if you sent in a
 file or dataname as input) - `out1` and `out2`: If you sent in two files or
 dataframes (train and test), you will get: - 1. `trainm`: a modified train
 dataframe with engineered and selected features from dataname and - 2. `testm`:
 a modified test dataframe with engineered and selected features from test_data.
+## Additional ![background](featurewiz_background.jpg) To learn more about how
+featurewiz works under the hood, watch this [video](https://www.youtube.com/
+embed/ZiNutwPcAU0)
+featurewiz was designed for selecting High Performance variables with the
+fewest steps. In most cases, featurewiz builds models with 20%-99% fewer
+features than your original data set with nearly the same or slightly lower
+performance (this is based on my trials. Your experience may vary).
+featurewiz is every Data Scientist's feature wizard that will:
+   1. Automatically pre-process data: you can send in your entire dataframe "as
+      is" and featurewiz will classify and change/label encode categorical
+      variables changes to help XGBoost processing. It classifies variables as
+      numeric or categorical or NLP or date-time variables automatically so it
+      can use them correctly to model.
+   2. Perform feature engineering automatically: The ability to create
+      "interaction" variables or adding "group-by" features or "target-
+      encoding" categorical variables is difficult and sifting through those
+      hundreds of new features is painstaking and left only to "experts". Now,
+      with featurewiz you can create hundreds or even thousands of new features
+      with the click of a mouse. This is very helpful when you have a small
+      number of features to start with. However, be careful with this option.
+      You can very easily create a monster with this option.
+   3. Perform feature reduction automatically. When you have small data sets
+      and you know your domain well, it is easy to perhaps do EDA and identify
+      which variables are important. But when you have a very large data set
+      with hundreds if not thousands of variables, selecting the best features
+      from your model can mean the difference between a bloated and highly
+      complex model or a simple model with the fewest and most information-rich
+      features. featurewiz uses XGBoost repeatedly to perform feature
+      selection. You must try it on your large data sets and compare!
+   4. Explain SULOV method graphically using networkx library so you can see
+      which variables are highly correlated to which ones and which of those
+      have high or low mutual information scores automatically. Just set
+      verbose = 2 to see the graph.
+   5. Build a fast XGBoost or LightGBM model using the features selected by
+      featurewiz. There is a function called "simple_lightgbm_model" which you
+      can use to build a fast model. It is a new module, so check it out.
+*** A Note of Gratitude ***:
+   1. Alex Lekov (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/
+      automl_alex) for his DataBunch and encoders modules which are used by the
+      tool (although with some modifications).
+   2. Category Encoders library in Python : This is an amazing library. Make
+      sure you read all about the encoders that featurewiz uses here: https://
+      contrib.scikit-learn.org/category_encoders/index.html
 ## Maintainers * [@AutoViML](https://github.com/AutoViML) ## Contributing See
 [the contributing file](CONTRIBUTING.md)! PRs accepted. ## License Apache
 License 2.0 Â© 2020 Ram Seshadri ## DISCLAIMER This project is not an official
 Google project. It is not supported by Google and Google specifically disclaims
 all warranties as to its quality, merchantability, or fitness for a particular
 purpose. Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
```

### Comparing `featurewiz-0.2.7/README.md` & `featurewiz-0.2.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,182 +1,157 @@
 # featurewiz
+`featurewiz` is a powerful feature selection library that has a number of features that make it stand out from the competition, including:
+<ol>
+<li>It provides one of the best automatic feature selection algorithms (Minimum Redundancy Maximum Relevance (MRMR)) described by wikipedia as: <a href="https://en.wikipedia.org/wiki/Minimum_redundancy_feature_selection">"The MRMR selection has been found to be more powerful than the maximum relevance feature selection"</a> such as Boruta.</li>
+<li>It selects the best number of un-correlated features that have maximum mutual information about the target without having to specify the number of features</li>
+<li>It is fast and easy to use, and comes with a number of helpful features, such as a built-in categorical-to-numeric encoder and a powerful feature engineering module</li>
+<li>It is well-documented, and it comes with a number of <a href="https://github.com/AutoViML/featurewiz/tree/main/examples">examples</a>.</li>
+<li>It is actively maintained, and it is regularly updated with new features and bug fixes.</li>
+</ol>
+If you are looking for a single feature selection library, we would definitely recommend checking out featurewiz. It is a powerful tool that can help you to improve the performance of your machine learning models.
 
-![banner](featurewiz_logos.png)
-
-##  Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
-<a href="updates.md">Check out more latest updates from this page</a><br>
-As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo), featurewiz is now available on conda-forge. You can try:<br>
-
-```
- conda install -c conda-forge featurewiz
-```
-
-### If the above conda install fails, you can try installing featurewiz this way:
-##Step 1: Install featurewiz first<br>
-
-```
- !pip install featurewiz --ignore-installed --no-deps
- !pip install xlrd --ignore-installed --no-deps 
-```
-
-##Step 2: Next, install Pillow since Kaggle has an incompatible version. <br>
+# Table of Contents
+<ul>
+<li><a href="#introduction">What is featurewiz</a></li>
+<li><a href="#working">How it works</a></li>
+<li><a href="#tips">Tips for using featurewiz</a></li>
+<li><a href="#install">How to install featurewiz</a></li>
+<li><a href="#usage">Usage</a></li>
+<li><a href="#api">API</a></li>
+<li><a href="#additional">Additional Tips</a></li>
+<li><a href="#maintainers">Maintainers</a></li>
+<li><a href="#contributing">Contributing</a></li>
+<li><a href="#license">License</a></li>
+<li><a href="#disclaimer">Disclaimer</a></li>
+</ul>
+<p>
 
-```
- !pip install Pillow==9.0.0
-```
+![banner](featurewiz_logos.png)
 
-## What is featurewiz?
+## Introduction
 `featurewiz` a new python library for creating and selecting the best features in your data set fast!
 `featurewiz` can be used in one or two ways. Both are explained below.
 
-## 1.  Feature Engineering
+### 1.  Feature Engineering
 <p>The first step is not absolutely necessary but it can be used to create new features that may or may not be helpful (be careful with automated feature engineering tools!).<p>
 1. <b>Performing Feature Engineering</b>: One of the gaps in open source AutoML tools and especially Auto_ViML has been the lack of feature engineering capabilities that high powered competitions such as Kaggle required. The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables was difficult and sifting through those hundreds of new features to find best features was difficult and left only to "experts" or "professionals". featurewiz was created to help you in this endeavor.<br>
 <p>featurewiz now enables you to add hundreds of such features with a single line of code. Set the "feature_engg" flag to "interactions", "groupby" or "target" and featurewiz will select the best encoders for each of those options and create hundreds (perhaps thousands) of features in one go. Not only that, using the next step, featurewiz will sift through numerous such variables and find only the least correlated and most relevant features to your model. All in one step!.<br>
 
-You must use this syntax for feature engg. Otherwise, featurewiz will give an error:
-
-```
-import featurewiz as FW
-outputs = FW.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
-		header=0, test_data='',feature_engg='', category_encoders='',
-		dask_xgboost_flag=False, nrows=None)
-```
-
 ![feature_engg](feature_engg.jpg)
 
-## 2.  Feature Selection
+### 2.  Feature Selection
 <p>The second step is Feature Selection. `featurewiz` uses the MRMR (Minimum Redundancy Maximum Relevance) algorithm as the basis for its feature selection. <br>
 <b> Why do Feature Selection</b>? Once you have created 100's of new features, you still have three questions left to answer:
 1. How do we interpret those newly created features?
 2. Which of these features is important and which are useless? How many of them are highly correlated to each other causing redundancy?
 3. Does the model overfit now on these new features and perform better or worse than before?
 <br>
 All are very important questions and featurewiz answers them by using the SULOV method and Recursive XGBoost to reduce features in your dataset to the best "minimum optimal" features for the model.<br>
 <p><b>SULOV</b>: SULOV stands for `Searching for Uncorrelated List of Variables`. The SULOV algorithm is based on the Minimum-Redundancy-Maximum-Relevance (MRMR) <a href="https://towardsdatascience.com/mrmr-explained-exactly-how-you-wished-someone-explained-to-you-9cf4ed27458b">algorithm explained in this article</a> as one of the best feature selection methods. To understand how MRMR works and how it is different from `Boruta` and other feature selection methods, see the chart below. Here "Minimal Optimal" refers to the MRMR and featurewiz kind of algorithms while "all-relevant" refers to Boruta kind of algorithms.<br>
 
 ![MRMR_chart](MRMR.png)
-<br>
-The working of the SULOV algorithm is as follows:
+
+## Working
+`featurewiz` performs feature selection in 2 steps. Each step is explained below.
+<b>The working of the `SULOV` algorithm</b> is as follows:
 <ol>
-<li>Find all the pairs of highly correlated variables exceeding a correlation threshold (say absolute(0.7)).
-<li>Then find their MIS score (Mutual Information Score) to the target variable. MIS is a non-parametric scoring method. So its suitable for all kinds of variables and target.
-<li>Now take each pair of correlated variables, then knock off the one with the lower MIS score.
-<li>What’s left is the ones with the highest Information scores and least correlation with each other.
+<li>Find all the pairs of highly correlated variables exceeding a correlation threshold (say absolute(0.7)).</li>
+<li>Then find their MIS score (Mutual Information Score) to the target variable. MIS is a non-parametric scoring method. So its suitable for all kinds of variables and target.</li>
+<li>Now take each pair of correlated variables, then knock off the one with the lower MIS score.</li>
+<li>What’s left is the ones with the highest Information scores and least correlation with each other.</li>
 </ol>
 
 ![sulov](SULOV.jpg)
 
-<b>Recursive XGBoost</b>: Once SULOV has selected variables that have high mutual information scores with least less correlation amongst them, we use XGBoost to repeatedly find best features among the remaining variables after SULOV. The Recursive XGBoost method is explained in this chart below.
-Here is how it works:
+<b>The working of the Recursive XGBoost</b> is as follows: 
+Once SULOV has selected variables that have high mutual information scores with least less correlation amongst them, featurewiz uses XGBoost to repeatedly find the best features among the remaining variables after SULOV. 
 <ol>
-<li>Select all variables in data set and the full data split into train and valid sets.
-<li>Find top X features (could be 10) on train using valid for early stopping (to prevent over-fitting)
-<li>Then take next set of vars and find top X
-<li>Do this 5 times. Combine all selected features and de-duplicate them.
+<li>Select all variables in data set and the full data split into train and valid sets.</li>
+<li>Find top X features (could be 10) on train using valid for early stopping (to prevent over-fitting)</li>
+<li>Then take next set of vars and find top X</li>
+<li>Do this 5 times. Combine all selected features and de-duplicate them.</li>
 </ol>
 
 ![xgboost](xgboost.jpg)
 
-<b>Building the simplest and most "interpretable" model</b>: featurewiz represents the "next best" step you must perform after doing feature engineering  since you might have added some highly correlated or even useless features when you use automated feature engineering. featurewiz ensures you have the least number of features needed to build a high performing or equivalent model.
-
-<b>A WORD OF CAUTION:</b> Just because you can engineer new features, doesn't mean you should always create tons of new features. You must make sure you understand what the new features stand for before you attempt to build a model with these (sometimes useless) features. featurewiz displays the SULOV chart which can show you how the 100's of newly created variables added to your dataset are highly correlated to each other and were removed. This will help you understand how feature selection works in featurewiz.
-
-## Table of Contents
-<ul>
-<li><a href="#background">Background</a></li>
-<li><a href="#install">Install</a></li>
-<li><a href="#usage">Usage</a></li>
-<li><a href="#api">API</a></li>
-<li><a href="#maintainers">Maintainers</a></li>
-<li><a href="#contributing">Contributing</a></li>
-<li><a href="#license">License</a></li>
-</ul>
-
-## Background
-
-![background](featurewiz_background.jpg)
-
-To learn more about how featurewiz works under the hood, watch this [video](https://www.youtube.com/embed/ZiNutwPcAU0)<br>
-
-<p>featurewiz was designed for selecting High Performance variables with the fewest steps.
-
-In most cases, featurewiz builds models with 20%-99% fewer features than your original data set with nearly the same or slightly lower performance (this is based on my trials. Your experience may vary).<br>
-<p>
-featurewiz is every Data Scientist's feature wizard that will:<ol>
-<li><b>Automatically pre-process data</b>: you can send in your entire dataframe "as is" and featurewiz will classify and change/label encode categorical variables changes to help XGBoost processing. It classifies variables as numeric or categorical or NLP or date-time variables automatically so it can use them correctly to model.<br>
-<li><b>Perform feature engineering automatically</b>: The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables is difficult and sifting through those hundreds of new features is painstaking and left only to "experts". Now, with featurewiz you can create hundreds or even thousands of new features with the click of a mouse. This is very helpful when you have a small number of features to start with. However, be careful with this option. You can very easily create a monster with this option.
-<li><b>Perform feature reduction automatically</b>. When you have small data sets and you know your domain well, it is easy to perhaps do EDA and identify which variables are important. But when you have a very large data set with hundreds if not thousands of variables, selecting the best features from your model can mean the difference between a bloated and highly complex model or a simple model with the fewest and most information-rich features. featurewiz uses XGBoost repeatedly to perform feature selection. You must try it on your large data sets and compare!<br>
-<li><b>Explain SULOV method graphically </b> using networkx library so you can see which variables are highly correlated to which ones and which of those have high or low mutual information scores automatically. Just set verbose = 2 to see the graph. <br>
-<li><b>Build a fast LightGBM model </b> using the features selected by featurewiz. There is a function called "simple_lightgbm_model" which you can use to build a fast model. It is a new module, so check it out.<br>
-</ol>
-
-<b>***  Notes of Gratitude ***</b>:<br>
+## Tips
+Here are some additional tips for ML engineers and data scientists when using featurewiz:
 <ol>
-<li><b>Alex Lekov</b> (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/automl_alex) for his DataBunch and encoders modules which are used by the tool (although with some modifications).</li>
-<li><b>Category Encoders</b> library in Python : This is an amazing library. Make sure you read all about the encoders that featurewiz uses here: https://contrib.scikit-learn.org/category_encoders/index.html </li>
+<li><b>Always cross-validate your results</b>: When you use a feature selection tool, it is important to cross-validate your results. This means that you should split your data into a training set and a test set. Use the training set to select features, and then evaluate your model on the test set. This will help you to ensure that your model is not overfitting to the training data.</li>
+<li><b>Use multiple feature selection tools</b>: It is a good idea to use multiple feature selection tools and compare the results. This will help you to get a better understanding of which features are most important for your data.</li>
+<li><b>Don't forget to engineer new features</b>: Feature selection is only one part of the process of building a good machine learning model. You should also spend time engineering your features to make them as informative as possible. This can involve things like creating new features, transforming existing features, and removing irrelevant features.</li>
+<li><b>Don't overfit your model</b>: It is important to avoid overfitting your model to the training data. Overfitting occurs when your model learns the noise in the training data, rather than the underlying signal. To avoid overfitting, you can use regularization techniques, such as lasso or elasticnet.</li>
+<li><b>Start with a small number of features</b>: When you are first starting out, it is a good idea to start with a small number of features. This will help you to avoid overfitting your model. As you become more experienced, you can experiment with adding more features.</li>
 </ol>
 
 ## Install
 
 **Prerequsites:**
 <ol>
 <li><b>featurewiz is built using xgboost, dask, numpy, pandas and matplotlib</b>. It should run on most Python 3 Anaconda installations. You won't have to import any special libraries other than "dask", "XGBoost" and "networkx" library. Optionally, it uses LightGBM for fast modeling, which it installs automatically. </li>
 <li><b>We use "networkx" library for charts and interpretability</b>. <br>But if you don't have these libraries, featurewiz will install those for you automatically.</li>
 </ol>
-- [Anaconda](https://docs.anaconda.com/anaconda/install/)
-
-To clone featurewiz, it is better to create a new environment, and install the required dependencies:
-
-To install from PyPi:
-
-```
-conda create -n <your_env_name> python=3.7 anaconda
-conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
-pip install featurewiz --ignore-installed --no-deps
-pip install lazytransform
-or
-pip install git+https://github.com/AutoViML/featurewiz.git
-```
-
 To install from source:
 
 ```
 cd <featurewiz_Destination>
 git clone git@github.com:AutoViML/featurewiz.git
 # or download and unzip https://github.com/AutoViML/featurewiz/archive/master.zip
 conda create -n <your_env_name> python=3.7 anaconda
 conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
 cd featurewiz
 pip install -r requirements.txt
 ```
 
+##  Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
+<a href="updates.md">Check out more latest updates from this page</a><br>
+As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo), featurewiz is now available on conda-forge. You can try:<br>
+
+```
+ conda install -c conda-forge featurewiz
+```
+
+### If the above conda install fails, you can try installing featurewiz this way:
+##Step 1: Install featurewiz first<br>
+
+```
+ !pip install featurewiz --ignore-installed --no-deps
+ !pip install xlrd --ignore-installed --no-deps 
+```
+
+##Step 2: Next, install Pillow since Kaggle has an incompatible version. <br>
+
+```
+ !pip install Pillow==9.0.0
+```
+
 ## Usage
 
-As of Jan 2022, you now invoke featurewiz in two ways for two different goals. For feature selection, you must use the scikit-learn compatible fit and predict transformer syntax such as below.
+For feature selection, you must use the newer syntax which is similar to the scikit-learn fit and predict transformer syntax below.
 
 ```
 from featurewiz import FeatureWiz
-features = FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='', dask_xgboost_flag=False, nrows=None, verbose=2)
-X_train_selected = features.fit_transform(X_train, y_train)
-X_test_selected = features.transform(X_test)
-features.features  ### provides the list of selected features ###
+fwiz = FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='', dask_xgboost_flag=False, nrows=None, verbose=2)
+X_train_selected = fwiz.fit_transform(X_train, y_train)
+X_test_selected = fwiz.transform(X_test)
+### get list of selected features ###
+fwiz.features  
 ```
 
 Alternatively, you can use featurewiz for feature engineering using this older syntax. Otherwise, it will give an error. If you want to combine feature engg and then feature selection, you must use this older syntax:
 
 ```
-import featurewiz as FW
-outputs = FW.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
+import featurewiz as fwiz
+outputs = fwiz.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
 		header=0, test_data='',feature_engg='', category_encoders='',
 		dask_xgboost_flag=False, nrows=None)
 ```
 
 `outputs`: There will always be multiple objects in output. The objects in that tuple can vary:
-1. "features" and "train": It be a list (of selected features) and one dataframe (if you sent in train only)
+1. "features" and "trainm": It be a list (of selected features) and one dataframe (if you sent in train only)
 2. "trainm" and "testm": It can be two dataframes when you send in both test and train but with selected features.
 <ol>
 <li>Both the selected features and dataframes are ready for you to now to do further modeling.
 <li>Featurewiz works on any multi-class, multi-label data Set. So you can have as many target labels as you want.
 <li>You don't have to tell Featurewiz whether it is a Regression or Classification problem. It will decide that automatically.
 </ol>
 
@@ -216,23 +191,46 @@
     - `WOEEncoder`: WOEEncoder uses the Weight of Evidence technique for categorical features. It supports only one kind of target: binary. For polynomial target support, it uses a PolynomialWrapper. It cannot be used for Regression.
     - `JamesSteinEncoder`: JamesSteinEncoder uses the James-Stein estimator. It supports 2 kinds of targets: binary and continuous. For polynomial target support, it uses PolynomialWrapper.
     For feature value i, James-Stein estimator returns a weighted average of:
     The mean target value for the observed feature value i.
     The mean target value (regardless of the feature value).
     - `dask_xgboost_flag`: Default is False. Set to True to use dask_xgboost estimator. You can turn it off if it gives an error. Then it will use pandas and regular xgboost to do the job.
     - `nrows`: default `None`. You can set the number of rows to read from your datafile if it is too large to fit into either dask or pandas. But you won't have to if you use dask. 
-**Return values**
+
+**Output values**
 -   `outputs`: Output is always a tuple. We can call our outputs in that tuple: out1 and out2.
     -   `out1` and `out2`: If you sent in just one dataframe or filename as input, you will get:
         - 1. `features`: It will be a list (of selected features) and
         - 2. `trainm`: It will be a dataframe (if you sent in a file or dataname as input)
     -   `out1` and `out2`: If you sent in two files or dataframes (train and test), you will get:
         - 1. `trainm`: a modified train dataframe with engineered and selected features from dataname and
         - 2. `testm`: a modified test dataframe with engineered and selected features from test_data.
 
+## Additional
+
+![background](featurewiz_background.jpg)
+
+To learn more about how featurewiz works under the hood, watch this [video](https://www.youtube.com/embed/ZiNutwPcAU0)<br>
+<p>featurewiz was designed for selecting High Performance variables with the fewest steps.
+In most cases, featurewiz builds models with 20%-99% fewer features than your original data set with nearly the same or slightly lower performance (this is based on my trials. Your experience may vary).<br>
+<p>
+featurewiz is every Data Scientist's feature wizard that will:<ol>
+<li><b>Automatically pre-process data</b>: you can send in your entire dataframe "as is" and featurewiz will classify and change/label encode categorical variables changes to help XGBoost processing. It classifies variables as numeric or categorical or NLP or date-time variables automatically so it can use them correctly to model.<br>
+<li><b>Perform feature engineering automatically</b>: The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables is difficult and sifting through those hundreds of new features is painstaking and left only to "experts". Now, with featurewiz you can create hundreds or even thousands of new features with the click of a mouse. This is very helpful when you have a small number of features to start with. However, be careful with this option. You can very easily create a monster with this option.
+<li><b>Perform feature reduction automatically</b>. When you have small data sets and you know your domain well, it is easy to perhaps do EDA and identify which variables are important. But when you have a very large data set with hundreds if not thousands of variables, selecting the best features from your model can mean the difference between a bloated and highly complex model or a simple model with the fewest and most information-rich features. featurewiz uses XGBoost repeatedly to perform feature selection. You must try it on your large data sets and compare!<br>
+<li><b>Explain SULOV method graphically </b> using networkx library so you can see which variables are highly correlated to which ones and which of those have high or low mutual information scores automatically. Just set verbose = 2 to see the graph. <br>
+<li><b>Build a fast XGBoost or LightGBM model using the features selected by featurewiz</b>. There is a function called "simple_lightgbm_model" which you can use to build a fast model. It is a new module, so check it out.<br>
+</ol>
+
+<b>*** A Note of Gratitude ***</b>:<br>
+<ol>
+<li><b>Alex Lekov</b> (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/automl_alex) for his DataBunch and encoders modules which are used by the tool (although with some modifications).</li>
+<li><b>Category Encoders</b> library in Python : This is an amazing library. Make sure you read all about the encoders that featurewiz uses here: https://contrib.scikit-learn.org/category_encoders/index.html </li>
+</ol>
+
 ## Maintainers
 
 * [@AutoViML](https://github.com/AutoViML)
 
 ## Contributing
 
 See [the contributing file](CONTRIBUTING.md)!
```

#### html2text {}

```diff
@@ -1,22 +1,40 @@
-# featurewiz ![banner](featurewiz_logos.png) ## Good News: You can install
-featurewiz on Colab and Kaggle easily in 2 steps! Check_out_more_latest_updates
-from_this_page
-As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo),
-featurewiz is now available on conda-forge. You can try:
-``` conda install -c conda-forge featurewiz ``` ### If the above conda install
-fails, you can try installing featurewiz this way: ##Step 1: Install featurewiz
-first
-``` !pip install featurewiz --ignore-installed --no-deps !pip install xlrd --
-ignore-installed --no-deps ``` ##Step 2: Next, install Pillow since Kaggle has
-an incompatible version.
-``` !pip install Pillow==9.0.0 ``` ## What is featurewiz? `featurewiz` a new
-python library for creating and selecting the best features in your data set
-fast! `featurewiz` can be used in one or two ways. Both are explained below. ##
-1. Feature Engineering
+# featurewiz `featurewiz` is a powerful feature selection library that has a
+number of features that make it stand out from the competition, including:
+   1. It provides one of the best automatic feature selection algorithms
+      (Minimum Redundancy Maximum Relevance (MRMR)) described by wikipedia as:
+      "The_MRMR_selection_has_been_found_to_be_more_powerful_than_the_maximum
+      relevance_feature_selection" such as Boruta.
+   2. It selects the best number of un-correlated features that have maximum
+      mutual information about the target without having to specify the number
+      of features
+   3. It is fast and easy to use, and comes with a number of helpful features,
+      such as a built-in categorical-to-numeric encoder and a powerful feature
+      engineering module
+   4. It is well-documented, and it comes with a number of examples.
+   5. It is actively maintained, and it is regularly updated with new features
+      and bug fixes.
+If you are looking for a single feature selection library, we would definitely
+recommend checking out featurewiz. It is a powerful tool that can help you to
+improve the performance of your machine learning models. # Table of Contents
+    * What_is_featurewiz
+    * How_it_works
+    * Tips_for_using_featurewiz
+    * How_to_install_featurewiz
+    * Usage
+    * API
+    * Additional_Tips
+    * Maintainers
+    * Contributing
+    * License
+    * Disclaimer
+![banner](featurewiz_logos.png) ## Introduction `featurewiz` a new python
+library for creating and selecting the best features in your data set fast!
+`featurewiz` can be used in one or two ways. Both are explained below. ### 1.
+Feature Engineering
 The first step is not absolutely necessary but it can be used to create new
 features that may or may not be helpful (be careful with automated feature
 engineering tools!).
 1. Performing Feature Engineering: One of the gaps in open source AutoML tools
 and especially Auto_ViML has been the lack of feature engineering capabilities
 that high powered competitions such as Kaggle required. The ability to create
 "interaction" variables or adding "group-by" features or "target-encoding"
@@ -26,19 +44,15 @@
 featurewiz now enables you to add hundreds of such features with a single line
 of code. Set the "feature_engg" flag to "interactions", "groupby" or "target"
 and featurewiz will select the best encoders for each of those options and
 create hundreds (perhaps thousands) of features in one go. Not only that, using
 the next step, featurewiz will sift through numerous such variables and find
 only the least correlated and most relevant features to your model. All in one
 step!.
-You must use this syntax for feature engg. Otherwise, featurewiz will give an
-error: ``` import featurewiz as FW outputs = FW.featurewiz(dataname=train,
-target=target, corr_limit=0.70, verbose=2, sep=',', header=0,
-test_data='',feature_engg='', category_encoders='', dask_xgboost_flag=False,
-nrows=None) ``` ![feature_engg](feature_engg.jpg) ## 2. Feature Selection
+![feature_engg](feature_engg.jpg) ### 2. Feature Selection
 The second step is Feature Selection. `featurewiz` uses the MRMR (Minimum
 Redundancy Maximum Relevance) algorithm as the basis for its feature selection.
 
 Why do Feature Selection? Once you have created 100's of new features, you
 still have three questions left to answer: 1. How do we interpret those newly
 created features? 2. Which of these features is important and which are
 useless? How many of them are highly correlated to each other causing
@@ -50,133 +64,100 @@
 SULOV: SULOV stands for `Searching for Uncorrelated List of Variables`. The
 SULOV algorithm is based on the Minimum-Redundancy-Maximum-Relevance (MRMR)
 algorithm_explained_in_this_article as one of the best feature selection
 methods. To understand how MRMR works and how it is different from `Boruta` and
 other feature selection methods, see the chart below. Here "Minimal Optimal"
 refers to the MRMR and featurewiz kind of algorithms while "all-relevant"
 refers to Boruta kind of algorithms.
-![MRMR_chart](MRMR.png)
-The working of the SULOV algorithm is as follows:
+![MRMR_chart](MRMR.png) ## Working `featurewiz` performs feature selection in 2
+steps. Each step is explained below. The working of the `SULOV` algorithm is as
+follows:
    1. Find all the pairs of highly correlated variables exceeding a correlation
       threshold (say absolute(0.7)).
    2. Then find their MIS score (Mutual Information Score) to the target
       variable. MIS is a non-parametric scoring method. So its suitable for all
       kinds of variables and target.
    3. Now take each pair of correlated variables, then knock off the one with
       the lower MIS score.
    4. Whatâs left is the ones with the highest Information scores and least
       correlation with each other.
-![sulov](SULOV.jpg) Recursive XGBoost: Once SULOV has selected variables that
-have high mutual information scores with least less correlation amongst them,
-we use XGBoost to repeatedly find best features among the remaining variables
-after SULOV. The Recursive XGBoost method is explained in this chart below.
-Here is how it works:
+![sulov](SULOV.jpg) The working of the Recursive XGBoost is as follows: Once
+SULOV has selected variables that have high mutual information scores with
+least less correlation amongst them, featurewiz uses XGBoost to repeatedly find
+the best features among the remaining variables after SULOV.
    1. Select all variables in data set and the full data split into train and
       valid sets.
    2. Find top X features (could be 10) on train using valid for early stopping
       (to prevent over-fitting)
    3. Then take next set of vars and find top X
    4. Do this 5 times. Combine all selected features and de-duplicate them.
-![xgboost](xgboost.jpg) Building the simplest and most "interpretable" model:
-featurewiz represents the "next best" step you must perform after doing feature
-engineering since you might have added some highly correlated or even useless
-features when you use automated feature engineering. featurewiz ensures you
-have the least number of features needed to build a high performing or
-equivalent model. A WORD OF CAUTION: Just because you can engineer new
-features, doesn't mean you should always create tons of new features. You must
-make sure you understand what the new features stand for before you attempt to
-build a model with these (sometimes useless) features. featurewiz displays the
-SULOV chart which can show you how the 100's of newly created variables added
-to your dataset are highly correlated to each other and were removed. This will
-help you understand how feature selection works in featurewiz. ## Table of
-Contents
-    * Background
-    * Install
-    * Usage
-    * API
-    * Maintainers
-    * Contributing
-    * License
-## Background ![background](featurewiz_background.jpg) To learn more about how
-featurewiz works under the hood, watch this [video](https://www.youtube.com/
-embed/ZiNutwPcAU0)
-featurewiz was designed for selecting High Performance variables with the
-fewest steps. In most cases, featurewiz builds models with 20%-99% fewer
-features than your original data set with nearly the same or slightly lower
-performance (this is based on my trials. Your experience may vary).
-featurewiz is every Data Scientist's feature wizard that will:
-   1. Automatically pre-process data: you can send in your entire dataframe "as
-      is" and featurewiz will classify and change/label encode categorical
-      variables changes to help XGBoost processing. It classifies variables as
-      numeric or categorical or NLP or date-time variables automatically so it
-      can use them correctly to model.
-   2. Perform feature engineering automatically: The ability to create
-      "interaction" variables or adding "group-by" features or "target-
-      encoding" categorical variables is difficult and sifting through those
-      hundreds of new features is painstaking and left only to "experts". Now,
-      with featurewiz you can create hundreds or even thousands of new features
-      with the click of a mouse. This is very helpful when you have a small
-      number of features to start with. However, be careful with this option.
-      You can very easily create a monster with this option.
-   3. Perform feature reduction automatically. When you have small data sets
-      and you know your domain well, it is easy to perhaps do EDA and identify
-      which variables are important. But when you have a very large data set
-      with hundreds if not thousands of variables, selecting the best features
-      from your model can mean the difference between a bloated and highly
-      complex model or a simple model with the fewest and most information-rich
-      features. featurewiz uses XGBoost repeatedly to perform feature
-      selection. You must try it on your large data sets and compare!
-   4. Explain SULOV method graphically using networkx library so you can see
-      which variables are highly correlated to which ones and which of those
-      have high or low mutual information scores automatically. Just set
-      verbose = 2 to see the graph.
-   5. Build a fast LightGBM model using the features selected by featurewiz.
-      There is a function called "simple_lightgbm_model" which you can use to
-      build a fast model. It is a new module, so check it out.
-*** Notes of Gratitude ***:
-   1. Alex Lekov (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/
-      automl_alex) for his DataBunch and encoders modules which are used by the
-      tool (although with some modifications).
-   2. Category Encoders library in Python : This is an amazing library. Make
-      sure you read all about the encoders that featurewiz uses here: https://
-      contrib.scikit-learn.org/category_encoders/index.html
+![xgboost](xgboost.jpg) ## Tips Here are some additional tips for ML engineers
+and data scientists when using featurewiz:
+   1. Always cross-validate your results: When you use a feature selection
+      tool, it is important to cross-validate your results. This means that you
+      should split your data into a training set and a test set. Use the
+      training set to select features, and then evaluate your model on the test
+      set. This will help you to ensure that your model is not overfitting to
+      the training data.
+   2. Use multiple feature selection tools: It is a good idea to use multiple
+      feature selection tools and compare the results. This will help you to
+      get a better understanding of which features are most important for your
+      data.
+   3. Don't forget to engineer new features: Feature selection is only one part
+      of the process of building a good machine learning model. You should also
+      spend time engineering your features to make them as informative as
+      possible. This can involve things like creating new features,
+      transforming existing features, and removing irrelevant features.
+   4. Don't overfit your model: It is important to avoid overfitting your model
+      to the training data. Overfitting occurs when your model learns the noise
+      in the training data, rather than the underlying signal. To avoid
+      overfitting, you can use regularization techniques, such as lasso or
+      elasticnet.
+   5. Start with a small number of features: When you are first starting out,
+      it is a good idea to start with a small number of features. This will
+      help you to avoid overfitting your model. As you become more experienced,
+      you can experiment with adding more features.
 ## Install **Prerequsites:**
    1. featurewiz is built using xgboost, dask, numpy, pandas and matplotlib. It
       should run on most Python 3 Anaconda installations. You won't have to
       import any special libraries other than "dask", "XGBoost" and "networkx"
       library. Optionally, it uses LightGBM for fast modeling, which it
       installs automatically.
    2. We use "networkx" library for charts and interpretability.
       But if you don't have these libraries, featurewiz will install those for
       you automatically.
-- [Anaconda](https://docs.anaconda.com/anaconda/install/) To clone featurewiz,
-it is better to create a new environment, and install the required
-dependencies: To install from PyPi: ``` conda create -n  python=3.7 anaconda
-conda activate  # ON WINDOWS: `source activate ` pip install featurewiz --
-ignore-installed --no-deps pip install lazytransform or pip install git+https:/
-/github.com/AutoViML/featurewiz.git ``` To install from source: ``` cd  git
-clone git@github.com:AutoViML/featurewiz.git # or download and unzip https://
-github.com/AutoViML/featurewiz/archive/master.zip conda create -n  python=3.7
-anaconda conda activate  # ON WINDOWS: `source activate ` cd featurewiz pip
-install -r requirements.txt ``` ## Usage As of Jan 2022, you now invoke
-featurewiz in two ways for two different goals. For feature selection, you must
-use the scikit-learn compatible fit and predict transformer syntax such as
-below. ``` from featurewiz import FeatureWiz features = FeatureWiz
-(corr_limit=0.70, feature_engg='', category_encoders='',
+To install from source: ``` cd  git clone git@github.com:AutoViML/
+featurewiz.git # or download and unzip https://github.com/AutoViML/featurewiz/
+archive/master.zip conda create -n  python=3.7 anaconda conda activate  # ON
+WINDOWS: `source activate ` cd featurewiz pip install -r requirements.txt ```
+## Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
+Check_out_more_latest_updates_from_this_page
+As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo),
+featurewiz is now available on conda-forge. You can try:
+``` conda install -c conda-forge featurewiz ``` ### If the above conda install
+fails, you can try installing featurewiz this way: ##Step 1: Install featurewiz
+first
+``` !pip install featurewiz --ignore-installed --no-deps !pip install xlrd --
+ignore-installed --no-deps ``` ##Step 2: Next, install Pillow since Kaggle has
+an incompatible version.
+``` !pip install Pillow==9.0.0 ``` ## Usage For feature selection, you must use
+the newer syntax which is similar to the scikit-learn fit and predict
+transformer syntax below. ``` from featurewiz import FeatureWiz fwiz =
+FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='',
 dask_xgboost_flag=False, nrows=None, verbose=2) X_train_selected =
-features.fit_transform(X_train, y_train) X_test_selected = features.transform
-(X_test) features.features ### provides the list of selected features ### ```
-Alternatively, you can use featurewiz for feature engineering using this older
-syntax. Otherwise, it will give an error. If you want to combine feature engg
-and then feature selection, you must use this older syntax: ``` import
-featurewiz as FW outputs = FW.featurewiz(dataname=train, target=target,
-corr_limit=0.70, verbose=2, sep=',', header=0, test_data='',feature_engg='',
+fwiz.fit_transform(X_train, y_train) X_test_selected = fwiz.transform(X_test)
+### get list of selected features ### fwiz.features ``` Alternatively, you can
+use featurewiz for feature engineering using this older syntax. Otherwise, it
+will give an error. If you want to combine feature engg and then feature
+selection, you must use this older syntax: ``` import featurewiz as fwiz
+outputs = fwiz.featurewiz(dataname=train, target=target, corr_limit=0.70,
+verbose=2, sep=',', header=0, test_data='',feature_engg='',
 category_encoders='', dask_xgboost_flag=False, nrows=None) ``` `outputs`: There
 will always be multiple objects in output. The objects in that tuple can vary:
-1. "features" and "train": It be a list (of selected features) and one
+1. "features" and "trainm": It be a list (of selected features) and one
 dataframe (if you sent in train only) 2. "trainm" and "testm": It can be two
 dataframes when you send in both test and train but with selected features.
    1. Both the selected features and dataframes are ready for you to now to do
       further modeling.
    2. Featurewiz works on any multi-class, multi-label data Set. So you can
       have as many target labels as you want.
    3. You don't have to tell Featurewiz whether it is a Regression or
@@ -248,22 +229,65 @@
 support, it uses PolynomialWrapper. For feature value i, James-Stein estimator
 returns a weighted average of: The mean target value for the observed feature
 value i. The mean target value (regardless of the feature value). -
 `dask_xgboost_flag`: Default is False. Set to True to use dask_xgboost
 estimator. You can turn it off if it gives an error. Then it will use pandas
 and regular xgboost to do the job. - `nrows`: default `None`. You can set the
 number of rows to read from your datafile if it is too large to fit into either
-dask or pandas. But you won't have to if you use dask. **Return values** -
+dask or pandas. But you won't have to if you use dask. **Output values** -
 `outputs`: Output is always a tuple. We can call our outputs in that tuple:
 out1 and out2. - `out1` and `out2`: If you sent in just one dataframe or
 filename as input, you will get: - 1. `features`: It will be a list (of
 selected features) and - 2. `trainm`: It will be a dataframe (if you sent in a
 file or dataname as input) - `out1` and `out2`: If you sent in two files or
 dataframes (train and test), you will get: - 1. `trainm`: a modified train
 dataframe with engineered and selected features from dataname and - 2. `testm`:
 a modified test dataframe with engineered and selected features from test_data.
+## Additional ![background](featurewiz_background.jpg) To learn more about how
+featurewiz works under the hood, watch this [video](https://www.youtube.com/
+embed/ZiNutwPcAU0)
+featurewiz was designed for selecting High Performance variables with the
+fewest steps. In most cases, featurewiz builds models with 20%-99% fewer
+features than your original data set with nearly the same or slightly lower
+performance (this is based on my trials. Your experience may vary).
+featurewiz is every Data Scientist's feature wizard that will:
+   1. Automatically pre-process data: you can send in your entire dataframe "as
+      is" and featurewiz will classify and change/label encode categorical
+      variables changes to help XGBoost processing. It classifies variables as
+      numeric or categorical or NLP or date-time variables automatically so it
+      can use them correctly to model.
+   2. Perform feature engineering automatically: The ability to create
+      "interaction" variables or adding "group-by" features or "target-
+      encoding" categorical variables is difficult and sifting through those
+      hundreds of new features is painstaking and left only to "experts". Now,
+      with featurewiz you can create hundreds or even thousands of new features
+      with the click of a mouse. This is very helpful when you have a small
+      number of features to start with. However, be careful with this option.
+      You can very easily create a monster with this option.
+   3. Perform feature reduction automatically. When you have small data sets
+      and you know your domain well, it is easy to perhaps do EDA and identify
+      which variables are important. But when you have a very large data set
+      with hundreds if not thousands of variables, selecting the best features
+      from your model can mean the difference between a bloated and highly
+      complex model or a simple model with the fewest and most information-rich
+      features. featurewiz uses XGBoost repeatedly to perform feature
+      selection. You must try it on your large data sets and compare!
+   4. Explain SULOV method graphically using networkx library so you can see
+      which variables are highly correlated to which ones and which of those
+      have high or low mutual information scores automatically. Just set
+      verbose = 2 to see the graph.
+   5. Build a fast XGBoost or LightGBM model using the features selected by
+      featurewiz. There is a function called "simple_lightgbm_model" which you
+      can use to build a fast model. It is a new module, so check it out.
+*** A Note of Gratitude ***:
+   1. Alex Lekov (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/
+      automl_alex) for his DataBunch and encoders modules which are used by the
+      tool (although with some modifications).
+   2. Category Encoders library in Python : This is an amazing library. Make
+      sure you read all about the encoders that featurewiz uses here: https://
+      contrib.scikit-learn.org/category_encoders/index.html
 ## Maintainers * [@AutoViML](https://github.com/AutoViML) ## Contributing See
 [the contributing file](CONTRIBUTING.md)! PRs accepted. ## License Apache
 License 2.0 Â© 2020 Ram Seshadri ## DISCLAIMER This project is not an official
 Google project. It is not supported by Google and Google specifically disclaims
 all warranties as to its quality, merchantability, or fitness for a particular
 purpose.
```

### Comparing `featurewiz-0.2.7/featurewiz/__init__.py` & `featurewiz-0.2.8/featurewiz/__init__.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/classify_method.py` & `featurewiz-0.2.8/featurewiz/classify_method.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/databunch.py` & `featurewiz-0.2.8/featurewiz/databunch.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/encoders.py` & `featurewiz-0.2.8/featurewiz/encoders.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/featurewiz.py` & `featurewiz-0.2.8/featurewiz/featurewiz.py`

 * *Files 0% similar despite different names*

```diff
@@ -4852,5571 +4852,5574 @@
 00012f30: 7320 2b3d 2069 6d70 5f66 6561 7473 5f31  s += imp_feats_1
 00012f40: 5b3a 746f 705f 6e75 6d5d 2e69 6e64 6578  [:top_num].index
 00012f50: 2e74 6f6c 6973 7428 290a 2020 2020 2020  .tolist().      
 00012f60: 2020 2020 2020 2020 2020 7072 696e 7428            print(
 00012f70: 2720 2020 2020 2020 2020 2020 2073 656c  '            sel
 00012f80: 6563 7469 6e67 2025 7320 6665 6174 7572  ecting %s featur
 00012f90: 6573 2069 6e20 7468 6973 2069 7465 7261  es in this itera
-00012fa0: 7469 6f6e 2720 256c 656e 2869 6d70 5f66  tion' %len(imp_f
-00012fb0: 6561 7473 5f31 5b3a 746f 705f 6e75 6d5d  eats_1[:top_num]
-00012fc0: 2929 0a20 2020 2020 2020 2020 2020 2065  )).            e
-00012fd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00012fe0: 2020 2020 2070 7269 6e74 2827 2020 2020       print('    
-00012ff0: 2020 2020 2020 2020 5365 6c65 6374 696e          Selectin
-00013000: 6720 616c 6c20 6665 6174 7572 6573 2e2e  g all features..
-00013010: 2e27 290a 2020 2020 2020 2020 2020 2020  .').            
-00013020: 2020 2020 2370 7269 6e74 2827 2020 2020      #print('    
-00013030: 2020 2020 2020 2020 2020 2020 4361 7574              Caut
-00013040: 696f 6e3a 2074 6865 7920 6d69 6768 7420  ion: they might 
-00013050: 6265 206c 6f77 2d71 7561 6c69 7479 2066  be low-quality f
-00013060: 6561 7475 7265 732e 2e2e 2729 0a20 2020  eatures...').   
-00013070: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
-00013080: 5f66 6561 7473 5f31 203d 2020 7064 2e53  _feats_1 =  pd.S
-00013090: 6572 6965 7328 696d 705f 6665 6174 7329  eries(imp_feats)
-000130a0: 2e73 6f72 745f 7661 6c75 6573 2861 7363  .sort_values(asc
-000130b0: 656e 6469 6e67 3d46 616c 7365 290a 2020  ending=False).  
-000130c0: 2020 2020 2020 2020 2020 2020 2020 696d                im
-000130d0: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
-000130e0: 202b 3d20 696d 705f 6665 6174 735f 315b   += imp_feats_1[
-000130f0: 3a5d 2e69 6e64 6578 2e74 6f6c 6973 7428  :].index.tolist(
-00013100: 290a 2020 2020 2020 2020 2020 2020 2323  ).            ##
-00013110: 2323 2323 2320 206f 7264 6572 2074 6869  #####  order thi
-00013120: 7320 696e 2074 6865 2073 616d 6520 6f72  s in the same or
-00013130: 6465 7220 696e 2077 6869 6368 2074 6865  der in which the
-00013140: 7920 7765 7265 2063 6f6c 6c65 6374 6564  y were collected
-00013150: 2023 2323 2323 230a 2020 2020 2020 2020   ######.        
-00013160: 2020 2020 696d 706f 7274 616e 745f 6665      important_fe
-00013170: 6174 7572 6573 203d 206c 6973 7428 4f72  atures = list(Or
-00013180: 6465 7265 6444 6963 742e 6672 6f6d 6b65  deredDict.fromke
-00013190: 7973 2869 6d70 6f72 7461 6e74 5f66 6561  ys(important_fea
-000131a0: 7475 7265 7329 290a 2020 2020 2020 2020  tures)).        
-000131b0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-000131c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131d0: 6966 2064 6173 6b5f 7867 626f 6f73 745f  if dask_xgboost_
-000131e0: 666c 6167 3a0a 2020 2020 2020 2020 2020  flag:.          
-000131f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00013200: 2720 2020 2020 2020 2020 2020 2054 696d  '            Tim
-00013210: 6520 7461 6b65 6e20 666f 7220 4441 534b  e taken for DASK
-00013220: 2058 4742 6f6f 7374 2066 6561 7475 7265   XGBoost feature
-00013230: 2073 656c 6563 7469 6f6e 203d 2025 302e   selection = %0.
-00013240: 3066 2073 6563 6f6e 6473 2720 2528 7469  0f seconds' %(ti
-00013250: 6d65 2e74 696d 6528 292d 7374 6172 745f  me.time()-start_
-00013260: 7469 6d65 3229 290a 2020 2020 2020 2020  time2)).        
-00013270: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2020 7072 696e 7428 2720 2020 2020 2020    print('       
-000132a0: 2020 2020 2054 696d 6520 7461 6b65 6e20       Time taken 
-000132b0: 666f 7220 7265 6775 6c61 7220 5847 426f  for regular XGBo
-000132c0: 6f73 7420 6665 6174 7572 6520 7365 6c65  ost feature sele
-000132d0: 6374 696f 6e20 3d20 2530 2e30 6620 7365  ction = %0.0f se
-000132e0: 636f 6e64 7327 2025 2874 696d 652e 7469  conds' %(time.ti
-000132f0: 6d65 2829 2d73 7461 7274 5f74 696d 6532  me()-start_time2
-00013300: 2929 0a20 2020 2020 2020 2023 2323 2320  )).        #### 
-00013310: 706c 6f74 2061 6c6c 2074 6865 2066 6561  plot all the fea
-00013320: 7475 7265 2069 6d70 6f72 7461 6e63 6573  ture importances
-00013330: 2069 6e20 6120 6772 6964 2023 2323 2323   in a grid #####
-00013340: 2323 2323 2323 0a20 2020 2020 2020 2069  ######.        i
-00013350: 6620 7665 7262 6f73 6520 3e3d 2032 3a0a  f verbose >= 2:.
-00013360: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00013370: 6574 7469 6e67 732e 6d75 6c74 695f 6c61  ettings.multi_la
-00013380: 6265 6c3a 0a20 2020 2020 2020 2020 2020  bel:.           
-00013390: 2020 2020 2064 7261 775f 6665 6174 7572       draw_featur
-000133a0: 655f 696d 706f 7274 616e 6365 735f 6d75  e_importances_mu
-000133b0: 6c74 695f 6c61 6265 6c28 6273 745f 6d6f  lti_label(bst_mo
-000133c0: 6465 6c73 2c20 6461 736b 5f78 6762 6f6f  dels, dask_xgboo
-000133d0: 7374 5f66 6c61 6729 0a20 2020 2020 2020  st_flag).       
-000133e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000133f0: 2020 2020 2020 2020 2020 2064 7261 775f             draw_
-00013400: 6665 6174 7572 655f 696d 706f 7274 616e  feature_importan
-00013410: 6365 735f 7369 6e67 6c65 5f6c 6162 656c  ces_single_label
-00013420: 2862 7374 5f6d 6f64 656c 732c 2064 6173  (bst_models, das
-00013430: 6b5f 7867 626f 6f73 745f 666c 6167 290a  k_xgboost_flag).
-00013440: 2020 2020 2020 2020 696d 706f 7274 616e          importan
-00013450: 745f 6665 6174 7572 6573 203d 206c 6973  t_features = lis
-00013460: 7428 4f72 6465 7265 6444 6963 742e 6672  t(OrderedDict.fr
-00013470: 6f6d 6b65 7973 2869 6d70 6f72 7461 6e74  omkeys(important
-00013480: 5f66 6561 7475 7265 7329 290a 2020 2020  _features)).    
-00013490: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000134a0: 2061 7320 653a 0a20 2020 2020 2020 2069   as e:.        i
-000134b0: 6620 6461 736b 5f78 6762 6f6f 7374 5f66  f dask_xgboost_f
-000134c0: 6c61 673a 0a20 2020 2020 2020 2020 2020  lag:.           
-000134d0: 2070 7269 6e74 2827 4461 736b 2058 4742   print('Dask XGB
-000134e0: 6f6f 7374 2069 7320 6372 6173 6869 6e67  oost is crashing
-000134f0: 2064 7565 2074 6f20 2573 2e20 5265 7475   due to %s. Retu
-00013500: 726e 696e 6720 7769 7468 2063 7572 7265  rning with curre
-00013510: 6e74 6c79 2073 656c 6563 7465 6420 6665  ntly selected fe
-00013520: 6174 7572 6573 2e2e 2e27 2025 6529 0a20  atures...' %e). 
-00013530: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00013540: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00013550: 5265 6775 6c61 7220 5847 426f 6f73 7420  Regular XGBoost 
-00013560: 6973 2063 7261 7368 696e 6720 6475 6520  is crashing due 
-00013570: 746f 2025 732e 2052 6574 7572 6e69 6e67  to %s. Returning
-00013580: 2077 6974 6820 6375 7272 656e 746c 7920   with currently 
-00013590: 7365 6c65 6374 6564 2066 6561 7475 7265  selected feature
-000135a0: 732e 2e2e 2720 2565 290a 2020 2020 2020  s...' %e).      
-000135b0: 2020 696d 706f 7274 616e 745f 6665 6174    important_feat
-000135c0: 7572 6573 203d 2063 6f70 792e 6465 6570  ures = copy.deep
-000135d0: 636f 7079 2870 7265 6473 290a 2020 2020  copy(preds).    
-000135e0: 2323 2323 2323 2020 2020 4520 2020 204e  ######    E    N
-000135f0: 2020 2020 2044 2020 2020 2020 4f20 2046       D      O  F
-00013600: 2020 2020 2020 5820 2047 2020 4220 204f        X  G  B  O
-00013610: 2020 4f20 2053 2020 5420 2020 2053 2045    O  S  T    S E
-00013620: 204c 2045 2043 2054 2049 204f 204e 2023   L E C T I O N #
-00013630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013640: 2323 230a 2020 2020 7072 696e 7428 2720  ###.    print(' 
-00013650: 2020 2043 6f6d 706c 6574 6564 2058 4742     Completed XGB
-00013660: 6f6f 7374 2066 6561 7475 7265 2073 656c  oost feature sel
-00013670: 6563 7469 6f6e 2069 6e20 2530 2e30 6620  ection in %0.0f 
-00013680: 7365 636f 6e64 7327 2025 2874 696d 652e  seconds' %(time.
-00013690: 7469 6d65 2829 2d73 7461 7274 5f74 696d  time()-start_tim
-000136a0: 6532 2929 0a20 2020 2069 6620 6c65 6e28  e2)).    if len(
-000136b0: 6964 636f 6c73 2920 3e20 303a 0a20 2020  idcols) > 0:.   
-000136c0: 2020 2020 2070 7269 6e74 2827 2020 2020       print('    
-000136d0: 416c 6572 743a 204e 6f20 4944 2076 6172  Alert: No ID var
-000136e0: 6961 626c 6573 2025 7320 6172 6520 696e  iables %s are in
-000136f0: 636c 7564 6564 2069 6e20 7365 6c65 6374  cluded in select
-00013700: 6564 2066 6561 7475 7265 7327 2025 6964  ed features' %id
-00013710: 636f 6c73 290a 2020 2020 7072 696e 7428  cols).    print(
-00013720: 2223 2323 2323 2323 2323 2323 2323 2323  "###############
-00013730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012fa0: 7469 6f6e 2720 2574 6f70 5f6e 756d 290a  tion' %top_num).
+00012fb0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00012fc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012fd0: 2020 7072 696e 7428 2720 2020 2020 2020    print('       
+00012fe0: 2020 2020 2053 656c 6563 7469 6e67 2025       Selecting %
+00012ff0: 7320 6665 6174 7572 6573 2066 726f 6d20  s features from 
+00013000: 7468 6973 2069 7465 7261 7469 6f6e 2e2e  this iteration..
+00013010: 2e27 2025 746f 705f 6e75 6d29 0a20 2020  .' %top_num).   
+00013020: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00013030: 6e74 2827 2020 2020 2020 2020 2020 2020  nt('            
+00013040: 2020 2020 4361 7574 696f 6e3a 2074 6865      Caution: the
+00013050: 7920 6d69 6768 7420 6265 206c 6f77 2d71  y might be low-q
+00013060: 7561 6c69 7479 2066 6561 7475 7265 7320  uality features 
+00013070: 7369 6e63 6520 7468 6569 7220 462d 7363  since their F-sc
+00013080: 6f72 6520 6973 206c 6573 7320 7468 616e  ore is less than
+00013090: 2031 2e2e 2e27 290a 2020 2020 2020 2020   1...').        
+000130a0: 2020 2020 2020 2020 696d 705f 6665 6174          imp_feat
+000130b0: 735f 3120 3d20 2070 642e 5365 7269 6573  s_1 =  pd.Series
+000130c0: 2869 6d70 5f66 6561 7473 292e 736f 7274  (imp_feats).sort
+000130d0: 5f76 616c 7565 7328 6173 6365 6e64 696e  _values(ascendin
+000130e0: 673d 4661 6c73 6529 0a20 2020 2020 2020  g=False).       
+000130f0: 2020 2020 2020 2020 2069 6d70 6f72 7461           importa
+00013100: 6e74 5f66 6561 7475 7265 7320 2b3d 2069  nt_features += i
+00013110: 6d70 5f66 6561 7473 5f31 5b3a 746f 705f  mp_feats_1[:top_
+00013120: 6e75 6d5d 2e69 6e64 6578 2e74 6f6c 6973  num].index.tolis
+00013130: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00013140: 2323 2323 2323 2320 206f 7264 6572 2074  #######  order t
+00013150: 6869 7320 696e 2074 6865 2073 616d 6520  his in the same 
+00013160: 6f72 6465 7220 696e 2077 6869 6368 2074  order in which t
+00013170: 6865 7920 7765 7265 2063 6f6c 6c65 6374  hey were collect
+00013180: 6564 2023 2323 2323 230a 2020 2020 2020  ed ######.      
+00013190: 2020 2020 2020 696d 706f 7274 616e 745f        important_
+000131a0: 6665 6174 7572 6573 203d 206c 6973 7428  features = list(
+000131b0: 4f72 6465 7265 6444 6963 742e 6672 6f6d  OrderedDict.from
+000131c0: 6b65 7973 2869 6d70 6f72 7461 6e74 5f66  keys(important_f
+000131d0: 6561 7475 7265 7329 290a 2020 2020 2020  eatures)).      
+000131e0: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+000131f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013200: 2020 6966 2064 6173 6b5f 7867 626f 6f73    if dask_xgboos
+00013210: 745f 666c 6167 3a0a 2020 2020 2020 2020  t_flag:.        
+00013220: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00013230: 7428 2720 2020 2020 2020 2020 2020 2054  t('            T
+00013240: 696d 6520 7461 6b65 6e20 666f 7220 4441  ime taken for DA
+00013250: 534b 2058 4742 6f6f 7374 2066 6561 7475  SK XGBoost featu
+00013260: 7265 2073 656c 6563 7469 6f6e 203d 2025  re selection = %
+00013270: 302e 3066 2073 6563 6f6e 6473 2720 2528  0.0f seconds' %(
+00013280: 7469 6d65 2e74 696d 6528 292d 7374 6172  time.time()-star
+00013290: 745f 7469 6d65 3229 290a 2020 2020 2020  t_time2)).      
+000132a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132c0: 2020 2020 7072 696e 7428 2720 2020 2020      print('     
+000132d0: 2020 2020 2020 2054 696d 6520 7461 6b65         Time take
+000132e0: 6e20 666f 7220 7265 6775 6c61 7220 5847  n for regular XG
+000132f0: 426f 6f73 7420 6665 6174 7572 6520 7365  Boost feature se
+00013300: 6c65 6374 696f 6e20 3d20 2530 2e30 6620  lection = %0.0f 
+00013310: 7365 636f 6e64 7327 2025 2874 696d 652e  seconds' %(time.
+00013320: 7469 6d65 2829 2d73 7461 7274 5f74 696d  time()-start_tim
+00013330: 6532 2929 0a20 2020 2020 2020 2023 2323  e2)).        ###
+00013340: 2320 706c 6f74 2061 6c6c 2074 6865 2066  # plot all the f
+00013350: 6561 7475 7265 2069 6d70 6f72 7461 6e63  eature importanc
+00013360: 6573 2069 6e20 6120 6772 6964 2023 2323  es in a grid ###
+00013370: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+00013380: 2069 6620 7665 7262 6f73 6520 3e3d 2032   if verbose >= 2
+00013390: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000133a0: 2073 6574 7469 6e67 732e 6d75 6c74 695f   settings.multi_
+000133b0: 6c61 6265 6c3a 0a20 2020 2020 2020 2020  label:.         
+000133c0: 2020 2020 2020 2064 7261 775f 6665 6174         draw_feat
+000133d0: 7572 655f 696d 706f 7274 616e 6365 735f  ure_importances_
+000133e0: 6d75 6c74 695f 6c61 6265 6c28 6273 745f  multi_label(bst_
+000133f0: 6d6f 6465 6c73 2c20 6461 736b 5f78 6762  models, dask_xgb
+00013400: 6f6f 7374 5f66 6c61 6729 0a20 2020 2020  oost_flag).     
+00013410: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013420: 2020 2020 2020 2020 2020 2020 2064 7261               dra
+00013430: 775f 6665 6174 7572 655f 696d 706f 7274  w_feature_import
+00013440: 616e 6365 735f 7369 6e67 6c65 5f6c 6162  ances_single_lab
+00013450: 656c 2862 7374 5f6d 6f64 656c 732c 2064  el(bst_models, d
+00013460: 6173 6b5f 7867 626f 6f73 745f 666c 6167  ask_xgboost_flag
+00013470: 290a 2020 2020 2020 2020 696d 706f 7274  ).        import
+00013480: 616e 745f 6665 6174 7572 6573 203d 206c  ant_features = l
+00013490: 6973 7428 4f72 6465 7265 6444 6963 742e  ist(OrderedDict.
+000134a0: 6672 6f6d 6b65 7973 2869 6d70 6f72 7461  fromkeys(importa
+000134b0: 6e74 5f66 6561 7475 7265 7329 290a 2020  nt_features)).  
+000134c0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+000134d0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+000134e0: 2069 6620 6461 736b 5f78 6762 6f6f 7374   if dask_xgboost
+000134f0: 5f66 6c61 673a 0a20 2020 2020 2020 2020  _flag:.         
+00013500: 2020 2070 7269 6e74 2827 4461 736b 2058     print('Dask X
+00013510: 4742 6f6f 7374 2069 7320 6372 6173 6869  GBoost is crashi
+00013520: 6e67 2064 7565 2074 6f20 2573 2e20 5265  ng due to %s. Re
+00013530: 7475 726e 696e 6720 7769 7468 2063 7572  turning with cur
+00013540: 7265 6e74 6c79 2073 656c 6563 7465 6420  rently selected 
+00013550: 6665 6174 7572 6573 2e2e 2e27 2025 6529  features...' %e)
+00013560: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00013570: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00013580: 2827 5265 6775 6c61 7220 5847 426f 6f73  ('Regular XGBoos
+00013590: 7420 6973 2063 7261 7368 696e 6720 6475  t is crashing du
+000135a0: 6520 746f 2025 732e 2052 6574 7572 6e69  e to %s. Returni
+000135b0: 6e67 2077 6974 6820 6375 7272 656e 746c  ng with currentl
+000135c0: 7920 7365 6c65 6374 6564 2066 6561 7475  y selected featu
+000135d0: 7265 732e 2e2e 2720 2565 290a 2020 2020  res...' %e).    
+000135e0: 2020 2020 696d 706f 7274 616e 745f 6665      important_fe
+000135f0: 6174 7572 6573 203d 2063 6f70 792e 6465  atures = copy.de
+00013600: 6570 636f 7079 2870 7265 6473 290a 2020  epcopy(preds).  
+00013610: 2020 2323 2323 2323 2020 2020 4520 2020    ######    E   
+00013620: 204e 2020 2020 2044 2020 2020 2020 4f20   N     D      O 
+00013630: 2046 2020 2020 2020 5820 2047 2020 4220   F      X  G  B 
+00013640: 204f 2020 4f20 2053 2020 5420 2020 2053   O  O  S  T    S
+00013650: 2045 204c 2045 2043 2054 2049 204f 204e   E L E C T I O N
+00013660: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00013670: 2323 2323 230a 2020 2020 7072 696e 7428  #####.    print(
+00013680: 2720 2020 2043 6f6d 706c 6574 6564 2058  '    Completed X
+00013690: 4742 6f6f 7374 2066 6561 7475 7265 2073  GBoost feature s
+000136a0: 656c 6563 7469 6f6e 2069 6e20 2530 2e30  election in %0.0
+000136b0: 6620 7365 636f 6e64 7327 2025 2874 696d  f seconds' %(tim
+000136c0: 652e 7469 6d65 2829 2d73 7461 7274 5f74  e.time()-start_t
+000136d0: 696d 6532 2929 0a20 2020 2069 6620 6c65  ime2)).    if le
+000136e0: 6e28 6964 636f 6c73 2920 3e20 303a 0a20  n(idcols) > 0:. 
+000136f0: 2020 2020 2020 2070 7269 6e74 2827 2020         print('  
+00013700: 2020 416c 6572 743a 204e 6f20 4944 2076    Alert: No ID v
+00013710: 6172 6961 626c 6573 2025 7320 6172 6520  ariables %s are 
+00013720: 696e 636c 7564 6564 2069 6e20 7365 6c65  included in sele
+00013730: 6374 6564 2066 6561 7475 7265 7327 2025  cted features' %
+00013740: 6964 636f 6c73 290a 2020 2020 7072 696e  idcols).    prin
+00013750: 7428 2223 2323 2323 2323 2323 2323 2323  t("#############
 00013760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013770: 2323 2323 2323 2323 2229 0a20 2020 2070  ########").    p
-00013780: 7269 6e74 2822 2323 2323 2320 2020 2020  rint("#####     
-00013790: 2020 2020 2046 2045 2041 2054 2055 2052       F E A T U R
-000137a0: 2045 2020 2053 2045 204c 2045 2043 2054   E   S E L E C T
-000137b0: 2049 204f 204e 2020 2043 204f 204d 2050   I O N   C O M P
-000137c0: 204c 2045 2054 2045 2044 2020 2020 2020   L E T E D      
-000137d0: 2020 2020 2020 2323 2323 2323 2322 290a        #######").
-000137e0: 2020 2020 7072 696e 7428 2223 2323 2323      print("#####
-000137f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000137a0: 2323 2323 2323 2323 2323 2229 0a20 2020  ##########").   
+000137b0: 2070 7269 6e74 2822 2323 2323 2320 2020   print("#####   
+000137c0: 2020 2020 2020 2046 2045 2041 2054 2055         F E A T U
+000137d0: 2052 2045 2020 2053 2045 204c 2045 2043   R E   S E L E C
+000137e0: 2054 2049 204f 204e 2020 2043 204f 204d   T I O N   C O M
+000137f0: 2050 204c 2045 2054 2045 2044 2020 2020   P L E T E D    
+00013800: 2020 2020 2020 2020 2323 2323 2323 2322          #######"
+00013810: 290a 2020 2020 7072 696e 7428 2223 2323  ).    print("###
 00013820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00013830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013840: 2323 2229 0a20 2020 2064 6963 746f 203d  ##").    dicto =
-00013850: 207b 7d0a 2020 2020 6d69 7373 696e 675f   {}.    missing_
-00013860: 666c 6167 7331 203d 205b 7b78 3a78 5b3a  flags1 = [{x:x[:
-00013870: 2d31 335d 7d20 666f 7220 7820 696e 2069  -13]} for x in i
-00013880: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-00013890: 7320 6966 2027 4d69 7373 696e 675f 466c  s if 'Missing_Fl
-000138a0: 6167 2720 696e 2078 5d0a 2020 2020 666f  ag' in x].    fo
-000138b0: 7220 6561 6368 5f66 6c61 6720 696e 206d  r each_flag in m
-000138c0: 6973 7369 6e67 5f66 6c61 6773 313a 0a20  issing_flags1:. 
-000138d0: 2020 2020 2020 2070 7269 6e74 2827 416c         print('Al
-000138e0: 6572 743a 2044 6f6e 7420 666f 7267 6574  ert: Dont forget
-000138f0: 2074 6f20 6164 6420 6120 6d69 7373 696e   to add a missin
-00013900: 6720 666c 6167 2074 6f20 2573 2074 6f20  g flag to %s to 
-00013910: 6372 6561 7465 2025 7320 636f 6c75 6d6e  create %s column
-00013920: 2720 2528 6c69 7374 2865 6163 685f 666c  ' %(list(each_fl
-00013930: 6167 2e76 616c 7565 7328 2929 5b30 5d2c  ag.values())[0],
-00013940: 206c 6973 7428 6561 6368 5f66 6c61 672e   list(each_flag.
-00013950: 6b65 7973 2829 295b 305d 2929 0a20 2020  keys())[0])).   
-00013960: 2020 2020 2064 6963 746f 2e75 7064 6174       dicto.updat
-00013970: 6528 6561 6368 5f66 6c61 6729 0a20 2020  e(each_flag).   
-00013980: 2069 6620 6c65 6e28 6469 6374 6f29 203e   if len(dicto) >
-00013990: 2030 3a0a 2020 2020 2020 2020 696d 706f   0:.        impo
-000139a0: 7274 616e 745f 6665 6174 7572 6573 203d  rtant_features =
-000139b0: 2020 5b64 6963 746f 2e67 6574 2869 7465    [dicto.get(ite
-000139c0: 6d2c 6974 656d 2920 2066 6f72 2069 7465  m,item)  for ite
-000139d0: 6d20 696e 2069 6d70 6f72 7461 6e74 5f66  m in important_f
-000139e0: 6561 7475 7265 735d 0a20 2020 2069 6620  eatures].    if 
-000139f0: 6c65 6e28 696d 706f 7274 616e 745f 6665  len(important_fe
-00013a00: 6174 7572 6573 2920 3c3d 2033 303a 0a20  atures) <= 30:. 
-00013a10: 2020 2020 2020 2070 7269 6e74 2827 5365         print('Se
-00013a20: 6c65 6374 6564 2025 6420 696d 706f 7274  lected %d import
-00013a30: 616e 7420 6665 6174 7572 6573 3a5c 6e25  ant features:\n%
-00013a40: 7327 2025 286c 656e 2869 6d70 6f72 7461  s' %(len(importa
-00013a50: 6e74 5f66 6561 7475 7265 7329 2c20 696d  nt_features), im
-00013a60: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
-00013a70: 2929 0a20 2020 2065 6c73 653a 0a20 2020  )).    else:.   
-00013a80: 2020 2020 2070 7269 6e74 2827 5365 6c65       print('Sele
-00013a90: 6374 6564 2025 6420 696d 706f 7274 616e  cted %d importan
-00013aa0: 7420 6665 6174 7572 6573 2e20 546f 6f20  t features. Too 
-00013ab0: 6d61 6e79 2074 6f20 7072 696e 742e 2e2e  many to print...
-00013ac0: 2720 256c 656e 2869 6d70 6f72 7461 6e74  ' %len(important
-00013ad0: 5f66 6561 7475 7265 7329 290a 2020 2020  _features)).    
-00013ae0: 6e75 6d76 6172 7320 3d20 5b78 2066 6f72  numvars = [x for
-00013af0: 2078 2069 6e20 6e75 6d76 6172 7320 6966   x in numvars if
-00013b00: 2078 2069 6e20 696d 706f 7274 616e 745f   x in important_
-00013b10: 6665 6174 7572 6573 5d0a 2020 2020 696d  features].    im
-00013b20: 706f 7274 616e 745f 6361 7473 203d 205b  portant_cats = [
-00013b30: 7820 666f 7220 7820 696e 2069 6d70 6f72  x for x in impor
-00013b40: 7461 6e74 5f63 6174 7320 6966 2078 2069  tant_cats if x i
-00013b50: 6e20 696d 706f 7274 616e 745f 6665 6174  n important_feat
-00013b60: 7572 6573 5d0a 2020 2020 7072 696e 7428  ures].    print(
-00013b70: 2754 6f74 616c 2054 696d 6520 7461 6b65  'Total Time take
-00013b80: 6e20 666f 7220 6665 6174 7572 6577 697a  n for featurewiz
-00013b90: 2073 656c 6563 7469 6f6e 203d 2025 302e   selection = %0.
-00013ba0: 3066 2073 6563 6f6e 6473 2720 2528 7469  0f seconds' %(ti
-00013bb0: 6d65 2e74 696d 6528 292d 7374 6172 745f  me.time()-start_
-00013bc0: 7469 6d65 2929 0a20 2020 2023 2323 2320  time)).    #### 
-00013bd0: 4e6f 7720 6368 616e 6765 2074 6865 2066  Now change the f
-00013be0: 6561 7475 7265 206e 616d 6573 2062 6163  eature names bac
-00013bf0: 6b20 746f 206f 7269 6769 6e61 6c20 6665  k to original fe
-00013c00: 6174 7572 6520 6e61 6d65 7320 2323 2323  ature names ####
-00013c10: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-00013c20: 2069 7465 6d5f 7265 706c 6163 6572 203d   item_replacer =
-00013c30: 2063 6f6c 5f6e 616d 655f 6d61 7070 6572   col_name_mapper
-00013c40: 2e67 6574 2020 2320 466f 7220 6661 7374  .get  # For fast
-00013c50: 6572 2067 6574 732e 0a20 2020 2023 2323  er gets..    ###
-00013c60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013870: 2323 2323 2229 0a20 2020 2064 6963 746f  ####").    dicto
+00013880: 203d 207b 7d0a 2020 2020 6d69 7373 696e   = {}.    missin
+00013890: 675f 666c 6167 7331 203d 205b 7b78 3a78  g_flags1 = [{x:x
+000138a0: 5b3a 2d31 335d 7d20 666f 7220 7820 696e  [:-13]} for x in
+000138b0: 2069 6d70 6f72 7461 6e74 5f66 6561 7475   important_featu
+000138c0: 7265 7320 6966 2027 4d69 7373 696e 675f  res if 'Missing_
+000138d0: 466c 6167 2720 696e 2078 5d0a 2020 2020  Flag' in x].    
+000138e0: 666f 7220 6561 6368 5f66 6c61 6720 696e  for each_flag in
+000138f0: 206d 6973 7369 6e67 5f66 6c61 6773 313a   missing_flags1:
+00013900: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+00013910: 416c 6572 743a 2044 6f6e 7420 666f 7267  Alert: Dont forg
+00013920: 6574 2074 6f20 6164 6420 6120 6d69 7373  et to add a miss
+00013930: 696e 6720 666c 6167 2074 6f20 2573 2074  ing flag to %s t
+00013940: 6f20 6372 6561 7465 2025 7320 636f 6c75  o create %s colu
+00013950: 6d6e 2720 2528 6c69 7374 2865 6163 685f  mn' %(list(each_
+00013960: 666c 6167 2e76 616c 7565 7328 2929 5b30  flag.values())[0
+00013970: 5d2c 206c 6973 7428 6561 6368 5f66 6c61  ], list(each_fla
+00013980: 672e 6b65 7973 2829 295b 305d 2929 0a20  g.keys())[0])). 
+00013990: 2020 2020 2020 2064 6963 746f 2e75 7064         dicto.upd
+000139a0: 6174 6528 6561 6368 5f66 6c61 6729 0a20  ate(each_flag). 
+000139b0: 2020 2069 6620 6c65 6e28 6469 6374 6f29     if len(dicto)
+000139c0: 203e 2030 3a0a 2020 2020 2020 2020 696d   > 0:.        im
+000139d0: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
+000139e0: 203d 2020 5b64 6963 746f 2e67 6574 2869   =  [dicto.get(i
+000139f0: 7465 6d2c 6974 656d 2920 2066 6f72 2069  tem,item)  for i
+00013a00: 7465 6d20 696e 2069 6d70 6f72 7461 6e74  tem in important
+00013a10: 5f66 6561 7475 7265 735d 0a20 2020 2069  _features].    i
+00013a20: 6620 6c65 6e28 696d 706f 7274 616e 745f  f len(important_
+00013a30: 6665 6174 7572 6573 2920 3c3d 2033 303a  features) <= 30:
+00013a40: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+00013a50: 5365 6c65 6374 6564 2025 6420 696d 706f  Selected %d impo
+00013a60: 7274 616e 7420 6665 6174 7572 6573 3a5c  rtant features:\
+00013a70: 6e25 7327 2025 286c 656e 2869 6d70 6f72  n%s' %(len(impor
+00013a80: 7461 6e74 5f66 6561 7475 7265 7329 2c20  tant_features), 
+00013a90: 696d 706f 7274 616e 745f 6665 6174 7572  important_featur
+00013aa0: 6573 2929 0a20 2020 2065 6c73 653a 0a20  es)).    else:. 
+00013ab0: 2020 2020 2020 2070 7269 6e74 2827 5365         print('Se
+00013ac0: 6c65 6374 6564 2025 6420 696d 706f 7274  lected %d import
+00013ad0: 616e 7420 6665 6174 7572 6573 2e20 546f  ant features. To
+00013ae0: 6f20 6d61 6e79 2074 6f20 7072 696e 742e  o many to print.
+00013af0: 2e2e 2720 256c 656e 2869 6d70 6f72 7461  ..' %len(importa
+00013b00: 6e74 5f66 6561 7475 7265 7329 290a 2020  nt_features)).  
+00013b10: 2020 6e75 6d76 6172 7320 3d20 5b78 2066    numvars = [x f
+00013b20: 6f72 2078 2069 6e20 6e75 6d76 6172 7320  or x in numvars 
+00013b30: 6966 2078 2069 6e20 696d 706f 7274 616e  if x in importan
+00013b40: 745f 6665 6174 7572 6573 5d0a 2020 2020  t_features].    
+00013b50: 696d 706f 7274 616e 745f 6361 7473 203d  important_cats =
+00013b60: 205b 7820 666f 7220 7820 696e 2069 6d70   [x for x in imp
+00013b70: 6f72 7461 6e74 5f63 6174 7320 6966 2078  ortant_cats if x
+00013b80: 2069 6e20 696d 706f 7274 616e 745f 6665   in important_fe
+00013b90: 6174 7572 6573 5d0a 2020 2020 7072 696e  atures].    prin
+00013ba0: 7428 2754 6f74 616c 2054 696d 6520 7461  t('Total Time ta
+00013bb0: 6b65 6e20 666f 7220 6665 6174 7572 6577  ken for featurew
+00013bc0: 697a 2073 656c 6563 7469 6f6e 203d 2025  iz selection = %
+00013bd0: 302e 3066 2073 6563 6f6e 6473 2720 2528  0.0f seconds' %(
+00013be0: 7469 6d65 2e74 696d 6528 292d 7374 6172  time.time()-star
+00013bf0: 745f 7469 6d65 2929 0a20 2020 2023 2323  t_time)).    ###
+00013c00: 2320 4e6f 7720 6368 616e 6765 2074 6865  # Now change the
+00013c10: 2066 6561 7475 7265 206e 616d 6573 2062   feature names b
+00013c20: 6163 6b20 746f 206f 7269 6769 6e61 6c20  ack to original 
+00013c30: 6665 6174 7572 6520 6e61 6d65 7320 2323  feature names ##
+00013c40: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+00013c50: 2020 2069 7465 6d5f 7265 706c 6163 6572     item_replacer
+00013c60: 203d 2063 6f6c 5f6e 616d 655f 6d61 7070   = col_name_mapp
+00013c70: 6572 2e67 6574 2020 2320 466f 7220 6661  er.get  # For fa
+00013c80: 7374 6572 2067 6574 732e 0a20 2020 2023  ster gets..    #
 00013c90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013ca0: 2323 2323 2323 230a 2020 2020 2323 2320  #######.    ### 
-00013cb0: 596f 7520 7365 6c65 6374 2074 6865 2066  You select the f
-00013cc0: 6561 7475 7265 7320 7769 7468 2074 6865  eatures with the
-00013cd0: 2073 616d 6520 6f6c 6420 6e61 6d65 7320   same old names 
-00013ce0: 6173 2062 6566 6f72 6520 6865 7265 2023  as before here #
-00013cf0: 2323 2323 2323 0a20 2020 2023 2323 2323  ######.    #####
-00013d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013ca0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013cd0: 2323 2323 2323 2323 230a 2020 2020 2323  #########.    ##
+00013ce0: 2320 596f 7520 7365 6c65 6374 2074 6865  # You select the
+00013cf0: 2066 6561 7475 7265 7320 7769 7468 2074   features with t
+00013d00: 6865 2073 616d 6520 6f6c 6420 6e61 6d65  he same old name
+00013d10: 7320 6173 2062 6566 6f72 6520 6865 7265  s as before here
+00013d20: 2023 2323 2323 2323 0a20 2020 2023 2323   #######.    ###
 00013d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00013d40: 2323 2323 230a 2020 2020 2323 2049 6e20  #####.    ## In 
-00013d50: 6f6e 6520 6361 7365 2c20 636f 6c75 6d6e  one case, column
-00013d60: 206e 616d 6573 2067 6574 2063 6861 6e67   names get chang
-00013d70: 6564 2069 6e20 7472 6169 6e20 6275 7420  ed in train but 
-00013d80: 6e6f 7420 696e 2074 6573 7420 7369 6e63  not in test sinc
-00013d90: 6520 6974 2074 6573 7420 6973 206e 6f74  e it test is not
-00013da0: 2061 7661 696c 6162 6c65 2e0a 2020 2020   available..    
-00013db0: 6966 2069 7369 6e73 7461 6e63 6528 7465  if isinstance(te
-00013dc0: 7374 5f64 6174 612c 2073 7472 2920 6f72  st_data, str) or
-00013dd0: 2074 6573 745f 6461 7461 2069 7320 4e6f   test_data is No
-00013de0: 6e65 3a0a 2020 2020 2020 2020 7072 696e  ne:.        prin
-00013df0: 7428 274f 7574 7075 7420 636f 6e74 6169  t('Output contai
-00013e00: 6e73 2061 206c 6973 7420 6f66 2025 7320  ns a list of %s 
-00013e10: 696d 706f 7274 616e 7420 6665 6174 7572  important featur
-00013e20: 6573 2061 6e64 2061 2074 7261 696e 2064  es and a train d
-00013e30: 6174 6166 7261 6d65 2720 256c 656e 2869  ataframe' %len(i
-00013e40: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-00013e50: 7329 290a 2020 2020 656c 7365 3a0a 2020  s)).    else:.  
-00013e60: 2020 2020 2020 7072 696e 7428 274f 7574        print('Out
-00013e70: 7075 7420 636f 6e74 6169 6e73 2074 776f  put contains two
-00013e80: 2064 6174 6166 7261 6d65 733a 2074 7261   dataframes: tra
-00013e90: 696e 2061 6e64 2074 6573 7420 7769 7468  in and test with
-00013ea0: 2025 6420 696d 706f 7274 616e 7420 6665   %d important fe
-00013eb0: 6174 7572 6573 2e27 2025 6c65 6e28 696d  atures.' %len(im
-00013ec0: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
-00013ed0: 2929 0a20 2020 2069 6620 6665 6174 7572  )).    if featur
-00013ee0: 655f 6765 6e20 6f72 2066 6561 7475 7265  e_gen or feature
-00013ef0: 5f74 7970 653a 0a20 2020 2020 2020 2069  _type:.        i
-00013f00: 6620 6973 696e 7374 616e 6365 2874 6573  f isinstance(tes
-00013f10: 745f 6461 7461 2c20 7374 7229 206f 7220  t_data, str) or 
-00013f20: 7465 7374 5f64 6174 6120 6973 204e 6f6e  test_data is Non
-00013f30: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-00013f40: 2323 2069 6620 6665 6174 7572 6520 656e  ## if feature en
-00013f50: 6767 2069 7320 7065 7266 6f72 6d65 642c  gg is performed,
-00013f60: 2069 6420 636f 6c75 6d6e 7320 6172 6520   id columns are 
-00013f70: 6472 6f70 7065 642e 2048 656e 6365 2074  dropped. Hence t
-00013f80: 6865 7920 6d75 7374 2072 656a 6f69 6e20  hey must rejoin 
-00013f90: 6865 7265 2e0a 2020 2020 2020 2020 2020  here..          
-00013fa0: 2020 6461 7461 6e61 6d65 203d 2070 642e    dataname = pd.
-00013fb0: 636f 6e63 6174 285b 7472 6169 6e5f 6964  concat([train_id
-00013fc0: 732c 2064 6174 616e 616d 655d 2c20 6178  s, dataname], ax
-00013fd0: 6973 3d31 290a 2020 2020 2020 2020 2020  is=1).          
-00013fe0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013ff0: 7461 7267 6574 2c20 7374 7229 3a0a 2020  target, str):.  
-00014000: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00014010: 7475 726e 2069 6d70 6f72 7461 6e74 5f66  turn important_f
-00014020: 6561 7475 7265 732c 2064 6174 616e 616d  eatures, datanam
-00014030: 655b 696d 706f 7274 616e 745f 6665 6174  e[important_feat
-00014040: 7572 6573 2b5b 7461 7267 6574 5d5d 0a20  ures+[target]]. 
-00014050: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00014060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014070: 2072 6574 7572 6e20 696d 706f 7274 616e   return importan
-00014080: 745f 6665 6174 7572 6573 2c20 6461 7461  t_features, data
-00014090: 6e61 6d65 5b69 6d70 6f72 7461 6e74 5f66  name[important_f
-000140a0: 6561 7475 7265 732b 7461 7267 6574 5d0a  eatures+target].
-000140b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000140c0: 2020 2020 2020 2020 2020 2323 2320 6966            ### if
-000140d0: 2066 6561 7475 7265 2065 6e67 6720 6973   feature engg is
-000140e0: 2070 6572 666f 726d 6564 2c20 6964 2063   performed, id c
-000140f0: 6f6c 756d 6e73 2061 7265 2064 726f 7070  olumns are dropp
-00014100: 6564 2e20 4865 6e63 6520 7468 6579 206d  ed. Hence they m
-00014110: 7573 7420 7265 6a6f 696e 2068 6572 652e  ust rejoin here.
-00014120: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00014130: 616e 616d 6520 3d20 7064 2e63 6f6e 6361  aname = pd.conca
-00014140: 7428 5b74 7261 696e 5f69 6473 2c20 6461  t([train_ids, da
-00014150: 7461 6e61 6d65 5d2c 2061 7869 733d 3129  taname], axis=1)
-00014160: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00014170: 745f 6461 7461 203d 2070 642e 636f 6e63  t_data = pd.conc
-00014180: 6174 285b 7465 7374 5f69 6473 2c20 7465  at([test_ids, te
-00014190: 7374 5f64 6174 615d 2c20 6178 6973 3d31  st_data], axis=1
-000141a0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000141b0: 2069 7369 6e73 7461 6e63 6528 7461 7267   isinstance(targ
-000141c0: 6574 2c20 7374 7229 3a0a 2020 2020 2020  et, str):.      
-000141d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000141e0: 2064 6174 616e 616d 655b 696d 706f 7274   dataname[import
-000141f0: 616e 745f 6665 6174 7572 6573 2b5b 7461  ant_features+[ta
-00014200: 7267 6574 5d5d 2c20 7465 7374 5f64 6174  rget]], test_dat
-00014210: 615b 696d 706f 7274 616e 745f 6665 6174  a[important_feat
-00014220: 7572 6573 5d0a 2020 2020 2020 2020 2020  ures].          
-00014230: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014240: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00014250: 6174 616e 616d 655b 696d 706f 7274 616e  ataname[importan
-00014260: 745f 6665 6174 7572 6573 2b74 6172 6765  t_features+targe
-00014270: 745d 2c20 7465 7374 5f64 6174 615b 696d  t], test_data[im
-00014280: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
-00014290: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
-000142a0: 2020 2020 2323 2320 596f 7520 7365 6c65      ### You sele
-000142b0: 6374 2074 6865 2066 6561 7475 7265 7320  ct the features 
-000142c0: 7769 7468 2074 6865 2073 616d 6520 6f6c  with the same ol
-000142d0: 6420 6e61 6d65 7320 6173 2062 6566 6f72  d names as befor
-000142e0: 6520 2323 2323 2323 230a 2020 2020 2020  e #######.      
-000142f0: 2020 6f6c 645f 696d 706f 7274 616e 745f    old_important_
-00014300: 6665 6174 7572 6573 203d 2063 6f70 792e  features = copy.
-00014310: 6465 6570 636f 7079 2869 6d70 6f72 7461  deepcopy(importa
-00014320: 6e74 5f66 6561 7475 7265 7329 0a20 2020  nt_features).   
-00014330: 2020 2020 2069 6620 6c65 6e28 6461 7465       if len(date
-00014340: 5f63 6f6c 7329 203e 2030 3a0a 2020 2020  _cols) > 0:.    
-00014350: 2020 2020 2020 2020 6461 7465 5f72 6570          date_rep
-00014360: 6c61 6365 7220 3d20 6461 7465 5f63 6f6c  lacer = date_col
-00014370: 5f6d 6170 7065 7273 2e67 6574 2020 2320  _mappers.get  # 
-00014380: 466f 7220 6661 7374 6572 2067 6574 732e  For faster gets.
-00014390: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-000143a0: 6f72 7461 6e74 5f66 6561 7475 7265 7331  ortant_features1
-000143b0: 203d 205b 6461 7465 5f72 6570 6c61 6365   = [date_replace
-000143c0: 7228 6e2c 206e 2920 666f 7220 6e20 696e  r(n, n) for n in
-000143d0: 2069 6d70 6f72 7461 6e74 5f66 6561 7475   important_featu
-000143e0: 7265 735d 0a20 2020 2020 2020 2065 6c73  res].        els
-000143f0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00014400: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-00014410: 7331 203d 205b 6974 656d 5f72 6570 6c61  s1 = [item_repla
-00014420: 6365 7228 6e2c 206e 2920 666f 7220 6e20  cer(n, n) for n 
-00014430: 696e 2069 6d70 6f72 7461 6e74 5f66 6561  in important_fea
-00014440: 7475 7265 735d 0a20 2020 2020 2020 2069  tures].        i
-00014450: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-00014460: 7320 3d20 6669 6e64 5f72 656d 6f76 655f  s = find_remove_
-00014470: 6475 706c 6963 6174 6573 2869 6d70 6f72  duplicates(impor
-00014480: 7461 6e74 5f66 6561 7475 7265 7331 290a  tant_features1).
-00014490: 2020 2020 2020 2020 6966 206f 6c64 5f69          if old_i
-000144a0: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-000144b0: 7320 3d3d 2069 6d70 6f72 7461 6e74 5f66  s == important_f
-000144c0: 6561 7475 7265 733a 0a20 2020 2020 2020  eatures:.       
-000144d0: 2020 2020 2023 2320 446f 6e27 7420 6472       ## Don't dr
-000144e0: 6f70 2074 6865 206f 6c64 2074 6172 6765  op the old targe
-000144f0: 7420 7369 6e63 6520 7468 6572 6520 6973  t since there is
-00014500: 206f 6e6c 7920 6f6e 6520 7461 7267 6574   only one target
-00014510: 2068 6572 6520 2323 230a 2020 2020 2020   here ###.      
-00014520: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00014530: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00014540: 2020 2020 2069 6620 6c65 6e28 6f6c 645f       if len(old_
-00014550: 696d 706f 7274 616e 745f 6665 6174 7572  important_featur
-00014560: 6573 2920 3d3d 206c 656e 2869 6d70 6f72  es) == len(impor
-00014570: 7461 6e74 5f66 6561 7475 7265 7329 3a0a  tant_features):.
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2323 2320 596f 7520 6a75 7374 206d 6f76  ### You just mov
-000145a0: 6520 7468 6520 7661 6c75 6573 2066 726f  e the values fro
-000145b0: 6d20 7468 6520 6e65 7720 6e61 6d65 7320  m the new names 
-000145c0: 746f 2074 6865 206f 6c64 2066 6561 7475  to the old featu
-000145d0: 7265 206e 616d 6573 2023 230a 2020 2020  re names ##.    
-000145e0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000145f0: 6e61 6d65 5b69 6d70 6f72 7461 6e74 5f66  name[important_f
-00014600: 6561 7475 7265 735d 203d 2064 6174 616e  eatures] = datan
-00014610: 616d 655b 6f6c 645f 696d 706f 7274 616e  ame[old_importan
-00014620: 745f 6665 6174 7572 6573 5d0a 2020 2020  t_features].    
-00014630: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00014640: 7369 6e73 7461 6e63 6528 7465 7374 5f64  sinstance(test_d
-00014650: 6174 612c 2073 7472 2920 6f72 2074 6573  ata, str) or tes
-00014660: 745f 6461 7461 2069 7320 4e6f 6e65 3a0a  t_data is None:.
-00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014680: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
-00014690: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000146a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146b0: 2020 2023 2323 2320 6966 2074 6865 7265     #### if there
-000146c0: 2069 7320 7465 7374 2064 6174 6120 7472   is test data tr
-000146d0: 616e 7366 6572 2076 616c 7565 7320 746f  ansfer values to
-000146e0: 2069 7420 2323 230a 2020 2020 2020 2020   it ###.        
-000146f0: 2020 2020 2020 2020 2020 2020 7465 7374              test
-00014700: 5f64 6174 615b 696d 706f 7274 616e 745f  _data[important_
-00014710: 6665 6174 7572 6573 5d20 3d20 7465 7374  features] = test
-00014720: 5f64 6174 615b 6f6c 645f 696d 706f 7274  _data[old_import
-00014730: 616e 745f 6665 6174 7572 6573 5d0a 2020  ant_features].  
-00014740: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014760: 2323 2320 6669 7273 7420 7472 7920 746f  ### first try to
-00014770: 2072 6574 7572 6e20 7769 7468 2074 6865   return with the
-00014780: 206e 6577 2069 6d70 6f72 7461 6e74 2066   new important f
-00014790: 6561 7475 7265 732c 2069 6620 7468 6174  eatures, if that
-000147a0: 2066 6169 6c73 2072 6574 7572 6e20 7769   fails return wi
-000147b0: 7468 206f 6c64 2066 6561 7475 7265 730a  th old features.
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000147e0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-000147f0: 5468 6572 6520 6172 6520 7370 6563 6961  There are specia
-00014800: 6c20 6368 6172 7320 696e 2063 6f6c 756d  l chars in colum
-00014810: 6e20 6e61 6d65 732e 2050 6c65 6173 6520  n names. Please 
-00014820: 7265 6d6f 7665 2074 6865 6d20 616e 6420  remove them and 
-00014830: 7472 7920 6167 6169 6e2e 2729 0a20 2020  try again.').   
-00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014850: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
-00014860: 6573 745f 6461 7461 2c20 7374 7229 206f  est_data, str) o
-00014870: 7220 7465 7374 5f64 6174 6120 6973 204e  r test_data is N
-00014880: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00014890: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000148a0: 7572 6e20 696d 706f 7274 616e 745f 6665  urn important_fe
-000148b0: 6174 7572 6573 2c20 6461 7461 6e61 6d65  atures, dataname
-000148c0: 5b69 6d70 6f72 7461 6e74 5f66 6561 7475  [important_featu
-000148d0: 7265 735d 0a20 2020 2020 2020 2020 2020  res].           
-000148e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014900: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00014910: 7461 6e61 6d65 5b69 6d70 6f72 7461 6e74  taname[important
-00014920: 5f66 6561 7475 7265 735d 2c20 7465 7374  _features], test
-00014930: 5f64 6174 615b 696d 706f 7274 616e 745f  _data[important_
-00014940: 6665 6174 7572 6573 5d0a 2020 2020 2020  features].      
-00014950: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00014960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014970: 2020 2020 2020 7072 696e 7428 2754 6865        print('The
-00014980: 7265 2061 7265 2073 7065 6369 616c 2063  re are special c
-00014990: 6861 7273 2069 6e20 636f 6c75 6d6e 206e  hars in column n
-000149a0: 616d 6573 2e20 5265 7475 726e 696e 6720  ames. Returning 
-000149b0: 7769 7468 2069 6d70 6f72 7461 6e74 2066  with important f
-000149c0: 6561 7475 7265 7320 616e 6420 7472 6169  eatures and trai
-000149d0: 6e2e 2729 0a20 2020 2020 2020 2020 2020  n.').           
-000149e0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-000149f0: 7374 616e 6365 2874 6573 745f 6461 7461  stance(test_data
-00014a00: 2c20 7374 7229 206f 7220 7465 7374 5f64  , str) or test_d
-00014a10: 6174 6120 6973 204e 6f6e 653a 0a20 2020  ata is None:.   
-00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a30: 2020 2020 2072 6574 7572 6e20 6f6c 645f       return old_
-00014a40: 696d 706f 7274 616e 745f 6665 6174 7572  important_featur
-00014a50: 6573 2c20 6461 7461 6e61 6d65 5b6f 6c64  es, dataname[old
-00014a60: 5f69 6d70 6f72 7461 6e74 5f66 6561 7475  _important_featu
-00014a70: 7265 735d 0a20 2020 2020 2020 2020 2020  res].           
-00014a80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014aa0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00014ab0: 7461 6e61 6d65 5b6f 6c64 5f69 6d70 6f72  taname[old_impor
-00014ac0: 7461 6e74 5f66 6561 7475 7265 735d 2c20  tant_features], 
-00014ad0: 7465 7374 5f64 6174 615b 6f6c 645f 696d  test_data[old_im
-00014ae0: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
-00014af0: 5d20 2020 0a20 2020 2020 2020 200a 2020  ]   .        .  
-00014b00: 2020 2020 2020 6f6c 645f 7461 7267 6574        old_target
-00014b10: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-00014b20: 2874 6172 6765 7429 0a20 2020 2020 2020  (target).       
-00014b30: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
-00014b40: 6172 6765 742c 2073 7472 293a 0a20 2020  arget, str):.   
-00014b50: 2020 2020 2020 2020 2074 6172 6765 7420           target 
-00014b60: 3d20 6974 656d 5f72 6570 6c61 6365 7228  = item_replacer(
-00014b70: 7461 7267 6574 2c20 7461 7267 6574 290a  target, target).
-00014b80: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00014b90: 6574 7320 3d20 5b74 6172 6765 745d 0a20  ets = [target]. 
-00014ba0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00014bb0: 2020 2020 2020 2020 2074 6172 6765 7420           target 
-00014bc0: 3d20 5b69 7465 6d5f 7265 706c 6163 6572  = [item_replacer
-00014bd0: 286e 2c20 6e29 2066 6f72 206e 2069 6e20  (n, n) for n in 
-00014be0: 7461 7267 6574 5d0a 2020 2020 2020 2020  target].        
-00014bf0: 2020 2020 7461 7267 6574 7320 3d20 636f      targets = co
-00014c00: 7079 2e64 6565 7063 6f70 7928 7461 7267  py.deepcopy(targ
-00014c10: 6574 290a 0a20 2020 2020 2020 2069 6620  et)..        if 
-00014c20: 6f6c 645f 7461 7267 6574 203d 3d20 7461  old_target == ta
-00014c30: 7267 6574 3a0a 2020 2020 2020 2020 2020  rget:.          
-00014c40: 2020 2323 2044 6f6e 2774 2064 726f 7020    ## Don't drop 
-00014c50: 7468 6520 6f6c 6420 7461 7267 6574 2073  the old target s
-00014c60: 696e 6365 2074 6865 7265 2069 7320 6f6e  ince there is on
-00014c70: 6c79 206f 6e65 2074 6172 6765 7420 6865  ly one target he
-00014c80: 7265 2023 2323 0a20 2020 2020 2020 2020  re ###.         
-00014c90: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00014ca0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014cb0: 2020 2323 2320 796f 7520 646f 6e27 7420    ### you don't 
-00014cc0: 6e65 6564 2064 726f 7020 7468 6520 636f  need drop the co
-00014cd0: 6c73 2074 6861 7420 6861 7665 2063 6861  ls that have cha
-00014ce0: 6e67 6564 2073 696e 6365 206f 6e6c 7920  nged since only 
-00014cf0: 6120 6665 7720 6172 6520 7365 6c65 6374  a few are select
-00014d00: 6564 2023 2323 2323 2323 0a20 2020 2020  ed #######.     
-00014d10: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00014d20: 616e 6365 2874 6172 6765 742c 2073 7472  ance(target, str
-00014d30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014d40: 2020 2064 6174 616e 616d 655b 7461 7267     dataname[targ
-00014d50: 6574 5d20 3d20 6461 7461 6e61 6d65 5b6f  et] = dataname[o
-00014d60: 6c64 5f74 6172 6765 745d 0a20 2020 2020  ld_target].     
-00014d70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00014d80: 2020 2020 2020 2020 2020 2020 2063 6f70               cop
-00014d90: 795f 7461 7267 6574 7320 3d20 636f 7079  y_targets = copy
-00014da0: 2e64 6565 7063 6f70 7928 7461 7267 6574  .deepcopy(target
-00014db0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00014dc0: 2020 2063 6f70 795f 6f6c 6420 3d20 636f     copy_old = co
-00014dd0: 7079 2e64 6565 7063 6f70 7928 6f6c 645f  py.deepcopy(old_
-00014de0: 7461 7267 6574 290a 2020 2020 2020 2020  target).        
-00014df0: 2020 2020 2020 2020 666f 7220 6561 6368          for each
-00014e00: 5f74 6172 6765 742c 2065 6163 685f 6f6c  _target, each_ol
-00014e10: 645f 7461 7267 6574 2069 6e20 7a69 7028  d_target in zip(
-00014e20: 636f 7079 5f74 6172 6765 7473 2c20 636f  copy_targets, co
-00014e30: 7079 5f6f 6c64 293a 0a20 2020 2020 2020  py_old):.       
-00014e40: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00014e50: 616e 616d 655b 6561 6368 5f74 6172 6765  aname[each_targe
-00014e60: 745d 203d 2064 6174 616e 616d 655b 6561  t] = dataname[ea
-00014e70: 6368 5f6f 6c64 5f74 6172 6765 745d 0a0a  ch_old_target]..
-00014e80: 2020 2020 2020 2020 2323 2323 2054 6869          #### Thi
-00014e90: 7320 6973 2077 6865 7265 2077 6520 6368  s is where we ch
-00014ea0: 6563 6b20 7768 6574 6865 7220 746f 2072  eck whether to r
-00014eb0: 6574 7572 6e20 7465 7374 2064 6174 6120  eturn test data 
-00014ec0: 6f72 206e 6f74 2023 2323 2323 230a 2020  or not ######.  
-00014ed0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00014ee0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00014ef0: 616e 6365 2874 6573 745f 6461 7461 2c20  ance(test_data, 
-00014f00: 7374 7229 206f 7220 7465 7374 5f64 6174  str) or test_dat
-00014f10: 6120 6973 204e 6f6e 653a 0a20 2020 2020  a is None:.     
-00014f20: 2020 2020 2020 2020 2020 2069 6620 6665             if fe
-00014f30: 6174 7572 655f 6765 6e20 6f72 2066 6561  ature_gen or fea
-00014f40: 7475 7265 5f74 7970 653a 0a20 2020 2020  ture_type:.     
-00014f50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00014f60: 2323 2069 6620 6665 6174 7572 6520 656e  ## if feature en
-00014f70: 6767 2069 7320 7065 7266 6f72 6d65 642c  gg is performed,
-00014f80: 2069 6420 636f 6c75 6d6e 7320 6172 6520   id columns are 
-00014f90: 6472 6f70 7065 642e 2048 656e 6365 2074  dropped. Hence t
-00014fa0: 6865 7920 6d75 7374 2072 656a 6f69 6e20  hey must rejoin 
-00014fb0: 6865 7265 2e0a 2020 2020 2020 2020 2020  here..          
-00014fc0: 2020 2020 2020 2020 2020 6461 7461 6e61            datana
-00014fd0: 6d65 203d 2070 642e 636f 6e63 6174 285b  me = pd.concat([
-00014fe0: 7472 6169 6e5f 6964 732c 2064 6174 616e  train_ids, datan
-00014ff0: 616d 655d 2c20 6178 6973 3d31 290a 2020  ame], axis=1).  
-00015000: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015010: 7475 726e 2069 6d70 6f72 7461 6e74 5f66  turn important_f
-00015020: 6561 7475 7265 732c 2064 6174 616e 616d  eatures, datanam
-00015030: 655b 696d 706f 7274 616e 745f 6665 6174  e[important_feat
-00015040: 7572 6573 2b74 6172 6765 745d 0a20 2020  ures+target].   
-00015050: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015060: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00015070: 2320 5468 6973 2069 7320 666f 7220 7465  # This is for te
-00015080: 7374 2064 6174 6120 6578 6973 7469 6e67  st data existing
-00015090: 2023 2323 230a 2020 2020 2020 2020 2020   ####.          
-000150a0: 2020 2020 2020 6966 2066 6561 7475 7265        if feature
-000150b0: 5f67 656e 206f 7220 6665 6174 7572 655f  _gen or feature_
-000150c0: 7479 7065 3a0a 2020 2020 2020 2020 2020  type:.          
-000150d0: 2020 2020 2020 2020 2020 2323 2320 6966            ### if
-000150e0: 2066 6561 7475 7265 2065 6e67 6720 6973   feature engg is
-000150f0: 2070 6572 666f 726d 6564 2c20 6964 2063   performed, id c
-00015100: 6f6c 756d 6e73 2061 7265 2064 726f 7070  olumns are dropp
-00015110: 6564 2e20 4865 6e63 6520 7468 6579 206d  ed. Hence they m
-00015120: 7573 7420 7265 6a6f 696e 2068 6572 652e  ust rejoin here.
-00015130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015140: 2020 2020 2064 6174 616e 616d 6520 3d20       dataname = 
-00015150: 7064 2e63 6f6e 6361 7428 5b74 7261 696e  pd.concat([train
-00015160: 5f69 6473 2c20 6461 7461 6e61 6d65 5d2c  _ids, dataname],
-00015170: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
-00015180: 2020 2020 2020 2020 2020 2020 2074 6573               tes
-00015190: 745f 6461 7461 203d 2070 642e 636f 6e63  t_data = pd.conc
-000151a0: 6174 285b 7465 7374 5f69 6473 2c20 7465  at([test_ids, te
-000151b0: 7374 5f64 6174 615d 2c20 6178 6973 3d31  st_data], axis=1
-000151c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000151d0: 2020 2323 2320 596f 7520 7365 6c65 6374    ### You select
-000151e0: 2074 6865 2066 6561 7475 7265 7320 7769   the features wi
-000151f0: 7468 2074 6865 2073 616d 6520 6f6c 6420  th the same old 
-00015200: 6e61 6d65 7320 6173 2062 6566 6f72 6520  names as before 
-00015210: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
-00015220: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00015230: 6174 616e 616d 655b 696d 706f 7274 616e  ataname[importan
-00015240: 745f 6665 6174 7572 6573 2b74 6172 6765  t_features+targe
-00015250: 7473 5d2c 2074 6573 745f 6461 7461 5b69  ts], test_data[i
-00015260: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-00015270: 735d 0a20 2020 2020 2020 2065 7863 6570  s].        excep
-00015280: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
-00015290: 7269 6e74 2827 5761 726e 696e 673a 2052  rint('Warning: R
-000152a0: 6574 7572 6e69 6e67 2077 6974 6820 696d  eturning with im
-000152b0: 706f 7274 616e 7420 6665 6174 7572 6573  portant features
-000152c0: 2061 6e64 2074 7261 696e 2e20 506c 6561   and train. Plea
-000152d0: 7365 2072 652d 6368 6563 6b20 796f 7572  se re-check your
-000152e0: 206f 7574 7075 7473 2e27 290a 2020 2020   outputs.').    
-000152f0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00015300: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
-00015310: 732c 2064 6174 616e 616d 655b 696d 706f  s, dataname[impo
-00015320: 7274 616e 745f 6665 6174 7572 6573 2b74  rtant_features+t
-00015330: 6172 6765 7473 5d0a 2323 2323 2323 2323  argets].########
-00015340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013d40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00013d70: 2323 2323 2323 230a 2020 2020 2323 2049  #######.    ## I
+00013d80: 6e20 6f6e 6520 6361 7365 2c20 636f 6c75  n one case, colu
+00013d90: 6d6e 206e 616d 6573 2067 6574 2063 6861  mn names get cha
+00013da0: 6e67 6564 2069 6e20 7472 6169 6e20 6275  nged in train bu
+00013db0: 7420 6e6f 7420 696e 2074 6573 7420 7369  t not in test si
+00013dc0: 6e63 6520 6974 2074 6573 7420 6973 206e  nce it test is n
+00013dd0: 6f74 2061 7661 696c 6162 6c65 2e0a 2020  ot available..  
+00013de0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00013df0: 7465 7374 5f64 6174 612c 2073 7472 2920  test_data, str) 
+00013e00: 6f72 2074 6573 745f 6461 7461 2069 7320  or test_data is 
+00013e10: 4e6f 6e65 3a0a 2020 2020 2020 2020 7072  None:.        pr
+00013e20: 696e 7428 274f 7574 7075 7420 636f 6e74  int('Output cont
+00013e30: 6169 6e73 2061 206c 6973 7420 6f66 2025  ains a list of %
+00013e40: 7320 696d 706f 7274 616e 7420 6665 6174  s important feat
+00013e50: 7572 6573 2061 6e64 2061 2074 7261 696e  ures and a train
+00013e60: 2064 6174 6166 7261 6d65 2720 256c 656e   dataframe' %len
+00013e70: 2869 6d70 6f72 7461 6e74 5f66 6561 7475  (important_featu
+00013e80: 7265 7329 290a 2020 2020 656c 7365 3a0a  res)).    else:.
+00013e90: 2020 2020 2020 2020 7072 696e 7428 274f          print('O
+00013ea0: 7574 7075 7420 636f 6e74 6169 6e73 2074  utput contains t
+00013eb0: 776f 2064 6174 6166 7261 6d65 733a 2074  wo dataframes: t
+00013ec0: 7261 696e 2061 6e64 2074 6573 7420 7769  rain and test wi
+00013ed0: 7468 2025 6420 696d 706f 7274 616e 7420  th %d important 
+00013ee0: 6665 6174 7572 6573 2e27 2025 6c65 6e28  features.' %len(
+00013ef0: 696d 706f 7274 616e 745f 6665 6174 7572  important_featur
+00013f00: 6573 2929 0a20 2020 2069 6620 6665 6174  es)).    if feat
+00013f10: 7572 655f 6765 6e20 6f72 2066 6561 7475  ure_gen or featu
+00013f20: 7265 5f74 7970 653a 0a20 2020 2020 2020  re_type:.       
+00013f30: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
+00013f40: 6573 745f 6461 7461 2c20 7374 7229 206f  est_data, str) o
+00013f50: 7220 7465 7374 5f64 6174 6120 6973 204e  r test_data is N
+00013f60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013f70: 2023 2323 2069 6620 6665 6174 7572 6520   ### if feature 
+00013f80: 656e 6767 2069 7320 7065 7266 6f72 6d65  engg is performe
+00013f90: 642c 2069 6420 636f 6c75 6d6e 7320 6172  d, id columns ar
+00013fa0: 6520 6472 6f70 7065 642e 2048 656e 6365  e dropped. Hence
+00013fb0: 2074 6865 7920 6d75 7374 2072 656a 6f69   they must rejoi
+00013fc0: 6e20 6865 7265 2e0a 2020 2020 2020 2020  n here..        
+00013fd0: 2020 2020 6461 7461 6e61 6d65 203d 2070      dataname = p
+00013fe0: 642e 636f 6e63 6174 285b 7472 6169 6e5f  d.concat([train_
+00013ff0: 6964 732c 2064 6174 616e 616d 655d 2c20  ids, dataname], 
+00014000: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+00014010: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00014020: 6528 7461 7267 6574 2c20 7374 7229 3a0a  e(target, str):.
+00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014040: 7265 7475 726e 2069 6d70 6f72 7461 6e74  return important
+00014050: 5f66 6561 7475 7265 732c 2064 6174 616e  _features, datan
+00014060: 616d 655b 696d 706f 7274 616e 745f 6665  ame[important_fe
+00014070: 6174 7572 6573 2b5b 7461 7267 6574 5d5d  atures+[target]]
+00014080: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00014090: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000140a0: 2020 2072 6574 7572 6e20 696d 706f 7274     return import
+000140b0: 616e 745f 6665 6174 7572 6573 2c20 6461  ant_features, da
+000140c0: 7461 6e61 6d65 5b69 6d70 6f72 7461 6e74  taname[important
+000140d0: 5f66 6561 7475 7265 732b 7461 7267 6574  _features+target
+000140e0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+000140f0: 2020 2020 2020 2020 2020 2020 2323 2320              ### 
+00014100: 6966 2066 6561 7475 7265 2065 6e67 6720  if feature engg 
+00014110: 6973 2070 6572 666f 726d 6564 2c20 6964  is performed, id
+00014120: 2063 6f6c 756d 6e73 2061 7265 2064 726f   columns are dro
+00014130: 7070 6564 2e20 4865 6e63 6520 7468 6579  pped. Hence they
+00014140: 206d 7573 7420 7265 6a6f 696e 2068 6572   must rejoin her
+00014150: 652e 0a20 2020 2020 2020 2020 2020 2064  e..            d
+00014160: 6174 616e 616d 6520 3d20 7064 2e63 6f6e  ataname = pd.con
+00014170: 6361 7428 5b74 7261 696e 5f69 6473 2c20  cat([train_ids, 
+00014180: 6461 7461 6e61 6d65 5d2c 2061 7869 733d  dataname], axis=
+00014190: 3129 0a20 2020 2020 2020 2020 2020 2074  1).            t
+000141a0: 6573 745f 6461 7461 203d 2070 642e 636f  est_data = pd.co
+000141b0: 6e63 6174 285b 7465 7374 5f69 6473 2c20  ncat([test_ids, 
+000141c0: 7465 7374 5f64 6174 615d 2c20 6178 6973  test_data], axis
+000141d0: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
+000141e0: 6966 2069 7369 6e73 7461 6e63 6528 7461  if isinstance(ta
+000141f0: 7267 6574 2c20 7374 7229 3a0a 2020 2020  rget, str):.    
+00014200: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014210: 726e 2064 6174 616e 616d 655b 696d 706f  rn dataname[impo
+00014220: 7274 616e 745f 6665 6174 7572 6573 2b5b  rtant_features+[
+00014230: 7461 7267 6574 5d5d 2c20 7465 7374 5f64  target]], test_d
+00014240: 6174 615b 696d 706f 7274 616e 745f 6665  ata[important_fe
+00014250: 6174 7572 6573 5d0a 2020 2020 2020 2020  atures].        
+00014260: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014270: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014280: 2064 6174 616e 616d 655b 696d 706f 7274   dataname[import
+00014290: 616e 745f 6665 6174 7572 6573 2b74 6172  ant_features+tar
+000142a0: 6765 745d 2c20 7465 7374 5f64 6174 615b  get], test_data[
+000142b0: 696d 706f 7274 616e 745f 6665 6174 7572  important_featur
+000142c0: 6573 5d0a 2020 2020 656c 7365 3a0a 2020  es].    else:.  
+000142d0: 2020 2020 2020 2323 2320 596f 7520 7365        ### You se
+000142e0: 6c65 6374 2074 6865 2066 6561 7475 7265  lect the feature
+000142f0: 7320 7769 7468 2074 6865 2073 616d 6520  s with the same 
+00014300: 6f6c 6420 6e61 6d65 7320 6173 2062 6566  old names as bef
+00014310: 6f72 6520 2323 2323 2323 230a 2020 2020  ore #######.    
+00014320: 2020 2020 6f6c 645f 696d 706f 7274 616e      old_importan
+00014330: 745f 6665 6174 7572 6573 203d 2063 6f70  t_features = cop
+00014340: 792e 6465 6570 636f 7079 2869 6d70 6f72  y.deepcopy(impor
+00014350: 7461 6e74 5f66 6561 7475 7265 7329 0a20  tant_features). 
+00014360: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
+00014370: 7465 5f63 6f6c 7329 203e 2030 3a0a 2020  te_cols) > 0:.  
+00014380: 2020 2020 2020 2020 2020 6461 7465 5f72            date_r
+00014390: 6570 6c61 6365 7220 3d20 6461 7465 5f63  eplacer = date_c
+000143a0: 6f6c 5f6d 6170 7065 7273 2e67 6574 2020  ol_mappers.get  
+000143b0: 2320 466f 7220 6661 7374 6572 2067 6574  # For faster get
+000143c0: 732e 0a20 2020 2020 2020 2020 2020 2069  s..            i
+000143d0: 6d70 6f72 7461 6e74 5f66 6561 7475 7265  mportant_feature
+000143e0: 7331 203d 205b 6461 7465 5f72 6570 6c61  s1 = [date_repla
+000143f0: 6365 7228 6e2c 206e 2920 666f 7220 6e20  cer(n, n) for n 
+00014400: 696e 2069 6d70 6f72 7461 6e74 5f66 6561  in important_fea
+00014410: 7475 7265 735d 0a20 2020 2020 2020 2065  tures].        e
+00014420: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014430: 2069 6d70 6f72 7461 6e74 5f66 6561 7475   important_featu
+00014440: 7265 7331 203d 205b 6974 656d 5f72 6570  res1 = [item_rep
+00014450: 6c61 6365 7228 6e2c 206e 2920 666f 7220  lacer(n, n) for 
+00014460: 6e20 696e 2069 6d70 6f72 7461 6e74 5f66  n in important_f
+00014470: 6561 7475 7265 735d 0a20 2020 2020 2020  eatures].       
+00014480: 2069 6d70 6f72 7461 6e74 5f66 6561 7475   important_featu
+00014490: 7265 7320 3d20 6669 6e64 5f72 656d 6f76  res = find_remov
+000144a0: 655f 6475 706c 6963 6174 6573 2869 6d70  e_duplicates(imp
+000144b0: 6f72 7461 6e74 5f66 6561 7475 7265 7331  ortant_features1
+000144c0: 290a 2020 2020 2020 2020 6966 206f 6c64  ).        if old
+000144d0: 5f69 6d70 6f72 7461 6e74 5f66 6561 7475  _important_featu
+000144e0: 7265 7320 3d3d 2069 6d70 6f72 7461 6e74  res == important
+000144f0: 5f66 6561 7475 7265 733a 0a20 2020 2020  _features:.     
+00014500: 2020 2020 2020 2023 2320 446f 6e27 7420         ## Don't 
+00014510: 6472 6f70 2074 6865 206f 6c64 2074 6172  drop the old tar
+00014520: 6765 7420 7369 6e63 6520 7468 6572 6520  get since there 
+00014530: 6973 206f 6e6c 7920 6f6e 6520 7461 7267  is only one targ
+00014540: 6574 2068 6572 6520 2323 230a 2020 2020  et here ###.    
+00014550: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00014560: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014570: 2020 2020 2020 2069 6620 6c65 6e28 6f6c         if len(ol
+00014580: 645f 696d 706f 7274 616e 745f 6665 6174  d_important_feat
+00014590: 7572 6573 2920 3d3d 206c 656e 2869 6d70  ures) == len(imp
+000145a0: 6f72 7461 6e74 5f66 6561 7475 7265 7329  ortant_features)
+000145b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000145c0: 2020 2323 2320 596f 7520 6a75 7374 206d    ### You just m
+000145d0: 6f76 6520 7468 6520 7661 6c75 6573 2066  ove the values f
+000145e0: 726f 6d20 7468 6520 6e65 7720 6e61 6d65  rom the new name
+000145f0: 7320 746f 2074 6865 206f 6c64 2066 6561  s to the old fea
+00014600: 7475 7265 206e 616d 6573 2023 230a 2020  ture names ##.  
+00014610: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00014620: 7461 6e61 6d65 5b69 6d70 6f72 7461 6e74  taname[important
+00014630: 5f66 6561 7475 7265 735d 203d 2064 6174  _features] = dat
+00014640: 616e 616d 655b 6f6c 645f 696d 706f 7274  aname[old_import
+00014650: 616e 745f 6665 6174 7572 6573 5d0a 2020  ant_features].  
+00014660: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014670: 2069 7369 6e73 7461 6e63 6528 7465 7374   isinstance(test
+00014680: 5f64 6174 612c 2073 7472 2920 6f72 2074  _data, str) or t
+00014690: 6573 745f 6461 7461 2069 7320 4e6f 6e65  est_data is None
+000146a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000146b0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+000146c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000146d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000146e0: 2020 2020 2023 2323 2320 6966 2074 6865       #### if the
+000146f0: 7265 2069 7320 7465 7374 2064 6174 6120  re is test data 
+00014700: 7472 616e 7366 6572 2076 616c 7565 7320  transfer values 
+00014710: 746f 2069 7420 2323 230a 2020 2020 2020  to it ###.      
+00014720: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00014730: 7374 5f64 6174 615b 696d 706f 7274 616e  st_data[importan
+00014740: 745f 6665 6174 7572 6573 5d20 3d20 7465  t_features] = te
+00014750: 7374 5f64 6174 615b 6f6c 645f 696d 706f  st_data[old_impo
+00014760: 7274 616e 745f 6665 6174 7572 6573 5d0a  rtant_features].
+00014770: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00014780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014790: 2020 2323 2320 6669 7273 7420 7472 7920    ### first try 
+000147a0: 746f 2072 6574 7572 6e20 7769 7468 2074  to return with t
+000147b0: 6865 206e 6577 2069 6d70 6f72 7461 6e74  he new important
+000147c0: 2066 6561 7475 7265 732c 2069 6620 7468   features, if th
+000147d0: 6174 2066 6169 6c73 2072 6574 7572 6e20  at fails return 
+000147e0: 7769 7468 206f 6c64 2066 6561 7475 7265  with old feature
+000147f0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00014800: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00014810: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00014820: 2827 5468 6572 6520 6172 6520 7370 6563  ('There are spec
+00014830: 6961 6c20 6368 6172 7320 696e 2063 6f6c  ial chars in col
+00014840: 756d 6e20 6e61 6d65 732e 2050 6c65 6173  umn names. Pleas
+00014850: 6520 7265 6d6f 7665 2074 6865 6d20 616e  e remove them an
+00014860: 6420 7472 7920 6167 6169 6e2e 2729 0a20  d try again.'). 
+00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014880: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00014890: 2874 6573 745f 6461 7461 2c20 7374 7229  (test_data, str)
+000148a0: 206f 7220 7465 7374 5f64 6174 6120 6973   or test_data is
+000148b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000148c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000148d0: 6574 7572 6e20 696d 706f 7274 616e 745f  eturn important_
+000148e0: 6665 6174 7572 6573 2c20 6461 7461 6e61  features, datana
+000148f0: 6d65 5b69 6d70 6f72 7461 6e74 5f66 6561  me[important_fea
+00014900: 7475 7265 735d 0a20 2020 2020 2020 2020  tures].         
+00014910: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00014920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014930: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00014940: 6461 7461 6e61 6d65 5b69 6d70 6f72 7461  dataname[importa
+00014950: 6e74 5f66 6561 7475 7265 735d 2c20 7465  nt_features], te
+00014960: 7374 5f64 6174 615b 696d 706f 7274 616e  st_data[importan
+00014970: 745f 6665 6174 7572 6573 5d0a 2020 2020  t_features].    
+00014980: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00014990: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+000149a0: 2020 2020 2020 2020 7072 696e 7428 2754          print('T
+000149b0: 6865 7265 2061 7265 2073 7065 6369 616c  here are special
+000149c0: 2063 6861 7273 2069 6e20 636f 6c75 6d6e   chars in column
+000149d0: 206e 616d 6573 2e20 5265 7475 726e 696e   names. Returnin
+000149e0: 6720 7769 7468 2069 6d70 6f72 7461 6e74  g with important
+000149f0: 2066 6561 7475 7265 7320 616e 6420 7472   features and tr
+00014a00: 6169 6e2e 2729 0a20 2020 2020 2020 2020  ain.').         
+00014a10: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00014a20: 696e 7374 616e 6365 2874 6573 745f 6461  instance(test_da
+00014a30: 7461 2c20 7374 7229 206f 7220 7465 7374  ta, str) or test
+00014a40: 5f64 6174 6120 6973 204e 6f6e 653a 0a20  _data is None:. 
+00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a60: 2020 2020 2020 2072 6574 7572 6e20 6f6c         return ol
+00014a70: 645f 696d 706f 7274 616e 745f 6665 6174  d_important_feat
+00014a80: 7572 6573 2c20 6461 7461 6e61 6d65 5b6f  ures, dataname[o
+00014a90: 6c64 5f69 6d70 6f72 7461 6e74 5f66 6561  ld_important_fea
+00014aa0: 7475 7265 735d 0a20 2020 2020 2020 2020  tures].         
+00014ab0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00014ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ad0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00014ae0: 6461 7461 6e61 6d65 5b6f 6c64 5f69 6d70  dataname[old_imp
+00014af0: 6f72 7461 6e74 5f66 6561 7475 7265 735d  ortant_features]
+00014b00: 2c20 7465 7374 5f64 6174 615b 6f6c 645f  , test_data[old_
+00014b10: 696d 706f 7274 616e 745f 6665 6174 7572  important_featur
+00014b20: 6573 5d20 2020 0a20 2020 2020 2020 200a  es]   .        .
+00014b30: 2020 2020 2020 2020 6f6c 645f 7461 7267          old_targ
+00014b40: 6574 203d 2063 6f70 792e 6465 6570 636f  et = copy.deepco
+00014b50: 7079 2874 6172 6765 7429 0a20 2020 2020  py(target).     
+00014b60: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00014b70: 2874 6172 6765 742c 2073 7472 293a 0a20  (target, str):. 
+00014b80: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00014b90: 7420 3d20 6974 656d 5f72 6570 6c61 6365  t = item_replace
+00014ba0: 7228 7461 7267 6574 2c20 7461 7267 6574  r(target, target
+00014bb0: 290a 2020 2020 2020 2020 2020 2020 7461  ).            ta
+00014bc0: 7267 6574 7320 3d20 5b74 6172 6765 745d  rgets = [target]
+00014bd0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00014be0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00014bf0: 7420 3d20 5b69 7465 6d5f 7265 706c 6163  t = [item_replac
+00014c00: 6572 286e 2c20 6e29 2066 6f72 206e 2069  er(n, n) for n i
+00014c10: 6e20 7461 7267 6574 5d0a 2020 2020 2020  n target].      
+00014c20: 2020 2020 2020 7461 7267 6574 7320 3d20        targets = 
+00014c30: 636f 7079 2e64 6565 7063 6f70 7928 7461  copy.deepcopy(ta
+00014c40: 7267 6574 290a 0a20 2020 2020 2020 2069  rget)..        i
+00014c50: 6620 6f6c 645f 7461 7267 6574 203d 3d20  f old_target == 
+00014c60: 7461 7267 6574 3a0a 2020 2020 2020 2020  target:.        
+00014c70: 2020 2020 2323 2044 6f6e 2774 2064 726f      ## Don't dro
+00014c80: 7020 7468 6520 6f6c 6420 7461 7267 6574  p the old target
+00014c90: 2073 696e 6365 2074 6865 7265 2069 7320   since there is 
+00014ca0: 6f6e 6c79 206f 6e65 2074 6172 6765 7420  only one target 
+00014cb0: 6865 7265 2023 2323 0a20 2020 2020 2020  here ###.       
+00014cc0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
+00014cd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00014ce0: 2020 2020 2323 2320 796f 7520 646f 6e27      ### you don'
+00014cf0: 7420 6e65 6564 2064 726f 7020 7468 6520  t need drop the 
+00014d00: 636f 6c73 2074 6861 7420 6861 7665 2063  cols that have c
+00014d10: 6861 6e67 6564 2073 696e 6365 206f 6e6c  hanged since onl
+00014d20: 7920 6120 6665 7720 6172 6520 7365 6c65  y a few are sele
+00014d30: 6374 6564 2023 2323 2323 2323 0a20 2020  cted #######.   
+00014d40: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00014d50: 7374 616e 6365 2874 6172 6765 742c 2073  stance(target, s
+00014d60: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00014d70: 2020 2020 2064 6174 616e 616d 655b 7461       dataname[ta
+00014d80: 7267 6574 5d20 3d20 6461 7461 6e61 6d65  rget] = dataname
+00014d90: 5b6f 6c64 5f74 6172 6765 745d 0a20 2020  [old_target].   
+00014da0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00014db0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014dc0: 6f70 795f 7461 7267 6574 7320 3d20 636f  opy_targets = co
+00014dd0: 7079 2e64 6565 7063 6f70 7928 7461 7267  py.deepcopy(targ
+00014de0: 6574 7329 0a20 2020 2020 2020 2020 2020  ets).           
+00014df0: 2020 2020 2063 6f70 795f 6f6c 6420 3d20       copy_old = 
+00014e00: 636f 7079 2e64 6565 7063 6f70 7928 6f6c  copy.deepcopy(ol
+00014e10: 645f 7461 7267 6574 290a 2020 2020 2020  d_target).      
+00014e20: 2020 2020 2020 2020 2020 666f 7220 6561            for ea
+00014e30: 6368 5f74 6172 6765 742c 2065 6163 685f  ch_target, each_
+00014e40: 6f6c 645f 7461 7267 6574 2069 6e20 7a69  old_target in zi
+00014e50: 7028 636f 7079 5f74 6172 6765 7473 2c20  p(copy_targets, 
+00014e60: 636f 7079 5f6f 6c64 293a 0a20 2020 2020  copy_old):.     
+00014e70: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00014e80: 6174 616e 616d 655b 6561 6368 5f74 6172  ataname[each_tar
+00014e90: 6765 745d 203d 2064 6174 616e 616d 655b  get] = dataname[
+00014ea0: 6561 6368 5f6f 6c64 5f74 6172 6765 745d  each_old_target]
+00014eb0: 0a0a 2020 2020 2020 2020 2323 2323 2054  ..        #### T
+00014ec0: 6869 7320 6973 2077 6865 7265 2077 6520  his is where we 
+00014ed0: 6368 6563 6b20 7768 6574 6865 7220 746f  check whether to
+00014ee0: 2072 6574 7572 6e20 7465 7374 2064 6174   return test dat
+00014ef0: 6120 6f72 206e 6f74 2023 2323 2323 230a  a or not ######.
+00014f00: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00014f10: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00014f20: 7374 616e 6365 2874 6573 745f 6461 7461  stance(test_data
+00014f30: 2c20 7374 7229 206f 7220 7465 7374 5f64  , str) or test_d
+00014f40: 6174 6120 6973 204e 6f6e 653a 0a20 2020  ata is None:.   
+00014f50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014f60: 6665 6174 7572 655f 6765 6e20 6f72 2066  feature_gen or f
+00014f70: 6561 7475 7265 5f74 7970 653a 0a20 2020  eature_type:.   
+00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f90: 2023 2323 2069 6620 6665 6174 7572 6520   ### if feature 
+00014fa0: 656e 6767 2069 7320 7065 7266 6f72 6d65  engg is performe
+00014fb0: 642c 2069 6420 636f 6c75 6d6e 7320 6172  d, id columns ar
+00014fc0: 6520 6472 6f70 7065 642e 2048 656e 6365  e dropped. Hence
+00014fd0: 2074 6865 7920 6d75 7374 2072 656a 6f69   they must rejoi
+00014fe0: 6e20 6865 7265 2e0a 2020 2020 2020 2020  n here..        
+00014ff0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00015000: 6e61 6d65 203d 2070 642e 636f 6e63 6174  name = pd.concat
+00015010: 285b 7472 6169 6e5f 6964 732c 2064 6174  ([train_ids, dat
+00015020: 616e 616d 655d 2c20 6178 6973 3d31 290a  aname], axis=1).
+00015030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015040: 7265 7475 726e 2069 6d70 6f72 7461 6e74  return important
+00015050: 5f66 6561 7475 7265 732c 2064 6174 616e  _features, datan
+00015060: 616d 655b 696d 706f 7274 616e 745f 6665  ame[important_fe
+00015070: 6174 7572 6573 2b74 6172 6765 745d 0a20  atures+target]. 
+00015080: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00015090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150a0: 2023 2320 5468 6973 2069 7320 666f 7220   ## This is for 
+000150b0: 7465 7374 2064 6174 6120 6578 6973 7469  test data existi
+000150c0: 6e67 2023 2323 230a 2020 2020 2020 2020  ng ####.        
+000150d0: 2020 2020 2020 2020 6966 2066 6561 7475          if featu
+000150e0: 7265 5f67 656e 206f 7220 6665 6174 7572  re_gen or featur
+000150f0: 655f 7479 7065 3a0a 2020 2020 2020 2020  e_type:.        
+00015100: 2020 2020 2020 2020 2020 2020 2323 2320              ### 
+00015110: 6966 2066 6561 7475 7265 2065 6e67 6720  if feature engg 
+00015120: 6973 2070 6572 666f 726d 6564 2c20 6964  is performed, id
+00015130: 2063 6f6c 756d 6e73 2061 7265 2064 726f   columns are dro
+00015140: 7070 6564 2e20 4865 6e63 6520 7468 6579  pped. Hence they
+00015150: 206d 7573 7420 7265 6a6f 696e 2068 6572   must rejoin her
+00015160: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+00015170: 2020 2020 2020 2064 6174 616e 616d 6520         dataname 
+00015180: 3d20 7064 2e63 6f6e 6361 7428 5b74 7261  = pd.concat([tra
+00015190: 696e 5f69 6473 2c20 6461 7461 6e61 6d65  in_ids, dataname
+000151a0: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
+000151b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000151c0: 6573 745f 6461 7461 203d 2070 642e 636f  est_data = pd.co
+000151d0: 6e63 6174 285b 7465 7374 5f69 6473 2c20  ncat([test_ids, 
+000151e0: 7465 7374 5f64 6174 615d 2c20 6178 6973  test_data], axis
+000151f0: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
+00015200: 2020 2020 2323 2320 596f 7520 7365 6c65      ### You sele
+00015210: 6374 2074 6865 2066 6561 7475 7265 7320  ct the features 
+00015220: 7769 7468 2074 6865 2073 616d 6520 6f6c  with the same ol
+00015230: 6420 6e61 6d65 7320 6173 2062 6566 6f72  d names as befor
+00015240: 6520 2323 2323 2323 230a 2020 2020 2020  e #######.      
+00015250: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00015260: 2064 6174 616e 616d 655b 696d 706f 7274   dataname[import
+00015270: 616e 745f 6665 6174 7572 6573 2b74 6172  ant_features+tar
+00015280: 6765 7473 5d2c 2074 6573 745f 6461 7461  gets], test_data
+00015290: 5b69 6d70 6f72 7461 6e74 5f66 6561 7475  [important_featu
+000152a0: 7265 735d 0a20 2020 2020 2020 2065 7863  res].        exc
+000152b0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+000152c0: 2070 7269 6e74 2827 5761 726e 696e 673a   print('Warning:
+000152d0: 2052 6574 7572 6e69 6e67 2077 6974 6820   Returning with 
+000152e0: 696d 706f 7274 616e 7420 6665 6174 7572  important featur
+000152f0: 6573 2061 6e64 2074 7261 696e 2e20 506c  es and train. Pl
+00015300: 6561 7365 2072 652d 6368 6563 6b20 796f  ease re-check yo
+00015310: 7572 206f 7574 7075 7473 2e27 290a 2020  ur outputs.').  
+00015320: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00015330: 2069 6d70 6f72 7461 6e74 5f66 6561 7475   important_featu
+00015340: 7265 732c 2064 6174 616e 616d 655b 696d  res, dataname[im
+00015350: 706f 7274 616e 745f 6665 6174 7572 6573  portant_features
+00015360: 2b74 6172 6765 7473 5d0a 2323 2323 2323  +targets].######
 00015370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015380: 2323 2323 2323 2323 0a64 6566 2072 656d  ########.def rem
-00015390: 6f76 655f 6869 6768 6c79 5f63 6f72 7265  ove_highly_corre
-000153a0: 6c61 7465 645f 7661 7273 5f66 6173 7428  lated_vars_fast(
-000153b0: 6466 2c20 636f 7272 5f6c 696d 6974 3d30  df, corr_limit=0
-000153c0: 2e37 3029 3a0a 2020 2020 2222 220a 2020  .70):.    """.  
-000153d0: 2020 5468 6973 2069 7320 6120 7369 6d70    This is a simp
-000153e0: 6c65 206d 6574 686f 6420 746f 2072 656d  le method to rem
-000153f0: 6f76 6520 6869 6768 6c79 2063 6f72 7265  ove highly corre
-00015400: 6c61 7465 6420 6665 6174 7572 6573 2066  lated features f
-00015410: 6173 7420 7573 696e 6720 5065 6172 736f  ast using Pearso
-00015420: 6e27 7320 436f 7272 656c 6174 696f 6e2e  n's Correlation.
-00015430: 0a20 2020 2055 7365 2074 6869 7320 6f6e  .    Use this on
-00015440: 6c79 2066 6f72 2066 6c6f 6174 2061 6e64  ly for float and
-00015450: 2069 6e74 6567 6572 2076 6172 6961 626c   integer variabl
-00015460: 6573 2e20 4974 2077 696c 6c20 6175 746f  es. It will auto
-00015470: 6d61 7469 6361 6c6c 7920 7365 6c65 6374  matically select
-00015480: 2074 686f 7365 206f 6e6c 792e 0a20 2020   those only..   
-00015490: 2049 7420 6361 6e20 6265 2075 7365 6420   It can be used 
-000154a0: 666f 7220 7665 7279 206c 6172 6765 2064  for very large d
-000154b0: 6174 6120 7365 7473 2077 6865 7265 2066  ata sets where f
-000154c0: 6561 7475 7265 7769 7a20 6861 7320 7472  eaturewiz has tr
-000154d0: 6f75 626c 6520 7769 7468 206d 656d 6f72  ouble with memor
-000154e0: 790a 2020 2020 2222 220a 2020 2020 2320  y.    """.    # 
-000154f0: 4372 6561 7469 6e67 2063 6f72 7265 6c61  Creating correla
-00015500: 7469 6f6e 206d 6174 7269 780a 2020 2020  tion matrix.    
-00015510: 636f 7272 656c 6174 696f 6e5f 6461 7461  correlation_data
-00015520: 6672 616d 6520 3d20 6466 2e63 6f72 7228  frame = df.corr(
-00015530: 292e 6162 7328 292e 6173 7479 7065 286e  ).abs().astype(n
-00015540: 702e 666c 6f61 7431 3629 0a20 2020 2023  p.float16).    #
-00015550: 2053 656c 6563 7469 6e67 2075 7070 6572   Selecting upper
-00015560: 2074 7269 616e 676c 6520 6f66 2063 6f72   triangle of cor
-00015570: 7265 6c61 7469 6f6e 206d 6174 7269 780a  relation matrix.
-00015580: 2020 2020 7570 7065 725f 7472 6920 3d20      upper_tri = 
-00015590: 636f 7272 656c 6174 696f 6e5f 6461 7461  correlation_data
-000155a0: 6672 616d 652e 7768 6572 6528 6e70 2e74  frame.where(np.t
-000155b0: 7269 7528 6e70 2e6f 6e65 7328 636f 7272  riu(np.ones(corr
-000155c0: 656c 6174 696f 6e5f 6461 7461 6672 616d  elation_datafram
-000155d0: 652e 7368 6170 6529 2c0a 2020 2020 2020  e.shape),.      
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155f0: 2020 2020 2020 2020 2020 2020 6b3d 3129              k=1)
-00015600: 2e61 7374 7970 6528 6e70 2e62 6f6f 6c29  .astype(np.bool)
-00015610: 290a 2020 2020 2320 4669 6e64 696e 6720  ).    # Finding 
-00015620: 696e 6465 7820 6f66 2066 6561 7475 7265  index of feature
-00015630: 2063 6f6c 756d 6e73 2077 6974 6820 636f   columns with co
-00015640: 7272 656c 6174 696f 6e20 6772 6561 7465  rrelation greate
-00015650: 7220 7468 616e 2030 2e39 350a 2020 2020  r than 0.95.    
-00015660: 746f 5f64 726f 7020 3d20 5b63 6f6c 756d  to_drop = [colum
-00015670: 6e20 666f 7220 636f 6c75 6d6e 2069 6e20  n for column in 
-00015680: 7570 7065 725f 7472 692e 636f 6c75 6d6e  upper_tri.column
-00015690: 7320 6966 2061 6e79 2875 7070 6572 5f74  s if any(upper_t
-000156a0: 7269 5b63 6f6c 756d 6e5d 203e 2063 6f72  ri[column] > cor
-000156b0: 725f 6c69 6d69 7429 5d0a 2020 2020 7072  r_limit)].    pr
-000156c0: 696e 7428 293b 0a20 2020 2070 7269 6e74  int();.    print
-000156d0: 2827 4869 6768 6c79 2063 6f72 7265 6c61  ('Highly correla
-000156e0: 7465 6420 636f 6c75 6d6e 7320 746f 2072  ted columns to r
-000156f0: 656d 6f76 653a 2025 7327 2025 746f 5f64  emove: %s' %to_d
-00015700: 726f 7029 0a20 2020 2072 6574 7572 6e20  rop).    return 
-00015710: 746f 5f64 726f 700a 2323 2323 2323 2323  to_drop.########
-00015720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000153a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000153b0: 2323 2323 2323 2323 2323 0a64 6566 2072  ##########.def r
+000153c0: 656d 6f76 655f 6869 6768 6c79 5f63 6f72  emove_highly_cor
+000153d0: 7265 6c61 7465 645f 7661 7273 5f66 6173  related_vars_fas
+000153e0: 7428 6466 2c20 636f 7272 5f6c 696d 6974  t(df, corr_limit
+000153f0: 3d30 2e37 3029 3a0a 2020 2020 2222 220a  =0.70):.    """.
+00015400: 2020 2020 5468 6973 2069 7320 6120 7369      This is a si
+00015410: 6d70 6c65 206d 6574 686f 6420 746f 2072  mple method to r
+00015420: 656d 6f76 6520 6869 6768 6c79 2063 6f72  emove highly cor
+00015430: 7265 6c61 7465 6420 6665 6174 7572 6573  related features
+00015440: 2066 6173 7420 7573 696e 6720 5065 6172   fast using Pear
+00015450: 736f 6e27 7320 436f 7272 656c 6174 696f  son's Correlatio
+00015460: 6e2e 0a20 2020 2055 7365 2074 6869 7320  n..    Use this 
+00015470: 6f6e 6c79 2066 6f72 2066 6c6f 6174 2061  only for float a
+00015480: 6e64 2069 6e74 6567 6572 2076 6172 6961  nd integer varia
+00015490: 626c 6573 2e20 4974 2077 696c 6c20 6175  bles. It will au
+000154a0: 746f 6d61 7469 6361 6c6c 7920 7365 6c65  tomatically sele
+000154b0: 6374 2074 686f 7365 206f 6e6c 792e 0a20  ct those only.. 
+000154c0: 2020 2049 7420 6361 6e20 6265 2075 7365     It can be use
+000154d0: 6420 666f 7220 7665 7279 206c 6172 6765  d for very large
+000154e0: 2064 6174 6120 7365 7473 2077 6865 7265   data sets where
+000154f0: 2066 6561 7475 7265 7769 7a20 6861 7320   featurewiz has 
+00015500: 7472 6f75 626c 6520 7769 7468 206d 656d  trouble with mem
+00015510: 6f72 790a 2020 2020 2222 220a 2020 2020  ory.    """.    
+00015520: 2320 4372 6561 7469 6e67 2063 6f72 7265  # Creating corre
+00015530: 6c61 7469 6f6e 206d 6174 7269 780a 2020  lation matrix.  
+00015540: 2020 636f 7272 656c 6174 696f 6e5f 6461    correlation_da
+00015550: 7461 6672 616d 6520 3d20 6466 2e63 6f72  taframe = df.cor
+00015560: 7228 292e 6162 7328 292e 6173 7479 7065  r().abs().astype
+00015570: 286e 702e 666c 6f61 7431 3629 0a20 2020  (np.float16).   
+00015580: 2023 2053 656c 6563 7469 6e67 2075 7070   # Selecting upp
+00015590: 6572 2074 7269 616e 676c 6520 6f66 2063  er triangle of c
+000155a0: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
+000155b0: 780a 2020 2020 7570 7065 725f 7472 6920  x.    upper_tri 
+000155c0: 3d20 636f 7272 656c 6174 696f 6e5f 6461  = correlation_da
+000155d0: 7461 6672 616d 652e 7768 6572 6528 6e70  taframe.where(np
+000155e0: 2e74 7269 7528 6e70 2e6f 6e65 7328 636f  .triu(np.ones(co
+000155f0: 7272 656c 6174 696f 6e5f 6461 7461 6672  rrelation_datafr
+00015600: 616d 652e 7368 6170 6529 2c0a 2020 2020  ame.shape),.    
+00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015620: 2020 2020 2020 2020 2020 2020 2020 6b3d                k=
+00015630: 3129 2e61 7374 7970 6528 6e70 2e62 6f6f  1).astype(np.boo
+00015640: 6c29 290a 2020 2020 2320 4669 6e64 696e  l)).    # Findin
+00015650: 6720 696e 6465 7820 6f66 2066 6561 7475  g index of featu
+00015660: 7265 2063 6f6c 756d 6e73 2077 6974 6820  re columns with 
+00015670: 636f 7272 656c 6174 696f 6e20 6772 6561  correlation grea
+00015680: 7465 7220 7468 616e 2030 2e39 350a 2020  ter than 0.95.  
+00015690: 2020 746f 5f64 726f 7020 3d20 5b63 6f6c    to_drop = [col
+000156a0: 756d 6e20 666f 7220 636f 6c75 6d6e 2069  umn for column i
+000156b0: 6e20 7570 7065 725f 7472 692e 636f 6c75  n upper_tri.colu
+000156c0: 6d6e 7320 6966 2061 6e79 2875 7070 6572  mns if any(upper
+000156d0: 5f74 7269 5b63 6f6c 756d 6e5d 203e 2063  _tri[column] > c
+000156e0: 6f72 725f 6c69 6d69 7429 5d0a 2020 2020  orr_limit)].    
+000156f0: 7072 696e 7428 293b 0a20 2020 2070 7269  print();.    pri
+00015700: 6e74 2827 4869 6768 6c79 2063 6f72 7265  nt('Highly corre
+00015710: 6c61 7465 6420 636f 6c75 6d6e 7320 746f  lated columns to
+00015720: 2072 656d 6f76 653a 2025 7327 2025 746f   remove: %s' %to
+00015730: 5f64 726f 7029 0a20 2020 2072 6574 7572  _drop).    retur
+00015740: 6e20 746f 5f64 726f 700a 2323 2323 2323  n to_drop.######
 00015750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015760: 2323 2323 2323 2323 2323 2323 230a 696d  #############.im
-00015770: 706f 7274 206d 756c 7469 7072 6f63 6573  port multiproces
-00015780: 7369 6e67 0a64 6566 2067 6574 5f63 7075  sing.def get_cpu
-00015790: 5f77 6f72 6b65 725f 636f 756e 7428 293a  _worker_count():
-000157a0: 0a20 2020 2072 6574 7572 6e20 6d75 6c74  .    return mult
-000157b0: 6970 726f 6365 7373 696e 672e 6370 755f  iprocessing.cpu_
-000157c0: 636f 756e 7428 290a 2323 2323 2323 2323  count().########
-000157d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000157e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000157f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015790: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+000157a0: 696d 706f 7274 206d 756c 7469 7072 6f63  import multiproc
+000157b0: 6573 7369 6e67 0a64 6566 2067 6574 5f63  essing.def get_c
+000157c0: 7075 5f77 6f72 6b65 725f 636f 756e 7428  pu_worker_count(
+000157d0: 293a 0a20 2020 2072 6574 7572 6e20 6d75  ):.    return mu
+000157e0: 6c74 6970 726f 6365 7373 696e 672e 6370  ltiprocessing.cp
+000157f0: 755f 636f 756e 7428 290a 2323 2323 2323  u_count().######
 00015800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00015810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015820: 2323 2323 230a 6672 6f6d 2069 7465 7274  #####.from itert
-00015830: 6f6f 6c73 2069 6d70 6f72 7420 636f 6d62  ools import comb
-00015840: 696e 6174 696f 6e73 0a69 6d70 6f72 7420  inations.import 
-00015850: 6d61 7470 6c6f 746c 6962 2e70 6174 6368  matplotlib.patch
-00015860: 6573 2061 7320 6d70 6174 6368 6573 0a69  es as mpatches.i
-00015870: 6d70 6f72 7420 6d61 7470 6c6f 746c 6962  mport matplotlib
-00015880: 2e70 7970 6c6f 7420 6173 2070 6c74 0a66  .pyplot as plt.f
-00015890: 726f 6d20 736b 6c65 6172 6e2e 6665 6174  rom sklearn.feat
-000158a0: 7572 655f 7365 6c65 6374 696f 6e20 696d  ure_selection im
-000158b0: 706f 7274 2063 6869 322c 206d 7574 7561  port chi2, mutua
-000158c0: 6c5f 696e 666f 5f72 6567 7265 7373 696f  l_info_regressio
-000158d0: 6e2c 206d 7574 7561 6c5f 696e 666f 5f63  n, mutual_info_c
-000158e0: 6c61 7373 6966 0a66 726f 6d20 736b 6c65  lassif.from skle
-000158f0: 6172 6e2e 6665 6174 7572 655f 7365 6c65  arn.feature_sele
-00015900: 6374 696f 6e20 696d 706f 7274 2053 656c  ction import Sel
-00015910: 6563 744b 4265 7374 0a69 6d70 6f72 7420  ectKBest.import 
-00015920: 7867 626f 6f73 740a 6465 6620 6472 6177  xgboost.def draw
-00015930: 5f66 6561 7475 7265 5f69 6d70 6f72 7461  _feature_importa
-00015940: 6e63 6573 5f6d 756c 7469 5f6c 6162 656c  nces_multi_label
-00015950: 2862 7374 5f6d 6f64 656c 732c 2064 6173  (bst_models, das
-00015960: 6b5f 7867 626f 6f73 745f 666c 6167 3d46  k_xgboost_flag=F
-00015970: 616c 7365 293a 0a20 2020 2072 6f77 7320  alse):.    rows 
-00015980: 3d20 696e 7428 6c65 6e28 6273 745f 6d6f  = int(len(bst_mo
-00015990: 6465 6c73 292f 3220 2b20 302e 3529 0a20  dels)/2 + 0.5). 
-000159a0: 2020 2063 6f6c 7573 203d 2032 0a20 2020     colus = 2.   
-000159b0: 2066 6967 2c20 6178 203d 2070 6c74 2e73   fig, ax = plt.s
-000159c0: 7562 706c 6f74 7328 726f 7773 2c20 636f  ubplots(rows, co
-000159d0: 6c75 7329 0a20 2020 2066 6967 2e73 6574  lus).    fig.set
-000159e0: 5f73 697a 655f 696e 6368 6573 286d 696e  _size_inches(min
-000159f0: 2863 6f6c 7573 2a35 2c32 3029 2c72 6f77  (colus*5,20),row
-00015a00: 732a 3529 0a20 2020 2066 6967 2e73 7562  s*5).    fig.sub
-00015a10: 706c 6f74 735f 6164 6a75 7374 2868 7370  plots_adjust(hsp
-00015a20: 6163 653d 302e 3529 2023 2323 2054 6869  ace=0.5) ### Thi
-00015a30: 7320 636f 6e74 726f 6c73 2074 6865 2073  s controls the s
-00015a40: 7061 6365 2062 6574 7765 6e20 726f 7773  pace betwen rows
-00015a50: 0a20 2020 2066 6967 2e73 7562 706c 6f74  .    fig.subplot
-00015a60: 735f 6164 6a75 7374 2877 7370 6163 653d  s_adjust(wspace=
-00015a70: 302e 3529 2023 2323 2054 6869 7320 636f  0.5) ### This co
-00015a80: 6e74 726f 6c73 2074 6865 2073 7061 6365  ntrols the space
-00015a90: 2062 6574 7765 656e 2063 6f6c 756d 6e73   between columns
-00015aa0: 0a20 2020 2063 6f75 6e74 6572 203d 2030  .    counter = 0
-00015ab0: 0a20 2020 2069 6620 726f 7773 203d 3d20  .    if rows == 
-00015ac0: 313a 0a20 2020 2020 2020 2061 7820 3d20  1:.        ax = 
-00015ad0: 6178 2e72 6573 6861 7065 282d 312c 3129  ax.reshape(-1,1)
-00015ae0: 2e54 0a20 2020 2066 6f72 206b 2069 6e20  .T.    for k in 
-00015af0: 6e70 2e61 7261 6e67 6528 726f 7773 293a  np.arange(rows):
-00015b00: 0a20 2020 2020 2020 2066 6f72 206c 2069  .        for l i
-00015b10: 6e20 6e70 2e61 7261 6e67 6528 636f 6c75  n np.arange(colu
-00015b20: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00015b30: 6966 2063 6f75 6e74 6572 203c 206c 656e  if counter < len
-00015b40: 2862 7374 5f6d 6f64 656c 7329 3a0a 2020  (bst_models):.  
-00015b50: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00015b60: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00015b70: 2020 2020 2020 2062 7374 5f62 6f6f 7374         bst_boost
-00015b80: 6572 203d 2062 7374 5f6d 6f64 656c 735b  er = bst_models[
-00015b90: 636f 756e 7465 725d 2e65 7374 696d 6174  counter].estimat
-00015ba0: 6f72 735f 5b30 5d0a 2020 2020 2020 2020  ors_[0].        
-00015bb0: 2020 2020 2020 2020 2020 2020 6178 3120              ax1 
-00015bc0: 3d20 7867 626f 6f73 742e 706c 6f74 5f69  = xgboost.plot_i
-00015bd0: 6d70 6f72 7461 6e63 6528 6273 745f 626f  mportance(bst_bo
-00015be0: 6f73 7465 722c 2068 6569 6768 743d 302e  oster, height=0.
-00015bf0: 382c 2073 686f 775f 7661 6c75 6573 3d46  8, show_values=F
-00015c00: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c20: 2020 696d 706f 7274 616e 6365 5f74 7970    importance_typ
-00015c30: 653d 2767 6169 6e27 2c20 6d61 785f 6e75  e='gain', max_nu
-00015c40: 6d5f 6665 6174 7572 6573 3d31 302c 2061  m_features=10, a
-00015c50: 783d 6178 5b6b 5d5b 6c5d 290a 2020 2020  x=ax[k][l]).    
-00015c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c70: 6178 312e 7365 745f 7469 746c 6528 274d  ax1.set_title('M
-00015c80: 756c 7469 5f6c 6162 656c 3a20 546f 7020  ulti_label: Top 
-00015c90: 3130 2066 6561 7475 7265 7320 666f 7220  10 features for 
-00015ca0: 6669 7273 7420 6c61 6265 6c3a 2072 6f75  first label: rou
-00015cb0: 6e64 2025 7327 2025 2863 6f75 6e74 6572  nd %s' %(counter
-00015cc0: 2b31 2929 0a20 2020 2020 2020 2020 2020  +1)).           
-00015cd0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
-00015d00: 2020 636f 756e 7465 7220 2b3d 2031 0a20    counter += 1. 
-00015d10: 2020 2070 6c74 2e73 686f 7728 293b 0a23     plt.show();.#
-00015d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015d40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015850: 2323 2323 2323 230a 6672 6f6d 2069 7465  #######.from ite
+00015860: 7274 6f6f 6c73 2069 6d70 6f72 7420 636f  rtools import co
+00015870: 6d62 696e 6174 696f 6e73 0a69 6d70 6f72  mbinations.impor
+00015880: 7420 6d61 7470 6c6f 746c 6962 2e70 6174  t matplotlib.pat
+00015890: 6368 6573 2061 7320 6d70 6174 6368 6573  ches as mpatches
+000158a0: 0a69 6d70 6f72 7420 6d61 7470 6c6f 746c  .import matplotl
+000158b0: 6962 2e70 7970 6c6f 7420 6173 2070 6c74  ib.pyplot as plt
+000158c0: 0a66 726f 6d20 736b 6c65 6172 6e2e 6665  .from sklearn.fe
+000158d0: 6174 7572 655f 7365 6c65 6374 696f 6e20  ature_selection 
+000158e0: 696d 706f 7274 2063 6869 322c 206d 7574  import chi2, mut
+000158f0: 7561 6c5f 696e 666f 5f72 6567 7265 7373  ual_info_regress
+00015900: 696f 6e2c 206d 7574 7561 6c5f 696e 666f  ion, mutual_info
+00015910: 5f63 6c61 7373 6966 0a66 726f 6d20 736b  _classif.from sk
+00015920: 6c65 6172 6e2e 6665 6174 7572 655f 7365  learn.feature_se
+00015930: 6c65 6374 696f 6e20 696d 706f 7274 2053  lection import S
+00015940: 656c 6563 744b 4265 7374 0a69 6d70 6f72  electKBest.impor
+00015950: 7420 7867 626f 6f73 740a 6465 6620 6472  t xgboost.def dr
+00015960: 6177 5f66 6561 7475 7265 5f69 6d70 6f72  aw_feature_impor
+00015970: 7461 6e63 6573 5f6d 756c 7469 5f6c 6162  tances_multi_lab
+00015980: 656c 2862 7374 5f6d 6f64 656c 732c 2064  el(bst_models, d
+00015990: 6173 6b5f 7867 626f 6f73 745f 666c 6167  ask_xgboost_flag
+000159a0: 3d46 616c 7365 293a 0a20 2020 2072 6f77  =False):.    row
+000159b0: 7320 3d20 696e 7428 6c65 6e28 6273 745f  s = int(len(bst_
+000159c0: 6d6f 6465 6c73 292f 3220 2b20 302e 3529  models)/2 + 0.5)
+000159d0: 0a20 2020 2063 6f6c 7573 203d 2032 0a20  .    colus = 2. 
+000159e0: 2020 2066 6967 2c20 6178 203d 2070 6c74     fig, ax = plt
+000159f0: 2e73 7562 706c 6f74 7328 726f 7773 2c20  .subplots(rows, 
+00015a00: 636f 6c75 7329 0a20 2020 2066 6967 2e73  colus).    fig.s
+00015a10: 6574 5f73 697a 655f 696e 6368 6573 286d  et_size_inches(m
+00015a20: 696e 2863 6f6c 7573 2a35 2c32 3029 2c72  in(colus*5,20),r
+00015a30: 6f77 732a 3529 0a20 2020 2066 6967 2e73  ows*5).    fig.s
+00015a40: 7562 706c 6f74 735f 6164 6a75 7374 2868  ubplots_adjust(h
+00015a50: 7370 6163 653d 302e 3529 2023 2323 2054  space=0.5) ### T
+00015a60: 6869 7320 636f 6e74 726f 6c73 2074 6865  his controls the
+00015a70: 2073 7061 6365 2062 6574 7765 6e20 726f   space betwen ro
+00015a80: 7773 0a20 2020 2066 6967 2e73 7562 706c  ws.    fig.subpl
+00015a90: 6f74 735f 6164 6a75 7374 2877 7370 6163  ots_adjust(wspac
+00015aa0: 653d 302e 3529 2023 2323 2054 6869 7320  e=0.5) ### This 
+00015ab0: 636f 6e74 726f 6c73 2074 6865 2073 7061  controls the spa
+00015ac0: 6365 2062 6574 7765 656e 2063 6f6c 756d  ce between colum
+00015ad0: 6e73 0a20 2020 2063 6f75 6e74 6572 203d  ns.    counter =
+00015ae0: 2030 0a20 2020 2069 6620 726f 7773 203d   0.    if rows =
+00015af0: 3d20 313a 0a20 2020 2020 2020 2061 7820  = 1:.        ax 
+00015b00: 3d20 6178 2e72 6573 6861 7065 282d 312c  = ax.reshape(-1,
+00015b10: 3129 2e54 0a20 2020 2066 6f72 206b 2069  1).T.    for k i
+00015b20: 6e20 6e70 2e61 7261 6e67 6528 726f 7773  n np.arange(rows
+00015b30: 293a 0a20 2020 2020 2020 2066 6f72 206c  ):.        for l
+00015b40: 2069 6e20 6e70 2e61 7261 6e67 6528 636f   in np.arange(co
+00015b50: 6c75 7329 3a0a 2020 2020 2020 2020 2020  lus):.          
+00015b60: 2020 6966 2063 6f75 6e74 6572 203c 206c    if counter < l
+00015b70: 656e 2862 7374 5f6d 6f64 656c 7329 3a0a  en(bst_models):.
+00015b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b90: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00015ba0: 2020 2020 2020 2020 2062 7374 5f62 6f6f           bst_boo
+00015bb0: 7374 6572 203d 2062 7374 5f6d 6f64 656c  ster = bst_model
+00015bc0: 735b 636f 756e 7465 725d 2e65 7374 696d  s[counter].estim
+00015bd0: 6174 6f72 735f 5b30 5d0a 2020 2020 2020  ators_[0].      
+00015be0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00015bf0: 3120 3d20 7867 626f 6f73 742e 706c 6f74  1 = xgboost.plot
+00015c00: 5f69 6d70 6f72 7461 6e63 6528 6273 745f  _importance(bst_
+00015c10: 626f 6f73 7465 722c 2068 6569 6768 743d  booster, height=
+00015c20: 302e 382c 2073 686f 775f 7661 6c75 6573  0.8, show_values
+00015c30: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00015c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c50: 2020 2020 696d 706f 7274 616e 6365 5f74      importance_t
+00015c60: 7970 653d 2767 6169 6e27 2c20 6d61 785f  ype='gain', max_
+00015c70: 6e75 6d5f 6665 6174 7572 6573 3d31 302c  num_features=10,
+00015c80: 2061 783d 6178 5b6b 5d5b 6c5d 290a 2020   ax=ax[k][l]).  
+00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ca0: 2020 6178 312e 7365 745f 7469 746c 6528    ax1.set_title(
+00015cb0: 274d 756c 7469 5f6c 6162 656c 3a20 546f  'Multi_label: To
+00015cc0: 7020 3130 2066 6561 7475 7265 7320 666f  p 10 features fo
+00015cd0: 7220 6669 7273 7420 6c61 6265 6c3a 2072  r first label: r
+00015ce0: 6f75 6e64 2025 7327 2025 2863 6f75 6e74  ound %s' %(count
+00015cf0: 6572 2b31 2929 0a20 2020 2020 2020 2020  er+1)).         
+00015d00: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d20: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+00015d30: 2020 2020 636f 756e 7465 7220 2b3d 2031      counter += 1
+00015d40: 0a20 2020 2070 6c74 2e73 686f 7728 293b  .    plt.show();
+00015d50: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
 00015d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015d70: 2323 2323 2323 230a 6465 6620 6472 6177  #######.def draw
-00015d80: 5f66 6561 7475 7265 5f69 6d70 6f72 7461  _feature_importa
-00015d90: 6e63 6573 5f73 696e 676c 655f 6c61 6265  nces_single_labe
-00015da0: 6c28 6273 745f 6d6f 6465 6c73 2c20 6461  l(bst_models, da
-00015db0: 736b 5f78 6762 6f6f 7374 5f66 6c61 673d  sk_xgboost_flag=
-00015dc0: 4661 6c73 6529 3a0a 2020 2020 726f 7773  False):.    rows
-00015dd0: 203d 2069 6e74 286c 656e 2862 7374 5f6d   = int(len(bst_m
-00015de0: 6f64 656c 7329 2f32 202b 2030 2e35 290a  odels)/2 + 0.5).
-00015df0: 2020 2020 636f 6c75 7320 3d20 320a 2020      colus = 2.  
-00015e00: 2020 6669 672c 2061 7820 3d20 706c 742e    fig, ax = plt.
-00015e10: 7375 6270 6c6f 7473 2872 6f77 732c 2063  subplots(rows, c
-00015e20: 6f6c 7573 290a 2020 2020 6669 672e 7365  olus).    fig.se
-00015e30: 745f 7369 7a65 5f69 6e63 6865 7328 6d69  t_size_inches(mi
-00015e40: 6e28 636f 6c75 732a 352c 3230 292c 726f  n(colus*5,20),ro
-00015e50: 7773 2a35 290a 2020 2020 6669 672e 7375  ws*5).    fig.su
-00015e60: 6270 6c6f 7473 5f61 646a 7573 7428 6873  bplots_adjust(hs
-00015e70: 7061 6365 3d30 2e35 2920 2323 2320 5468  pace=0.5) ### Th
-00015e80: 6973 2063 6f6e 7472 6f6c 7320 7468 6520  is controls the 
-00015e90: 7370 6163 6520 6265 7477 656e 2072 6f77  space betwen row
-00015ea0: 730a 2020 2020 6669 672e 7375 6270 6c6f  s.    fig.subplo
-00015eb0: 7473 5f61 646a 7573 7428 7773 7061 6365  ts_adjust(wspace
-00015ec0: 3d30 2e35 2920 2323 2320 5468 6973 2063  =0.5) ### This c
-00015ed0: 6f6e 7472 6f6c 7320 7468 6520 7370 6163  ontrols the spac
-00015ee0: 6520 6265 7477 6565 6e20 636f 6c75 6d6e  e between column
-00015ef0: 730a 2020 2020 636f 756e 7465 7220 3d20  s.    counter = 
-00015f00: 300a 2020 2020 6966 2072 6f77 7320 3d3d  0.    if rows ==
-00015f10: 2031 3a0a 2020 2020 2020 2020 6178 203d   1:.        ax =
-00015f20: 2061 782e 7265 7368 6170 6528 2d31 2c31   ax.reshape(-1,1
-00015f30: 292e 540a 2020 2020 666f 7220 6b20 696e  ).T.    for k in
-00015f40: 206e 702e 6172 616e 6765 2872 6f77 7329   np.arange(rows)
-00015f50: 3a0a 2020 2020 2020 2020 666f 7220 6c20  :.        for l 
-00015f60: 696e 206e 702e 6172 616e 6765 2863 6f6c  in np.arange(col
-00015f70: 7573 293a 0a20 2020 2020 2020 2020 2020  us):.           
-00015f80: 2069 6620 636f 756e 7465 7220 3c20 6c65   if counter < le
-00015f90: 6e28 6273 745f 6d6f 6465 6c73 293a 0a20  n(bst_models):. 
-00015fa0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00015fb0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00015fc0: 2020 2020 2020 2020 6273 745f 626f 6f73          bst_boos
-00015fd0: 7465 7220 3d20 6273 745f 6d6f 6465 6c73  ter = bst_models
-00015fe0: 5b63 6f75 6e74 6572 5d0a 2020 2020 2020  [counter].      
-00015ff0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-00016000: 3120 3d20 7867 626f 6f73 742e 706c 6f74  1 = xgboost.plot
-00016010: 5f69 6d70 6f72 7461 6e63 6528 6273 745f  _importance(bst_
-00016020: 626f 6f73 7465 722c 2068 6569 6768 743d  booster, height=
-00016030: 302e 382c 2073 686f 775f 7661 6c75 6573  0.8, show_values
-00016040: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00016050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016060: 2020 2020 696d 706f 7274 616e 6365 5f74      importance_t
-00016070: 7970 653d 2767 6169 6e27 2c20 6d61 785f  ype='gain', max_
-00016080: 6e75 6d5f 6665 6174 7572 6573 3d31 302c  num_features=10,
-00016090: 2061 783d 6178 5b6b 5d5b 6c5d 290a 2020   ax=ax[k][l]).  
-000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160b0: 2020 6178 312e 7365 745f 7469 746c 6528    ax1.set_title(
-000160c0: 2754 6f70 2031 3020 6665 6174 7572 6573  'Top 10 features
-000160d0: 2077 6974 6820 5847 4220 6d6f 6465 6c20   with XGB model 
-000160e0: 2573 2720 2528 636f 756e 7465 722b 3129  %s' %(counter+1)
-000160f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016100: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00016110: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016120: 7373 0a20 2020 2020 2020 2020 2020 2063  ss.            c
-00016130: 6f75 6e74 6572 202b 3d20 310a 2020 2020  ounter += 1.    
-00016140: 706c 742e 7368 6f77 2829 3b0a 2323 2323  plt.show();.####
-00016150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015da0: 2323 2323 2323 2323 230a 6465 6620 6472  #########.def dr
+00015db0: 6177 5f66 6561 7475 7265 5f69 6d70 6f72  aw_feature_impor
+00015dc0: 7461 6e63 6573 5f73 696e 676c 655f 6c61  tances_single_la
+00015dd0: 6265 6c28 6273 745f 6d6f 6465 6c73 2c20  bel(bst_models, 
+00015de0: 6461 736b 5f78 6762 6f6f 7374 5f66 6c61  dask_xgboost_fla
+00015df0: 673d 4661 6c73 6529 3a0a 2020 2020 726f  g=False):.    ro
+00015e00: 7773 203d 2069 6e74 286c 656e 2862 7374  ws = int(len(bst
+00015e10: 5f6d 6f64 656c 7329 2f32 202b 2030 2e35  _models)/2 + 0.5
+00015e20: 290a 2020 2020 636f 6c75 7320 3d20 320a  ).    colus = 2.
+00015e30: 2020 2020 6669 672c 2061 7820 3d20 706c      fig, ax = pl
+00015e40: 742e 7375 6270 6c6f 7473 2872 6f77 732c  t.subplots(rows,
+00015e50: 2063 6f6c 7573 290a 2020 2020 6669 672e   colus).    fig.
+00015e60: 7365 745f 7369 7a65 5f69 6e63 6865 7328  set_size_inches(
+00015e70: 6d69 6e28 636f 6c75 732a 352c 3230 292c  min(colus*5,20),
+00015e80: 726f 7773 2a35 290a 2020 2020 6669 672e  rows*5).    fig.
+00015e90: 7375 6270 6c6f 7473 5f61 646a 7573 7428  subplots_adjust(
+00015ea0: 6873 7061 6365 3d30 2e35 2920 2323 2320  hspace=0.5) ### 
+00015eb0: 5468 6973 2063 6f6e 7472 6f6c 7320 7468  This controls th
+00015ec0: 6520 7370 6163 6520 6265 7477 656e 2072  e space betwen r
+00015ed0: 6f77 730a 2020 2020 6669 672e 7375 6270  ows.    fig.subp
+00015ee0: 6c6f 7473 5f61 646a 7573 7428 7773 7061  lots_adjust(wspa
+00015ef0: 6365 3d30 2e35 2920 2323 2320 5468 6973  ce=0.5) ### This
+00015f00: 2063 6f6e 7472 6f6c 7320 7468 6520 7370   controls the sp
+00015f10: 6163 6520 6265 7477 6565 6e20 636f 6c75  ace between colu
+00015f20: 6d6e 730a 2020 2020 636f 756e 7465 7220  mns.    counter 
+00015f30: 3d20 300a 2020 2020 6966 2072 6f77 7320  = 0.    if rows 
+00015f40: 3d3d 2031 3a0a 2020 2020 2020 2020 6178  == 1:.        ax
+00015f50: 203d 2061 782e 7265 7368 6170 6528 2d31   = ax.reshape(-1
+00015f60: 2c31 292e 540a 2020 2020 666f 7220 6b20  ,1).T.    for k 
+00015f70: 696e 206e 702e 6172 616e 6765 2872 6f77  in np.arange(row
+00015f80: 7329 3a0a 2020 2020 2020 2020 666f 7220  s):.        for 
+00015f90: 6c20 696e 206e 702e 6172 616e 6765 2863  l in np.arange(c
+00015fa0: 6f6c 7573 293a 0a20 2020 2020 2020 2020  olus):.         
+00015fb0: 2020 2069 6620 636f 756e 7465 7220 3c20     if counter < 
+00015fc0: 6c65 6e28 6273 745f 6d6f 6465 6c73 293a  len(bst_models):
+00015fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015fe0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00015ff0: 2020 2020 2020 2020 2020 6273 745f 626f            bst_bo
+00016000: 6f73 7465 7220 3d20 6273 745f 6d6f 6465  oster = bst_mode
+00016010: 6c73 5b63 6f75 6e74 6572 5d0a 2020 2020  ls[counter].    
+00016020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016030: 6178 3120 3d20 7867 626f 6f73 742e 706c  ax1 = xgboost.pl
+00016040: 6f74 5f69 6d70 6f72 7461 6e63 6528 6273  ot_importance(bs
+00016050: 745f 626f 6f73 7465 722c 2068 6569 6768  t_booster, heigh
+00016060: 743d 302e 382c 2073 686f 775f 7661 6c75  t=0.8, show_valu
+00016070: 6573 3d46 616c 7365 2c0a 2020 2020 2020  es=False,.      
+00016080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016090: 2020 2020 2020 696d 706f 7274 616e 6365        importance
+000160a0: 5f74 7970 653d 2767 6169 6e27 2c20 6d61  _type='gain', ma
+000160b0: 785f 6e75 6d5f 6665 6174 7572 6573 3d31  x_num_features=1
+000160c0: 302c 2061 783d 6178 5b6b 5d5b 6c5d 290a  0, ax=ax[k][l]).
+000160d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160e0: 2020 2020 6178 312e 7365 745f 7469 746c      ax1.set_titl
+000160f0: 6528 2754 6f70 2031 3020 6665 6174 7572  e('Top 10 featur
+00016100: 6573 2077 6974 6820 5847 4220 6d6f 6465  es with XGB mode
+00016110: 6c20 2573 2720 2528 636f 756e 7465 722b  l %s' %(counter+
+00016120: 3129 290a 2020 2020 2020 2020 2020 2020  1)).            
+00016130: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016150: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00016160: 2063 6f75 6e74 6572 202b 3d20 310a 2020   counter += 1.  
+00016170: 2020 706c 742e 7368 6f77 2829 3b0a 2323    plt.show();.##
 00016180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000161a0: 2323 0a64 6566 2072 6564 7563 655f 6d65  ##.def reduce_me
-000161b0: 6d5f 7573 6167 6528 6466 293a 0a20 2020  m_usage(df):.   
-000161c0: 2022 2222 0a20 2020 2023 2323 2323 2323   """.    #######
-000161d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000161e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000161f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016200: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-00016210: 2020 2047 7265 6174 6c79 2069 6e64 6562     Greatly indeb
-00016220: 7465 6420 746f 203a 0a20 2020 2068 7474  ted to :.    htt
-00016230: 7073 3a2f 2f77 7777 2e6b 6167 676c 652e  ps://www.kaggle.
-00016240: 636f 6d2f 6172 6a61 6e73 6f2f 7265 6475  com/arjanso/redu
-00016250: 6369 6e67 2d64 6174 6166 7261 6d65 2d6d  cing-dataframe-m
-00016260: 656d 6f72 792d 7369 7a65 2d62 792d 3635  emory-size-by-65
-00016270: 0a20 2020 2020 2020 2066 6f72 2074 6869  .        for thi
-00016280: 7320 6675 6e63 7469 6f6e 2074 6f20 7265  s function to re
-00016290: 6475 6365 206d 656d 6f72 7920 7573 6167  duce memory usag
-000162a0: 652e 0a20 2020 2023 2323 2323 2323 2323  e..    #########
-000162b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000162c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000162d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000162e0: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-000162f0: 2049 7420 6973 2061 2062 6974 2073 6c6f   It is a bit slo
-00016300: 7720 6173 2069 7420 6974 6572 6174 6573  w as it iterates
-00016310: 2074 6872 6f75 6768 2061 6c6c 2074 6865   through all the
-00016320: 2063 6f6c 756d 6e73 206f 6620 6120 6461   columns of a da
-00016330: 7461 6672 616d 6520 616e 6420 6d6f 6469  taframe and modi
-00016340: 6669 6573 2064 6174 6120 7479 7065 730a  fies data types.
-00016350: 2020 2020 2020 2020 746f 2072 6564 7563          to reduc
-00016360: 6520 6d65 6d6f 7279 2075 7361 6765 2e20  e memory usage. 
-00016370: 4275 7420 6974 2068 6173 2062 6565 6e20  But it has been 
-00016380: 7368 6f77 6e20 746f 2072 6564 7563 6520  shown to reduce 
-00016390: 6d65 6d6f 7279 2075 7361 6765 2062 7920  memory usage by 
-000163a0: 3635 2520 6f72 2073 6f2e 2020 2020 2020  65% or so.      
-000163b0: 200a 2020 2020 2222 220a 2020 2020 7374   .    """.    st
-000163c0: 6172 745f 6d65 6d20 3d20 6466 2e6d 656d  art_mem = df.mem
-000163d0: 6f72 795f 7573 6167 6528 292e 7375 6d28  ory_usage().sum(
-000163e0: 2920 2f20 3130 3234 2a2a 320a 2020 2020  ) / 1024**2.    
-000163f0: 6966 2074 7970 6528 6466 2920 3d3d 2064  if type(df) == d
-00016400: 6173 6b2e 6461 7461 6672 616d 652e 636f  ask.dataframe.co
-00016410: 7265 2e44 6174 6146 7261 6d65 3a0a 2020  re.DataFrame:.  
-00016420: 2020 2020 2020 7374 6172 745f 6d65 6d20        start_mem 
-00016430: 3d20 7374 6172 745f 6d65 6d2e 636f 6d70  = start_mem.comp
-00016440: 7574 6528 290a 2020 2020 7072 696e 7428  ute().    print(
-00016450: 2720 2020 2043 6175 7469 6f6e 3a20 5765  '    Caution: We
-00016460: 2077 696c 6c20 7472 7920 746f 2072 6564   will try to red
-00016470: 7563 6520 7468 6520 6d65 6d6f 7279 2075  uce the memory u
-00016480: 7361 6765 206f 6620 6461 7461 6672 616d  sage of datafram
-00016490: 6520 6672 6f6d 207b 3a2e 3266 7d20 4d42  e from {:.2f} MB
-000164a0: 272e 666f 726d 6174 2873 7461 7274 5f6d  '.format(start_m
-000164b0: 656d 2929 0a20 2020 2063 6f6c 7320 3d20  em)).    cols = 
-000164c0: 6466 2e63 6f6c 756d 6e73 0a20 2020 2069  df.columns.    i
-000164d0: 6620 7479 7065 2864 6629 203d 3d20 6461  f type(df) == da
-000164e0: 736b 2e64 6174 6166 7261 6d65 2e63 6f72  sk.dataframe.cor
-000164f0: 652e 4461 7461 4672 616d 653a 0a20 2020  e.DataFrame:.   
-00016500: 2020 2020 2063 6f6c 7320 3d20 636f 6c73       cols = cols
-00016510: 2e74 6f6c 6973 7428 290a 0a20 2020 2066  .tolist()..    f
-00016520: 6f72 2063 6f6c 2069 6e20 636f 6c73 3a0a  or col in cols:.
-00016530: 2020 2020 2020 2020 636f 6c5f 7479 7065          col_type
-00016540: 203d 2064 665b 636f 6c5d 2e64 7479 7065   = df[col].dtype
-00016550: 0a20 2020 2020 2020 2069 6620 636f 6c5f  .        if col_
-00016560: 7479 7065 2021 3d20 6f62 6a65 6374 3a0a  type != object:.
-00016570: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00016580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016590: 2063 5f6d 696e 203d 2064 665b 636f 6c5d   c_min = df[col]
-000165a0: 2e6d 696e 2829 0a20 2020 2020 2020 2020  .min().         
-000165b0: 2020 2020 2020 2063 5f6d 6178 203d 2064         c_max = d
-000165c0: 665b 636f 6c5d 2e6d 6178 2829 0a20 2020  f[col].max().   
-000165d0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-000165e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165f0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00016600: 2020 2020 2020 6966 2074 7970 6528 6466        if type(df
-00016610: 2920 3d3d 2064 6173 6b2e 6461 7461 6672  ) == dask.datafr
-00016620: 616d 652e 636f 7265 2e44 6174 6146 7261  ame.core.DataFra
-00016630: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-00016640: 2020 2020 635f 6d69 6e20 3d20 635f 6d69      c_min = c_mi
-00016650: 6e2e 636f 6d70 7574 6528 290a 2020 2020  n.compute().    
-00016660: 2020 2020 2020 2020 2020 2020 635f 6d61              c_ma
-00016670: 7820 3d20 635f 6d61 782e 636f 6d70 7574  x = c_max.comput
-00016680: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00016690: 6966 2073 7472 2863 6f6c 5f74 7970 6529  if str(col_type)
-000166a0: 5b3a 335d 203d 3d20 2769 6e74 273a 0a20  [:3] == 'int':. 
-000166b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000166c0: 6620 635f 6d69 6e20 3e20 6e70 2e69 696e  f c_min > np.iin
-000166d0: 666f 286e 702e 696e 7438 292e 6d69 6e20  fo(np.int8).min 
-000166e0: 616e 6420 635f 6d61 7820 3c20 6e70 2e69  and c_max < np.i
-000166f0: 696e 666f 286e 702e 696e 7438 292e 6d61  info(np.int8).ma
-00016700: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-00016710: 2020 2020 2020 2064 665b 636f 6c5d 203d         df[col] =
-00016720: 2064 665b 636f 6c5d 2e61 7374 7970 6528   df[col].astype(
-00016730: 6e70 2e69 6e74 3829 0a20 2020 2020 2020  np.int8).       
-00016740: 2020 2020 2020 2020 2065 6c69 6620 635f           elif c_
-00016750: 6d69 6e20 3e20 6e70 2e69 696e 666f 286e  min > np.iinfo(n
-00016760: 702e 696e 7431 3629 2e6d 696e 2061 6e64  p.int16).min and
-00016770: 2063 5f6d 6178 203c 206e 702e 6969 6e66   c_max < np.iinf
-00016780: 6f28 6e70 2e69 6e74 3136 292e 6d61 783a  o(np.int16).max:
-00016790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000167a0: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
-000167b0: 665b 636f 6c5d 2e61 7374 7970 6528 6e70  f[col].astype(np
-000167c0: 2e69 6e74 3136 290a 2020 2020 2020 2020  .int16).        
-000167d0: 2020 2020 2020 2020 656c 6966 2063 5f6d          elif c_m
-000167e0: 696e 203e 206e 702e 6969 6e66 6f28 6e70  in > np.iinfo(np
-000167f0: 2e69 6e74 3332 292e 6d69 6e20 616e 6420  .int32).min and 
-00016800: 635f 6d61 7820 3c20 6e70 2e69 696e 666f  c_max < np.iinfo
-00016810: 286e 702e 696e 7433 3229 2e6d 6178 3a0a  (np.int32).max:.
-00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016830: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
-00016840: 5b63 6f6c 5d2e 6173 7479 7065 286e 702e  [col].astype(np.
-00016850: 696e 7433 3229 0a20 2020 2020 2020 2020  int32).         
-00016860: 2020 2020 2020 2065 6c69 6620 635f 6d69         elif c_mi
-00016870: 6e20 3e20 6e70 2e69 696e 666f 286e 702e  n > np.iinfo(np.
-00016880: 696e 7436 3429 2e6d 696e 2061 6e64 2063  int64).min and c
-00016890: 5f6d 6178 203c 206e 702e 6969 6e66 6f28  _max < np.iinfo(
-000168a0: 6e70 2e69 6e74 3634 292e 6d61 783a 0a20  np.int64).max:. 
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 2020 2064 665b 636f 6c5d 203d 2064 665b     df[col] = df[
-000168d0: 636f 6c5d 2e61 7374 7970 6528 6e70 2e69  col].astype(np.i
-000168e0: 6e74 3634 2920 200a 2020 2020 2020 2020  nt64)  .        
-000168f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00016900: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00016910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016920: 2020 2069 6620 635f 6d69 6e20 3e20 6e70     if c_min > np
-00016930: 2e66 696e 666f 286e 702e 666c 6f61 7431  .finfo(np.float1
-00016940: 3629 2e6d 696e 2061 6e64 2063 5f6d 6178  6).min and c_max
-00016950: 203c 206e 702e 6669 6e66 6f28 6e70 2e66   < np.finfo(np.f
-00016960: 6c6f 6174 3136 292e 6d61 783a 0a20 2020  loat16).max:.   
-00016970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016980: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
-00016990: 665b 636f 6c5d 2e61 7374 7970 6528 6e70  f[col].astype(np
-000169a0: 2e66 6c6f 6174 3136 290a 2020 2020 2020  .float16).      
-000169b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000169c0: 6966 2063 5f6d 696e 203e 206e 702e 6669  if c_min > np.fi
-000169d0: 6e66 6f28 6e70 2e66 6c6f 6174 3332 292e  nfo(np.float32).
-000169e0: 6d69 6e20 616e 6420 635f 6d61 7820 3c20  min and c_max < 
-000169f0: 6e70 2e66 696e 666f 286e 702e 666c 6f61  np.finfo(np.floa
-00016a00: 7433 3229 2e6d 6178 3a0a 2020 2020 2020  t32).max:.      
-00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a20: 2020 6466 5b63 6f6c 5d20 3d20 6466 5b63    df[col] = df[c
-00016a30: 6f6c 5d2e 6173 7479 7065 286e 702e 666c  ol].astype(np.fl
-00016a40: 6f61 7433 3229 0a20 2020 2020 2020 2020  oat32).         
-00016a50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00016a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016a70: 2020 2020 2020 2020 2064 665b 636f 6c5d           df[col]
-00016a80: 203d 2064 665b 636f 6c5d 2e61 7374 7970   = df[col].astyp
-00016a90: 6528 6e70 2e66 6c6f 6174 3634 290a 2020  e(np.float64).  
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00016ab0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-00016ac0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00016ad0: 7565 0a20 2020 2020 2020 2065 6c73 653a  ue.        else:
-00016ae0: 0a20 2020 2020 2020 2020 2020 2064 665b  .            df[
-00016af0: 636f 6c5d 203d 2064 665b 636f 6c5d 2e61  col] = df[col].a
-00016b00: 7374 7970 6528 2763 6174 6567 6f72 7927  stype('category'
-00016b10: 290a 0a20 2020 2023 2323 2323 2323 2020  )..    #######  
-00016b20: 5265 7375 6c74 7320 6166 7465 7220 6d65  Results after me
-00016b30: 6d6f 7279 2075 7361 6765 2066 756e 6374  mory usage funct
-00016b40: 696f 6e20 2323 2323 2323 2323 2323 2323  ion ############
-00016b50: 2323 2323 2323 230a 2020 2020 656e 645f  #######.    end_
-00016b60: 6d65 6d20 3d20 6466 2e6d 656d 6f72 795f  mem = df.memory_
-00016b70: 7573 6167 6528 292e 7375 6d28 2920 2f20  usage().sum() / 
-00016b80: 3130 3234 2a2a 320a 2020 2020 6966 2074  1024**2.    if t
-00016b90: 7970 6528 6466 2920 3d3d 2064 6173 6b2e  ype(df) == dask.
-00016ba0: 6461 7461 6672 616d 652e 636f 7265 2e44  dataframe.core.D
-00016bb0: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
-00016bc0: 2020 656e 645f 6d65 6d20 3d20 656e 645f    end_mem = end_
-00016bd0: 6d65 6d2e 636f 6d70 7574 6528 290a 2020  mem.compute().  
-00016be0: 2020 7072 696e 7428 2720 2020 2020 2020    print('       
-00016bf0: 206d 656d 6f72 7920 7573 6167 6520 6166   memory usage af
-00016c00: 7465 7220 6f70 7469 6d69 7a61 7469 6f6e  ter optimization
-00016c10: 2069 733a 207b 3a2e 3266 7d20 4d42 272e   is: {:.2f} MB'.
-00016c20: 666f 726d 6174 2865 6e64 5f6d 656d 2929  format(end_mem))
-00016c30: 0a20 2020 2070 7269 6e74 2827 2020 2020  .    print('    
-00016c40: 2020 2020 6465 6372 6561 7365 6420 6279      decreased by
-00016c50: 207b 3a2e 3166 7d25 272e 666f 726d 6174   {:.1f}%'.format
-00016c60: 2831 3030 202a 2028 7374 6172 745f 6d65  (100 * (start_me
-00016c70: 6d20 2d20 656e 645f 6d65 6d29 202f 2073  m - end_mem) / s
-00016c80: 7461 7274 5f6d 656d 2929 0a20 2020 200a  tart_mem)).    .
-00016c90: 2020 2020 7265 7475 726e 2064 660a 2323      return df.##
-00016ca0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000161a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000161b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000161c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000161d0: 2323 2323 0a64 6566 2072 6564 7563 655f  ####.def reduce_
+000161e0: 6d65 6d5f 7573 6167 6528 6466 293a 0a20  mem_usage(df):. 
+000161f0: 2020 2022 2222 0a20 2020 2023 2323 2323     """.    #####
+00016200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016240: 0a20 2020 2047 7265 6174 6c79 2069 6e64  .    Greatly ind
+00016250: 6562 7465 6420 746f 203a 0a20 2020 2068  ebted to :.    h
+00016260: 7474 7073 3a2f 2f77 7777 2e6b 6167 676c  ttps://www.kaggl
+00016270: 652e 636f 6d2f 6172 6a61 6e73 6f2f 7265  e.com/arjanso/re
+00016280: 6475 6369 6e67 2d64 6174 6166 7261 6d65  ducing-dataframe
+00016290: 2d6d 656d 6f72 792d 7369 7a65 2d62 792d  -memory-size-by-
+000162a0: 3635 0a20 2020 2020 2020 2066 6f72 2074  65.        for t
+000162b0: 6869 7320 6675 6e63 7469 6f6e 2074 6f20  his function to 
+000162c0: 7265 6475 6365 206d 656d 6f72 7920 7573  reduce memory us
+000162d0: 6167 652e 0a20 2020 2023 2323 2323 2323  age..    #######
+000162e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000162f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016310: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+00016320: 2020 2049 7420 6973 2061 2062 6974 2073     It is a bit s
+00016330: 6c6f 7720 6173 2069 7420 6974 6572 6174  low as it iterat
+00016340: 6573 2074 6872 6f75 6768 2061 6c6c 2074  es through all t
+00016350: 6865 2063 6f6c 756d 6e73 206f 6620 6120  he columns of a 
+00016360: 6461 7461 6672 616d 6520 616e 6420 6d6f  dataframe and mo
+00016370: 6469 6669 6573 2064 6174 6120 7479 7065  difies data type
+00016380: 730a 2020 2020 2020 2020 746f 2072 6564  s.        to red
+00016390: 7563 6520 6d65 6d6f 7279 2075 7361 6765  uce memory usage
+000163a0: 2e20 4275 7420 6974 2068 6173 2062 6565  . But it has bee
+000163b0: 6e20 7368 6f77 6e20 746f 2072 6564 7563  n shown to reduc
+000163c0: 6520 6d65 6d6f 7279 2075 7361 6765 2062  e memory usage b
+000163d0: 7920 3635 2520 6f72 2073 6f2e 2020 2020  y 65% or so.    
+000163e0: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
+000163f0: 7374 6172 745f 6d65 6d20 3d20 6466 2e6d  start_mem = df.m
+00016400: 656d 6f72 795f 7573 6167 6528 292e 7375  emory_usage().su
+00016410: 6d28 2920 2f20 3130 3234 2a2a 320a 2020  m() / 1024**2.  
+00016420: 2020 6966 2074 7970 6528 6466 2920 3d3d    if type(df) ==
+00016430: 2064 6173 6b2e 6461 7461 6672 616d 652e   dask.dataframe.
+00016440: 636f 7265 2e44 6174 6146 7261 6d65 3a0a  core.DataFrame:.
+00016450: 2020 2020 2020 2020 7374 6172 745f 6d65          start_me
+00016460: 6d20 3d20 7374 6172 745f 6d65 6d2e 636f  m = start_mem.co
+00016470: 6d70 7574 6528 290a 2020 2020 7072 696e  mpute().    prin
+00016480: 7428 2720 2020 2043 6175 7469 6f6e 3a20  t('    Caution: 
+00016490: 5765 2077 696c 6c20 7472 7920 746f 2072  We will try to r
+000164a0: 6564 7563 6520 7468 6520 6d65 6d6f 7279  educe the memory
+000164b0: 2075 7361 6765 206f 6620 6461 7461 6672   usage of datafr
+000164c0: 616d 6520 6672 6f6d 207b 3a2e 3266 7d20  ame from {:.2f} 
+000164d0: 4d42 272e 666f 726d 6174 2873 7461 7274  MB'.format(start
+000164e0: 5f6d 656d 2929 0a20 2020 2063 6f6c 7320  _mem)).    cols 
+000164f0: 3d20 6466 2e63 6f6c 756d 6e73 0a20 2020  = df.columns.   
+00016500: 2069 6620 7479 7065 2864 6629 203d 3d20   if type(df) == 
+00016510: 6461 736b 2e64 6174 6166 7261 6d65 2e63  dask.dataframe.c
+00016520: 6f72 652e 4461 7461 4672 616d 653a 0a20  ore.DataFrame:. 
+00016530: 2020 2020 2020 2063 6f6c 7320 3d20 636f         cols = co
+00016540: 6c73 2e74 6f6c 6973 7428 290a 0a20 2020  ls.tolist()..   
+00016550: 2066 6f72 2063 6f6c 2069 6e20 636f 6c73   for col in cols
+00016560: 3a0a 2020 2020 2020 2020 636f 6c5f 7479  :.        col_ty
+00016570: 7065 203d 2064 665b 636f 6c5d 2e64 7479  pe = df[col].dty
+00016580: 7065 0a20 2020 2020 2020 2069 6620 636f  pe.        if co
+00016590: 6c5f 7479 7065 2021 3d20 6f62 6a65 6374  l_type != object
+000165a0: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+000165b0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+000165c0: 2020 2063 5f6d 696e 203d 2064 665b 636f     c_min = df[co
+000165d0: 6c5d 2e6d 696e 2829 0a20 2020 2020 2020  l].min().       
+000165e0: 2020 2020 2020 2020 2063 5f6d 6178 203d           c_max =
+000165f0: 2064 665b 636f 6c5d 2e6d 6178 2829 0a20   df[col].max(). 
+00016600: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00016610: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00016620: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00016630: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00016640: 6466 2920 3d3d 2064 6173 6b2e 6461 7461  df) == dask.data
+00016650: 6672 616d 652e 636f 7265 2e44 6174 6146  frame.core.DataF
+00016660: 7261 6d65 3a0a 2020 2020 2020 2020 2020  rame:.          
+00016670: 2020 2020 2020 635f 6d69 6e20 3d20 635f        c_min = c_
+00016680: 6d69 6e2e 636f 6d70 7574 6528 290a 2020  min.compute().  
+00016690: 2020 2020 2020 2020 2020 2020 2020 635f                c_
+000166a0: 6d61 7820 3d20 635f 6d61 782e 636f 6d70  max = c_max.comp
+000166b0: 7574 6528 290a 2020 2020 2020 2020 2020  ute().          
+000166c0: 2020 6966 2073 7472 2863 6f6c 5f74 7970    if str(col_typ
+000166d0: 6529 5b3a 335d 203d 3d20 2769 6e74 273a  e)[:3] == 'int':
+000166e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000166f0: 2069 6620 635f 6d69 6e20 3e20 6e70 2e69   if c_min > np.i
+00016700: 696e 666f 286e 702e 696e 7438 292e 6d69  info(np.int8).mi
+00016710: 6e20 616e 6420 635f 6d61 7820 3c20 6e70  n and c_max < np
+00016720: 2e69 696e 666f 286e 702e 696e 7438 292e  .iinfo(np.int8).
+00016730: 6d61 783a 0a20 2020 2020 2020 2020 2020  max:.           
+00016740: 2020 2020 2020 2020 2064 665b 636f 6c5d           df[col]
+00016750: 203d 2064 665b 636f 6c5d 2e61 7374 7970   = df[col].astyp
+00016760: 6528 6e70 2e69 6e74 3829 0a20 2020 2020  e(np.int8).     
+00016770: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00016780: 635f 6d69 6e20 3e20 6e70 2e69 696e 666f  c_min > np.iinfo
+00016790: 286e 702e 696e 7431 3629 2e6d 696e 2061  (np.int16).min a
+000167a0: 6e64 2063 5f6d 6178 203c 206e 702e 6969  nd c_max < np.ii
+000167b0: 6e66 6f28 6e70 2e69 6e74 3136 292e 6d61  nfo(np.int16).ma
+000167c0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
+000167d0: 2020 2020 2020 2064 665b 636f 6c5d 203d         df[col] =
+000167e0: 2064 665b 636f 6c5d 2e61 7374 7970 6528   df[col].astype(
+000167f0: 6e70 2e69 6e74 3136 290a 2020 2020 2020  np.int16).      
+00016800: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
+00016810: 5f6d 696e 203e 206e 702e 6969 6e66 6f28  _min > np.iinfo(
+00016820: 6e70 2e69 6e74 3332 292e 6d69 6e20 616e  np.int32).min an
+00016830: 6420 635f 6d61 7820 3c20 6e70 2e69 696e  d c_max < np.iin
+00016840: 666f 286e 702e 696e 7433 3229 2e6d 6178  fo(np.int32).max
+00016850: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016860: 2020 2020 2020 6466 5b63 6f6c 5d20 3d20        df[col] = 
+00016870: 6466 5b63 6f6c 5d2e 6173 7479 7065 286e  df[col].astype(n
+00016880: 702e 696e 7433 3229 0a20 2020 2020 2020  p.int32).       
+00016890: 2020 2020 2020 2020 2065 6c69 6620 635f           elif c_
+000168a0: 6d69 6e20 3e20 6e70 2e69 696e 666f 286e  min > np.iinfo(n
+000168b0: 702e 696e 7436 3429 2e6d 696e 2061 6e64  p.int64).min and
+000168c0: 2063 5f6d 6178 203c 206e 702e 6969 6e66   c_max < np.iinf
+000168d0: 6f28 6e70 2e69 6e74 3634 292e 6d61 783a  o(np.int64).max:
+000168e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000168f0: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
+00016900: 665b 636f 6c5d 2e61 7374 7970 6528 6e70  f[col].astype(np
+00016910: 2e69 6e74 3634 2920 200a 2020 2020 2020  .int64)  .      
+00016920: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016930: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00016940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016950: 2020 2020 2069 6620 635f 6d69 6e20 3e20       if c_min > 
+00016960: 6e70 2e66 696e 666f 286e 702e 666c 6f61  np.finfo(np.floa
+00016970: 7431 3629 2e6d 696e 2061 6e64 2063 5f6d  t16).min and c_m
+00016980: 6178 203c 206e 702e 6669 6e66 6f28 6e70  ax < np.finfo(np
+00016990: 2e66 6c6f 6174 3136 292e 6d61 783a 0a20  .float16).max:. 
+000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169b0: 2020 2020 2020 2064 665b 636f 6c5d 203d         df[col] =
+000169c0: 2064 665b 636f 6c5d 2e61 7374 7970 6528   df[col].astype(
+000169d0: 6e70 2e66 6c6f 6174 3136 290a 2020 2020  np.float16).    
+000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169f0: 656c 6966 2063 5f6d 696e 203e 206e 702e  elif c_min > np.
+00016a00: 6669 6e66 6f28 6e70 2e66 6c6f 6174 3332  finfo(np.float32
+00016a10: 292e 6d69 6e20 616e 6420 635f 6d61 7820  ).min and c_max 
+00016a20: 3c20 6e70 2e66 696e 666f 286e 702e 666c  < np.finfo(np.fl
+00016a30: 6f61 7433 3229 2e6d 6178 3a0a 2020 2020  oat32).max:.    
+00016a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a50: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
+00016a60: 5b63 6f6c 5d2e 6173 7479 7065 286e 702e  [col].astype(np.
+00016a70: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
+00016a80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00016a90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00016aa0: 2020 2020 2020 2020 2020 2064 665b 636f             df[co
+00016ab0: 6c5d 203d 2064 665b 636f 6c5d 2e61 7374  l] = df[col].ast
+00016ac0: 7970 6528 6e70 2e66 6c6f 6174 3634 290a  ype(np.float64).
+00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ae0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00016af0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00016b00: 696e 7565 0a20 2020 2020 2020 2065 6c73  inue.        els
+00016b10: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
+00016b20: 665b 636f 6c5d 203d 2064 665b 636f 6c5d  f[col] = df[col]
+00016b30: 2e61 7374 7970 6528 2763 6174 6567 6f72  .astype('categor
+00016b40: 7927 290a 0a20 2020 2023 2323 2323 2323  y')..    #######
+00016b50: 2020 5265 7375 6c74 7320 6166 7465 7220    Results after 
+00016b60: 6d65 6d6f 7279 2075 7361 6765 2066 756e  memory usage fun
+00016b70: 6374 696f 6e20 2323 2323 2323 2323 2323  ction ##########
+00016b80: 2323 2323 2323 2323 230a 2020 2020 656e  #########.    en
+00016b90: 645f 6d65 6d20 3d20 6466 2e6d 656d 6f72  d_mem = df.memor
+00016ba0: 795f 7573 6167 6528 292e 7375 6d28 2920  y_usage().sum() 
+00016bb0: 2f20 3130 3234 2a2a 320a 2020 2020 6966  / 1024**2.    if
+00016bc0: 2074 7970 6528 6466 2920 3d3d 2064 6173   type(df) == das
+00016bd0: 6b2e 6461 7461 6672 616d 652e 636f 7265  k.dataframe.core
+00016be0: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
+00016bf0: 2020 2020 656e 645f 6d65 6d20 3d20 656e      end_mem = en
+00016c00: 645f 6d65 6d2e 636f 6d70 7574 6528 290a  d_mem.compute().
+00016c10: 2020 2020 7072 696e 7428 2720 2020 2020      print('     
+00016c20: 2020 206d 656d 6f72 7920 7573 6167 6520     memory usage 
+00016c30: 6166 7465 7220 6f70 7469 6d69 7a61 7469  after optimizati
+00016c40: 6f6e 2069 733a 207b 3a2e 3266 7d20 4d42  on is: {:.2f} MB
+00016c50: 272e 666f 726d 6174 2865 6e64 5f6d 656d  '.format(end_mem
+00016c60: 2929 0a20 2020 2070 7269 6e74 2827 2020  )).    print('  
+00016c70: 2020 2020 2020 6465 6372 6561 7365 6420        decreased 
+00016c80: 6279 207b 3a2e 3166 7d25 272e 666f 726d  by {:.1f}%'.form
+00016c90: 6174 2831 3030 202a 2028 7374 6172 745f  at(100 * (start_
+00016ca0: 6d65 6d20 2d20 656e 645f 6d65 6d29 202f  mem - end_mem) /
+00016cb0: 2073 7461 7274 5f6d 656d 2929 0a20 2020   start_mem)).   
+00016cc0: 200a 2020 2020 7265 7475 726e 2064 660a   .    return df.
 00016cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016cf0: 0a64 6566 2046 455f 7374 6172 745f 656e  .def FE_start_en
-00016d00: 645f 6461 7465 5f74 696d 655f 6665 6174  d_date_time_feat
-00016d10: 7572 6573 2873 6d61 6c6c 6466 2c20 7374  ures(smalldf, st
-00016d20: 6172 7454 696d 652c 2065 6e64 5469 6d65  artTime, endTime
-00016d30: 2c20 7370 6c69 7474 6572 5f64 6174 655f  , splitter_date_
-00016d40: 7374 7269 6e67 3d22 2f22 2c73 706c 6974  string="/",split
-00016d50: 7465 725f 686f 7572 5f73 7472 696e 673d  ter_hour_string=
-00016d60: 223a 2229 3a0a 2020 2020 2222 220a 2020  ":"):.    """.  
-00016d70: 2020 4645 2073 7461 6e64 7320 666f 7220    FE stands for 
-00016d80: 4665 6174 7572 6520 456e 6769 6e65 6572  Feature Engineer
-00016d90: 696e 6720 2d20 6974 206d 6561 6e73 2074  ing - it means t
-00016da0: 6869 7320 6675 6e63 7469 6f6e 2070 6572  his function per
-00016db0: 666f 726d 7320 6665 6174 7572 6520 656e  forms feature en
-00016dc0: 6769 6e65 6572 696e 670a 2020 2020 2323  gineering.    ##
-00016dd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016de0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016df0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016d20: 2323 0a64 6566 2046 455f 7374 6172 745f  ##.def FE_start_
+00016d30: 656e 645f 6461 7465 5f74 696d 655f 6665  end_date_time_fe
+00016d40: 6174 7572 6573 2873 6d61 6c6c 6466 2c20  atures(smalldf, 
+00016d50: 7374 6172 7454 696d 652c 2065 6e64 5469  startTime, endTi
+00016d60: 6d65 2c20 7370 6c69 7474 6572 5f64 6174  me, splitter_dat
+00016d70: 655f 7374 7269 6e67 3d22 2f22 2c73 706c  e_string="/",spl
+00016d80: 6974 7465 725f 686f 7572 5f73 7472 696e  itter_hour_strin
+00016d90: 673d 223a 2229 3a0a 2020 2020 2222 220a  g=":"):.    """.
+00016da0: 2020 2020 4645 2073 7461 6e64 7320 666f      FE stands fo
+00016db0: 7220 4665 6174 7572 6520 456e 6769 6e65  r Feature Engine
+00016dc0: 6572 696e 6720 2d20 6974 206d 6561 6e73  ering - it means
+00016dd0: 2074 6869 7320 6675 6e63 7469 6f6e 2070   this function p
+00016de0: 6572 666f 726d 7320 6665 6174 7572 6520  erforms feature 
+00016df0: 656e 6769 6e65 6572 696e 670a 2020 2020  engineering.    
 00016e00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00016e10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00016e20: 2323 2323 0a20 2020 2054 6869 7320 6675  ####.    This fu
-00016e30: 6e63 7469 6f6e 2069 7320 7573 6564 2077  nction is used w
-00016e40: 6865 6e20 796f 7520 6861 7665 2073 7461  hen you have sta
-00016e50: 7274 2061 6e64 2065 6e64 2064 6174 6520  rt and end date 
-00016e60: 7469 6d65 2073 7461 6d70 7320 696e 2079  time stamps in y
-00016e70: 6f75 7220 6461 7461 7365 742e 0a20 2020  our dataset..   
-00016e80: 2020 2020 202d 2049 6620 7468 6572 6520       - If there 
-00016e90: 6973 206e 6f20 7374 6172 7420 616e 6420  is no start and 
-00016ea0: 656e 6420 7469 6d65 2066 6561 7475 7265  end time feature
-00016eb0: 732c 2064 6f6e 2774 2075 7365 2069 742e  s, don't use it.
-00016ec0: 2042 6f74 6820 6d75 7374 2062 6520 7072   Both must be pr
-00016ed0: 6573 656e 7421 0a20 2020 2020 2020 202d  esent!.        -
-00016ee0: 2074 6869 7320 6d6f 6475 6c65 2077 696c   this module wil
-00016ef0: 6c20 6372 6561 7465 2061 6464 6974 696f  l create additio
-00016f00: 6e61 6c20 6665 6174 7572 6573 2066 6f72  nal features for
-00016f10: 2073 7563 6820 6669 656c 6473 2e0a 2020   such fields..  
-00016f20: 2020 2020 2020 2d20 796f 7520 6d75 7374        - you must
-00016f30: 2070 726f 7669 6465 2061 2073 7461 7274   provide a start
-00016f40: 2064 6174 6520 7469 6d65 2073 7461 6d70   date time stamp
-00016f50: 2066 6965 6c64 2061 6e64 2061 6e20 656e   field and an en
-00016f60: 6420 6461 7465 2074 696d 6520 7374 616d  d date time stam
-00016f70: 7020 6669 656c 640a 2020 2020 4f74 6865  p field.    Othe
-00016f80: 7277 6973 652c 2079 6f75 2061 7265 2062  rwise, you are b
-00016f90: 6574 7465 7220 6f66 6620 7573 696e 6720  etter off using 
-00016fa0: 7468 6520 4645 5f63 7265 6174 655f 6461  the FE_create_da
-00016fb0: 7465 5f74 696d 655f 6665 6174 7572 6573  te_time_features
-00016fc0: 2829 206d 6f64 756c 6520 696e 2074 6869  () module in thi
-00016fd0: 7320 6c69 6272 6172 792e 0a0a 2020 2020  s library...    
-00016fe0: 496e 7075 7473 3a0a 2020 2020 736d 616c  Inputs:.    smal
-00016ff0: 6c64 663a 2044 6174 6166 7261 6d65 2063  ldf: Dataframe c
-00017000: 6f6e 7461 696e 696e 6720 796f 7572 2064  ontaining your d
-00017010: 6174 6520 7469 6d65 2066 6965 6c64 730a  ate time fields.
-00017020: 2020 2020 7374 6172 7454 696d 653a 2074      startTime: t
-00017030: 6869 7320 6973 2068 6f70 6566 756c 6c79  his is hopefully
-00017040: 2061 2073 7472 696e 6720 6669 656c 6420   a string field 
-00017050: 7768 6963 6820 636f 6e76 6572 7473 2074  which converts t
-00017060: 6f20 6120 6461 7465 2074 696d 6520 7374  o a date time st
-00017070: 616d 7020 6561 7369 6c79 2e20 4d61 6b65  amp easily. Make
-00017080: 2073 7572 6520 6974 2069 7320 6120 7374   sure it is a st
-00017090: 7269 6e67 2e0a 2020 2020 656e 6454 696d  ring..    endTim
-000170a0: 653a 2074 6869 7320 616c 736f 206d 7573  e: this also mus
-000170b0: 7420 6265 2061 2073 7472 696e 6720 6669  t be a string fi
-000170c0: 656c 6420 7768 6963 6820 636f 6e76 6572  eld which conver
-000170d0: 7473 2074 6f20 6120 6461 7465 2074 696d  ts to a date tim
-000170e0: 6520 7374 616d 7020 6561 7369 6c79 2e20  e stamp easily. 
-000170f0: 4d61 6b65 2073 7572 6520 6974 2069 7320  Make sure it is 
-00017100: 6120 7374 7269 6e67 2e0a 2020 2020 7370  a string..    sp
-00017110: 6c69 7474 6572 5f64 6174 655f 7374 7269  litter_date_stri
-00017120: 6e67 3a20 7573 7561 6c6c 7920 7468 6572  ng: usually ther
-00017130: 6520 6973 2061 2073 7472 696e 6720 7375  e is a string su
-00017140: 6368 2061 7320 272f 2720 6f72 2027 2e27  ch as '/' or '.'
-00017150: 2062 6574 7765 656e 2064 6179 2f6d 6f6e   between day/mon
-00017160: 7468 2f79 6561 7220 6574 632e 2044 6566  th/year etc. Def
-00017170: 6175 6c74 2069 7320 6173 7375 6d65 6420  ault is assumed 
-00017180: 2f20 6865 7265 2e0a 2020 2020 7370 6c69  / here..    spli
-00017190: 7474 6572 5f68 6f75 725f 7374 7269 6e67  tter_hour_string
-000171a0: 3a20 7573 7561 6c6c 7920 7468 6572 6520  : usually there 
-000171b0: 6973 2061 2073 7472 696e 6720 7375 6368  is a string such
-000171c0: 2061 7320 273a 2720 6f72 2027 2e27 2062   as ':' or '.' b
-000171d0: 6574 7765 656e 2068 6f75 723a 6d69 6e3a  etween hour:min:
-000171e0: 7365 6320 6574 632e 2044 6566 6175 6c74  sec etc. Default
-000171f0: 2069 7320 6173 7375 6d65 6420 3a20 6865   is assumed : he
-00017200: 7265 2e0a 0a20 2020 204f 7574 7075 7473  re...    Outputs
-00017210: 3a0a 2020 2020 5468 6520 6f72 6967 696e  :.    The origin
-00017220: 616c 2070 616e 6461 7320 6461 7461 6672  al pandas datafr
-00017230: 616d 6520 7769 7468 2061 6464 6974 696f  ame with additio
-00017240: 6e61 6c20 6669 656c 6473 2063 7265 6174  nal fields creat
-00017250: 6564 2062 7920 7370 6c69 7474 696e 6720  ed by splitting 
-00017260: 7468 6520 7374 6172 7420 616e 6420 656e  the start and en
-00017270: 6420 7469 6d65 2066 6965 6c64 730a 2020  d time fields.  
-00017280: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-00017290: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000172a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000172b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016e20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016e30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016e40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00016e50: 2323 2323 2323 0a20 2020 2054 6869 7320  ######.    This 
+00016e60: 6675 6e63 7469 6f6e 2069 7320 7573 6564  function is used
+00016e70: 2077 6865 6e20 796f 7520 6861 7665 2073   when you have s
+00016e80: 7461 7274 2061 6e64 2065 6e64 2064 6174  tart and end dat
+00016e90: 6520 7469 6d65 2073 7461 6d70 7320 696e  e time stamps in
+00016ea0: 2079 6f75 7220 6461 7461 7365 742e 0a20   your dataset.. 
+00016eb0: 2020 2020 2020 202d 2049 6620 7468 6572         - If ther
+00016ec0: 6520 6973 206e 6f20 7374 6172 7420 616e  e is no start an
+00016ed0: 6420 656e 6420 7469 6d65 2066 6561 7475  d end time featu
+00016ee0: 7265 732c 2064 6f6e 2774 2075 7365 2069  res, don't use i
+00016ef0: 742e 2042 6f74 6820 6d75 7374 2062 6520  t. Both must be 
+00016f00: 7072 6573 656e 7421 0a20 2020 2020 2020  present!.       
+00016f10: 202d 2074 6869 7320 6d6f 6475 6c65 2077   - this module w
+00016f20: 696c 6c20 6372 6561 7465 2061 6464 6974  ill create addit
+00016f30: 696f 6e61 6c20 6665 6174 7572 6573 2066  ional features f
+00016f40: 6f72 2073 7563 6820 6669 656c 6473 2e0a  or such fields..
+00016f50: 2020 2020 2020 2020 2d20 796f 7520 6d75          - you mu
+00016f60: 7374 2070 726f 7669 6465 2061 2073 7461  st provide a sta
+00016f70: 7274 2064 6174 6520 7469 6d65 2073 7461  rt date time sta
+00016f80: 6d70 2066 6965 6c64 2061 6e64 2061 6e20  mp field and an 
+00016f90: 656e 6420 6461 7465 2074 696d 6520 7374  end date time st
+00016fa0: 616d 7020 6669 656c 640a 2020 2020 4f74  amp field.    Ot
+00016fb0: 6865 7277 6973 652c 2079 6f75 2061 7265  herwise, you are
+00016fc0: 2062 6574 7465 7220 6f66 6620 7573 696e   better off usin
+00016fd0: 6720 7468 6520 4645 5f63 7265 6174 655f  g the FE_create_
+00016fe0: 6461 7465 5f74 696d 655f 6665 6174 7572  date_time_featur
+00016ff0: 6573 2829 206d 6f64 756c 6520 696e 2074  es() module in t
+00017000: 6869 7320 6c69 6272 6172 792e 0a0a 2020  his library...  
+00017010: 2020 496e 7075 7473 3a0a 2020 2020 736d    Inputs:.    sm
+00017020: 616c 6c64 663a 2044 6174 6166 7261 6d65  alldf: Dataframe
+00017030: 2063 6f6e 7461 696e 696e 6720 796f 7572   containing your
+00017040: 2064 6174 6520 7469 6d65 2066 6965 6c64   date time field
+00017050: 730a 2020 2020 7374 6172 7454 696d 653a  s.    startTime:
+00017060: 2074 6869 7320 6973 2068 6f70 6566 756c   this is hopeful
+00017070: 6c79 2061 2073 7472 696e 6720 6669 656c  ly a string fiel
+00017080: 6420 7768 6963 6820 636f 6e76 6572 7473  d which converts
+00017090: 2074 6f20 6120 6461 7465 2074 696d 6520   to a date time 
+000170a0: 7374 616d 7020 6561 7369 6c79 2e20 4d61  stamp easily. Ma
+000170b0: 6b65 2073 7572 6520 6974 2069 7320 6120  ke sure it is a 
+000170c0: 7374 7269 6e67 2e0a 2020 2020 656e 6454  string..    endT
+000170d0: 696d 653a 2074 6869 7320 616c 736f 206d  ime: this also m
+000170e0: 7573 7420 6265 2061 2073 7472 696e 6720  ust be a string 
+000170f0: 6669 656c 6420 7768 6963 6820 636f 6e76  field which conv
+00017100: 6572 7473 2074 6f20 6120 6461 7465 2074  erts to a date t
+00017110: 696d 6520 7374 616d 7020 6561 7369 6c79  ime stamp easily
+00017120: 2e20 4d61 6b65 2073 7572 6520 6974 2069  . Make sure it i
+00017130: 7320 6120 7374 7269 6e67 2e0a 2020 2020  s a string..    
+00017140: 7370 6c69 7474 6572 5f64 6174 655f 7374  splitter_date_st
+00017150: 7269 6e67 3a20 7573 7561 6c6c 7920 7468  ring: usually th
+00017160: 6572 6520 6973 2061 2073 7472 696e 6720  ere is a string 
+00017170: 7375 6368 2061 7320 272f 2720 6f72 2027  such as '/' or '
+00017180: 2e27 2062 6574 7765 656e 2064 6179 2f6d  .' between day/m
+00017190: 6f6e 7468 2f79 6561 7220 6574 632e 2044  onth/year etc. D
+000171a0: 6566 6175 6c74 2069 7320 6173 7375 6d65  efault is assume
+000171b0: 6420 2f20 6865 7265 2e0a 2020 2020 7370  d / here..    sp
+000171c0: 6c69 7474 6572 5f68 6f75 725f 7374 7269  litter_hour_stri
+000171d0: 6e67 3a20 7573 7561 6c6c 7920 7468 6572  ng: usually ther
+000171e0: 6520 6973 2061 2073 7472 696e 6720 7375  e is a string su
+000171f0: 6368 2061 7320 273a 2720 6f72 2027 2e27  ch as ':' or '.'
+00017200: 2062 6574 7765 656e 2068 6f75 723a 6d69   between hour:mi
+00017210: 6e3a 7365 6320 6574 632e 2044 6566 6175  n:sec etc. Defau
+00017220: 6c74 2069 7320 6173 7375 6d65 6420 3a20  lt is assumed : 
+00017230: 6865 7265 2e0a 0a20 2020 204f 7574 7075  here...    Outpu
+00017240: 7473 3a0a 2020 2020 5468 6520 6f72 6967  ts:.    The orig
+00017250: 696e 616c 2070 616e 6461 7320 6461 7461  inal pandas data
+00017260: 6672 616d 6520 7769 7468 2061 6464 6974  frame with addit
+00017270: 696f 6e61 6c20 6669 656c 6473 2063 7265  ional fields cre
+00017280: 6174 6564 2062 7920 7370 6c69 7474 696e  ated by splittin
+00017290: 6720 7468 6520 7374 6172 7420 616e 6420  g the start and 
+000172a0: 656e 6420 7469 6d65 2066 6965 6c64 730a  end time fields.
+000172b0: 2020 2020 2323 2323 2323 2323 2323 2323      ############
 000172c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000172d0: 2323 2323 2323 2323 0a20 2020 2022 2222  ########.    """
-000172e0: 0a20 2020 2073 6d61 6c6c 6466 203d 2073  .    smalldf = s
-000172f0: 6d61 6c6c 6466 2e63 6f70 7928 290a 2020  malldf.copy().  
-00017300: 2020 6164 645f 636f 6c73 203d 205b 5d0a    add_cols = [].
-00017310: 2020 2020 6461 7465 5f74 696d 655f 7661      date_time_va
-00017320: 7269 6162 6c65 5f66 6c61 6720 3d20 4661  riable_flag = Fa
-00017330: 6c73 650a 2020 2020 6966 2073 6d61 6c6c  lse.    if small
-00017340: 6466 5b73 7461 7274 5469 6d65 5d2e 6474  df[startTime].dt
-00017350: 7970 6520 696e 205b 2764 6174 6574 696d  ype in ['datetim
-00017360: 6536 345b 6e73 5d27 2c27 6461 7465 7469  e64[ns]','dateti
-00017370: 6d65 3136 5b6e 735d 272c 2764 6174 6574  me16[ns]','datet
-00017380: 696d 6533 325b 6e73 5d27 5d3a 0a20 2020  ime32[ns]']:.   
-00017390: 2020 2020 2070 7269 6e74 2827 2573 2076       print('%s v
-000173a0: 6172 6961 626c 6520 6973 2061 2064 6174  ariable is a dat
-000173b0: 652d 7469 6d65 2076 6172 6961 626c 6527  e-time variable'
-000173c0: 2025 7374 6172 7454 696d 6529 0a20 2020   %startTime).   
-000173d0: 2020 2020 2064 6174 655f 7469 6d65 5f76       date_time_v
-000173e0: 6172 6961 626c 655f 666c 6167 203d 2054  ariable_flag = T
-000173f0: 7275 650a 2020 2020 6966 2064 6174 655f  rue.    if date_
-00017400: 7469 6d65 5f76 6172 6961 626c 655f 666c  time_variable_fl
-00017410: 6167 3a0a 2020 2020 2020 2020 7669 6577  ag:.        view
-00017420: 5f64 6179 7320 3d20 2770 726f 6365 7373  _days = 'process
-00017430: 696e 6727 2b73 7461 7274 5469 6d65 2b27  ing'+startTime+'
-00017440: 5f65 6c61 7073 6564 5f64 6179 7327 0a20  _elapsed_days'. 
-00017450: 2020 2020 2020 2073 6d61 6c6c 6466 5b76         smalldf[v
-00017460: 6965 775f 6461 7973 5d20 3d20 2873 6d61  iew_days] = (sma
-00017470: 6c6c 6466 5b65 6e64 5469 6d65 5d20 2d20  lldf[endTime] - 
-00017480: 736d 616c 6c64 665b 7374 6172 7454 696d  smalldf[startTim
-00017490: 655d 292e 6173 7479 7065 2827 7469 6d65  e]).astype('time
-000174a0: 6465 6c74 6136 345b 735d 2729 2f28 3630  delta64[s]')/(60
-000174b0: 2a36 302a 3234 290a 2020 2020 2020 2020  *60*24).        
-000174c0: 736d 616c 6c64 665b 7669 6577 5f64 6179  smalldf[view_day
-000174d0: 735d 203d 2073 6d61 6c6c 6466 5b76 6965  s] = smalldf[vie
-000174e0: 775f 6461 7973 5d2e 6173 7479 7065 2869  w_days].astype(i
-000174f0: 6e74 290a 2020 2020 2020 2020 6164 645f  nt).        add_
-00017500: 636f 6c73 2e61 7070 656e 6428 7669 6577  cols.append(view
-00017510: 5f64 6179 7329 0a20 2020 2020 2020 2076  _days).        v
-00017520: 6965 775f 7469 6d65 203d 2027 7072 6f63  iew_time = 'proc
-00017530: 6573 7369 6e67 272b 7374 6172 7454 696d  essing'+startTim
-00017540: 652b 275f 656c 6170 7365 645f 7469 6d65  e+'_elapsed_time
-00017550: 270a 2020 2020 2020 2020 736d 616c 6c64  '.        smalld
-00017560: 665b 7669 6577 5f74 696d 655d 203d 2028  f[view_time] = (
-00017570: 736d 616c 6c64 665b 656e 6454 696d 655d  smalldf[endTime]
-00017580: 202d 2073 6d61 6c6c 6466 5b73 7461 7274   - smalldf[start
-00017590: 5469 6d65 5d29 2e61 7374 7970 6528 2774  Time]).astype('t
-000175a0: 696d 6564 656c 7461 3634 5b73 5d27 292e  imedelta64[s]').
-000175b0: 7661 6c75 6573 0a20 2020 2020 2020 2061  values.        a
-000175c0: 6464 5f63 6f6c 732e 6170 7065 6e64 2876  dd_cols.append(v
-000175d0: 6965 775f 7469 6d65 290a 2020 2020 656c  iew_time).    el
-000175e0: 7365 3a0a 2020 2020 2020 2020 7374 6172  se:.        star
-000175f0: 745f 6461 7465 203d 2027 7072 6f63 6573  t_date = 'proces
-00017600: 7369 6e67 272b 7374 6172 7454 696d 652b  sing'+startTime+
-00017610: 275f 7374 6172 745f 6461 7465 270a 2020  '_start_date'.  
-00017620: 2020 2020 2020 736d 616c 6c64 665b 7374        smalldf[st
-00017630: 6172 745f 6461 7465 5d20 3d20 736d 616c  art_date] = smal
-00017640: 6c64 665b 7374 6172 7454 696d 655d 2e6d  ldf[startTime].m
-00017650: 6170 286c 616d 6264 6120 783a 2078 2e73  ap(lambda x: x.s
-00017660: 706c 6974 2822 2022 295b 305d 290a 2020  plit(" ")[0]).  
-00017670: 2020 2020 2020 6164 645f 636f 6c73 2e61        add_cols.a
-00017680: 7070 656e 6428 7374 6172 745f 6461 7465  ppend(start_date
-00017690: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-000176a0: 2020 2020 2020 2020 2020 2073 7461 7274             start
-000176b0: 5f74 696d 6520 3d20 2770 726f 6365 7373  _time = 'process
-000176c0: 696e 6727 2b73 7461 7274 5469 6d65 2b27  ing'+startTime+'
-000176d0: 5f73 7461 7274 5f74 696d 6527 0a20 2020  _start_time'.   
-000176e0: 2020 2020 2020 2020 2073 6d61 6c6c 6466           smalldf
-000176f0: 5b73 7461 7274 5f74 696d 655d 203d 2073  [start_time] = s
-00017700: 6d61 6c6c 6466 5b73 7461 7274 5469 6d65  malldf[startTime
-00017710: 5d2e 6d61 7028 6c61 6d62 6461 2078 3a20  ].map(lambda x: 
-00017720: 782e 7370 6c69 7428 2220 2229 5b31 5d29  x.split(" ")[1])
-00017730: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-00017740: 5f63 6f6c 732e 6170 7065 6e64 2873 7461  _cols.append(sta
-00017750: 7274 5f74 696d 6529 0a20 2020 2020 2020  rt_time).       
-00017760: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00017770: 2020 2020 2023 2323 2074 6865 7265 2069       ### there i
-00017780: 7320 6e6f 2068 6f75 722d 6d69 6e75 7465  s no hour-minute
-00017790: 7320 7061 7274 206f 6620 7468 6973 2064  s part of this d
-000177a0: 6174 6520 7469 6d65 2073 7461 6d70 2066  ate time stamp f
-000177b0: 6965 6c64 2e20 596f 7520 6361 6e20 6a75  ield. You can ju
-000177c0: 7374 2073 6b69 7020 6974 2069 6620 6974  st skip it if it
-000177d0: 2069 7320 6e6f 7420 7468 6572 650a 2020   is not there.  
-000177e0: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-000177f0: 2020 2020 2020 2065 6e64 5f64 6174 6520         end_date 
-00017800: 3d20 2770 726f 6365 7373 696e 6727 2b65  = 'processing'+e
-00017810: 6e64 5469 6d65 2b27 5f65 6e64 5f64 6174  ndTime+'_end_dat
-00017820: 6527 0a20 2020 2020 2020 2073 6d61 6c6c  e'.        small
-00017830: 6466 5b65 6e64 5f64 6174 655d 203d 2073  df[end_date] = s
-00017840: 6d61 6c6c 6466 5b65 6e64 5469 6d65 5d2e  malldf[endTime].
-00017850: 6d61 7028 6c61 6d62 6461 2078 3a20 782e  map(lambda x: x.
-00017860: 7370 6c69 7428 2220 2229 5b30 5d29 0a20  split(" ")[0]). 
-00017870: 2020 2020 2020 2061 6464 5f63 6f6c 732e         add_cols.
-00017880: 6170 7065 6e64 2865 6e64 5f64 6174 6529  append(end_date)
-00017890: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000178a0: 2020 2020 2020 2020 2020 656e 645f 7469            end_ti
-000178b0: 6d65 203d 2027 7072 6f63 6573 7369 6e67  me = 'processing
-000178c0: 272b 656e 6454 696d 652b 275f 656e 645f  '+endTime+'_end_
-000178d0: 7469 6d65 270a 2020 2020 2020 2020 2020  time'.          
-000178e0: 2020 736d 616c 6c64 665b 656e 645f 7469    smalldf[end_ti
-000178f0: 6d65 5d20 3d20 736d 616c 6c64 665b 656e  me] = smalldf[en
-00017900: 6454 696d 655d 2e6d 6170 286c 616d 6264  dTime].map(lambd
-00017910: 6120 783a 2078 2e73 706c 6974 2822 2022  a x: x.split(" "
-00017920: 295b 315d 290a 2020 2020 2020 2020 2020  )[1]).          
-00017930: 2020 6164 645f 636f 6c73 2e61 7070 656e    add_cols.appen
-00017940: 6428 656e 645f 7469 6d65 290a 2020 2020  d(end_time).    
-00017950: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-00017960: 2020 2020 2020 2020 2323 2320 7468 6572          ### ther
-00017970: 6520 6973 206e 6f20 686f 7572 2d6d 696e  e is no hour-min
-00017980: 7574 6573 2070 6172 7420 6f66 2074 6869  utes part of thi
-00017990: 7320 6461 7465 2074 696d 6520 7374 616d  s date time stam
-000179a0: 7020 6669 656c 642e 2059 6f75 2063 616e  p field. You can
-000179b0: 206a 7573 7420 736b 6970 2069 7420 6966   just skip it if
-000179c0: 2069 7420 6973 206e 6f74 2074 6865 7265   it is not there
-000179d0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-000179e0: 730a 2020 2020 2020 2020 7669 6577 5f64  s.        view_d
-000179f0: 6179 7320 3d20 2770 726f 6365 7373 696e  ays = 'processin
-00017a00: 6727 2b73 7461 7274 5469 6d65 2b27 5f65  g'+startTime+'_e
-00017a10: 6c61 7073 6564 5f64 6179 7327 0a20 2020  lapsed_days'.   
-00017a20: 2020 2020 2073 6d61 6c6c 6466 5b76 6965       smalldf[vie
-00017a30: 775f 6461 7973 5d20 3d20 2870 642e 746f  w_days] = (pd.to
-00017a40: 5f64 6174 6574 696d 6528 736d 616c 6c64  _datetime(smalld
-00017a50: 665b 656e 645f 6461 7465 5d29 202d 2070  f[end_date]) - p
-00017a60: 642e 746f 5f64 6174 6574 696d 6528 736d  d.to_datetime(sm
-00017a70: 616c 6c64 665b 7374 6172 745f 6461 7465  alldf[start_date
-00017a80: 5d29 292e 7661 6c75 6573 2e61 7374 7970  ])).values.astyp
-00017a90: 6528 696e 7429 0a20 2020 2020 2020 2061  e(int).        a
-00017aa0: 6464 5f63 6f6c 732e 6170 7065 6e64 2876  dd_cols.append(v
-00017ab0: 6965 775f 6461 7973 290a 2020 2020 2020  iew_days).      
-00017ac0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00017ad0: 2020 2076 6965 775f 7469 6d65 203d 2027     view_time = '
-00017ae0: 7072 6f63 6573 7369 6e67 272b 7374 6172  processing'+star
-00017af0: 7454 696d 652b 275f 656c 6170 7365 645f  tTime+'_elapsed_
-00017b00: 7469 6d65 270a 2020 2020 2020 2020 2020  time'.          
-00017b10: 2020 736d 616c 6c64 665b 7669 6577 5f74    smalldf[view_t
-00017b20: 696d 655d 203d 2028 7064 2e74 6f5f 6461  ime] = (pd.to_da
-00017b30: 7465 7469 6d65 2873 6d61 6c6c 6466 5b65  tetime(smalldf[e
-00017b40: 6e64 5f74 696d 655d 2920 2d20 7064 2e74  nd_time]) - pd.t
-00017b50: 6f5f 6461 7465 7469 6d65 2873 6d61 6c6c  o_datetime(small
-00017b60: 6466 5b73 7461 7274 5f74 696d 655d 2929  df[start_time]))
-00017b70: 2e61 7374 7970 6528 2774 696d 6564 656c  .astype('timedel
-00017b80: 7461 3634 5b73 5d27 292e 7661 6c75 6573  ta64[s]').values
-00017b90: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-00017ba0: 5f63 6f6c 732e 6170 7065 6e64 2876 6965  _cols.append(vie
-00017bb0: 775f 7469 6d65 290a 2020 2020 2020 2020  w_time).        
-00017bc0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00017bd0: 2020 2020 2323 2320 496e 2073 6f6d 6520      ### In some 
-00017be0: 6461 7465 2074 696d 6520 6669 656c 6473  date time fields
-00017bf0: 2074 6869 7320 6769 7665 7320 616e 2065   this gives an e
-00017c00: 7272 6f72 2073 6f20 736b 6970 2069 7420  rror so skip it 
-00017c10: 696e 2074 6861 7420 6361 7365 0a20 2020  in that case.   
-00017c20: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-00017c30: 2020 2020 2020 2323 2323 2054 6865 2072        #### The r
-00017c40: 6561 736f 6e20 7765 2063 686f 7365 2065  eason we chose e
-00017c50: 6e64 5469 6d65 2068 6572 6520 6973 2074  ndTime here is t
-00017c60: 6861 7420 7374 6172 7454 696d 6520 6973  hat startTime is
-00017c70: 2075 7375 616c 6c79 2074 616b 656e 2063   usually taken c
-00017c80: 6172 6520 6f66 2062 7920 616e 6f74 6865  are of by anothe
-00017c90: 7220 6c69 6272 6172 792e 2053 6f20 6265  r library. So be
-00017ca0: 7474 6572 2074 6f20 646f 2074 6869 7320  tter to do this 
-00017cb0: 616c 6f6e 652e 0a20 2020 2020 2020 2079  alone..        y
-00017cc0: 6561 7220 3d20 2770 726f 6365 7373 696e  ear = 'processin
-00017cd0: 6727 2b65 6e64 5469 6d65 2b27 5f65 6e64  g'+endTime+'_end
-00017ce0: 5f79 6561 7227 0a20 2020 2020 2020 2073  _year'.        s
-00017cf0: 6d61 6c6c 6466 5b79 6561 725d 203d 2073  malldf[year] = s
-00017d00: 6d61 6c6c 6466 5b65 6e64 5f64 6174 655d  malldf[end_date]
-00017d10: 2e6d 6170 286c 616d 6264 6120 783a 2073  .map(lambda x: s
-00017d20: 7472 2878 292e 7370 6c69 7428 7370 6c69  tr(x).split(spli
-00017d30: 7474 6572 5f64 6174 655f 7374 7269 6e67  tter_date_string
-00017d40: 295b 305d 292e 7661 6c75 6573 0a20 2020  )[0]).values.   
-00017d50: 2020 2020 2061 6464 5f63 6f6c 732e 6170       add_cols.ap
-00017d60: 7065 6e64 2879 6561 7229 0a20 2020 2020  pend(year).     
-00017d70: 2020 2023 2323 2320 5468 6520 7265 6173     #### The reas
-00017d80: 6f6e 2077 6520 6368 6f73 6520 656e 6454  on we chose endT
-00017d90: 696d 6520 6865 7265 2069 7320 7468 6174  ime here is that
-00017da0: 2073 7461 7274 5469 6d65 2069 7320 7573   startTime is us
-00017db0: 7561 6c6c 7920 7461 6b65 6e20 6361 7265  ually taken care
-00017dc0: 206f 6620 6279 2061 6e6f 7468 6572 206c   of by another l
-00017dd0: 6962 7261 7279 2e20 536f 2062 6574 7465  ibrary. So bette
-00017de0: 7220 746f 2064 6f20 7468 6973 2061 6c6f  r to do this alo
-00017df0: 6e65 2e0a 2020 2020 2020 2020 6d6f 6e74  ne..        mont
-00017e00: 6820 3d20 2770 726f 6365 7373 696e 6727  h = 'processing'
-00017e10: 2b65 6e64 5469 6d65 2b27 5f65 6e64 5f6d  +endTime+'_end_m
-00017e20: 6f6e 7468 270a 2020 2020 2020 2020 736d  onth'.        sm
-00017e30: 616c 6c64 665b 6d6f 6e74 685d 203d 2073  alldf[month] = s
-00017e40: 6d61 6c6c 6466 5b65 6e64 5f64 6174 655d  malldf[end_date]
-00017e50: 2e6d 6170 286c 616d 6264 6120 783a 2073  .map(lambda x: s
-00017e60: 7472 2878 292e 7370 6c69 7428 7370 6c69  tr(x).split(spli
-00017e70: 7474 6572 5f64 6174 655f 7374 7269 6e67  tter_date_string
-00017e80: 295b 315d 292e 7661 6c75 6573 0a20 2020  )[1]).values.   
-00017e90: 2020 2020 2061 6464 5f63 6f6c 732e 6170       add_cols.ap
-00017ea0: 7065 6e64 286d 6f6e 7468 290a 2020 2020  pend(month).    
-00017eb0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00017ec0: 2020 2020 2023 2323 2320 5468 6520 7265       #### The re
-00017ed0: 6173 6f6e 2077 6520 6368 6f73 6520 656e  ason we chose en
-00017ee0: 6454 696d 6520 6865 7265 2069 7320 7468  dTime here is th
-00017ef0: 6174 2073 7461 7274 5469 6d65 2069 7320  at startTime is 
-00017f00: 7573 7561 6c6c 7920 7461 6b65 6e20 6361  usually taken ca
-00017f10: 7265 206f 6620 6279 2061 6e6f 7468 6572  re of by another
-00017f20: 206c 6962 7261 7279 2e20 536f 2062 6574   library. So bet
-00017f30: 7465 7220 746f 2064 6f20 7468 6973 2061  ter to do this a
-00017f40: 6c6f 6e65 2e0a 2020 2020 2020 2020 2020  lone..          
-00017f50: 2020 6461 796e 756d 203d 2027 7072 6f63    daynum = 'proc
-00017f60: 6573 7369 6e67 272b 656e 6454 696d 652b  essing'+endTime+
-00017f70: 275f 656e 645f 6461 795f 6e75 6d62 6572  '_end_day_number
-00017f80: 270a 2020 2020 2020 2020 2020 2020 736d  '.            sm
-00017f90: 616c 6c64 665b 6461 796e 756d 5d20 3d20  alldf[daynum] = 
-00017fa0: 736d 616c 6c64 665b 656e 645f 6461 7465  smalldf[end_date
-00017fb0: 5d2e 6d61 7028 6c61 6d62 6461 2078 3a20  ].map(lambda x: 
-00017fc0: 7374 7228 7829 2e73 706c 6974 2873 706c  str(x).split(spl
-00017fd0: 6974 7465 725f 6461 7465 5f73 7472 696e  itter_date_strin
-00017fe0: 6729 5b32 5d29 2e76 616c 7565 730a 2020  g)[2]).values.  
-00017ff0: 2020 2020 2020 2020 2020 6164 645f 636f            add_co
-00018000: 6c73 2e61 7070 656e 6428 6461 796e 756d  ls.append(daynum
-00018010: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00018020: 3a0a 2020 2020 2020 2020 2020 2020 2323  :.            ##
-00018030: 2320 496e 2073 6f6d 6520 6461 7465 2074  # In some date t
-00018040: 696d 6520 6669 656c 6473 2074 6865 2064  ime fields the d
-00018050: 6179 206e 756d 6265 7220 6973 206e 6f74  ay number is not
-00018060: 2074 6865 7265 2e20 4966 206e 6f74 2c20   there. If not, 
-00018070: 6a75 7374 2073 6b69 7020 6974 2023 2323  just skip it ###
-00018080: 230a 2020 2020 2020 2020 2020 2020 7061  #.            pa
-00018090: 7373 0a20 2020 2020 2020 2023 2323 2320  ss.        #### 
-000180a0: 496e 2073 6f6d 6520 6461 7465 2074 696d  In some date tim
-000180b0: 6520 6669 656c 6473 2c20 7468 6520 686f  e fields, the ho
-000180c0: 7572 2061 6e64 206d 696e 7574 6520 6973  ur and minute is
-000180d0: 206e 6f74 2074 6865 7265 2c20 736f 2073   not there, so s
-000180e0: 6b69 7020 6974 2069 6e20 7468 6174 2063  kip it in that c
-000180f0: 6173 6520 6966 2069 7420 6572 726f 7273  ase if it errors
-00018100: 210a 2020 2020 2020 2020 7472 793a 0a20  !.        try:. 
-00018110: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00018120: 5f68 6f75 7220 3d20 2770 726f 6365 7373  _hour = 'process
-00018130: 696e 6727 2b73 7461 7274 5469 6d65 2b27  ing'+startTime+'
-00018140: 5f73 7461 7274 5f68 6f75 7227 0a20 2020  _start_hour'.   
-00018150: 2020 2020 2020 2020 2073 6d61 6c6c 6466           smalldf
-00018160: 5b73 7461 7274 5f68 6f75 725d 203d 2073  [start_hour] = s
-00018170: 6d61 6c6c 6466 5b73 7461 7274 5f74 696d  malldf[start_tim
-00018180: 655d 2e6d 6170 286c 616d 6264 6120 783a  e].map(lambda x:
-00018190: 2073 7472 2878 292e 7370 6c69 7428 7370   str(x).split(sp
-000181a0: 6c69 7474 6572 5f68 6f75 725f 7374 7269  litter_hour_stri
-000181b0: 6e67 295b 305d 292e 7661 6c75 6573 0a20  ng)[0]).values. 
-000181c0: 2020 2020 2020 2020 2020 2061 6464 5f63             add_c
-000181d0: 6f6c 732e 6170 7065 6e64 2873 7461 7274  ols.append(start
-000181e0: 5f68 6f75 7229 0a20 2020 2020 2020 2020  _hour).         
-000181f0: 2020 2073 7461 7274 5f6d 696e 203d 2027     start_min = '
-00018200: 7072 6f63 6573 7369 6e67 272b 7374 6172  processing'+star
-00018210: 7454 696d 652b 275f 7374 6172 745f 686f  tTime+'_start_ho
-00018220: 7572 270a 2020 2020 2020 2020 2020 2020  ur'.            
-00018230: 736d 616c 6c64 665b 7374 6172 745f 6d69  smalldf[start_mi
-00018240: 6e5d 203d 2073 6d61 6c6c 6466 5b73 7461  n] = smalldf[sta
-00018250: 7274 5f74 696d 655d 2e6d 6170 286c 616d  rt_time].map(lam
-00018260: 6264 6120 783a 2073 7472 2878 292e 7370  bda x: str(x).sp
-00018270: 6c69 7428 7370 6c69 7474 6572 5f68 6f75  lit(splitter_hou
-00018280: 725f 7374 7269 6e67 295b 315d 292e 7661  r_string)[1]).va
-00018290: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
-000182a0: 2061 6464 5f63 6f6c 732e 6170 7065 6e64   add_cols.append
-000182b0: 2873 7461 7274 5f6d 696e 290a 2020 2020  (start_min).    
-000182c0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-000182d0: 2020 2020 2020 2020 2323 2320 4966 2069          ### If i
-000182e0: 7420 6572 726f 7273 2c20 736b 6970 2069  t errors, skip i
-000182f0: 740a 2020 2020 2020 2020 2020 2020 7061  t.            pa
-00018300: 7373 0a20 2020 2020 2020 2023 2323 2320  ss.        #### 
-00018310: 4368 6563 6b20 6966 2074 6865 7265 2069  Check if there i
-00018320: 7320 6120 7765 656b 6461 7920 616e 6420  s a weekday and 
-00018330: 7765 656b 656e 6473 2069 6e20 6461 7465  weekends in date
-00018340: 2074 696d 6520 636f 6c75 6d6e 7320 7573   time columns us
-00018350: 696e 6720 656e 6454 696d 6520 6f6e 6c79  ing endTime only
-00018360: 0a20 2020 2020 2020 2077 6565 6b64 6179  .        weekday
-00018370: 5f6e 756d 203d 2027 7072 6f63 6573 7369  _num = 'processi
-00018380: 6e67 272b 656e 6454 696d 652b 275f 656e  ng'+endTime+'_en
-00018390: 645f 7765 656b 6461 795f 6e75 6d62 6572  d_weekday_number
-000183a0: 270a 2020 2020 2020 2020 736d 616c 6c64  '.        smalld
-000183b0: 665b 7765 656b 6461 795f 6e75 6d5d 203d  f[weekday_num] =
-000183c0: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
-000183d0: 736d 616c 6c64 665b 656e 645f 6461 7465  smalldf[end_date
-000183e0: 5d29 2e64 742e 7765 656b 6461 792e 7661  ]).dt.weekday.va
-000183f0: 6c75 6573 0a20 2020 2020 2020 2061 6464  lues.        add
-00018400: 5f63 6f6c 732e 6170 7065 6e64 2877 6565  _cols.append(wee
-00018410: 6b64 6179 5f6e 756d 290a 2020 2020 2020  kday_num).      
-00018420: 2020 7765 656b 656e 6420 3d20 2770 726f    weekend = 'pro
-00018430: 6365 7373 696e 6727 2b65 6e64 5469 6d65  cessing'+endTime
-00018440: 2b27 5f65 6e64 5f77 6565 6b65 6e64 5f66  +'_end_weekend_f
-00018450: 6c61 6727 0a20 2020 2020 2020 2073 6d61  lag'.        sma
-00018460: 6c6c 6466 5b77 6565 6b65 6e64 5d20 3d20  lldf[weekend] = 
-00018470: 736d 616c 6c64 665b 7765 656b 6461 795f  smalldf[weekday_
-00018480: 6e75 6d5d 2e6d 6170 286c 616d 6264 6120  num].map(lambda 
-00018490: 783a 2031 2069 6620 7820 696e 5b35 2c36  x: 1 if x in[5,6
-000184a0: 5d20 656c 7365 2030 290a 2020 2020 2020  ] else 0).      
-000184b0: 2020 6164 645f 636f 6c73 2e61 7070 656e    add_cols.appen
-000184c0: 6428 7765 656b 656e 6429 0a20 2020 2023  d(weekend).    #
-000184d0: 2323 2320 4966 2065 7665 7279 7468 696e  ### If everythin
-000184e0: 6720 776f 726b 7320 7765 6c6c 2c20 7468  g works well, th
-000184f0: 6572 6520 7368 6f75 6c64 2062 6520 3133  ere should be 13
-00018500: 206e 6577 2063 6f6c 756d 6e73 2061 6464   new columns add
-00018510: 6564 2062 7920 6d6f 6475 6c65 2e20 416c  ed by module. Al
-00018520: 6c20 7468 6520 6265 7374 210a 2020 2020  l the best!.    
-00018530: 7072 696e 7428 2725 6420 636f 6c75 6d6e  print('%d column
-00018540: 7320 6164 6465 6420 7573 696e 6720 7374  s added using st
-00018550: 6172 7420 6461 7465 3d25 7320 616e 6420  art date=%s and 
-00018560: 656e 6420 6461 7465 3d25 7320 7072 6f63  end date=%s proc
-00018570: 6573 7369 6e67 2e2e 2e27 2025 286c 656e  essing...' %(len
-00018580: 2861 6464 5f63 6f6c 7329 2c73 7461 7274  (add_cols),start
-00018590: 5469 6d65 2c65 6e64 5469 6d65 2929 0a20  Time,endTime)). 
-000185a0: 2020 2072 6574 7572 6e20 736d 616c 6c64     return smalld
-000185b0: 660a 2323 2323 2323 2323 2323 2323 2323  f.##############
-000185c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000185d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000185e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000185f0: 2323 2323 2323 2323 2323 2323 230a 6465  #############.de
-00018600: 6620 4645 5f73 706c 6974 5f6f 6e65 5f66  f FE_split_one_f
-00018610: 6965 6c64 5f69 6e74 6f5f 6d61 6e79 2864  ield_into_many(d
-00018620: 665f 696e 2c20 6669 656c 642c 2073 706c  f_in, field, spl
-00018630: 6974 7465 722c 2066 696c 6c65 722c 206e  itter, filler, n
-00018640: 6577 5f6e 616d 6573 5f6c 6973 743d 2727  ew_names_list=''
-00018650: 2c20 6164 645f 636f 756e 745f 6669 656c  , add_count_fiel
-00018660: 643d 4661 6c73 6529 3a0a 2020 2020 2222  d=False):.    ""
-00018670: 220a 2020 2020 4645 2073 7461 6e64 7320  ".    FE stands 
-00018680: 666f 7220 4665 6174 7572 6520 456e 6769  for Feature Engi
-00018690: 6e65 6572 696e 6720 2d20 6974 206d 6561  neering - it mea
-000186a0: 6e73 2074 6869 7320 6675 6e63 7469 6f6e  ns this function
-000186b0: 2070 6572 666f 726d 7320 6665 6174 7572   performs featur
-000186c0: 6520 656e 6769 6e65 6572 696e 670a 2020  e engineering.  
-000186d0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-000186e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000186f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000172d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000172e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000172f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00017300: 2323 2323 2323 2323 2323 0a20 2020 2022  ##########.    "
+00017310: 2222 0a20 2020 2073 6d61 6c6c 6466 203d  "".    smalldf =
+00017320: 2073 6d61 6c6c 6466 2e63 6f70 7928 290a   smalldf.copy().
+00017330: 2020 2020 6164 645f 636f 6c73 203d 205b      add_cols = [
+00017340: 5d0a 2020 2020 6461 7465 5f74 696d 655f  ].    date_time_
+00017350: 7661 7269 6162 6c65 5f66 6c61 6720 3d20  variable_flag = 
+00017360: 4661 6c73 650a 2020 2020 6966 2073 6d61  False.    if sma
+00017370: 6c6c 6466 5b73 7461 7274 5469 6d65 5d2e  lldf[startTime].
+00017380: 6474 7970 6520 696e 205b 2764 6174 6574  dtype in ['datet
+00017390: 696d 6536 345b 6e73 5d27 2c27 6461 7465  ime64[ns]','date
+000173a0: 7469 6d65 3136 5b6e 735d 272c 2764 6174  time16[ns]','dat
+000173b0: 6574 696d 6533 325b 6e73 5d27 5d3a 0a20  etime32[ns]']:. 
+000173c0: 2020 2020 2020 2070 7269 6e74 2827 2573         print('%s
+000173d0: 2076 6172 6961 626c 6520 6973 2061 2064   variable is a d
+000173e0: 6174 652d 7469 6d65 2076 6172 6961 626c  ate-time variabl
+000173f0: 6527 2025 7374 6172 7454 696d 6529 0a20  e' %startTime). 
+00017400: 2020 2020 2020 2064 6174 655f 7469 6d65         date_time
+00017410: 5f76 6172 6961 626c 655f 666c 6167 203d  _variable_flag =
+00017420: 2054 7275 650a 2020 2020 6966 2064 6174   True.    if dat
+00017430: 655f 7469 6d65 5f76 6172 6961 626c 655f  e_time_variable_
+00017440: 666c 6167 3a0a 2020 2020 2020 2020 7669  flag:.        vi
+00017450: 6577 5f64 6179 7320 3d20 2770 726f 6365  ew_days = 'proce
+00017460: 7373 696e 6727 2b73 7461 7274 5469 6d65  ssing'+startTime
+00017470: 2b27 5f65 6c61 7073 6564 5f64 6179 7327  +'_elapsed_days'
+00017480: 0a20 2020 2020 2020 2073 6d61 6c6c 6466  .        smalldf
+00017490: 5b76 6965 775f 6461 7973 5d20 3d20 2873  [view_days] = (s
+000174a0: 6d61 6c6c 6466 5b65 6e64 5469 6d65 5d20  malldf[endTime] 
+000174b0: 2d20 736d 616c 6c64 665b 7374 6172 7454  - smalldf[startT
+000174c0: 696d 655d 292e 6173 7479 7065 2827 7469  ime]).astype('ti
+000174d0: 6d65 6465 6c74 6136 345b 735d 2729 2f28  medelta64[s]')/(
+000174e0: 3630 2a36 302a 3234 290a 2020 2020 2020  60*60*24).      
+000174f0: 2020 736d 616c 6c64 665b 7669 6577 5f64    smalldf[view_d
+00017500: 6179 735d 203d 2073 6d61 6c6c 6466 5b76  ays] = smalldf[v
+00017510: 6965 775f 6461 7973 5d2e 6173 7479 7065  iew_days].astype
+00017520: 2869 6e74 290a 2020 2020 2020 2020 6164  (int).        ad
+00017530: 645f 636f 6c73 2e61 7070 656e 6428 7669  d_cols.append(vi
+00017540: 6577 5f64 6179 7329 0a20 2020 2020 2020  ew_days).       
+00017550: 2076 6965 775f 7469 6d65 203d 2027 7072   view_time = 'pr
+00017560: 6f63 6573 7369 6e67 272b 7374 6172 7454  ocessing'+startT
+00017570: 696d 652b 275f 656c 6170 7365 645f 7469  ime+'_elapsed_ti
+00017580: 6d65 270a 2020 2020 2020 2020 736d 616c  me'.        smal
+00017590: 6c64 665b 7669 6577 5f74 696d 655d 203d  ldf[view_time] =
+000175a0: 2028 736d 616c 6c64 665b 656e 6454 696d   (smalldf[endTim
+000175b0: 655d 202d 2073 6d61 6c6c 6466 5b73 7461  e] - smalldf[sta
+000175c0: 7274 5469 6d65 5d29 2e61 7374 7970 6528  rtTime]).astype(
+000175d0: 2774 696d 6564 656c 7461 3634 5b73 5d27  'timedelta64[s]'
+000175e0: 292e 7661 6c75 6573 0a20 2020 2020 2020  ).values.       
+000175f0: 2061 6464 5f63 6f6c 732e 6170 7065 6e64   add_cols.append
+00017600: 2876 6965 775f 7469 6d65 290a 2020 2020  (view_time).    
+00017610: 656c 7365 3a0a 2020 2020 2020 2020 7374  else:.        st
+00017620: 6172 745f 6461 7465 203d 2027 7072 6f63  art_date = 'proc
+00017630: 6573 7369 6e67 272b 7374 6172 7454 696d  essing'+startTim
+00017640: 652b 275f 7374 6172 745f 6461 7465 270a  e+'_start_date'.
+00017650: 2020 2020 2020 2020 736d 616c 6c64 665b          smalldf[
+00017660: 7374 6172 745f 6461 7465 5d20 3d20 736d  start_date] = sm
+00017670: 616c 6c64 665b 7374 6172 7454 696d 655d  alldf[startTime]
+00017680: 2e6d 6170 286c 616d 6264 6120 783a 2078  .map(lambda x: x
+00017690: 2e73 706c 6974 2822 2022 295b 305d 290a  .split(" ")[0]).
+000176a0: 2020 2020 2020 2020 6164 645f 636f 6c73          add_cols
+000176b0: 2e61 7070 656e 6428 7374 6172 745f 6461  .append(start_da
+000176c0: 7465 290a 2020 2020 2020 2020 7472 793a  te).        try:
+000176d0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+000176e0: 7274 5f74 696d 6520 3d20 2770 726f 6365  rt_time = 'proce
+000176f0: 7373 696e 6727 2b73 7461 7274 5469 6d65  ssing'+startTime
+00017700: 2b27 5f73 7461 7274 5f74 696d 6527 0a20  +'_start_time'. 
+00017710: 2020 2020 2020 2020 2020 2073 6d61 6c6c             small
+00017720: 6466 5b73 7461 7274 5f74 696d 655d 203d  df[start_time] =
+00017730: 2073 6d61 6c6c 6466 5b73 7461 7274 5469   smalldf[startTi
+00017740: 6d65 5d2e 6d61 7028 6c61 6d62 6461 2078  me].map(lambda x
+00017750: 3a20 782e 7370 6c69 7428 2220 2229 5b31  : x.split(" ")[1
+00017760: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+00017770: 6464 5f63 6f6c 732e 6170 7065 6e64 2873  dd_cols.append(s
+00017780: 7461 7274 5f74 696d 6529 0a20 2020 2020  tart_time).     
+00017790: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+000177a0: 2020 2020 2020 2023 2323 2074 6865 7265         ### there
+000177b0: 2069 7320 6e6f 2068 6f75 722d 6d69 6e75   is no hour-minu
+000177c0: 7465 7320 7061 7274 206f 6620 7468 6973  tes part of this
+000177d0: 2064 6174 6520 7469 6d65 2073 7461 6d70   date time stamp
+000177e0: 2066 6965 6c64 2e20 596f 7520 6361 6e20   field. You can 
+000177f0: 6a75 7374 2073 6b69 7020 6974 2069 6620  just skip it if 
+00017800: 6974 2069 7320 6e6f 7420 7468 6572 650a  it is not there.
+00017810: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00017820: 0a20 2020 2020 2020 2065 6e64 5f64 6174  .        end_dat
+00017830: 6520 3d20 2770 726f 6365 7373 696e 6727  e = 'processing'
+00017840: 2b65 6e64 5469 6d65 2b27 5f65 6e64 5f64  +endTime+'_end_d
+00017850: 6174 6527 0a20 2020 2020 2020 2073 6d61  ate'.        sma
+00017860: 6c6c 6466 5b65 6e64 5f64 6174 655d 203d  lldf[end_date] =
+00017870: 2073 6d61 6c6c 6466 5b65 6e64 5469 6d65   smalldf[endTime
+00017880: 5d2e 6d61 7028 6c61 6d62 6461 2078 3a20  ].map(lambda x: 
+00017890: 782e 7370 6c69 7428 2220 2229 5b30 5d29  x.split(" ")[0])
+000178a0: 0a20 2020 2020 2020 2061 6464 5f63 6f6c  .        add_col
+000178b0: 732e 6170 7065 6e64 2865 6e64 5f64 6174  s.append(end_dat
+000178c0: 6529 0a20 2020 2020 2020 2074 7279 3a0a  e).        try:.
+000178d0: 2020 2020 2020 2020 2020 2020 656e 645f              end_
+000178e0: 7469 6d65 203d 2027 7072 6f63 6573 7369  time = 'processi
+000178f0: 6e67 272b 656e 6454 696d 652b 275f 656e  ng'+endTime+'_en
+00017900: 645f 7469 6d65 270a 2020 2020 2020 2020  d_time'.        
+00017910: 2020 2020 736d 616c 6c64 665b 656e 645f      smalldf[end_
+00017920: 7469 6d65 5d20 3d20 736d 616c 6c64 665b  time] = smalldf[
+00017930: 656e 6454 696d 655d 2e6d 6170 286c 616d  endTime].map(lam
+00017940: 6264 6120 783a 2078 2e73 706c 6974 2822  bda x: x.split("
+00017950: 2022 295b 315d 290a 2020 2020 2020 2020   ")[1]).        
+00017960: 2020 2020 6164 645f 636f 6c73 2e61 7070      add_cols.app
+00017970: 656e 6428 656e 645f 7469 6d65 290a 2020  end(end_time).  
+00017980: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00017990: 2020 2020 2020 2020 2020 2323 2320 7468            ### th
+000179a0: 6572 6520 6973 206e 6f20 686f 7572 2d6d  ere is no hour-m
+000179b0: 696e 7574 6573 2070 6172 7420 6f66 2074  inutes part of t
+000179c0: 6869 7320 6461 7465 2074 696d 6520 7374  his date time st
+000179d0: 616d 7020 6669 656c 642e 2059 6f75 2063  amp field. You c
+000179e0: 616e 206a 7573 7420 736b 6970 2069 7420  an just skip it 
+000179f0: 6966 2069 7420 6973 206e 6f74 2074 6865  if it is not the
+00017a00: 7265 0a20 2020 2020 2020 2020 2020 2070  re.            p
+00017a10: 6173 730a 2020 2020 2020 2020 7669 6577  ass.        view
+00017a20: 5f64 6179 7320 3d20 2770 726f 6365 7373  _days = 'process
+00017a30: 696e 6727 2b73 7461 7274 5469 6d65 2b27  ing'+startTime+'
+00017a40: 5f65 6c61 7073 6564 5f64 6179 7327 0a20  _elapsed_days'. 
+00017a50: 2020 2020 2020 2073 6d61 6c6c 6466 5b76         smalldf[v
+00017a60: 6965 775f 6461 7973 5d20 3d20 2870 642e  iew_days] = (pd.
+00017a70: 746f 5f64 6174 6574 696d 6528 736d 616c  to_datetime(smal
+00017a80: 6c64 665b 656e 645f 6461 7465 5d29 202d  ldf[end_date]) -
+00017a90: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
+00017aa0: 736d 616c 6c64 665b 7374 6172 745f 6461  smalldf[start_da
+00017ab0: 7465 5d29 292e 7661 6c75 6573 2e61 7374  te])).values.ast
+00017ac0: 7970 6528 696e 7429 0a20 2020 2020 2020  ype(int).       
+00017ad0: 2061 6464 5f63 6f6c 732e 6170 7065 6e64   add_cols.append
+00017ae0: 2876 6965 775f 6461 7973 290a 2020 2020  (view_days).    
+00017af0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00017b00: 2020 2020 2076 6965 775f 7469 6d65 203d       view_time =
+00017b10: 2027 7072 6f63 6573 7369 6e67 272b 7374   'processing'+st
+00017b20: 6172 7454 696d 652b 275f 656c 6170 7365  artTime+'_elapse
+00017b30: 645f 7469 6d65 270a 2020 2020 2020 2020  d_time'.        
+00017b40: 2020 2020 736d 616c 6c64 665b 7669 6577      smalldf[view
+00017b50: 5f74 696d 655d 203d 2028 7064 2e74 6f5f  _time] = (pd.to_
+00017b60: 6461 7465 7469 6d65 2873 6d61 6c6c 6466  datetime(smalldf
+00017b70: 5b65 6e64 5f74 696d 655d 2920 2d20 7064  [end_time]) - pd
+00017b80: 2e74 6f5f 6461 7465 7469 6d65 2873 6d61  .to_datetime(sma
+00017b90: 6c6c 6466 5b73 7461 7274 5f74 696d 655d  lldf[start_time]
+00017ba0: 2929 2e61 7374 7970 6528 2774 696d 6564  )).astype('timed
+00017bb0: 656c 7461 3634 5b73 5d27 292e 7661 6c75  elta64[s]').valu
+00017bc0: 6573 0a20 2020 2020 2020 2020 2020 2061  es.            a
+00017bd0: 6464 5f63 6f6c 732e 6170 7065 6e64 2876  dd_cols.append(v
+00017be0: 6965 775f 7469 6d65 290a 2020 2020 2020  iew_time).      
+00017bf0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00017c00: 2020 2020 2020 2323 2320 496e 2073 6f6d        ### In som
+00017c10: 6520 6461 7465 2074 696d 6520 6669 656c  e date time fiel
+00017c20: 6473 2074 6869 7320 6769 7665 7320 616e  ds this gives an
+00017c30: 2065 7272 6f72 2073 6f20 736b 6970 2069   error so skip i
+00017c40: 7420 696e 2074 6861 7420 6361 7365 0a20  t in that case. 
+00017c50: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00017c60: 2020 2020 2020 2020 2323 2323 2054 6865          #### The
+00017c70: 2072 6561 736f 6e20 7765 2063 686f 7365   reason we chose
+00017c80: 2065 6e64 5469 6d65 2068 6572 6520 6973   endTime here is
+00017c90: 2074 6861 7420 7374 6172 7454 696d 6520   that startTime 
+00017ca0: 6973 2075 7375 616c 6c79 2074 616b 656e  is usually taken
+00017cb0: 2063 6172 6520 6f66 2062 7920 616e 6f74   care of by anot
+00017cc0: 6865 7220 6c69 6272 6172 792e 2053 6f20  her library. So 
+00017cd0: 6265 7474 6572 2074 6f20 646f 2074 6869  better to do thi
+00017ce0: 7320 616c 6f6e 652e 0a20 2020 2020 2020  s alone..       
+00017cf0: 2079 6561 7220 3d20 2770 726f 6365 7373   year = 'process
+00017d00: 696e 6727 2b65 6e64 5469 6d65 2b27 5f65  ing'+endTime+'_e
+00017d10: 6e64 5f79 6561 7227 0a20 2020 2020 2020  nd_year'.       
+00017d20: 2073 6d61 6c6c 6466 5b79 6561 725d 203d   smalldf[year] =
+00017d30: 2073 6d61 6c6c 6466 5b65 6e64 5f64 6174   smalldf[end_dat
+00017d40: 655d 2e6d 6170 286c 616d 6264 6120 783a  e].map(lambda x:
+00017d50: 2073 7472 2878 292e 7370 6c69 7428 7370   str(x).split(sp
+00017d60: 6c69 7474 6572 5f64 6174 655f 7374 7269  litter_date_stri
+00017d70: 6e67 295b 305d 292e 7661 6c75 6573 0a20  ng)[0]).values. 
+00017d80: 2020 2020 2020 2061 6464 5f63 6f6c 732e         add_cols.
+00017d90: 6170 7065 6e64 2879 6561 7229 0a20 2020  append(year).   
+00017da0: 2020 2020 2023 2323 2320 5468 6520 7265       #### The re
+00017db0: 6173 6f6e 2077 6520 6368 6f73 6520 656e  ason we chose en
+00017dc0: 6454 696d 6520 6865 7265 2069 7320 7468  dTime here is th
+00017dd0: 6174 2073 7461 7274 5469 6d65 2069 7320  at startTime is 
+00017de0: 7573 7561 6c6c 7920 7461 6b65 6e20 6361  usually taken ca
+00017df0: 7265 206f 6620 6279 2061 6e6f 7468 6572  re of by another
+00017e00: 206c 6962 7261 7279 2e20 536f 2062 6574   library. So bet
+00017e10: 7465 7220 746f 2064 6f20 7468 6973 2061  ter to do this a
+00017e20: 6c6f 6e65 2e0a 2020 2020 2020 2020 6d6f  lone..        mo
+00017e30: 6e74 6820 3d20 2770 726f 6365 7373 696e  nth = 'processin
+00017e40: 6727 2b65 6e64 5469 6d65 2b27 5f65 6e64  g'+endTime+'_end
+00017e50: 5f6d 6f6e 7468 270a 2020 2020 2020 2020  _month'.        
+00017e60: 736d 616c 6c64 665b 6d6f 6e74 685d 203d  smalldf[month] =
+00017e70: 2073 6d61 6c6c 6466 5b65 6e64 5f64 6174   smalldf[end_dat
+00017e80: 655d 2e6d 6170 286c 616d 6264 6120 783a  e].map(lambda x:
+00017e90: 2073 7472 2878 292e 7370 6c69 7428 7370   str(x).split(sp
+00017ea0: 6c69 7474 6572 5f64 6174 655f 7374 7269  litter_date_stri
+00017eb0: 6e67 295b 315d 292e 7661 6c75 6573 0a20  ng)[1]).values. 
+00017ec0: 2020 2020 2020 2061 6464 5f63 6f6c 732e         add_cols.
+00017ed0: 6170 7065 6e64 286d 6f6e 7468 290a 2020  append(month).  
+00017ee0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00017ef0: 2020 2020 2020 2023 2323 2320 5468 6520         #### The 
+00017f00: 7265 6173 6f6e 2077 6520 6368 6f73 6520  reason we chose 
+00017f10: 656e 6454 696d 6520 6865 7265 2069 7320  endTime here is 
+00017f20: 7468 6174 2073 7461 7274 5469 6d65 2069  that startTime i
+00017f30: 7320 7573 7561 6c6c 7920 7461 6b65 6e20  s usually taken 
+00017f40: 6361 7265 206f 6620 6279 2061 6e6f 7468  care of by anoth
+00017f50: 6572 206c 6962 7261 7279 2e20 536f 2062  er library. So b
+00017f60: 6574 7465 7220 746f 2064 6f20 7468 6973  etter to do this
+00017f70: 2061 6c6f 6e65 2e0a 2020 2020 2020 2020   alone..        
+00017f80: 2020 2020 6461 796e 756d 203d 2027 7072      daynum = 'pr
+00017f90: 6f63 6573 7369 6e67 272b 656e 6454 696d  ocessing'+endTim
+00017fa0: 652b 275f 656e 645f 6461 795f 6e75 6d62  e+'_end_day_numb
+00017fb0: 6572 270a 2020 2020 2020 2020 2020 2020  er'.            
+00017fc0: 736d 616c 6c64 665b 6461 796e 756d 5d20  smalldf[daynum] 
+00017fd0: 3d20 736d 616c 6c64 665b 656e 645f 6461  = smalldf[end_da
+00017fe0: 7465 5d2e 6d61 7028 6c61 6d62 6461 2078  te].map(lambda x
+00017ff0: 3a20 7374 7228 7829 2e73 706c 6974 2873  : str(x).split(s
+00018000: 706c 6974 7465 725f 6461 7465 5f73 7472  plitter_date_str
+00018010: 696e 6729 5b32 5d29 2e76 616c 7565 730a  ing)[2]).values.
+00018020: 2020 2020 2020 2020 2020 2020 6164 645f              add_
+00018030: 636f 6c73 2e61 7070 656e 6428 6461 796e  cols.append(dayn
+00018040: 756d 290a 2020 2020 2020 2020 6578 6365  um).        exce
+00018050: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00018060: 2323 2320 496e 2073 6f6d 6520 6461 7465  ### In some date
+00018070: 2074 696d 6520 6669 656c 6473 2074 6865   time fields the
+00018080: 2064 6179 206e 756d 6265 7220 6973 206e   day number is n
+00018090: 6f74 2074 6865 7265 2e20 4966 206e 6f74  ot there. If not
+000180a0: 2c20 6a75 7374 2073 6b69 7020 6974 2023  , just skip it #
+000180b0: 2323 230a 2020 2020 2020 2020 2020 2020  ###.            
+000180c0: 7061 7373 0a20 2020 2020 2020 2023 2323  pass.        ###
+000180d0: 2320 496e 2073 6f6d 6520 6461 7465 2074  # In some date t
+000180e0: 696d 6520 6669 656c 6473 2c20 7468 6520  ime fields, the 
+000180f0: 686f 7572 2061 6e64 206d 696e 7574 6520  hour and minute 
+00018100: 6973 206e 6f74 2074 6865 7265 2c20 736f  is not there, so
+00018110: 2073 6b69 7020 6974 2069 6e20 7468 6174   skip it in that
+00018120: 2063 6173 6520 6966 2069 7420 6572 726f   case if it erro
+00018130: 7273 210a 2020 2020 2020 2020 7472 793a  rs!.        try:
+00018140: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00018150: 7274 5f68 6f75 7220 3d20 2770 726f 6365  rt_hour = 'proce
+00018160: 7373 696e 6727 2b73 7461 7274 5469 6d65  ssing'+startTime
+00018170: 2b27 5f73 7461 7274 5f68 6f75 7227 0a20  +'_start_hour'. 
+00018180: 2020 2020 2020 2020 2020 2073 6d61 6c6c             small
+00018190: 6466 5b73 7461 7274 5f68 6f75 725d 203d  df[start_hour] =
+000181a0: 2073 6d61 6c6c 6466 5b73 7461 7274 5f74   smalldf[start_t
+000181b0: 696d 655d 2e6d 6170 286c 616d 6264 6120  ime].map(lambda 
+000181c0: 783a 2073 7472 2878 292e 7370 6c69 7428  x: str(x).split(
+000181d0: 7370 6c69 7474 6572 5f68 6f75 725f 7374  splitter_hour_st
+000181e0: 7269 6e67 295b 305d 292e 7661 6c75 6573  ring)[0]).values
+000181f0: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+00018200: 5f63 6f6c 732e 6170 7065 6e64 2873 7461  _cols.append(sta
+00018210: 7274 5f68 6f75 7229 0a20 2020 2020 2020  rt_hour).       
+00018220: 2020 2020 2073 7461 7274 5f6d 696e 203d       start_min =
+00018230: 2027 7072 6f63 6573 7369 6e67 272b 7374   'processing'+st
+00018240: 6172 7454 696d 652b 275f 7374 6172 745f  artTime+'_start_
+00018250: 686f 7572 270a 2020 2020 2020 2020 2020  hour'.          
+00018260: 2020 736d 616c 6c64 665b 7374 6172 745f    smalldf[start_
+00018270: 6d69 6e5d 203d 2073 6d61 6c6c 6466 5b73  min] = smalldf[s
+00018280: 7461 7274 5f74 696d 655d 2e6d 6170 286c  tart_time].map(l
+00018290: 616d 6264 6120 783a 2073 7472 2878 292e  ambda x: str(x).
+000182a0: 7370 6c69 7428 7370 6c69 7474 6572 5f68  split(splitter_h
+000182b0: 6f75 725f 7374 7269 6e67 295b 315d 292e  our_string)[1]).
+000182c0: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+000182d0: 2020 2061 6464 5f63 6f6c 732e 6170 7065     add_cols.appe
+000182e0: 6e64 2873 7461 7274 5f6d 696e 290a 2020  nd(start_min).  
+000182f0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00018300: 2020 2020 2020 2020 2020 2323 2320 4966            ### If
+00018310: 2069 7420 6572 726f 7273 2c20 736b 6970   it errors, skip
+00018320: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
+00018330: 7061 7373 0a20 2020 2020 2020 2023 2323  pass.        ###
+00018340: 2320 4368 6563 6b20 6966 2074 6865 7265  # Check if there
+00018350: 2069 7320 6120 7765 656b 6461 7920 616e   is a weekday an
+00018360: 6420 7765 656b 656e 6473 2069 6e20 6461  d weekends in da
+00018370: 7465 2074 696d 6520 636f 6c75 6d6e 7320  te time columns 
+00018380: 7573 696e 6720 656e 6454 696d 6520 6f6e  using endTime on
+00018390: 6c79 0a20 2020 2020 2020 2077 6565 6b64  ly.        weekd
+000183a0: 6179 5f6e 756d 203d 2027 7072 6f63 6573  ay_num = 'proces
+000183b0: 7369 6e67 272b 656e 6454 696d 652b 275f  sing'+endTime+'_
+000183c0: 656e 645f 7765 656b 6461 795f 6e75 6d62  end_weekday_numb
+000183d0: 6572 270a 2020 2020 2020 2020 736d 616c  er'.        smal
+000183e0: 6c64 665b 7765 656b 6461 795f 6e75 6d5d  ldf[weekday_num]
+000183f0: 203d 2070 642e 746f 5f64 6174 6574 696d   = pd.to_datetim
+00018400: 6528 736d 616c 6c64 665b 656e 645f 6461  e(smalldf[end_da
+00018410: 7465 5d29 2e64 742e 7765 656b 6461 792e  te]).dt.weekday.
+00018420: 7661 6c75 6573 0a20 2020 2020 2020 2061  values.        a
+00018430: 6464 5f63 6f6c 732e 6170 7065 6e64 2877  dd_cols.append(w
+00018440: 6565 6b64 6179 5f6e 756d 290a 2020 2020  eekday_num).    
+00018450: 2020 2020 7765 656b 656e 6420 3d20 2770      weekend = 'p
+00018460: 726f 6365 7373 696e 6727 2b65 6e64 5469  rocessing'+endTi
+00018470: 6d65 2b27 5f65 6e64 5f77 6565 6b65 6e64  me+'_end_weekend
+00018480: 5f66 6c61 6727 0a20 2020 2020 2020 2073  _flag'.        s
+00018490: 6d61 6c6c 6466 5b77 6565 6b65 6e64 5d20  malldf[weekend] 
+000184a0: 3d20 736d 616c 6c64 665b 7765 656b 6461  = smalldf[weekda
+000184b0: 795f 6e75 6d5d 2e6d 6170 286c 616d 6264  y_num].map(lambd
+000184c0: 6120 783a 2031 2069 6620 7820 696e 5b35  a x: 1 if x in[5
+000184d0: 2c36 5d20 656c 7365 2030 290a 2020 2020  ,6] else 0).    
+000184e0: 2020 2020 6164 645f 636f 6c73 2e61 7070      add_cols.app
+000184f0: 656e 6428 7765 656b 656e 6429 0a20 2020  end(weekend).   
+00018500: 2023 2323 2320 4966 2065 7665 7279 7468   #### If everyth
+00018510: 696e 6720 776f 726b 7320 7765 6c6c 2c20  ing works well, 
+00018520: 7468 6572 6520 7368 6f75 6c64 2062 6520  there should be 
+00018530: 3133 206e 6577 2063 6f6c 756d 6e73 2061  13 new columns a
+00018540: 6464 6564 2062 7920 6d6f 6475 6c65 2e20  dded by module. 
+00018550: 416c 6c20 7468 6520 6265 7374 210a 2020  All the best!.  
+00018560: 2020 7072 696e 7428 2725 6420 636f 6c75    print('%d colu
+00018570: 6d6e 7320 6164 6465 6420 7573 696e 6720  mns added using 
+00018580: 7374 6172 7420 6461 7465 3d25 7320 616e  start date=%s an
+00018590: 6420 656e 6420 6461 7465 3d25 7320 7072  d end date=%s pr
+000185a0: 6f63 6573 7369 6e67 2e2e 2e27 2025 286c  ocessing...' %(l
+000185b0: 656e 2861 6464 5f63 6f6c 7329 2c73 7461  en(add_cols),sta
+000185c0: 7274 5469 6d65 2c65 6e64 5469 6d65 2929  rtTime,endTime))
+000185d0: 0a20 2020 2072 6574 7572 6e20 736d 616c  .    return smal
+000185e0: 6c64 660a 2323 2323 2323 2323 2323 2323  ldf.############
+000185f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018620: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00018630: 6465 6620 4645 5f73 706c 6974 5f6f 6e65  def FE_split_one
+00018640: 5f66 6965 6c64 5f69 6e74 6f5f 6d61 6e79  _field_into_many
+00018650: 2864 665f 696e 2c20 6669 656c 642c 2073  (df_in, field, s
+00018660: 706c 6974 7465 722c 2066 696c 6c65 722c  plitter, filler,
+00018670: 206e 6577 5f6e 616d 6573 5f6c 6973 743d   new_names_list=
+00018680: 2727 2c20 6164 645f 636f 756e 745f 6669  '', add_count_fi
+00018690: 656c 643d 4661 6c73 6529 3a0a 2020 2020  eld=False):.    
+000186a0: 2222 220a 2020 2020 4645 2073 7461 6e64  """.    FE stand
+000186b0: 7320 666f 7220 4665 6174 7572 6520 456e  s for Feature En
+000186c0: 6769 6e65 6572 696e 6720 2d20 6974 206d  gineering - it m
+000186d0: 6561 6e73 2074 6869 7320 6675 6e63 7469  eans this functi
+000186e0: 6f6e 2070 6572 666f 726d 7320 6665 6174  on performs feat
+000186f0: 7572 6520 656e 6769 6e65 6572 696e 670a  ure engineering.
+00018700: 2020 2020 2323 2323 2323 2323 2323 2323      ############
 00018710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018720: 2323 2323 2323 2323 0a20 2020 2054 6869  ########.    Thi
-00018730: 7320 6675 6e63 7469 6f6e 2074 616b 6573  s function takes
-00018740: 2061 6e79 2064 6174 6120 6672 616d 6520   any data frame 
-00018750: 6669 656c 6420 2873 7472 696e 6720 7661  field (string va
-00018760: 7269 6162 6c65 7320 6f6e 6c79 2920 616e  riables only) an
-00018770: 6420 7370 6c69 7473 0a20 2020 2069 7420  d splits.    it 
-00018780: 696e 746f 2061 7320 6d61 6e79 2066 6965  into as many fie
-00018790: 6c64 7320 6173 2079 6f75 2077 616e 7420  lds as you want 
-000187a0: 696e 2074 6865 206e 6577 5f6e 616d 6573  in the new_names
-000187b0: 5f6c 6973 742e 0a0a 2020 2020 496e 7075  _list...    Inpu
-000187c0: 7473 3a0a 2020 2020 2020 2020 6466 743a  ts:.        dft:
-000187d0: 2070 616e 6461 7320 4461 7461 4672 616d   pandas DataFram
-000187e0: 650a 2020 2020 2020 2020 6669 656c 643a  e.        field:
-000187f0: 206e 616d 6520 6f66 2073 7472 696e 6720   name of string 
-00018800: 636f 6c75 6d6e 2074 6861 7420 796f 7520  column that you 
-00018810: 7761 6e74 2074 6f20 7370 6c69 7420 7573  want to split us
-00018820: 696e 6720 7468 6520 7370 6c69 7474 6572  ing the splitter
-00018830: 2073 7472 696e 6720 7370 6563 6966 6965   string specifie
-00018840: 640a 2020 2020 2020 2020 7370 6c69 7474  d.        splitt
-00018850: 6572 3a20 7370 6563 6966 7920 7768 6174  er: specify what
-00018860: 2073 7472 696e 6720 746f 2073 706c 6974   string to split
-00018870: 206f 6e20 7573 696e 6720 7468 6520 7370   on using the sp
-00018880: 6c69 7474 6572 2061 7267 756d 656e 742e  litter argument.
-00018890: 0a20 2020 2020 2020 2066 696c 6c65 723a  .        filler:
-000188a0: 2059 6f75 2063 616e 2061 6c73 6f20 6669   You can also fi
-000188b0: 6c6c 204e 756c 6c20 7661 6c75 6573 2074  ll Null values t
-000188c0: 6861 7420 6d61 7920 6861 7070 656e 2064  hat may happen d
-000188d0: 7565 2074 6f20 796f 7572 2073 706c 6974  ue to your split
-000188e0: 7469 6e67 2062 7920 7370 6563 6966 7969  ting by specifyi
-000188f0: 6e67 2061 2066 696c 6c65 722e 0a20 2020  ng a filler..   
-00018900: 2020 2020 206e 6577 5f6e 616d 6573 5f6c       new_names_l
-00018910: 6973 743a 2049 6620 6e6f 206e 6577 5f6e  ist: If no new_n
-00018920: 616d 6573 5f6c 6973 7420 6973 2067 6976  ames_list is giv
-00018930: 656e 2c20 7468 656e 2077 6520 7573 6520  en, then we use 
-00018940: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-00018950: 6669 656c 6420 6974 7365 6c66 2074 6f20  field itself to 
-00018960: 6372 6561 7465 206e 6577 2063 6f6c 756d  create new colum
-00018970: 6e73 2e0a 2020 2020 2020 2020 6164 645f  ns..        add_
-00018980: 636f 756e 745f 6669 656c 643a 2046 616c  count_field: Fal
-00018990: 7365 2028 6465 6661 756c 7429 2e20 4966  se (default). If
-000189a0: 2054 7275 652c 2069 7420 7769 6c6c 2063   True, it will c
-000189b0: 6f75 6e74 2074 6865 206e 756d 6265 7220  ount the number 
-000189c0: 6f66 2069 7465 6d73 2069 6e0a 2020 2020  of items in.    
-000189d0: 2020 2020 2020 2020 7468 6520 2266 6965          the "fie
-000189e0: 6c64 2220 636f 6c75 6d6e 2062 6566 6f72  ld" column befor
-000189f0: 6520 7468 6520 7370 6c69 742e 2054 6869  e the split. Thi
-00018a00: 7320 6d61 7920 6265 206e 6565 6465 6420  s may be needed 
-00018a10: 696e 206e 6573 7465 6420 6469 6374 696f  in nested dictio
-00018a20: 6e61 7279 2066 6965 6c64 732e 0a0a 2020  nary fields...  
-00018a30: 2020 4f75 7470 7574 733a 0a20 2020 2020    Outputs:.     
-00018a40: 2020 2064 6674 3a20 6f72 6967 696e 616c     dft: original
-00018a50: 2064 6174 6166 7261 6d65 2077 6974 6820   dataframe with 
-00018a60: 6164 6469 7469 6f6e 616c 2063 6f6c 756d  additional colum
-00018a70: 6e73 2063 7265 6174 6564 2062 7920 7370  ns created by sp
-00018a80: 6c69 7474 696e 6720 7468 6520 6669 656c  litting the fiel
-00018a90: 642e 0a20 2020 2020 2020 206e 6577 5f6e  d..        new_n
-00018aa0: 616d 6573 5f6c 6973 743a 2074 6865 206c  ames_list: the l
-00018ab0: 6973 7420 6f66 206e 6577 2063 6f6c 756d  ist of new colum
-00018ac0: 6e73 2063 7265 6174 6564 2062 7920 7468  ns created by th
-00018ad0: 6973 2066 756e 6374 696f 6e0a 2020 2020  is function.    
-00018ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018750: 2323 2323 2323 2323 2323 0a20 2020 2054  ##########.    T
+00018760: 6869 7320 6675 6e63 7469 6f6e 2074 616b  his function tak
+00018770: 6573 2061 6e79 2064 6174 6120 6672 616d  es any data fram
+00018780: 6520 6669 656c 6420 2873 7472 696e 6720  e field (string 
+00018790: 7661 7269 6162 6c65 7320 6f6e 6c79 2920  variables only) 
+000187a0: 616e 6420 7370 6c69 7473 0a20 2020 2069  and splits.    i
+000187b0: 7420 696e 746f 2061 7320 6d61 6e79 2066  t into as many f
+000187c0: 6965 6c64 7320 6173 2079 6f75 2077 616e  ields as you wan
+000187d0: 7420 696e 2074 6865 206e 6577 5f6e 616d  t in the new_nam
+000187e0: 6573 5f6c 6973 742e 0a0a 2020 2020 496e  es_list...    In
+000187f0: 7075 7473 3a0a 2020 2020 2020 2020 6466  puts:.        df
+00018800: 743a 2070 616e 6461 7320 4461 7461 4672  t: pandas DataFr
+00018810: 616d 650a 2020 2020 2020 2020 6669 656c  ame.        fiel
+00018820: 643a 206e 616d 6520 6f66 2073 7472 696e  d: name of strin
+00018830: 6720 636f 6c75 6d6e 2074 6861 7420 796f  g column that yo
+00018840: 7520 7761 6e74 2074 6f20 7370 6c69 7420  u want to split 
+00018850: 7573 696e 6720 7468 6520 7370 6c69 7474  using the splitt
+00018860: 6572 2073 7472 696e 6720 7370 6563 6966  er string specif
+00018870: 6965 640a 2020 2020 2020 2020 7370 6c69  ied.        spli
+00018880: 7474 6572 3a20 7370 6563 6966 7920 7768  tter: specify wh
+00018890: 6174 2073 7472 696e 6720 746f 2073 706c  at string to spl
+000188a0: 6974 206f 6e20 7573 696e 6720 7468 6520  it on using the 
+000188b0: 7370 6c69 7474 6572 2061 7267 756d 656e  splitter argumen
+000188c0: 742e 0a20 2020 2020 2020 2066 696c 6c65  t..        fille
+000188d0: 723a 2059 6f75 2063 616e 2061 6c73 6f20  r: You can also 
+000188e0: 6669 6c6c 204e 756c 6c20 7661 6c75 6573  fill Null values
+000188f0: 2074 6861 7420 6d61 7920 6861 7070 656e   that may happen
+00018900: 2064 7565 2074 6f20 796f 7572 2073 706c   due to your spl
+00018910: 6974 7469 6e67 2062 7920 7370 6563 6966  itting by specif
+00018920: 7969 6e67 2061 2066 696c 6c65 722e 0a20  ying a filler.. 
+00018930: 2020 2020 2020 206e 6577 5f6e 616d 6573         new_names
+00018940: 5f6c 6973 743a 2049 6620 6e6f 206e 6577  _list: If no new
+00018950: 5f6e 616d 6573 5f6c 6973 7420 6973 2067  _names_list is g
+00018960: 6976 656e 2c20 7468 656e 2077 6520 7573  iven, then we us
+00018970: 6520 7468 6520 6e61 6d65 206f 6620 7468  e the name of th
+00018980: 6520 6669 656c 6420 6974 7365 6c66 2074  e field itself t
+00018990: 6f20 6372 6561 7465 206e 6577 2063 6f6c  o create new col
+000189a0: 756d 6e73 2e0a 2020 2020 2020 2020 6164  umns..        ad
+000189b0: 645f 636f 756e 745f 6669 656c 643a 2046  d_count_field: F
+000189c0: 616c 7365 2028 6465 6661 756c 7429 2e20  alse (default). 
+000189d0: 4966 2054 7275 652c 2069 7420 7769 6c6c  If True, it will
+000189e0: 2063 6f75 6e74 2074 6865 206e 756d 6265   count the numbe
+000189f0: 7220 6f66 2069 7465 6d73 2069 6e0a 2020  r of items in.  
+00018a00: 2020 2020 2020 2020 2020 7468 6520 2266            the "f
+00018a10: 6965 6c64 2220 636f 6c75 6d6e 2062 6566  ield" column bef
+00018a20: 6f72 6520 7468 6520 7370 6c69 742e 2054  ore the split. T
+00018a30: 6869 7320 6d61 7920 6265 206e 6565 6465  his may be neede
+00018a40: 6420 696e 206e 6573 7465 6420 6469 6374  d in nested dict
+00018a50: 696f 6e61 7279 2066 6965 6c64 732e 0a0a  ionary fields...
+00018a60: 2020 2020 4f75 7470 7574 733a 0a20 2020      Outputs:.   
+00018a70: 2020 2020 2064 6674 3a20 6f72 6967 696e       dft: origin
+00018a80: 616c 2064 6174 6166 7261 6d65 2077 6974  al dataframe wit
+00018a90: 6820 6164 6469 7469 6f6e 616c 2063 6f6c  h additional col
+00018aa0: 756d 6e73 2063 7265 6174 6564 2062 7920  umns created by 
+00018ab0: 7370 6c69 7474 696e 6720 7468 6520 6669  splitting the fi
+00018ac0: 656c 642e 0a20 2020 2020 2020 206e 6577  eld..        new
+00018ad0: 5f6e 616d 6573 5f6c 6973 743a 2074 6865  _names_list: the
+00018ae0: 206c 6973 7420 6f66 206e 6577 2063 6f6c   list of new col
+00018af0: 756d 6e73 2063 7265 6174 6564 2062 7920  umns created by 
+00018b00: 7468 6973 2066 756e 6374 696f 6e0a 2020  this function.  
+00018b10: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
 00018b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018b30: 2323 2323 2323 0a20 2020 2022 2222 0a20  ######.    """. 
-00018b40: 2020 2064 665f 6669 656c 6420 3d20 6466     df_field = df
-00018b50: 5f69 6e5b 6669 656c 645d 2e76 616c 7565  _in[field].value
-00018b60: 730a 2020 2020 6466 203d 2063 6f70 792e  s.    df = copy.
-00018b70: 6465 6570 636f 7079 2864 665f 696e 290a  deepcopy(df_in).
-00018b80: 2020 2020 2323 2320 4669 7273 7420 636f      ### First co
-00018b90: 7079 2020 7768 6174 6576 6572 2069 7320  py  whatever is 
-00018ba0: 696e 2074 6861 7420 6669 656c 6420 736f  in that field so
-00018bb0: 2077 6520 6361 6e20 7361 7665 2069 7420   we can save it 
-00018bc0: 666f 7220 6c61 7465 7220 2323 230a 2020  for later ###.  
-00018bd0: 2020 2323 2320 5265 6d65 6d62 6572 2074    ### Remember t
-00018be0: 6861 7420 6669 6c6c 6e61 206f 6e6c 7920  hat fillna only 
-00018bf0: 776f 726b 7320 6174 2064 6174 6166 7261  works at datafra
-00018c00: 6d65 206c 6576 656c 2120 2323 230a 2020  me level! ###.  
-00018c10: 2020 6466 5b5b 6669 656c 645d 5d20 3d20    df[[field]] = 
-00018c20: 6466 5b5b 6669 656c 645d 5d2e 6669 6c6c  df[[field]].fill
-00018c30: 6e61 2866 696c 6c65 7229 0a20 2020 2069  na(filler).    i
-00018c40: 6620 6164 645f 636f 756e 745f 6669 656c  f add_count_fiel
-00018c50: 643a 0a20 2020 2020 2020 2023 2323 2074  d:.        ### t
-00018c60: 6865 7265 2077 696c 6c20 6265 206f 6e65  here will be one
-00018c70: 2065 7874 7261 2066 6965 6c64 2063 7265   extra field cre
-00018c80: 6174 6564 2077 6865 6e20 7765 2063 6f75  ated when we cou
-00018c90: 6e74 2074 6865 206e 756d 6265 7220 6f66  nt the number of
-00018ca0: 2063 6f6e 7465 6e74 7320 696e 2065 6163   contents in eac
-00018cb0: 6820 6669 656c 6420 2323 230a 2020 2020  h field ###.    
-00018cc0: 2020 2020 6d61 785f 7468 696e 6773 203d      max_things =
-00018cd0: 2064 665b 6669 656c 645d 2e6d 6170 286c   df[field].map(l
-00018ce0: 616d 6264 6120 783a 206c 656e 2878 2e73  ambda x: len(x.s
-00018cf0: 706c 6974 2873 706c 6974 7465 7229 2929  plit(splitter)))
-00018d00: 2e6d 6178 2829 202b 2031 0a20 2020 2065  .max() + 1.    e
-00018d10: 6c73 653a 0a20 2020 2020 2020 206d 6178  lse:.        max
-00018d20: 5f74 6869 6e67 7320 3d20 6466 5b66 6965  _things = df[fie
-00018d30: 6c64 5d2e 6d61 7028 6c61 6d62 6461 2078  ld].map(lambda x
-00018d40: 3a20 6c65 6e28 782e 7370 6c69 7428 7370  : len(x.split(sp
-00018d50: 6c69 7474 6572 2929 292e 6d61 7828 290a  litter))).max().
-00018d60: 2020 2020 6966 206c 656e 286e 6577 5f6e      if len(new_n
-00018d70: 616d 6573 5f6c 6973 7429 203d 3d20 303a  ames_list) == 0:
-00018d80: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-00018d90: 2020 2020 4d61 782e 2063 6f6c 756d 6e73      Max. columns
-00018da0: 2063 7265 6174 6564 2062 7920 7370 6c69   created by spli
-00018db0: 7474 696e 6720 2573 2066 6965 6c64 2069  tting %s field i
-00018dc0: 7320 2564 2e27 2025 280a 2020 2020 2020  s %d.' %(.      
-00018dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018de0: 2020 2020 2020 6669 656c 642c 6d61 785f        field,max_
-00018df0: 7468 696e 6773 2929 0a20 2020 2065 6c73  things)).    els
-00018e00: 653a 0a20 2020 2020 2020 2069 6620 6e6f  e:.        if no
-00018e10: 7420 6d61 785f 7468 696e 6773 203d 3d20  t max_things == 
-00018e20: 6c65 6e28 6e65 775f 6e61 6d65 735f 6c69  len(new_names_li
-00018e30: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
-00018e40: 2070 7269 6e74 2822 2222 2020 2020 4d61   print("""    Ma
-00018e50: 782e 2063 6f6c 756d 6e73 2063 7265 6174  x. columns creat
-00018e60: 6564 2062 7920 7370 6c69 7474 696e 6720  ed by splitting 
-00018e70: 2573 2066 6965 6c64 2069 7320 2564 2062  %s field is %d b
-00018e80: 7574 2079 6f75 2068 6176 6520 6769 7665  ut you have give
-00018e90: 6e20 2564 0a20 2020 2020 2020 2020 2020  n %d.           
-00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018eb0: 2076 6172 6961 626c 6520 6e61 6d65 7320   variable names 
-00018ec0: 6f6e 6c79 2e20 5365 6c65 6374 696e 6720  only. Selecting 
-00018ed0: 6669 7273 7420 2564 2222 2220 2528 0a20  first %d""" %(. 
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ef0: 2020 2020 2020 2066 6965 6c64 2c6d 6178         field,max
-00018f00: 5f74 6869 6e67 732c 6c65 6e28 6e65 775f  _things,len(new_
-00018f10: 6e61 6d65 735f 6c69 7374 292c 6c65 6e28  names_list),len(
-00018f20: 6e65 775f 6e61 6d65 735f 6c69 7374 2929  new_names_list))
-00018f30: 290a 2020 2020 2323 2320 5468 6973 2063  ).    ### This c
-00018f40: 7265 6174 6573 2061 206e 6577 2066 6965  reates a new fie
-00018f50: 6c64 2074 6861 7420 636f 756e 7473 2074  ld that counts t
-00018f60: 6865 206e 756d 6265 7220 6f66 2074 6869  he number of thi
-00018f70: 6e67 7320 7468 6174 2061 7265 2069 6e20  ngs that are in 
-00018f80: 7468 6174 2066 6965 6c64 2e0a 2020 2020  that field..    
-00018f90: 6966 2061 6464 5f63 6f75 6e74 5f66 6965  if add_count_fie
-00018fa0: 6c64 3a0a 2020 2020 2020 2020 2323 2323  ld:.        ####
-00018fb0: 2074 6869 7320 636f 756e 7473 2074 6865   this counts the
-00018fc0: 206e 756d 6265 7220 6f66 2063 6f6e 7465   number of conte
-00018fd0: 6e74 7320 6166 7465 7220 7370 6c69 7474  nts after splitt
-00018fe0: 696e 6720 6561 6368 2072 6f77 2077 6869  ing each row whi
-00018ff0: 6368 2076 6172 6965 732e 2048 656e 6365  ch varies. Hence
-00019000: 2069 7420 6865 6c70 732e 0a20 2020 2020   it helps..     
-00019010: 2020 206e 756d 5f70 726f 6475 6374 735f     num_products_
-00019020: 7669 6577 6564 203d 2027 436f 6e74 656e  viewed = 'Conten
-00019030: 745f 436f 756e 745f 696e 5f27 2b66 6965  t_Count_in_'+fie
-00019040: 6c64 0a20 2020 2020 2020 2064 665b 6e75  ld.        df[nu
-00019050: 6d5f 7072 6f64 7563 7473 5f76 6965 7765  m_products_viewe
-00019060: 645d 203d 2064 665b 6669 656c 645d 2e6d  d] = df[field].m
-00019070: 6170 286c 616d 6264 6120 783a 206c 656e  ap(lambda x: len
-00019080: 2878 2e73 706c 6974 2873 706c 6974 7465  (x.split(splitte
-00019090: 7229 2929 2e76 616c 7565 730a 2020 2020  r))).values.    
-000190a0: 2323 2320 436c 6561 6e20 7570 2074 6865  ### Clean up the
-000190b0: 2066 6965 6c64 2073 7563 6820 7468 6174   field such that
-000190c0: 2069 7420 6861 7320 7468 6520 7269 6768   it has the righ
-000190d0: 7420 6e75 6d62 6572 206f 6620 7370 6c69  t number of spli
-000190e0: 7420 6368 6172 7320 6f74 6865 7277 6973  t chars otherwis
-000190f0: 6520 6164 6420 746f 2069 740a 2020 2020  e add to it.    
-00019100: 2323 2320 5468 6973 2066 696c 6c73 2075  ### This fills u
-00019110: 7020 7468 6520 6669 656c 6420 7769 7468  p the field with
-00019120: 2065 6d70 7479 2073 7472 696e 6773 2062   empty strings b
-00019130: 6574 7765 656e 2065 6163 6820 7370 6c69  etween each spli
-00019140: 7474 6572 2e20 596f 7520 6361 6e27 7420  tter. You can't 
-00019150: 646f 206d 7563 6820 6162 6f75 7420 6974  do much about it
-00019160: 2e0a 2020 2020 2323 2323 204c 6561 7665  ..    #### Leave
-00019170: 2074 6869 7320 6173 2069 7420 6973 2e20   this as it is. 
-00019180: 4974 2069 7320 6e6f 7420 736f 6d65 7468  It is not someth
-00019190: 696e 6720 796f 7520 6361 6e20 646f 2072  ing you can do r
-000191a0: 6967 6874 206e 6f77 2e20 4974 2077 6f72  ight now. It wor
-000191b0: 6b73 2e0a 2020 2020 6669 6c6c 5f73 7472  ks..    fill_str
-000191c0: 696e 6720 3d20 7370 6c69 7474 6572 202b  ing = splitter +
-000191d0: 2066 696c 6c65 720a 2020 2020 6466 5b66   filler.    df[f
-000191e0: 6965 6c64 5d20 3d20 6466 5b66 6965 6c64  ield] = df[field
-000191f0: 5d2e 6d61 7028 6c61 6d62 6461 2078 3a20  ].map(lambda x: 
-00019200: 782b 6669 6c6c 5f73 7472 696e 672a 286d  x+fill_string*(m
-00019210: 6178 5f74 6869 6e67 732d 6c65 6e28 782e  ax_things-len(x.
-00019220: 7370 6c69 7428 7370 6c69 7474 6572 2929  split(splitter))
-00019230: 2920 6966 206c 656e 280a 2020 2020 2020  ) if len(.      
-00019240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019250: 2020 2020 2020 2020 2020 2020 2020 782e                x.
-00019260: 7370 6c69 7428 7370 6c69 7474 6572 2929  split(splitter))
-00019270: 203c 206d 6178 5f74 6869 6e67 7320 656c   < max_things el
-00019280: 7365 2078 290a 2020 2020 2323 2323 2323  se x).    ######
-00019290: 204e 6f77 2079 6f75 2063 7265 6174 6520   Now you create 
-000192a0: 6e65 7720 6669 656c 6473 2062 7920 7370  new fields by sp
-000192b0: 6c69 7420 7468 6520 6f6e 6520 6c61 7267  lit the one larg
-000192c0: 6520 6669 656c 6420 2323 2323 2323 2323  e field ########
-000192d0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-000192e0: 6365 286e 6577 5f6e 616d 6573 5f6c 6973  ce(new_names_lis
-000192f0: 742c 2073 7472 293a 0a20 2020 2020 2020  t, str):.       
-00019300: 2069 6620 6e65 775f 6e61 6d65 735f 6c69   if new_names_li
-00019310: 7374 203d 3d20 2727 3a0a 2020 2020 2020  st == '':.      
-00019320: 2020 2020 2020 6e65 775f 6e61 6d65 735f        new_names_
-00019330: 6c69 7374 203d 205b 6669 656c 642b 275f  list = [field+'_
-00019340: 272b 7374 7228 6929 2066 6f72 2069 2069  '+str(i) for i i
-00019350: 6e20 7261 6e67 6528 312c 6d61 785f 7468  n range(1,max_th
-00019360: 696e 6773 2b31 295d 0a20 2020 2020 2020  ings+1)].       
-00019370: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00019380: 2020 206e 6577 5f6e 616d 6573 5f6c 6973     new_names_lis
-00019390: 7420 3d20 5b6e 6577 5f6e 616d 6573 5f6c  t = [new_names_l
-000193a0: 6973 745d 0a20 2020 2023 2323 2046 6972  ist].    ### Fir
-000193b0: 7374 2066 696c 6c20 656d 7074 7920 7370  st fill empty sp
-000193c0: 6163 6573 206f 7220 4e61 4e73 2077 6974  aces or NaNs wit
-000193d0: 6820 6669 6c6c 6572 2023 2323 0a20 2020  h filler ###.   
-000193e0: 2064 662e 6c6f 635b 6466 5b66 6965 6c64   df.loc[df[field
-000193f0: 5d20 3d3d 2073 706c 6974 7465 722c 2066  ] == splitter, f
-00019400: 6965 6c64 5d20 3d20 6669 6c6c 6572 0a20  ield] = filler. 
-00019410: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00019420: 6528 6c65 6e28 6e65 775f 6e61 6d65 735f  e(len(new_names_
-00019430: 6c69 7374 2929 3a0a 2020 2020 2020 2020  list)):.        
-00019440: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00019450: 2064 665b 6e65 775f 6e61 6d65 735f 6c69   df[new_names_li
-00019460: 7374 5b69 5d5d 203d 2064 665b 6669 656c  st[i]] = df[fiel
-00019470: 645d 2e6d 6170 286c 616d 6264 6120 783a  d].map(lambda x:
-00019480: 2078 2e73 706c 6974 2873 706c 6974 7465   x.split(splitte
-00019490: 7229 5b69 5d0a 2020 2020 2020 2020 2020  r)[i].          
-000194a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194c0: 6966 2073 706c 6974 7465 7220 696e 2078  if splitter in x
-000194d0: 2065 6c73 6520 6669 6c6c 6572 290a 2020   else filler).  
-000194e0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-000194f0: 2020 2020 2020 2020 2020 6466 5b6e 6577            df[new
-00019500: 5f6e 616d 6573 5f6c 6973 745b 695d 5d20  _names_list[i]] 
-00019510: 3d20 6669 6c6c 6572 0a20 2020 2020 2020  = filler.       
-00019520: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00019530: 2020 2323 2320 7468 6572 6520 6973 2072    ### there is r
-00019540: 6561 6c6c 7920 6e6f 7468 696e 6720 796f  eally nothing yo
-00019550: 7520 6361 6e20 646f 2074 6f20 6669 6c6c  u can do to fill
-00019560: 2075 7020 7369 6e63 6520 7468 6579 2061   up since they a
-00019570: 7265 2066 696c 6c65 6420 7769 7468 2065  re filled with e
-00019580: 6d70 7479 2073 7472 696e 6773 2e0a 2020  mpty strings..  
-00019590: 2020 2323 2323 204c 6561 7665 2074 6869    #### Leave thi
-000195a0: 7320 6173 2069 7420 6973 2e20 4974 2069  s as it is. It i
-000195b0: 7320 6e6f 7420 736f 6d65 7468 696e 6720  s not something 
-000195c0: 796f 7520 6361 6e20 646f 2072 6967 6874  you can do right
-000195d0: 206e 6f77 2e20 4974 2077 6f72 6b73 2e0a   now. It works..
-000195e0: 2020 2020 6466 5b66 6965 6c64 5d20 3d20      df[field] = 
-000195f0: 6466 5f66 6965 6c64 0a20 2020 2072 6574  df_field.    ret
-00019600: 7572 6e20 6466 2c20 6e65 775f 6e61 6d65  urn df, new_name
-00019610: 735f 6c69 7374 0a23 2323 2323 2323 2323  s_list.#########
-00019620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018b60: 2323 2323 2323 2323 0a20 2020 2022 2222  ########.    """
+00018b70: 0a20 2020 2064 665f 6669 656c 6420 3d20  .    df_field = 
+00018b80: 6466 5f69 6e5b 6669 656c 645d 2e76 616c  df_in[field].val
+00018b90: 7565 730a 2020 2020 6466 203d 2063 6f70  ues.    df = cop
+00018ba0: 792e 6465 6570 636f 7079 2864 665f 696e  y.deepcopy(df_in
+00018bb0: 290a 2020 2020 2323 2320 4669 7273 7420  ).    ### First 
+00018bc0: 636f 7079 2020 7768 6174 6576 6572 2069  copy  whatever i
+00018bd0: 7320 696e 2074 6861 7420 6669 656c 6420  s in that field 
+00018be0: 736f 2077 6520 6361 6e20 7361 7665 2069  so we can save i
+00018bf0: 7420 666f 7220 6c61 7465 7220 2323 230a  t for later ###.
+00018c00: 2020 2020 2323 2320 5265 6d65 6d62 6572      ### Remember
+00018c10: 2074 6861 7420 6669 6c6c 6e61 206f 6e6c   that fillna onl
+00018c20: 7920 776f 726b 7320 6174 2064 6174 6166  y works at dataf
+00018c30: 7261 6d65 206c 6576 656c 2120 2323 230a  rame level! ###.
+00018c40: 2020 2020 6466 5b5b 6669 656c 645d 5d20      df[[field]] 
+00018c50: 3d20 6466 5b5b 6669 656c 645d 5d2e 6669  = df[[field]].fi
+00018c60: 6c6c 6e61 2866 696c 6c65 7229 0a20 2020  llna(filler).   
+00018c70: 2069 6620 6164 645f 636f 756e 745f 6669   if add_count_fi
+00018c80: 656c 643a 0a20 2020 2020 2020 2023 2323  eld:.        ###
+00018c90: 2074 6865 7265 2077 696c 6c20 6265 206f   there will be o
+00018ca0: 6e65 2065 7874 7261 2066 6965 6c64 2063  ne extra field c
+00018cb0: 7265 6174 6564 2077 6865 6e20 7765 2063  reated when we c
+00018cc0: 6f75 6e74 2074 6865 206e 756d 6265 7220  ount the number 
+00018cd0: 6f66 2063 6f6e 7465 6e74 7320 696e 2065  of contents in e
+00018ce0: 6163 6820 6669 656c 6420 2323 230a 2020  ach field ###.  
+00018cf0: 2020 2020 2020 6d61 785f 7468 696e 6773        max_things
+00018d00: 203d 2064 665b 6669 656c 645d 2e6d 6170   = df[field].map
+00018d10: 286c 616d 6264 6120 783a 206c 656e 2878  (lambda x: len(x
+00018d20: 2e73 706c 6974 2873 706c 6974 7465 7229  .split(splitter)
+00018d30: 2929 2e6d 6178 2829 202b 2031 0a20 2020  )).max() + 1.   
+00018d40: 2065 6c73 653a 0a20 2020 2020 2020 206d   else:.        m
+00018d50: 6178 5f74 6869 6e67 7320 3d20 6466 5b66  ax_things = df[f
+00018d60: 6965 6c64 5d2e 6d61 7028 6c61 6d62 6461  ield].map(lambda
+00018d70: 2078 3a20 6c65 6e28 782e 7370 6c69 7428   x: len(x.split(
+00018d80: 7370 6c69 7474 6572 2929 292e 6d61 7828  splitter))).max(
+00018d90: 290a 2020 2020 6966 206c 656e 286e 6577  ).    if len(new
+00018da0: 5f6e 616d 6573 5f6c 6973 7429 203d 3d20  _names_list) == 
+00018db0: 303a 0a20 2020 2020 2020 2070 7269 6e74  0:.        print
+00018dc0: 2827 2020 2020 4d61 782e 2063 6f6c 756d  ('    Max. colum
+00018dd0: 6e73 2063 7265 6174 6564 2062 7920 7370  ns created by sp
+00018de0: 6c69 7474 696e 6720 2573 2066 6965 6c64  litting %s field
+00018df0: 2069 7320 2564 2e27 2025 280a 2020 2020   is %d.' %(.    
+00018e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e10: 2020 2020 2020 2020 6669 656c 642c 6d61          field,ma
+00018e20: 785f 7468 696e 6773 2929 0a20 2020 2065  x_things)).    e
+00018e30: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
+00018e40: 6e6f 7420 6d61 785f 7468 696e 6773 203d  not max_things =
+00018e50: 3d20 6c65 6e28 6e65 775f 6e61 6d65 735f  = len(new_names_
+00018e60: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
+00018e70: 2020 2070 7269 6e74 2822 2222 2020 2020     print("""    
+00018e80: 4d61 782e 2063 6f6c 756d 6e73 2063 7265  Max. columns cre
+00018e90: 6174 6564 2062 7920 7370 6c69 7474 696e  ated by splittin
+00018ea0: 6720 2573 2066 6965 6c64 2069 7320 2564  g %s field is %d
+00018eb0: 2062 7574 2079 6f75 2068 6176 6520 6769   but you have gi
+00018ec0: 7665 6e20 2564 0a20 2020 2020 2020 2020  ven %d.         
+00018ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ee0: 2020 2076 6172 6961 626c 6520 6e61 6d65     variable name
+00018ef0: 7320 6f6e 6c79 2e20 5365 6c65 6374 696e  s only. Selectin
+00018f00: 6720 6669 7273 7420 2564 2222 2220 2528  g first %d""" %(
+00018f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018f20: 2020 2020 2020 2020 2066 6965 6c64 2c6d           field,m
+00018f30: 6178 5f74 6869 6e67 732c 6c65 6e28 6e65  ax_things,len(ne
+00018f40: 775f 6e61 6d65 735f 6c69 7374 292c 6c65  w_names_list),le
+00018f50: 6e28 6e65 775f 6e61 6d65 735f 6c69 7374  n(new_names_list
+00018f60: 2929 290a 2020 2020 2323 2320 5468 6973  ))).    ### This
+00018f70: 2063 7265 6174 6573 2061 206e 6577 2066   creates a new f
+00018f80: 6965 6c64 2074 6861 7420 636f 756e 7473  ield that counts
+00018f90: 2074 6865 206e 756d 6265 7220 6f66 2074   the number of t
+00018fa0: 6869 6e67 7320 7468 6174 2061 7265 2069  hings that are i
+00018fb0: 6e20 7468 6174 2066 6965 6c64 2e0a 2020  n that field..  
+00018fc0: 2020 6966 2061 6464 5f63 6f75 6e74 5f66    if add_count_f
+00018fd0: 6965 6c64 3a0a 2020 2020 2020 2020 2323  ield:.        ##
+00018fe0: 2323 2074 6869 7320 636f 756e 7473 2074  ## this counts t
+00018ff0: 6865 206e 756d 6265 7220 6f66 2063 6f6e  he number of con
+00019000: 7465 6e74 7320 6166 7465 7220 7370 6c69  tents after spli
+00019010: 7474 696e 6720 6561 6368 2072 6f77 2077  tting each row w
+00019020: 6869 6368 2076 6172 6965 732e 2048 656e  hich varies. Hen
+00019030: 6365 2069 7420 6865 6c70 732e 0a20 2020  ce it helps..   
+00019040: 2020 2020 206e 756d 5f70 726f 6475 6374       num_product
+00019050: 735f 7669 6577 6564 203d 2027 436f 6e74  s_viewed = 'Cont
+00019060: 656e 745f 436f 756e 745f 696e 5f27 2b66  ent_Count_in_'+f
+00019070: 6965 6c64 0a20 2020 2020 2020 2064 665b  ield.        df[
+00019080: 6e75 6d5f 7072 6f64 7563 7473 5f76 6965  num_products_vie
+00019090: 7765 645d 203d 2064 665b 6669 656c 645d  wed] = df[field]
+000190a0: 2e6d 6170 286c 616d 6264 6120 783a 206c  .map(lambda x: l
+000190b0: 656e 2878 2e73 706c 6974 2873 706c 6974  en(x.split(split
+000190c0: 7465 7229 2929 2e76 616c 7565 730a 2020  ter))).values.  
+000190d0: 2020 2323 2320 436c 6561 6e20 7570 2074    ### Clean up t
+000190e0: 6865 2066 6965 6c64 2073 7563 6820 7468  he field such th
+000190f0: 6174 2069 7420 6861 7320 7468 6520 7269  at it has the ri
+00019100: 6768 7420 6e75 6d62 6572 206f 6620 7370  ght number of sp
+00019110: 6c69 7420 6368 6172 7320 6f74 6865 7277  lit chars otherw
+00019120: 6973 6520 6164 6420 746f 2069 740a 2020  ise add to it.  
+00019130: 2020 2323 2320 5468 6973 2066 696c 6c73    ### This fills
+00019140: 2075 7020 7468 6520 6669 656c 6420 7769   up the field wi
+00019150: 7468 2065 6d70 7479 2073 7472 696e 6773  th empty strings
+00019160: 2062 6574 7765 656e 2065 6163 6820 7370   between each sp
+00019170: 6c69 7474 6572 2e20 596f 7520 6361 6e27  litter. You can'
+00019180: 7420 646f 206d 7563 6820 6162 6f75 7420  t do much about 
+00019190: 6974 2e0a 2020 2020 2323 2323 204c 6561  it..    #### Lea
+000191a0: 7665 2074 6869 7320 6173 2069 7420 6973  ve this as it is
+000191b0: 2e20 4974 2069 7320 6e6f 7420 736f 6d65  . It is not some
+000191c0: 7468 696e 6720 796f 7520 6361 6e20 646f  thing you can do
+000191d0: 2072 6967 6874 206e 6f77 2e20 4974 2077   right now. It w
+000191e0: 6f72 6b73 2e0a 2020 2020 6669 6c6c 5f73  orks..    fill_s
+000191f0: 7472 696e 6720 3d20 7370 6c69 7474 6572  tring = splitter
+00019200: 202b 2066 696c 6c65 720a 2020 2020 6466   + filler.    df
+00019210: 5b66 6965 6c64 5d20 3d20 6466 5b66 6965  [field] = df[fie
+00019220: 6c64 5d2e 6d61 7028 6c61 6d62 6461 2078  ld].map(lambda x
+00019230: 3a20 782b 6669 6c6c 5f73 7472 696e 672a  : x+fill_string*
+00019240: 286d 6178 5f74 6869 6e67 732d 6c65 6e28  (max_things-len(
+00019250: 782e 7370 6c69 7428 7370 6c69 7474 6572  x.split(splitter
+00019260: 2929 2920 6966 206c 656e 280a 2020 2020  ))) if len(.    
+00019270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019290: 782e 7370 6c69 7428 7370 6c69 7474 6572  x.split(splitter
+000192a0: 2929 203c 206d 6178 5f74 6869 6e67 7320  )) < max_things 
+000192b0: 656c 7365 2078 290a 2020 2020 2323 2323  else x).    ####
+000192c0: 2323 204e 6f77 2079 6f75 2063 7265 6174  ## Now you creat
+000192d0: 6520 6e65 7720 6669 656c 6473 2062 7920  e new fields by 
+000192e0: 7370 6c69 7420 7468 6520 6f6e 6520 6c61  split the one la
+000192f0: 7267 6520 6669 656c 6420 2323 2323 2323  rge field ######
+00019300: 2323 0a20 2020 2069 6620 6973 696e 7374  ##.    if isinst
+00019310: 616e 6365 286e 6577 5f6e 616d 6573 5f6c  ance(new_names_l
+00019320: 6973 742c 2073 7472 293a 0a20 2020 2020  ist, str):.     
+00019330: 2020 2069 6620 6e65 775f 6e61 6d65 735f     if new_names_
+00019340: 6c69 7374 203d 3d20 2727 3a0a 2020 2020  list == '':.    
+00019350: 2020 2020 2020 2020 6e65 775f 6e61 6d65          new_name
+00019360: 735f 6c69 7374 203d 205b 6669 656c 642b  s_list = [field+
+00019370: 275f 272b 7374 7228 6929 2066 6f72 2069  '_'+str(i) for i
+00019380: 2069 6e20 7261 6e67 6528 312c 6d61 785f   in range(1,max_
+00019390: 7468 696e 6773 2b31 295d 0a20 2020 2020  things+1)].     
+000193a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000193b0: 2020 2020 206e 6577 5f6e 616d 6573 5f6c       new_names_l
+000193c0: 6973 7420 3d20 5b6e 6577 5f6e 616d 6573  ist = [new_names
+000193d0: 5f6c 6973 745d 0a20 2020 2023 2323 2046  _list].    ### F
+000193e0: 6972 7374 2066 696c 6c20 656d 7074 7920  irst fill empty 
+000193f0: 7370 6163 6573 206f 7220 4e61 4e73 2077  spaces or NaNs w
+00019400: 6974 6820 6669 6c6c 6572 2023 2323 0a20  ith filler ###. 
+00019410: 2020 2064 662e 6c6f 635b 6466 5b66 6965     df.loc[df[fie
+00019420: 6c64 5d20 3d3d 2073 706c 6974 7465 722c  ld] == splitter,
+00019430: 2066 6965 6c64 5d20 3d20 6669 6c6c 6572   field] = filler
+00019440: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+00019450: 6e67 6528 6c65 6e28 6e65 775f 6e61 6d65  nge(len(new_name
+00019460: 735f 6c69 7374 2929 3a0a 2020 2020 2020  s_list)):.      
+00019470: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00019480: 2020 2064 665b 6e65 775f 6e61 6d65 735f     df[new_names_
+00019490: 6c69 7374 5b69 5d5d 203d 2064 665b 6669  list[i]] = df[fi
+000194a0: 656c 645d 2e6d 6170 286c 616d 6264 6120  eld].map(lambda 
+000194b0: 783a 2078 2e73 706c 6974 2873 706c 6974  x: x.split(split
+000194c0: 7465 7229 5b69 5d0a 2020 2020 2020 2020  ter)[i].        
+000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194f0: 2020 6966 2073 706c 6974 7465 7220 696e    if splitter in
+00019500: 2078 2065 6c73 6520 6669 6c6c 6572 290a   x else filler).
+00019510: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+00019520: 2020 2020 2020 2020 2020 2020 6466 5b6e              df[n
+00019530: 6577 5f6e 616d 6573 5f6c 6973 745b 695d  ew_names_list[i]
+00019540: 5d20 3d20 6669 6c6c 6572 0a20 2020 2020  ] = filler.     
+00019550: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00019560: 2020 2020 2323 2320 7468 6572 6520 6973      ### there is
+00019570: 2072 6561 6c6c 7920 6e6f 7468 696e 6720   really nothing 
+00019580: 796f 7520 6361 6e20 646f 2074 6f20 6669  you can do to fi
+00019590: 6c6c 2075 7020 7369 6e63 6520 7468 6579  ll up since they
+000195a0: 2061 7265 2066 696c 6c65 6420 7769 7468   are filled with
+000195b0: 2065 6d70 7479 2073 7472 696e 6773 2e0a   empty strings..
+000195c0: 2020 2020 2323 2323 204c 6561 7665 2074      #### Leave t
+000195d0: 6869 7320 6173 2069 7420 6973 2e20 4974  his as it is. It
+000195e0: 2069 7320 6e6f 7420 736f 6d65 7468 696e   is not somethin
+000195f0: 6720 796f 7520 6361 6e20 646f 2072 6967  g you can do rig
+00019600: 6874 206e 6f77 2e20 4974 2077 6f72 6b73  ht now. It works
+00019610: 2e0a 2020 2020 6466 5b66 6965 6c64 5d20  ..    df[field] 
+00019620: 3d20 6466 5f66 6965 6c64 0a20 2020 2072  = df_field.    r
+00019630: 6574 7572 6e20 6466 2c20 6e65 775f 6e61  eturn df, new_na
+00019640: 6d65 735f 6c69 7374 0a23 2323 2323 2323  mes_list.#######
 00019650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019660: 2323 0a64 6566 2046 455f 6164 645f 6772  ##.def FE_add_gr
-00019670: 6f75 7062 795f 6665 6174 7572 6573 5f61  oupby_features_a
-00019680: 6767 7265 6761 7465 645f 746f 5f64 6174  ggregated_to_dat
-00019690: 6166 7261 6d65 2874 7261 696e 2c0a 2020  aframe(train,.  
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 6167 675f 7479 7065 732c 2020 6772    agg_types,  gr
-000196c0: 6f75 7062 795f 636f 6c75 6d6e 732c 2069  oupby_columns, i
-000196d0: 676e 6f72 655f 7661 7269 6162 6c65 732c  gnore_variables,
-000196e0: 2074 6573 743d 2222 293a 0a20 2020 2022   test=""):.    "
-000196f0: 2222 0a20 2020 2046 4520 7374 616e 6473  "".    FE stands
-00019700: 2066 6f72 2046 6561 7475 7265 2045 6e67   for Feature Eng
-00019710: 696e 6565 7269 6e67 2e20 5468 6973 2066  ineering. This f
-00019720: 756e 6374 696f 6e20 7065 7266 6f72 6d73  unction performs
-00019730: 2066 6561 7475 7265 2065 6e67 696e 6565   feature enginee
-00019740: 7269 6e67 206f 6e20 6461 7461 2e0a 2020  ring on data..  
-00019750: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-00019760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019690: 2323 2323 0a64 6566 2046 455f 6164 645f  ####.def FE_add_
+000196a0: 6772 6f75 7062 795f 6665 6174 7572 6573  groupby_features
+000196b0: 5f61 6767 7265 6761 7465 645f 746f 5f64  _aggregated_to_d
+000196c0: 6174 6166 7261 6d65 2874 7261 696e 2c0a  ataframe(train,.
+000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196e0: 2020 2020 6167 675f 7479 7065 732c 2020      agg_types,  
+000196f0: 6772 6f75 7062 795f 636f 6c75 6d6e 732c  groupby_columns,
+00019700: 2069 676e 6f72 655f 7661 7269 6162 6c65   ignore_variable
+00019710: 732c 2074 6573 743d 2222 293a 0a20 2020  s, test=""):.   
+00019720: 2022 2222 0a20 2020 2046 4520 7374 616e   """.    FE stan
+00019730: 6473 2066 6f72 2046 6561 7475 7265 2045  ds for Feature E
+00019740: 6e67 696e 6565 7269 6e67 2e20 5468 6973  ngineering. This
+00019750: 2066 756e 6374 696f 6e20 7065 7266 6f72   function perfor
+00019760: 6d73 2066 6561 7475 7265 2065 6e67 696e  ms feature engin
+00019770: 6565 7269 6e67 206f 6e20 6461 7461 2e0a  eering on data..
+00019780: 2020 2020 2323 2323 2323 2323 2323 2323      ############
 00019790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000197a0: 2323 2323 2323 2323 0a20 2020 2023 2323  ########.    ###
-000197b0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
-000197c0: 2069 7320 6120 7665 7279 2066 6173 7420   is a very fast 
-000197d0: 6675 6e63 7469 6f6e 2074 6861 7420 7769  function that wi
-000197e0: 6c6c 2063 6f6d 7075 7465 2061 6767 7265  ll compute aggre
-000197f0: 6761 7465 7320 666f 7220 6e75 6d65 7269  gates for numeri
-00019800: 6373 0a20 2020 2023 2323 2020 2049 7420  cs.    ###   It 
-00019810: 7265 7475 726e 7320 6f72 6967 696e 616c  returns original
-00019820: 2064 6174 6166 7261 6d65 2077 6974 6820   dataframe with 
-00019830: 6164 6465 6420 6665 6174 7572 6573 2066  added features f
-00019840: 726f 6d20 6e75 6d65 7269 6320 7661 7269  rom numeric vari
-00019850: 6162 6c65 7320 6167 6772 6567 6174 6564  ables aggregated
-00019860: 0a20 2020 2023 2323 2020 2057 6861 7420  .    ###   What 
-00019870: 646f 2079 6f75 206d 6561 6e20 6167 6772  do you mean aggr
-00019880: 6567 6174 653f 2061 6767 7265 6761 7465  egate? aggregate
-00019890: 7320 6361 6e20 6265 2022 636f 756e 742c  s can be "count,
-000198a0: 2022 6d65 616e 222c 2022 6d65 6469 616e   "mean", "median
-000198b0: 222c 2065 7463 2e0a 2020 2020 2323 2320  ", etc..    ### 
-000198c0: 2020 5768 6174 2064 6f20 796f 7520 6167    What do you ag
-000198d0: 6772 6567 7261 7465 3f20 616c 6c20 6e75  gregrate? all nu
-000198e0: 6d65 7269 6320 636f 6c75 6d6e 7320 696e  meric columns in
-000198f0: 2079 6f75 7220 6461 7461 0a20 2020 2023   your data.    #
-00019900: 2323 2020 2057 6861 7420 646f 2079 6f75  ##   What do you
-00019910: 2067 726f 7570 6279 3f20 6f6e 6520 6772   groupby? one gr
-00019920: 6f75 7062 7920 636f 6c75 6d6e 2061 7420  oupby column at 
-00019930: 6120 7469 6d65 206f 7220 6d75 6c74 6970  a time or multip
-00019940: 6c65 2063 6f6c 756d 6e73 206f 6e65 2062  le columns one b
-00019950: 7920 6f6e 650a 2020 2020 2323 2320 2020  y one.    ###   
-00019960: 2020 2d2d 2069 6620 796f 7520 6769 7665    -- if you give
-00019970: 2069 7420 6120 6c69 7374 206f 6620 636f   it a list of co
-00019980: 6c75 6d6e 732c 2069 7420 7769 6c6c 2065  lumns, it will e
-00019990: 7865 6375 7465 2074 6865 2067 726f 7570  xecute the group
-000199a0: 696e 6720 6f6e 6520 6279 206f 6e65 0a20  ing one by one. 
-000199b0: 2020 2023 2323 2020 2057 6861 7420 6973     ###   What is
-000199c0: 2074 6865 2069 676e 6f72 655f 7661 7269   the ignore_vari
-000199d0: 6162 6c65 7320 666f 723f 2069 7420 7769  ables for? it wi
-000199e0: 6c6c 2069 676e 6f72 6520 7468 6573 6520  ll ignore these 
-000199f0: 7661 7269 6162 6c65 7320 6672 6f6d 2067  variables from g
-00019a00: 726f 7570 696e 672e 0a20 2020 2023 2323  rouping..    ###
-00019a10: 2020 204d 616b 6520 7375 7265 2074 6f20     Make sure to 
-00019a20: 7265 6475 6365 2063 6f72 7265 6c61 7465  reduce correlate
-00019a30: 6420 6665 6174 7572 6573 2075 7369 6e67  d features using
-00019a40: 2046 455f 7265 6d6f 7665 5f76 6172 6961   FE_remove_varia
-00019a50: 626c 6573 5f75 7369 6e67 5f53 554c 4f56  bles_using_SULOV
-00019a60: 5f6d 6574 686f 6428 290a 2020 2020 2323  _method().    ##
-00019a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019a80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000197a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000197b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000197c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000197d0: 2323 2323 2323 2323 2323 0a20 2020 2023  ##########.    #
+000197e0: 2323 2020 2054 6869 7320 6675 6e63 7469  ##   This functi
+000197f0: 6f6e 2069 7320 6120 7665 7279 2066 6173  on is a very fas
+00019800: 7420 6675 6e63 7469 6f6e 2074 6861 7420  t function that 
+00019810: 7769 6c6c 2063 6f6d 7075 7465 2061 6767  will compute agg
+00019820: 7265 6761 7465 7320 666f 7220 6e75 6d65  regates for nume
+00019830: 7269 6373 0a20 2020 2023 2323 2020 2049  rics.    ###   I
+00019840: 7420 7265 7475 726e 7320 6f72 6967 696e  t returns origin
+00019850: 616c 2064 6174 6166 7261 6d65 2077 6974  al dataframe wit
+00019860: 6820 6164 6465 6420 6665 6174 7572 6573  h added features
+00019870: 2066 726f 6d20 6e75 6d65 7269 6320 7661   from numeric va
+00019880: 7269 6162 6c65 7320 6167 6772 6567 6174  riables aggregat
+00019890: 6564 0a20 2020 2023 2323 2020 2057 6861  ed.    ###   Wha
+000198a0: 7420 646f 2079 6f75 206d 6561 6e20 6167  t do you mean ag
+000198b0: 6772 6567 6174 653f 2061 6767 7265 6761  gregate? aggrega
+000198c0: 7465 7320 6361 6e20 6265 2022 636f 756e  tes can be "coun
+000198d0: 742c 2022 6d65 616e 222c 2022 6d65 6469  t, "mean", "medi
+000198e0: 616e 222c 2065 7463 2e0a 2020 2020 2323  an", etc..    ##
+000198f0: 2320 2020 5768 6174 2064 6f20 796f 7520  #   What do you 
+00019900: 6167 6772 6567 7261 7465 3f20 616c 6c20  aggregrate? all 
+00019910: 6e75 6d65 7269 6320 636f 6c75 6d6e 7320  numeric columns 
+00019920: 696e 2079 6f75 7220 6461 7461 0a20 2020  in your data.   
+00019930: 2023 2323 2020 2057 6861 7420 646f 2079   ###   What do y
+00019940: 6f75 2067 726f 7570 6279 3f20 6f6e 6520  ou groupby? one 
+00019950: 6772 6f75 7062 7920 636f 6c75 6d6e 2061  groupby column a
+00019960: 7420 6120 7469 6d65 206f 7220 6d75 6c74  t a time or mult
+00019970: 6970 6c65 2063 6f6c 756d 6e73 206f 6e65  iple columns one
+00019980: 2062 7920 6f6e 650a 2020 2020 2323 2320   by one.    ### 
+00019990: 2020 2020 2d2d 2069 6620 796f 7520 6769      -- if you gi
+000199a0: 7665 2069 7420 6120 6c69 7374 206f 6620  ve it a list of 
+000199b0: 636f 6c75 6d6e 732c 2069 7420 7769 6c6c  columns, it will
+000199c0: 2065 7865 6375 7465 2074 6865 2067 726f   execute the gro
+000199d0: 7570 696e 6720 6f6e 6520 6279 206f 6e65  uping one by one
+000199e0: 0a20 2020 2023 2323 2020 2057 6861 7420  .    ###   What 
+000199f0: 6973 2074 6865 2069 676e 6f72 655f 7661  is the ignore_va
+00019a00: 7269 6162 6c65 7320 666f 723f 2069 7420  riables for? it 
+00019a10: 7769 6c6c 2069 676e 6f72 6520 7468 6573  will ignore thes
+00019a20: 6520 7661 7269 6162 6c65 7320 6672 6f6d  e variables from
+00019a30: 2067 726f 7570 696e 672e 0a20 2020 2023   grouping..    #
+00019a40: 2323 2020 204d 616b 6520 7375 7265 2074  ##   Make sure t
+00019a50: 6f20 7265 6475 6365 2063 6f72 7265 6c61  o reduce correla
+00019a60: 7465 6420 6665 6174 7572 6573 2075 7369  ted features usi
+00019a70: 6e67 2046 455f 7265 6d6f 7665 5f76 6172  ng FE_remove_var
+00019a80: 6961 626c 6573 5f75 7369 6e67 5f53 554c  iables_using_SUL
+00019a90: 4f56 5f6d 6574 686f 6428 290a 2020 2020  OV_method().    
 00019aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00019ab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019ac0: 2323 2323 0a20 2020 2023 2323 2049 6e70  ####.    ### Inp
-00019ad0: 7574 733a 0a20 2020 2023 2323 2020 2074  uts:.    ###   t
-00019ae0: 7261 696e 3a20 4a75 7374 2073 656e 7420  rain: Just sent 
-00019af0: 696e 2074 6865 2064 6174 6120 6672 616d  in the data fram
-00019b00: 6520 7768 6572 6520 796f 7520 7761 6e74  e where you want
-00019b10: 2061 6767 7265 6761 7465 6420 6665 6174   aggregated feat
-00019b20: 7572 6573 2066 6f72 2e0a 2020 2020 2323  ures for..    ##
-00019b30: 2320 2020 6167 675f 7479 7065 733a 206c  #   agg_types: l
-00019b40: 6973 7420 6f66 2063 6f6d 7075 7461 7469  ist of computati
-00019b50: 6f6e 616c 2074 7970 6573 3a20 276d 6561  onal types: 'mea
-00019b60: 6e27 2c27 6d65 6469 616e 272c 2763 6f75  n','median','cou
-00019b70: 6e74 272c 200a 2020 2020 2323 2320 2020  nt', .    ###   
-00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b90: 2020 276d 6178 272c 2027 6d69 6e27 2c20    'max', 'min', 
-00019ba0: 2773 756d 272c 2065 7463 2e0a 2020 2020  'sum', etc..    
-00019bb0: 2323 2320 2020 2020 2020 2020 4f6e 6520  ###         One 
-00019bc0: 6361 7665 6174 3a20 7468 6573 6520 6167  caveat: these ag
-00019bd0: 675f 7479 7065 7320 6d75 7374 2062 6520  g_types must be 
-00019be0: 666f 756e 6420 696e 2074 6865 2066 6f6c  found in the fol
-00019bf0: 6c6f 7769 6e67 2061 6767 5f66 756e 6320  lowing agg_func 
-00019c00: 6f66 200a 2020 2020 2323 2320 2020 2020  of .    ###     
-00019c10: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00019c20: 6d70 7920 6f72 2070 616e 6461 7320 6772  mpy or pandas gr
-00019c30: 6f75 7062 7920 7374 6174 656d 656e 742e  oupby statement.
-00019c40: 0a20 2020 2023 2323 2020 2020 2020 2020  .    ###        
-00019c50: 204c 6973 7420 6f66 2061 6767 7265 6761   List of aggrega
-00019c60: 7465 7320 6176 6169 6c61 626c 653a 207b  tes available: {
-00019c70: 2763 6f75 6e74 272c 2773 756d 272c 276d  'count','sum','m
-00019c80: 6561 6e27 2c27 6d61 6427 2c27 6d65 6469  ean','mad','medi
-00019c90: 616e 272c 276d 696e 272c 276d 6178 272c  an','min','max',
-00019ca0: 0a20 2020 2023 2323 2020 2020 2020 2020  .    ###        
-00019cb0: 2020 2020 2020 2027 6d6f 6465 272c 2761         'mode','a
-00019cc0: 6273 272c 2027 7072 6f64 272c 2773 7464  bs', 'prod','std
-00019cd0: 272c 2776 6172 272c 2773 656d 272c 2773  ','var','sem','s
-00019ce0: 6b65 7727 2c27 6b75 7274 272c 0a20 2020  kew','kurt',.   
-00019cf0: 2023 2323 2020 2020 2020 2020 2020 2020   ###            
-00019d00: 2020 2020 2771 7561 6e74 696c 6527 2c27      'quantile','
-00019d10: 6375 6d73 756d 272c 2763 756d 7072 6f64  cumsum','cumprod
-00019d20: 272c 2763 756d 6d61 7827 2c27 6375 6d6d  ','cummax','cumm
-00019d30: 696e 277d 0a20 2020 2023 2323 2020 2067  in'}.    ###   g
-00019d40: 726f 7570 6279 5f63 6f6c 756d 6e73 3a20  roupby_columns: 
-00019d50: 6361 6e20 6265 2061 2073 7472 696e 6720  can be a string 
-00019d60: 7265 7072 6573 656e 7469 6e67 2061 2073  representing a s
-00019d70: 696e 676c 6520 636f 6c75 6d6e 206f 7220  ingle column or 
-00019d80: 6120 6c69 7374 206f 6620 0a20 2020 2023  a list of .    #
-00019d90: 2323 2020 2020 2020 2020 2020 2020 2020  ##              
-00019da0: 2020 2020 2020 206d 756c 7469 706c 6520         multiple 
-00019db0: 636f 6c75 6d6e 730a 2020 2020 2323 2320  columns.    ### 
-00019dc0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00019dd0: 6974 2077 696c 6c20 6772 6f75 7062 7920  it will groupby 
-00019de0: 616c 6c20 7468 6520 6e75 6d65 7269 6320  all the numeric 
-00019df0: 6665 6174 7572 6573 2075 7369 6e67 206f  features using o
-00019e00: 6e65 2067 726f 7570 6279 2063 6f6c 756d  ne groupby colum
-00019e10: 6e20 0a20 2020 2023 2323 2020 2020 2020  n .    ###      
-00019e20: 2020 2020 2020 2020 2020 2020 2020 6174                at
-00019e30: 2061 2074 696d 6520 696e 2061 206c 6f6f   a time in a loo
-00019e40: 702e 0a20 2020 2023 2323 2020 2069 676e  p..    ###   ign
-00019e50: 6f72 655f 7661 7269 6162 6c65 733a 206c  ore_variables: l
-00019e60: 6973 7420 6f66 2076 6172 6961 626c 6573  ist of variables
-00019e70: 2074 6f20 6967 6e6f 7265 2061 6d6f 6e67   to ignore among
-00019e80: 206e 756d 6572 6963 2076 6172 6961 626c   numeric variabl
-00019e90: 6573 2069 6e0a 2020 2020 2323 2320 2020  es in.    ###   
-00019ea0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00019eb0: 6120 7369 6e63 6520 7468 6579 206d 6179  a since they may
-00019ec0: 2062 6520 4944 2076 6172 6961 626c 6573   be ID variables
-00019ed0: 2e0a 2020 2020 2323 2320 4f75 7470 7574  ..    ### Output
-00019ee0: 733a 0a20 2020 2023 2323 2020 2020 2052  s:.    ###     R
-00019ef0: 6574 7572 6e73 2074 6865 206f 7269 6769  eturns the origi
-00019f00: 6e61 6c20 6461 7461 6672 616d 6520 7769  nal dataframe wi
-00019f10: 7468 2061 6464 6974 696f 6e61 6c20 6665  th additional fe
-00019f20: 6174 7572 6573 2063 7265 6174 6564 2062  atures created b
-00019f30: 7920 7468 6973 2066 756e 6374 696f 6e2e  y this function.
-00019f40: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00019f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019f70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019af0: 2323 2323 2323 0a20 2020 2023 2323 2049  ######.    ### I
+00019b00: 6e70 7574 733a 0a20 2020 2023 2323 2020  nputs:.    ###  
+00019b10: 2074 7261 696e 3a20 4a75 7374 2073 656e   train: Just sen
+00019b20: 7420 696e 2074 6865 2064 6174 6120 6672  t in the data fr
+00019b30: 616d 6520 7768 6572 6520 796f 7520 7761  ame where you wa
+00019b40: 6e74 2061 6767 7265 6761 7465 6420 6665  nt aggregated fe
+00019b50: 6174 7572 6573 2066 6f72 2e0a 2020 2020  atures for..    
+00019b60: 2323 2320 2020 6167 675f 7479 7065 733a  ###   agg_types:
+00019b70: 206c 6973 7420 6f66 2063 6f6d 7075 7461   list of computa
+00019b80: 7469 6f6e 616c 2074 7970 6573 3a20 276d  tional types: 'm
+00019b90: 6561 6e27 2c27 6d65 6469 616e 272c 2763  ean','median','c
+00019ba0: 6f75 6e74 272c 200a 2020 2020 2323 2320  ount', .    ### 
+00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bc0: 2020 2020 276d 6178 272c 2027 6d69 6e27      'max', 'min'
+00019bd0: 2c20 2773 756d 272c 2065 7463 2e0a 2020  , 'sum', etc..  
+00019be0: 2020 2323 2320 2020 2020 2020 2020 4f6e    ###         On
+00019bf0: 6520 6361 7665 6174 3a20 7468 6573 6520  e caveat: these 
+00019c00: 6167 675f 7479 7065 7320 6d75 7374 2062  agg_types must b
+00019c10: 6520 666f 756e 6420 696e 2074 6865 2066  e found in the f
+00019c20: 6f6c 6c6f 7769 6e67 2061 6767 5f66 756e  ollowing agg_fun
+00019c30: 6320 6f66 200a 2020 2020 2323 2320 2020  c of .    ###   
+00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c50: 6e75 6d70 7920 6f72 2070 616e 6461 7320  numpy or pandas 
+00019c60: 6772 6f75 7062 7920 7374 6174 656d 656e  groupby statemen
+00019c70: 742e 0a20 2020 2023 2323 2020 2020 2020  t..    ###      
+00019c80: 2020 204c 6973 7420 6f66 2061 6767 7265     List of aggre
+00019c90: 6761 7465 7320 6176 6169 6c61 626c 653a  gates available:
+00019ca0: 207b 2763 6f75 6e74 272c 2773 756d 272c   {'count','sum',
+00019cb0: 276d 6561 6e27 2c27 6d61 6427 2c27 6d65  'mean','mad','me
+00019cc0: 6469 616e 272c 276d 696e 272c 276d 6178  dian','min','max
+00019cd0: 272c 0a20 2020 2023 2323 2020 2020 2020  ',.    ###      
+00019ce0: 2020 2020 2020 2020 2027 6d6f 6465 272c           'mode',
+00019cf0: 2761 6273 272c 2027 7072 6f64 272c 2773  'abs', 'prod','s
+00019d00: 7464 272c 2776 6172 272c 2773 656d 272c  td','var','sem',
+00019d10: 2773 6b65 7727 2c27 6b75 7274 272c 0a20  'skew','kurt',. 
+00019d20: 2020 2023 2323 2020 2020 2020 2020 2020     ###          
+00019d30: 2020 2020 2020 2771 7561 6e74 696c 6527        'quantile'
+00019d40: 2c27 6375 6d73 756d 272c 2763 756d 7072  ,'cumsum','cumpr
+00019d50: 6f64 272c 2763 756d 6d61 7827 2c27 6375  od','cummax','cu
+00019d60: 6d6d 696e 277d 0a20 2020 2023 2323 2020  mmin'}.    ###  
+00019d70: 2067 726f 7570 6279 5f63 6f6c 756d 6e73   groupby_columns
+00019d80: 3a20 6361 6e20 6265 2061 2073 7472 696e  : can be a strin
+00019d90: 6720 7265 7072 6573 656e 7469 6e67 2061  g representing a
+00019da0: 2073 696e 676c 6520 636f 6c75 6d6e 206f   single column o
+00019db0: 7220 6120 6c69 7374 206f 6620 0a20 2020  r a list of .   
+00019dc0: 2023 2323 2020 2020 2020 2020 2020 2020   ###            
+00019dd0: 2020 2020 2020 2020 206d 756c 7469 706c           multipl
+00019de0: 6520 636f 6c75 6d6e 730a 2020 2020 2323  e columns.    ##
+00019df0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00019e00: 2d20 6974 2077 696c 6c20 6772 6f75 7062  - it will groupb
+00019e10: 7920 616c 6c20 7468 6520 6e75 6d65 7269  y all the numeri
+00019e20: 6320 6665 6174 7572 6573 2075 7369 6e67  c features using
+00019e30: 206f 6e65 2067 726f 7570 6279 2063 6f6c   one groupby col
+00019e40: 756d 6e20 0a20 2020 2023 2323 2020 2020  umn .    ###    
+00019e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e60: 6174 2061 2074 696d 6520 696e 2061 206c  at a time in a l
+00019e70: 6f6f 702e 0a20 2020 2023 2323 2020 2069  oop..    ###   i
+00019e80: 676e 6f72 655f 7661 7269 6162 6c65 733a  gnore_variables:
+00019e90: 206c 6973 7420 6f66 2076 6172 6961 626c   list of variabl
+00019ea0: 6573 2074 6f20 6967 6e6f 7265 2061 6d6f  es to ignore amo
+00019eb0: 6e67 206e 756d 6572 6963 2076 6172 6961  ng numeric varia
+00019ec0: 626c 6573 2069 6e0a 2020 2020 2323 2320  bles in.    ### 
+00019ed0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00019ee0: 6174 6120 7369 6e63 6520 7468 6579 206d  ata since they m
+00019ef0: 6179 2062 6520 4944 2076 6172 6961 626c  ay be ID variabl
+00019f00: 6573 2e0a 2020 2020 2323 2320 4f75 7470  es..    ### Outp
+00019f10: 7574 733a 0a20 2020 2023 2323 2020 2020  uts:.    ###    
+00019f20: 2052 6574 7572 6e73 2074 6865 206f 7269   Returns the ori
+00019f30: 6769 6e61 6c20 6461 7461 6672 616d 6520  ginal dataframe 
+00019f40: 7769 7468 2061 6464 6974 696f 6e61 6c20  with additional 
+00019f50: 6665 6174 7572 6573 2063 7265 6174 6564  features created
+00019f60: 2062 7920 7468 6973 2066 756e 6374 696f   by this functio
+00019f70: 6e2e 0a20 2020 2023 2323 2323 2323 2323  n..    #########
 00019f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00019f90: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
-00019fa0: 2222 220a 2020 2020 7472 6169 6e78 203d  """.    trainx =
-00019fb0: 2063 6f70 792e 6465 6570 636f 7079 2874   copy.deepcopy(t
-00019fc0: 7261 696e 290a 2020 2020 7465 7374 7820  rain).    testx 
-00019fd0: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
-00019fe0: 7465 7374 290a 2020 2020 6966 2069 7369  test).    if isi
-00019ff0: 6e73 7461 6e63 6528 6772 6f75 7062 795f  nstance(groupby_
-0001a000: 636f 6c75 6d6e 732c 2073 7472 293a 0a20  columns, str):. 
-0001a010: 2020 2020 2020 2067 726f 7570 6279 5f63         groupby_c
-0001a020: 6f6c 756d 6e73 203d 205b 6772 6f75 7062  olumns = [groupb
-0001a030: 795f 636f 6c75 6d6e 735d 0a20 2020 206e  y_columns].    n
-0001a040: 756d 6572 6963 7320 3d20 7472 6169 6e78  umerics = trainx
-0001a050: 2e73 656c 6563 745f 6474 7970 6573 2869  .select_dtypes(i
-0001a060: 6e63 6c75 6465 3d27 6e75 6d62 6572 2729  nclude='number')
-0001a070: 2e63 6f6c 756d 6e73 2e74 6f6c 6973 7428  .columns.tolist(
-0001a080: 290a 2020 2020 6e75 6d65 7269 6373 203d  ).    numerics =
-0001a090: 205b 7820 666f 7220 7820 696e 206e 756d   [x for x in num
-0001a0a0: 6572 6963 7320 6966 2078 206e 6f74 2069  erics if x not i
-0001a0b0: 6e20 6967 6e6f 7265 5f76 6172 6961 626c  n ignore_variabl
-0001a0c0: 6573 5d0a 2020 2020 4d47 4220 3d20 4772  es].    MGB = Gr
-0001a0d0: 6f75 7062 795f 4167 6772 6567 6174 6f72  oupby_Aggregator
-0001a0e0: 2863 6174 6567 6f72 6963 616c 733d 6772  (categoricals=gr
-0001a0f0: 6f75 7062 795f 636f 6c75 6d6e 732c 0a20  oupby_columns,. 
-0001a100: 2020 2020 2020 2020 2020 2061 6767 7265             aggre
-0001a110: 6761 7465 733d 6167 675f 7479 7065 732c  gates=agg_types,
-0001a120: 206e 756d 6572 6963 733d 6e75 6d65 7269   numerics=numeri
-0001a130: 6373 290a 2020 2020 7472 6169 6e5f 636f  cs).    train_co
-0001a140: 7079 203d 204d 4742 2e66 6974 5f74 7261  py = MGB.fit_tra
-0001a150: 6e73 666f 726d 2874 7261 696e 7829 0a20  nsform(trainx). 
-0001a160: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0001a170: 2874 6573 7478 2c20 7374 7229 206f 7220  (testx, str) or 
-0001a180: 7465 7374 7820 6973 204e 6f6e 653a 0a20  testx is None:. 
-0001a190: 2020 2020 2020 2074 6573 745f 636f 7079         test_copy
-0001a1a0: 203d 2074 6573 7478 0a20 2020 2065 6c73   = testx.    els
-0001a1b0: 653a 0a20 2020 2020 2020 2074 6573 745f  e:.        test_
-0001a1c0: 636f 7079 203d 204d 4742 2e74 7261 6e73  copy = MGB.trans
-0001a1d0: 666f 726d 2874 6573 7478 290a 2020 2020  form(testx).    
-0001a1e0: 2323 2320 7265 7475 726e 2074 6865 2064  ### return the d
-0001a1f0: 6174 6166 7261 6d65 7320 2323 2323 2323  ataframes ######
-0001a200: 2323 2323 230a 2020 2020 7265 7475 726e  #####.    return
-0001a210: 2074 7261 696e 5f63 6f70 792c 2074 6573   train_copy, tes
-0001a220: 745f 636f 7079 0a23 2323 2323 2323 2323  t_copy.#########
-0001a230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019f90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019fa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00019fc0: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
+00019fd0: 2020 2222 220a 2020 2020 7472 6169 6e78    """.    trainx
+00019fe0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+00019ff0: 2874 7261 696e 290a 2020 2020 7465 7374  (train).    test
+0001a000: 7820 3d20 636f 7079 2e64 6565 7063 6f70  x = copy.deepcop
+0001a010: 7928 7465 7374 290a 2020 2020 6966 2069  y(test).    if i
+0001a020: 7369 6e73 7461 6e63 6528 6772 6f75 7062  sinstance(groupb
+0001a030: 795f 636f 6c75 6d6e 732c 2073 7472 293a  y_columns, str):
+0001a040: 0a20 2020 2020 2020 2067 726f 7570 6279  .        groupby
+0001a050: 5f63 6f6c 756d 6e73 203d 205b 6772 6f75  _columns = [grou
+0001a060: 7062 795f 636f 6c75 6d6e 735d 0a20 2020  pby_columns].   
+0001a070: 206e 756d 6572 6963 7320 3d20 7472 6169   numerics = trai
+0001a080: 6e78 2e73 656c 6563 745f 6474 7970 6573  nx.select_dtypes
+0001a090: 2869 6e63 6c75 6465 3d27 6e75 6d62 6572  (include='number
+0001a0a0: 2729 2e63 6f6c 756d 6e73 2e74 6f6c 6973  ').columns.tolis
+0001a0b0: 7428 290a 2020 2020 6e75 6d65 7269 6373  t().    numerics
+0001a0c0: 203d 205b 7820 666f 7220 7820 696e 206e   = [x for x in n
+0001a0d0: 756d 6572 6963 7320 6966 2078 206e 6f74  umerics if x not
+0001a0e0: 2069 6e20 6967 6e6f 7265 5f76 6172 6961   in ignore_varia
+0001a0f0: 626c 6573 5d0a 2020 2020 4d47 4220 3d20  bles].    MGB = 
+0001a100: 4772 6f75 7062 795f 4167 6772 6567 6174  Groupby_Aggregat
+0001a110: 6f72 2863 6174 6567 6f72 6963 616c 733d  or(categoricals=
+0001a120: 6772 6f75 7062 795f 636f 6c75 6d6e 732c  groupby_columns,
+0001a130: 0a20 2020 2020 2020 2020 2020 2061 6767  .            agg
+0001a140: 7265 6761 7465 733d 6167 675f 7479 7065  regates=agg_type
+0001a150: 732c 206e 756d 6572 6963 733d 6e75 6d65  s, numerics=nume
+0001a160: 7269 6373 290a 2020 2020 7472 6169 6e5f  rics).    train_
+0001a170: 636f 7079 203d 204d 4742 2e66 6974 5f74  copy = MGB.fit_t
+0001a180: 7261 6e73 666f 726d 2874 7261 696e 7829  ransform(trainx)
+0001a190: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+0001a1a0: 6365 2874 6573 7478 2c20 7374 7229 206f  ce(testx, str) o
+0001a1b0: 7220 7465 7374 7820 6973 204e 6f6e 653a  r testx is None:
+0001a1c0: 0a20 2020 2020 2020 2074 6573 745f 636f  .        test_co
+0001a1d0: 7079 203d 2074 6573 7478 0a20 2020 2065  py = testx.    e
+0001a1e0: 6c73 653a 0a20 2020 2020 2020 2074 6573  lse:.        tes
+0001a1f0: 745f 636f 7079 203d 204d 4742 2e74 7261  t_copy = MGB.tra
+0001a200: 6e73 666f 726d 2874 6573 7478 290a 2020  nsform(testx).  
+0001a210: 2020 2323 2320 7265 7475 726e 2074 6865    ### return the
+0001a220: 2064 6174 6166 7261 6d65 7320 2323 2323   dataframes ####
+0001a230: 2323 2323 2323 230a 2020 2020 7265 7475  #######.    retu
+0001a240: 726e 2074 7261 696e 5f63 6f70 792c 2074  rn train_copy, t
+0001a250: 6573 745f 636f 7079 0a23 2323 2323 2323  est_copy.#######
 0001a260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001a270: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a280: 2323 2323 2323 2323 2323 2323 0a64 6566  ############.def
-0001a290: 2046 455f 636f 6d62 696e 655f 7261 7265   FE_combine_rare
-0001a2a0: 5f63 6174 6567 6f72 6965 7328 7472 6169  _categories(trai
-0001a2b0: 6e5f 6466 2c20 6361 7465 676f 7269 6361  n_df, categorica
-0001a2c0: 6c5f 6665 6174 7572 6573 2c20 7465 7374  l_features, test
-0001a2d0: 5f64 663d 2222 293a 0a20 2020 2022 2222  _df=""):.    """
-0001a2e0: 0a20 2020 2049 6e20 7468 6973 2066 756e  .    In this fun
-0001a2f0: 6374 696f 6e2c 2077 6520 7769 6c6c 2073  ction, we will s
-0001a300: 656c 6563 7420 616c 6c20 7261 7265 2063  elect all rare c
-0001a310: 6c61 7373 6573 2068 6176 696e 6720 7265  lasses having re
-0001a320: 7072 6573 656e 7461 7469 6f6e 203c 3125  presentation <1%
-0001a330: 206f 6620 706f 7075 6c61 7469 6f6e 2061   of population a
-0001a340: 6e64 0a20 2020 2067 726f 7570 2074 6865  nd.    group the
-0001a350: 6d20 746f 6765 7468 6572 2075 6e64 6572  m together under
-0001a360: 2061 206e 6577 206c 6162 656c 2063 616c   a new label cal
-0001a370: 6c65 6420 2752 4152 4527 2e20 5765 2077  led 'RARE'. We w
-0001a380: 696c 6c20 6170 706c 7920 7468 6973 206f  ill apply this o
-0001a390: 6e20 7472 6169 6e20 616e 6420 7465 7374  n train and test
-0001a3a0: 2028 6f70 7469 6f6e 616c 290a 2020 2020   (optional).    
-0001a3b0: 2222 220a 2020 2020 7472 6169 6e5f 6466  """.    train_df
-0001a3c0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-0001a3d0: 2874 7261 696e 5f64 6629 0a20 2020 2074  (train_df).    t
-0001a3e0: 6573 745f 6466 203d 2063 6f70 792e 6465  est_df = copy.de
-0001a3f0: 6570 636f 7079 2874 6573 745f 6466 290a  epcopy(test_df).
-0001a400: 2020 2020 7472 6169 6e5f 6466 5b63 6174      train_df[cat
-0001a410: 6567 6f72 6963 616c 5f66 6561 7475 7265  egorical_feature
-0001a420: 735d 203d 2074 7261 696e 5f64 665b 6361  s] = train_df[ca
-0001a430: 7465 676f 7269 6361 6c5f 6665 6174 7572  tegorical_featur
-0001a440: 6573 5d2e 6170 706c 7928 0a20 2020 2020  es].apply(.     
-0001a450: 2020 2020 2020 206c 616d 6264 6120 783a         lambda x:
-0001a460: 2078 2e6d 6173 6b28 782e 6d61 7028 782e   x.mask(x.map(x.
-0001a470: 7661 6c75 655f 636f 756e 7473 2829 293c  value_counts())<
-0001a480: 2028 302e 3031 2a74 7261 696e 5f64 662e   (0.01*train_df.
-0001a490: 7368 6170 655b 305d 292c 2027 5241 5245  shape[0]), 'RARE
-0001a4a0: 2729 290a 2020 2020 666f 7220 636f 6c20  ')).    for col 
-0001a4b0: 696e 2063 6174 6567 6f72 6963 616c 5f66  in categorical_f
-0001a4c0: 6561 7475 7265 733a 0a20 2020 2020 2020  eatures:.       
-0001a4d0: 2076 616c 7320 3d20 6c69 7374 2874 7261   vals = list(tra
-0001a4e0: 696e 5f64 665b 636f 6c5d 2e75 6e69 7175  in_df[col].uniqu
-0001a4f0: 6528 2929 0a20 2020 2020 2020 2069 6620  e()).        if 
-0001a500: 6973 696e 7374 616e 6365 2874 6573 745f  isinstance(test_
-0001a510: 6466 2c20 7374 7229 206f 7220 7465 7374  df, str) or test
-0001a520: 5f64 6620 6973 204e 6f6e 653a 0a20 2020  _df is None:.   
-0001a530: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001a540: 7472 6169 6e5f 6466 2c20 7465 7374 5f64  train_df, test_d
-0001a550: 660a 2020 2020 2020 2020 656c 7365 3a0a  f.        else:.
-0001a560: 2020 2020 2020 2020 2020 2020 7465 7374              test
-0001a570: 5f64 665b 636f 6c5d 203d 2074 6573 745f  _df[col] = test_
-0001a580: 6466 5b63 6f6c 5d2e 6170 706c 7928 6c61  df[col].apply(la
-0001a590: 6d62 6461 2078 3a20 2752 4152 4527 2069  mbda x: 'RARE' i
-0001a5a0: 6620 7820 6e6f 7420 696e 2076 616c 7320  f x not in vals 
-0001a5b0: 656c 7365 2078 290a 2020 2020 2020 2020  else x).        
-0001a5c0: 2020 2020 7265 7475 726e 2074 7261 696e      return train
-0001a5d0: 5f64 662c 2074 6573 745f 6466 0a0a 2323  _df, test_df..##
-0001a5e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a5f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a280: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a290: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a2a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a2b0: 2323 2323 2323 2323 2323 2323 2323 0a64  ##############.d
+0001a2c0: 6566 2046 455f 636f 6d62 696e 655f 7261  ef FE_combine_ra
+0001a2d0: 7265 5f63 6174 6567 6f72 6965 7328 7472  re_categories(tr
+0001a2e0: 6169 6e5f 6466 2c20 6361 7465 676f 7269  ain_df, categori
+0001a2f0: 6361 6c5f 6665 6174 7572 6573 2c20 7465  cal_features, te
+0001a300: 7374 5f64 663d 2222 293a 0a20 2020 2022  st_df=""):.    "
+0001a310: 2222 0a20 2020 2049 6e20 7468 6973 2066  "".    In this f
+0001a320: 756e 6374 696f 6e2c 2077 6520 7769 6c6c  unction, we will
+0001a330: 2073 656c 6563 7420 616c 6c20 7261 7265   select all rare
+0001a340: 2063 6c61 7373 6573 2068 6176 696e 6720   classes having 
+0001a350: 7265 7072 6573 656e 7461 7469 6f6e 203c  representation <
+0001a360: 3125 206f 6620 706f 7075 6c61 7469 6f6e  1% of population
+0001a370: 2061 6e64 0a20 2020 2067 726f 7570 2074   and.    group t
+0001a380: 6865 6d20 746f 6765 7468 6572 2075 6e64  hem together und
+0001a390: 6572 2061 206e 6577 206c 6162 656c 2063  er a new label c
+0001a3a0: 616c 6c65 6420 2752 4152 4527 2e20 5765  alled 'RARE'. We
+0001a3b0: 2077 696c 6c20 6170 706c 7920 7468 6973   will apply this
+0001a3c0: 206f 6e20 7472 6169 6e20 616e 6420 7465   on train and te
+0001a3d0: 7374 2028 6f70 7469 6f6e 616c 290a 2020  st (optional).  
+0001a3e0: 2020 2222 220a 2020 2020 7472 6169 6e5f    """.    train_
+0001a3f0: 6466 203d 2063 6f70 792e 6465 6570 636f  df = copy.deepco
+0001a400: 7079 2874 7261 696e 5f64 6629 0a20 2020  py(train_df).   
+0001a410: 2074 6573 745f 6466 203d 2063 6f70 792e   test_df = copy.
+0001a420: 6465 6570 636f 7079 2874 6573 745f 6466  deepcopy(test_df
+0001a430: 290a 2020 2020 7472 6169 6e5f 6466 5b63  ).    train_df[c
+0001a440: 6174 6567 6f72 6963 616c 5f66 6561 7475  ategorical_featu
+0001a450: 7265 735d 203d 2074 7261 696e 5f64 665b  res] = train_df[
+0001a460: 6361 7465 676f 7269 6361 6c5f 6665 6174  categorical_feat
+0001a470: 7572 6573 5d2e 6170 706c 7928 0a20 2020  ures].apply(.   
+0001a480: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+0001a490: 783a 2078 2e6d 6173 6b28 782e 6d61 7028  x: x.mask(x.map(
+0001a4a0: 782e 7661 6c75 655f 636f 756e 7473 2829  x.value_counts()
+0001a4b0: 293c 2028 302e 3031 2a74 7261 696e 5f64  )< (0.01*train_d
+0001a4c0: 662e 7368 6170 655b 305d 292c 2027 5241  f.shape[0]), 'RA
+0001a4d0: 5245 2729 290a 2020 2020 666f 7220 636f  RE')).    for co
+0001a4e0: 6c20 696e 2063 6174 6567 6f72 6963 616c  l in categorical
+0001a4f0: 5f66 6561 7475 7265 733a 0a20 2020 2020  _features:.     
+0001a500: 2020 2076 616c 7320 3d20 6c69 7374 2874     vals = list(t
+0001a510: 7261 696e 5f64 665b 636f 6c5d 2e75 6e69  rain_df[col].uni
+0001a520: 7175 6528 2929 0a20 2020 2020 2020 2069  que()).        i
+0001a530: 6620 6973 696e 7374 616e 6365 2874 6573  f isinstance(tes
+0001a540: 745f 6466 2c20 7374 7229 206f 7220 7465  t_df, str) or te
+0001a550: 7374 5f64 6620 6973 204e 6f6e 653a 0a20  st_df is None:. 
+0001a560: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001a570: 6e20 7472 6169 6e5f 6466 2c20 7465 7374  n train_df, test
+0001a580: 5f64 660a 2020 2020 2020 2020 656c 7365  _df.        else
+0001a590: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+0001a5a0: 7374 5f64 665b 636f 6c5d 203d 2074 6573  st_df[col] = tes
+0001a5b0: 745f 6466 5b63 6f6c 5d2e 6170 706c 7928  t_df[col].apply(
+0001a5c0: 6c61 6d62 6461 2078 3a20 2752 4152 4527  lambda x: 'RARE'
+0001a5d0: 2069 6620 7820 6e6f 7420 696e 2076 616c   if x not in val
+0001a5e0: 7320 656c 7365 2078 290a 2020 2020 2020  s else x).      
+0001a5f0: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
+0001a600: 696e 5f64 662c 2074 6573 745f 6466 0a0a  in_df, test_df..
 0001a610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001a620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001a630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a640: 2323 230a 6465 6620 4645 5f67 6574 5f6c  ###.def FE_get_l
-0001a650: 6174 6573 745f 7661 6c75 6573 5f62 6173  atest_values_bas
-0001a660: 6564 5f6f 6e5f 6461 7465 5f63 6f6c 756d  ed_on_date_colum
-0001a670: 6e28 6466 742c 2069 645f 636f 6c2c 2064  n(dft, id_col, d
-0001a680: 6174 655f 636f 6c2c 2063 6f6c 732c 2061  ate_col, cols, a
-0001a690: 7363 656e 6469 6e67 3d46 616c 7365 293a  scending=False):
-0001a6a0: 0a20 2020 2022 2222 0a20 2020 2046 4520  .    """.    FE 
-0001a6b0: 6d65 616e 7320 4645 4154 5552 4520 454e  means FEATURE EN
-0001a6c0: 4749 4e45 4552 494e 4720 2d20 5468 6174  GINEERING - That
-0001a6d0: 206d 6561 6e73 2074 6869 7320 6675 6e63   means this func
-0001a6e0: 7469 6f6e 2077 696c 6c20 6372 6561 7465  tion will create
-0001a6f0: 206e 6577 2066 6561 7475 7265 730a 2020   new features.  
-0001a700: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-0001a710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a670: 2323 2323 230a 6465 6620 4645 5f67 6574  #####.def FE_get
+0001a680: 5f6c 6174 6573 745f 7661 6c75 6573 5f62  _latest_values_b
+0001a690: 6173 6564 5f6f 6e5f 6461 7465 5f63 6f6c  ased_on_date_col
+0001a6a0: 756d 6e28 6466 742c 2069 645f 636f 6c2c  umn(dft, id_col,
+0001a6b0: 2064 6174 655f 636f 6c2c 2063 6f6c 732c   date_col, cols,
+0001a6c0: 2061 7363 656e 6469 6e67 3d46 616c 7365   ascending=False
+0001a6d0: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
+0001a6e0: 4520 6d65 616e 7320 4645 4154 5552 4520  E means FEATURE 
+0001a6f0: 454e 4749 4e45 4552 494e 4720 2d20 5468  ENGINEERING - Th
+0001a700: 6174 206d 6561 6e73 2074 6869 7320 6675  at means this fu
+0001a710: 6e63 7469 6f6e 2077 696c 6c20 6372 6561  nction will crea
+0001a720: 7465 206e 6577 2066 6561 7475 7265 730a  te new features.
+0001a730: 2020 2020 2323 2323 2323 2323 2323 2323      ############
 0001a740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a750: 2323 2323 2323 2323 0a20 2020 2054 6869  ########.    Thi
-0001a760: 7320 6675 6e63 7469 6f6e 2067 6574 7320  s function gets 
-0001a770: 796f 7520 7468 6520 6c61 7465 7374 2076  you the latest v
-0001a780: 616c 7565 7320 6f66 2074 6865 2063 6f6c  alues of the col
-0001a790: 756d 6e73 2069 6e20 636f 6c73 2066 726f  umns in cols fro
-0001a7a0: 6d20 6120 6461 7465 2063 6f6c 756d 6e20  m a date column 
-0001a7b0: 6461 7465 5f63 6f6c 2e0a 0a20 2020 2049  date_col...    I
-0001a7c0: 6e70 7574 733a 0a20 2020 2064 6674 3a20  nputs:.    dft: 
-0001a7d0: 6461 7461 6672 616d 652c 2070 616e 6461  dataframe, panda
-0001a7e0: 730a 2020 2020 6964 5f63 6f6c 3a20 796f  s.    id_col: yo
-0001a7f0: 7520 6e65 6564 2074 6f20 7072 6f76 6964  u need to provid
-0001a800: 6520 616e 2049 4420 636f 6c75 6d6e 2074  e an ID column t
-0001a810: 6f20 6772 6f75 7062 7920 7468 6520 636f  o groupby the co
-0001a820: 6c73 2061 6e64 2074 6865 6e20 736f 7274  ls and then sort
-0001a830: 2074 6865 6d20 6279 2064 6174 655f 636f   them by date_co
-0001a840: 6c2e 0a20 2020 2064 6174 655f 636f 6c3a  l..    date_col:
-0001a850: 2074 6869 7320 6d75 7374 2062 6520 6120   this must be a 
-0001a860: 7661 6c69 6420 7061 6e64 6173 2064 6174  valid pandas dat
-0001a870: 652d 7469 6d65 2063 6f6c 756d 6e2e 2049  e-time column. I
-0001a880: 6620 6974 2069 7320 6120 7374 7269 6e67  f it is a string
-0001a890: 2063 6f6c 756d 6e2c 0a20 2020 2020 2020   column,.       
-0001a8a0: 2020 2020 6d61 6b65 2073 7572 6520 796f      make sure yo
-0001a8b0: 7520 6368 616e 6765 2069 7420 746f 2061  u change it to a
-0001a8c0: 2064 6174 652d 7469 6d65 2063 6f6c 756d   date-time colum
-0001a8d0: 6e2e 0a20 2020 2020 2020 2020 2049 7420  n..          It 
-0001a8e0: 736f 7274 7320 6561 6368 2067 726f 7570  sorts each group
-0001a8f0: 2062 7920 7468 6520 6c61 7465 7374 2064   by the latest d
-0001a900: 6174 6520 2864 6573 6365 6e64 696e 6729  ate (descending)
-0001a910: 2061 6e64 2073 656c 6563 7473 2074 6861   and selects tha
-0001a920: 7420 746f 7020 726f 772e 0a20 2020 2063  t top row..    c
-0001a930: 6f6c 733a 2074 6865 7365 2061 7265 2074  ols: these are t
-0001a940: 6865 206c 6973 7420 6f66 2063 6f6c 756d  he list of colum
-0001a950: 6e73 2079 6f75 2077 616e 7420 7468 6569  ns you want thei
-0001a960: 7220 6c61 7465 7374 2076 616c 7565 2062  r latest value b
-0001a970: 6173 6564 206f 6e20 7468 6520 6461 7465  ased on the date
-0001a980: 2d63 6f6c 2079 6f75 2073 7065 6369 6679  -col you specify
-0001a990: 2e0a 2020 2020 2020 2020 2054 6865 7365  ..         These
-0001a9a0: 2063 6f6c 7320 6361 6e20 6265 2061 6e79   cols can be any
-0001a9b0: 2074 7970 6520 6f66 2063 6f6c 756d 6e3a   type of column:
-0001a9c0: 206e 756d 6572 6963 206f 7220 7374 7269   numeric or stri
-0001a9d0: 6e67 2e0a 2020 2020 6173 6365 6e64 696e  ng..    ascendin
-0001a9e0: 673a 2053 6574 2074 6869 7320 6173 2054  g: Set this as T
-0001a9f0: 7275 6520 6f72 2046 616c 7365 2064 6570  rue or False dep
-0001aa00: 656e 6469 6e67 206f 6e20 7768 6574 6865  ending on whethe
-0001aa10: 7220 796f 7520 7761 6e74 2073 6d61 6c6c  r you want small
-0001aa20: 6573 7420 6f72 2062 6967 6765 7374 206f  est or biggest o
-0001aa30: 6e20 746f 702e 0a0a 2020 2020 4f75 7470  n top...    Outp
-0001aa40: 7574 733a 0a20 2020 2052 6574 7572 6e73  uts:.    Returns
-0001aa50: 2061 2064 6174 6166 7261 6d65 2074 6861   a dataframe tha
-0001aa60: 7420 6973 2073 6d61 6c6c 6572 2074 6861  t is smaller tha
-0001aa70: 6e20 696e 7075 7420 6461 7461 6672 616d  n input datafram
-0001aa80: 6520 7369 6e63 6520 6974 2067 726f 7570  e since it group
-0001aa90: 7320 636f 6c73 2062 7920 4944 5f63 6f6c  s cols by ID_col
-0001aaa0: 756d 6e2e 0a20 2020 2023 2323 2323 2323  umn..    #######
-0001aab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001aac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001aad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a780: 2323 2323 2323 2323 2323 0a20 2020 2054  ##########.    T
+0001a790: 6869 7320 6675 6e63 7469 6f6e 2067 6574  his function get
+0001a7a0: 7320 796f 7520 7468 6520 6c61 7465 7374  s you the latest
+0001a7b0: 2076 616c 7565 7320 6f66 2074 6865 2063   values of the c
+0001a7c0: 6f6c 756d 6e73 2069 6e20 636f 6c73 2066  olumns in cols f
+0001a7d0: 726f 6d20 6120 6461 7465 2063 6f6c 756d  rom a date colum
+0001a7e0: 6e20 6461 7465 5f63 6f6c 2e0a 0a20 2020  n date_col...   
+0001a7f0: 2049 6e70 7574 733a 0a20 2020 2064 6674   Inputs:.    dft
+0001a800: 3a20 6461 7461 6672 616d 652c 2070 616e  : dataframe, pan
+0001a810: 6461 730a 2020 2020 6964 5f63 6f6c 3a20  das.    id_col: 
+0001a820: 796f 7520 6e65 6564 2074 6f20 7072 6f76  you need to prov
+0001a830: 6964 6520 616e 2049 4420 636f 6c75 6d6e  ide an ID column
+0001a840: 2074 6f20 6772 6f75 7062 7920 7468 6520   to groupby the 
+0001a850: 636f 6c73 2061 6e64 2074 6865 6e20 736f  cols and then so
+0001a860: 7274 2074 6865 6d20 6279 2064 6174 655f  rt them by date_
+0001a870: 636f 6c2e 0a20 2020 2064 6174 655f 636f  col..    date_co
+0001a880: 6c3a 2074 6869 7320 6d75 7374 2062 6520  l: this must be 
+0001a890: 6120 7661 6c69 6420 7061 6e64 6173 2064  a valid pandas d
+0001a8a0: 6174 652d 7469 6d65 2063 6f6c 756d 6e2e  ate-time column.
+0001a8b0: 2049 6620 6974 2069 7320 6120 7374 7269   If it is a stri
+0001a8c0: 6e67 2063 6f6c 756d 6e2c 0a20 2020 2020  ng column,.     
+0001a8d0: 2020 2020 2020 6d61 6b65 2073 7572 6520        make sure 
+0001a8e0: 796f 7520 6368 616e 6765 2069 7420 746f  you change it to
+0001a8f0: 2061 2064 6174 652d 7469 6d65 2063 6f6c   a date-time col
+0001a900: 756d 6e2e 0a20 2020 2020 2020 2020 2049  umn..          I
+0001a910: 7420 736f 7274 7320 6561 6368 2067 726f  t sorts each gro
+0001a920: 7570 2062 7920 7468 6520 6c61 7465 7374  up by the latest
+0001a930: 2064 6174 6520 2864 6573 6365 6e64 696e   date (descendin
+0001a940: 6729 2061 6e64 2073 656c 6563 7473 2074  g) and selects t
+0001a950: 6861 7420 746f 7020 726f 772e 0a20 2020  hat top row..   
+0001a960: 2063 6f6c 733a 2074 6865 7365 2061 7265   cols: these are
+0001a970: 2074 6865 206c 6973 7420 6f66 2063 6f6c   the list of col
+0001a980: 756d 6e73 2079 6f75 2077 616e 7420 7468  umns you want th
+0001a990: 6569 7220 6c61 7465 7374 2076 616c 7565  eir latest value
+0001a9a0: 2062 6173 6564 206f 6e20 7468 6520 6461   based on the da
+0001a9b0: 7465 2d63 6f6c 2079 6f75 2073 7065 6369  te-col you speci
+0001a9c0: 6679 2e0a 2020 2020 2020 2020 2054 6865  fy..         The
+0001a9d0: 7365 2063 6f6c 7320 6361 6e20 6265 2061  se cols can be a
+0001a9e0: 6e79 2074 7970 6520 6f66 2063 6f6c 756d  ny type of colum
+0001a9f0: 6e3a 206e 756d 6572 6963 206f 7220 7374  n: numeric or st
+0001aa00: 7269 6e67 2e0a 2020 2020 6173 6365 6e64  ring..    ascend
+0001aa10: 696e 673a 2053 6574 2074 6869 7320 6173  ing: Set this as
+0001aa20: 2054 7275 6520 6f72 2046 616c 7365 2064   True or False d
+0001aa30: 6570 656e 6469 6e67 206f 6e20 7768 6574  epending on whet
+0001aa40: 6865 7220 796f 7520 7761 6e74 2073 6d61  her you want sma
+0001aa50: 6c6c 6573 7420 6f72 2062 6967 6765 7374  llest or biggest
+0001aa60: 206f 6e20 746f 702e 0a0a 2020 2020 4f75   on top...    Ou
+0001aa70: 7470 7574 733a 0a20 2020 2052 6574 7572  tputs:.    Retur
+0001aa80: 6e73 2061 2064 6174 6166 7261 6d65 2074  ns a dataframe t
+0001aa90: 6861 7420 6973 2073 6d61 6c6c 6572 2074  hat is smaller t
+0001aaa0: 6861 6e20 696e 7075 7420 6461 7461 6672  han input datafr
+0001aab0: 616d 6520 7369 6e63 6520 6974 2067 726f  ame since it gro
+0001aac0: 7570 7320 636f 6c73 2062 7920 4944 5f63  ups cols by ID_c
+0001aad0: 6f6c 756d 6e2e 0a20 2020 2023 2323 2323  olumn..    #####
 0001aae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001aaf0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-0001ab00: 2020 2020 4265 7761 7265 2120 596f 7520      Beware! You 
-0001ab10: 7769 6c6c 2067 6574 2061 2064 6174 6166  will get a dataf
-0001ab20: 7261 6d65 2074 6861 7420 6861 7320 6665  rame that has fe
-0001ab30: 7765 7220 636f 6c73 2074 6861 6e20 796f  wer cols than yo
-0001ab40: 7572 2069 6e70 7574 2077 6974 6820 6665  ur input with fe
-0001ab50: 7765 7220 726f 7773 2074 6861 6e20 696e  wer rows than in
-0001ab60: 7075 742e 0a20 2020 2022 2222 0a20 2020  put..    """.   
-0001ab70: 2064 6674 203d 2063 6f70 792e 6465 6570   dft = copy.deep
-0001ab80: 636f 7079 2864 6674 290a 2020 2020 7472  copy(dft).    tr
-0001ab90: 793a 0a20 2020 2020 2020 2069 6620 6973  y:.        if is
-0001aba0: 696e 7374 616e 6365 2863 6f6c 732c 2073  instance(cols, s
-0001abb0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0001abc0: 2063 6f6c 7320 3d20 5b63 6f6c 735d 0a20   cols = [cols]. 
-0001abd0: 2020 2020 2020 2074 7261 696e 5f61 6464         train_add
-0001abe0: 203d 2064 6674 2e67 726f 7570 6279 285b   = dft.groupby([
-0001abf0: 6964 5f63 6f6c 5d2c 2073 6f72 743d 4661  id_col], sort=Fa
-0001ac00: 6c73 6529 2e61 7070 6c79 286c 616d 6264  lse).apply(lambd
-0001ac10: 6120 783a 2078 2e73 6f72 745f 7661 6c75  a x: x.sort_valu
-0001ac20: 6573 285b 6461 7465 5f63 6f6c 5d2c 0a20  es([date_col],. 
-0001ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac70: 2020 2020 2020 2061 7363 656e 6469 6e67         ascending
-0001ac80: 3d61 7363 656e 6469 6e67 2929 0a20 2020  =ascending)).   
-0001ac90: 2020 2020 2074 7261 696e 5f61 6464 203d       train_add =
-0001aca0: 2074 7261 696e 5f61 6464 5b63 6f6c 735d   train_add[cols]
-0001acb0: 2e72 6573 6574 5f69 6e64 6578 2829 0a20  .reset_index(). 
+0001aaf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ab00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ab10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ab20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ab30: 230a 2020 2020 4265 7761 7265 2120 596f  #.    Beware! Yo
+0001ab40: 7520 7769 6c6c 2067 6574 2061 2064 6174  u will get a dat
+0001ab50: 6166 7261 6d65 2074 6861 7420 6861 7320  aframe that has 
+0001ab60: 6665 7765 7220 636f 6c73 2074 6861 6e20  fewer cols than 
+0001ab70: 796f 7572 2069 6e70 7574 2077 6974 6820  your input with 
+0001ab80: 6665 7765 7220 726f 7773 2074 6861 6e20  fewer rows than 
+0001ab90: 696e 7075 742e 0a20 2020 2022 2222 0a20  input..    """. 
+0001aba0: 2020 2064 6674 203d 2063 6f70 792e 6465     dft = copy.de
+0001abb0: 6570 636f 7079 2864 6674 290a 2020 2020  epcopy(dft).    
+0001abc0: 7472 793a 0a20 2020 2020 2020 2069 6620  try:.        if 
+0001abd0: 6973 696e 7374 616e 6365 2863 6f6c 732c  isinstance(cols,
+0001abe0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+0001abf0: 2020 2063 6f6c 7320 3d20 5b63 6f6c 735d     cols = [cols]
+0001ac00: 0a20 2020 2020 2020 2074 7261 696e 5f61  .        train_a
+0001ac10: 6464 203d 2064 6674 2e67 726f 7570 6279  dd = dft.groupby
+0001ac20: 285b 6964 5f63 6f6c 5d2c 2073 6f72 743d  ([id_col], sort=
+0001ac30: 4661 6c73 6529 2e61 7070 6c79 286c 616d  False).apply(lam
+0001ac40: 6264 6120 783a 2078 2e73 6f72 745f 7661  bda x: x.sort_va
+0001ac50: 6c75 6573 285b 6461 7465 5f63 6f6c 5d2c  lues([date_col],
+0001ac60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aca0: 2020 2020 2020 2020 2061 7363 656e 6469           ascendi
+0001acb0: 6e67 3d61 7363 656e 6469 6e67 2929 0a20  ng=ascending)). 
 0001acc0: 2020 2020 2020 2074 7261 696e 5f61 6464         train_add
-0001acd0: 203d 2074 7261 696e 5f61 6464 2e67 726f   = train_add.gro
-0001ace0: 7570 6279 2869 645f 636f 6c29 2e68 6561  upby(id_col).hea
-0001acf0: 6428 3129 2e72 6573 6574 5f69 6e64 6578  d(1).reset_index
-0001ad00: 2864 726f 703d 5472 7565 292e 6472 6f70  (drop=True).drop
-0001ad10: 2827 6c65 7665 6c5f 3127 2c61 7869 733d  ('level_1',axis=
-0001ad20: 3129 0a20 2020 2065 7863 6570 743a 0a20  1).    except:. 
-0001ad30: 2020 2020 2020 2070 7269 6e74 2827 2020         print('  
-0001ad40: 2020 4572 726f 7220 696e 2067 6574 7469    Error in getti
-0001ad50: 6e67 206c 6174 6573 7420 7374 6174 7573  ng latest status
-0001ad60: 206f 6620 636f 6c75 6d6e 7320 6261 7365   of columns base
-0001ad70: 6420 6f6e 2025 732e 2052 6574 7572 6e69  d on %s. Returni
-0001ad80: 6e67 2e2e 2e27 2025 6461 7465 5f63 6f6c  ng...' %date_col
-0001ad90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001ada0: 2064 6674 0a20 2020 2072 6574 7572 6e20   dft.    return 
-0001adb0: 7472 6169 6e5f 6164 640a 2323 2323 2323  train_add.######
-0001adc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001add0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ade0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001acd0: 203d 2074 7261 696e 5f61 6464 5b63 6f6c   = train_add[col
+0001ace0: 735d 2e72 6573 6574 5f69 6e64 6578 2829  s].reset_index()
+0001acf0: 0a20 2020 2020 2020 2074 7261 696e 5f61  .        train_a
+0001ad00: 6464 203d 2074 7261 696e 5f61 6464 2e67  dd = train_add.g
+0001ad10: 726f 7570 6279 2869 645f 636f 6c29 2e68  roupby(id_col).h
+0001ad20: 6561 6428 3129 2e72 6573 6574 5f69 6e64  ead(1).reset_ind
+0001ad30: 6578 2864 726f 703d 5472 7565 292e 6472  ex(drop=True).dr
+0001ad40: 6f70 2827 6c65 7665 6c5f 3127 2c61 7869  op('level_1',axi
+0001ad50: 733d 3129 0a20 2020 2065 7863 6570 743a  s=1).    except:
+0001ad60: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+0001ad70: 2020 2020 4572 726f 7220 696e 2067 6574      Error in get
+0001ad80: 7469 6e67 206c 6174 6573 7420 7374 6174  ting latest stat
+0001ad90: 7573 206f 6620 636f 6c75 6d6e 7320 6261  us of columns ba
+0001ada0: 7365 6420 6f6e 2025 732e 2052 6574 7572  sed on %s. Retur
+0001adb0: 6e69 6e67 2e2e 2e27 2025 6461 7465 5f63  ning...' %date_c
+0001adc0: 6f6c 290a 2020 2020 2020 2020 7265 7475  ol).        retu
+0001add0: 726e 2064 6674 0a20 2020 2072 6574 7572  rn dft.    retur
+0001ade0: 6e20 7472 6169 6e5f 6164 640a 2323 2323  n train_add.####
 0001adf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ae00: 2323 2323 2323 2323 2323 230a 6672 6f6d  ###########.from
-0001ae10: 2066 756e 6374 6f6f 6c73 2069 6d70 6f72   functools impor
-0001ae20: 7420 7265 6475 6365 0a64 6566 2046 455f  t reduce.def FE_
-0001ae30: 7370 6c69 745f 6164 645f 636f 6c75 6d6e  split_add_column
-0001ae40: 2864 6674 2c20 636f 6c2c 2073 706c 6974  (dft, col, split
-0001ae50: 7465 723d 272c 272c 2061 6374 696f 6e3d  ter=',', action=
-0001ae60: 2761 6464 2729 3a0a 2020 2020 2222 220a  'add'):.    """.
-0001ae70: 2020 2020 4645 206d 6561 6e73 2046 4541      FE means FEA
-0001ae80: 5455 5245 2045 4e47 494e 4545 5249 4e47  TURE ENGINEERING
-0001ae90: 202d 2054 6861 7420 6d65 616e 7320 7468   - That means th
-0001aea0: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-0001aeb0: 2063 7265 6174 6520 6e65 7720 6665 6174   create new feat
-0001aec0: 7572 6573 0a20 2020 2023 2323 2323 2323  ures.    #######
-0001aed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001aee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001aef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ae00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ae10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ae20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ae30: 2323 2323 2323 2323 2323 2323 230a 6672  #############.fr
+0001ae40: 6f6d 2066 756e 6374 6f6f 6c73 2069 6d70  om functools imp
+0001ae50: 6f72 7420 7265 6475 6365 0a64 6566 2046  ort reduce.def F
+0001ae60: 455f 7370 6c69 745f 6164 645f 636f 6c75  E_split_add_colu
+0001ae70: 6d6e 2864 6674 2c20 636f 6c2c 2073 706c  mn(dft, col, spl
+0001ae80: 6974 7465 723d 272c 272c 2061 6374 696f  itter=',', actio
+0001ae90: 6e3d 2761 6464 2729 3a0a 2020 2020 2222  n='add'):.    ""
+0001aea0: 220a 2020 2020 4645 206d 6561 6e73 2046  ".    FE means F
+0001aeb0: 4541 5455 5245 2045 4e47 494e 4545 5249  EATURE ENGINEERI
+0001aec0: 4e47 202d 2054 6861 7420 6d65 616e 7320  NG - That means 
+0001aed0: 7468 6973 2066 756e 6374 696f 6e20 7769  this function wi
+0001aee0: 6c6c 2063 7265 6174 6520 6e65 7720 6665  ll create new fe
+0001aef0: 6174 7572 6573 0a20 2020 2023 2323 2323  atures.    #####
 0001af00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001af10: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-0001af20: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-0001af30: 6e20 7769 6c6c 2073 706c 6974 2061 2063  n will split a c
-0001af40: 6f6c 756d 6e27 7320 7661 6c75 6573 2062  olumn's values b
-0001af50: 6173 6564 206f 6e20 6120 7370 6c69 7474  ased on a splitt
-0001af60: 6572 2079 6f75 2073 7065 6369 6679 2061  er you specify a
-0001af70: 6e64 0a20 2020 2077 696c 6c20 6569 7468  nd.    will eith
-0001af80: 6572 2061 6464 2074 6865 6d20 6f72 2063  er add them or c
-0001af90: 6f6e 6361 7465 6e61 7465 2074 6865 6d20  oncatenate them 
-0001afa0: 6173 2079 6f75 2073 7065 6369 6679 2069  as you specify i
-0001afb0: 6e20 7468 6520 6163 7469 6f6e 2061 7267  n the action arg
-0001afc0: 756d 656e 742e 0a0a 2020 2020 496e 7075  ument...    Inpu
-0001afd0: 7473 3a0a 2020 2020 6466 743a 2070 616e  ts:.    dft: pan
-0001afe0: 6461 7320 4461 7461 4672 616d 650a 2020  das DataFrame.  
-0001aff0: 2020 636f 6c3a 206e 616d 6520 6f66 2063    col: name of c
-0001b000: 6f6c 756d 6e20 7468 6174 2079 6f75 2077  olumn that you w
-0001b010: 616e 7420 746f 2073 706c 6974 2069 6e74  ant to split int
-0001b020: 6f20 6974 7320 636f 6e73 7469 7475 656e  o its constituen
-0001b030: 7420 7061 7274 732e 2049 7420 6d75 7374  t parts. It must
-0001b040: 2062 6520 6120 7374 7269 6e67 2063 6f6c   be a string col
-0001b050: 756d 6e2e 0a20 2020 2073 706c 6974 7465  umn..    splitte
-0001b060: 723a 2073 706c 6974 7465 7220 6361 6e20  r: splitter can 
-0001b070: 6265 2061 6e79 2073 7472 696e 6720 7468  be any string th
-0001b080: 6174 2069 7320 666f 756e 6420 696e 2079  at is found in y
-0001b090: 6f75 7220 636f 6c75 6d6e 2061 6e64 2074  our column and t
-0001b0a0: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
-0001b0b0: 7370 6c69 7420 6279 2e0a 2020 2020 6163  split by..    ac
-0001b0c0: 7469 6f6e 3a20 6361 6e20 6265 2061 6e79  tion: can be any
-0001b0d0: 206f 6e65 206f 6620 666f 6c6c 6f77 696e   one of followin
-0001b0e0: 673a 207b 2761 6464 272c 2027 7375 6274  g: {'add', 'subt
-0001b0f0: 7261 6374 272c 2027 6d75 6c74 6970 6c79  ract', 'multiply
-0001b100: 272c 2027 6469 7669 6465 272c 2027 636f  ', 'divide', 'co
-0001b110: 6e63 6174 272c 2027 636f 6e63 6174 656e  ncat', 'concaten
-0001b120: 6174 6527 7d0a 2020 2020 2323 2323 2323  ate'}.    ######
-0001b130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001af10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001af20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001af30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001af40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001af50: 230a 2020 2020 5468 6973 2066 756e 6374  #.    This funct
+0001af60: 696f 6e20 7769 6c6c 2073 706c 6974 2061  ion will split a
+0001af70: 2063 6f6c 756d 6e27 7320 7661 6c75 6573   column's values
+0001af80: 2062 6173 6564 206f 6e20 6120 7370 6c69   based on a spli
+0001af90: 7474 6572 2079 6f75 2073 7065 6369 6679  tter you specify
+0001afa0: 2061 6e64 0a20 2020 2077 696c 6c20 6569   and.    will ei
+0001afb0: 7468 6572 2061 6464 2074 6865 6d20 6f72  ther add them or
+0001afc0: 2063 6f6e 6361 7465 6e61 7465 2074 6865   concatenate the
+0001afd0: 6d20 6173 2079 6f75 2073 7065 6369 6679  m as you specify
+0001afe0: 2069 6e20 7468 6520 6163 7469 6f6e 2061   in the action a
+0001aff0: 7267 756d 656e 742e 0a0a 2020 2020 496e  rgument...    In
+0001b000: 7075 7473 3a0a 2020 2020 6466 743a 2070  puts:.    dft: p
+0001b010: 616e 6461 7320 4461 7461 4672 616d 650a  andas DataFrame.
+0001b020: 2020 2020 636f 6c3a 206e 616d 6520 6f66      col: name of
+0001b030: 2063 6f6c 756d 6e20 7468 6174 2079 6f75   column that you
+0001b040: 2077 616e 7420 746f 2073 706c 6974 2069   want to split i
+0001b050: 6e74 6f20 6974 7320 636f 6e73 7469 7475  nto its constitu
+0001b060: 656e 7420 7061 7274 732e 2049 7420 6d75  ent parts. It mu
+0001b070: 7374 2062 6520 6120 7374 7269 6e67 2063  st be a string c
+0001b080: 6f6c 756d 6e2e 0a20 2020 2073 706c 6974  olumn..    split
+0001b090: 7465 723a 2073 706c 6974 7465 7220 6361  ter: splitter ca
+0001b0a0: 6e20 6265 2061 6e79 2073 7472 696e 6720  n be any string 
+0001b0b0: 7468 6174 2069 7320 666f 756e 6420 696e  that is found in
+0001b0c0: 2079 6f75 7220 636f 6c75 6d6e 2061 6e64   your column and
+0001b0d0: 2074 6861 7420 796f 7520 7761 6e74 2074   that you want t
+0001b0e0: 6f20 7370 6c69 7420 6279 2e0a 2020 2020  o split by..    
+0001b0f0: 6163 7469 6f6e 3a20 6361 6e20 6265 2061  action: can be a
+0001b100: 6e79 206f 6e65 206f 6620 666f 6c6c 6f77  ny one of follow
+0001b110: 696e 673a 207b 2761 6464 272c 2027 7375  ing: {'add', 'su
+0001b120: 6274 7261 6374 272c 2027 6d75 6c74 6970  btract', 'multip
+0001b130: 6c79 272c 2027 6469 7669 6465 272c 2027  ly', 'divide', '
+0001b140: 636f 6e63 6174 272c 2027 636f 6e63 6174  concat', 'concat
+0001b150: 656e 6174 6527 7d0a 2020 2020 2323 2323  enate'}.    ####
 0001b160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b170: 2323 2323 2323 2323 2323 0a20 2020 2052  ##########.    R
-0001b180: 6574 7572 6e73 2061 2064 6174 6166 7261  eturns a datafra
-0001b190: 6d65 2077 6974 6820 6120 6e65 7720 636f  me with a new co
-0001b1a0: 6c75 6d6e 2074 6861 7420 6973 2061 206d  lumn that is a m
-0001b1b0: 6f64 6966 6963 6174 696f 6e20 6f66 2074  odification of t
-0001b1c0: 6865 206f 6c64 2063 6f6c 756d 6e0a 2020  he old column.  
-0001b1d0: 2020 2222 220a 2020 2020 6466 7420 3d20    """.    dft = 
-0001b1e0: 636f 7079 2e64 6565 7063 6f70 7928 6466  copy.deepcopy(df
-0001b1f0: 7429 0a20 2020 206e 6577 5f63 6f6c 203d  t).    new_col =
-0001b200: 2063 6f6c 202b 2027 5f73 706c 6974 5f61   col + '_split_a
-0001b210: 7070 6c79 270a 2020 2020 7072 696e 7428  pply'.    print(
-0001b220: 2743 7265 6174 696e 6720 636f 6c75 6d6e  'Creating column
-0001b230: 203d 2025 7320 7573 696e 6720 7370 6c69   = %s using spli
-0001b240: 745f 6164 6420 6665 6174 7572 6520 656e  t_add feature en
-0001b250: 6769 6e65 6572 696e 672e 2e2e 2720 256e  gineering...' %n
-0001b260: 6577 5f63 6f6c 290a 2020 2020 6966 2061  ew_col).    if a
-0001b270: 6374 696f 6e20 696e 205b 272b 272c 272d  ction in ['+','-
-0001b280: 272c 272a 272c 272f 272c 2761 6464 272c  ','*','/','add',
-0001b290: 2773 7562 7472 6163 7427 2c27 6d75 6c74  'subtract','mult
-0001b2a0: 6970 6c79 272c 2764 6976 6964 6527 5d3a  iply','divide']:
-0001b2b0: 0a20 2020 2020 2020 2069 6620 6163 7469  .        if acti
-0001b2c0: 6f6e 2069 6e20 5b27 6164 6427 2c27 2b27  on in ['add','+'
-0001b2d0: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
-0001b2e0: 6967 6e20 3d20 272b 270a 2020 2020 2020  ign = '+'.      
-0001b2f0: 2020 656c 6966 2061 6374 696f 6e20 696e    elif action in
-0001b300: 205b 272d 272c 2027 7375 6274 7261 6374   ['-', 'subtract
-0001b310: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-0001b320: 7369 676e 203d 2027 2d27 0a20 2020 2020  sign = '-'.     
-0001b330: 2020 2065 6c69 6620 6163 7469 6f6e 2069     elif action i
-0001b340: 6e20 5b27 2a27 2c20 276d 756c 7469 706c  n ['*', 'multipl
-0001b350: 7927 5d3a 0a20 2020 2020 2020 2020 2020  y']:.           
-0001b360: 2073 6967 6e20 3d20 272a 270a 2020 2020   sign = '*'.    
-0001b370: 2020 2020 656c 6966 2061 6374 696f 6e20      elif action 
-0001b380: 696e 205b 272f 272c 2027 6469 7669 6465  in ['/', 'divide
-0001b390: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-0001b3a0: 7369 676e 203d 2027 2f27 0a20 2020 2020  sign = '/'.     
-0001b3b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001b3c0: 2020 2020 2073 6967 6e20 3d20 272b 270a       sign = '+'.
-0001b3d0: 2020 2020 2020 2020 2320 7573 696e 6720          # using 
-0001b3e0: 7265 6475 6365 2074 6f20 636f 6d70 7574  reduce to comput
-0001b3f0: 6520 7375 6d20 6f66 206c 6973 740a 2020  e sum of list.  
-0001b400: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0001b410: 2020 2020 2020 2074 7261 696e 7820 3d20         trainx = 
-0001b420: 6466 745b 636f 6c5d 2e61 7374 7970 6528  dft[col].astype(
-0001b430: 7374 7229 0a20 2020 2020 2020 2020 2020  str).           
-0001b440: 2074 7261 696e 7820 3d20 7472 6169 6e78   trainx = trainx
-0001b450: 2e6d 6170 286c 616d 6264 6120 783a 2020  .map(lambda x:  
-0001b460: 3020 6966 2078 2069 7320 6e70 2e6e 616e  0 if x is np.nan
-0001b470: 2065 6c73 6520 3020 6966 2078 203d 3d20   else 0 if x == 
-0001b480: 2727 2065 6c73 6520 782e 7370 6c69 7428  '' else x.split(
-0001b490: 7370 6c69 7474 6572 2929 2e6d 6170 280a  splitter)).map(.
-0001b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4c0: 6c61 6d62 6461 206c 6973 7478 3a20 5b69  lambda listx: [i
-0001b4d0: 6e74 2878 2920 6966 2078 2021 3d20 2727  nt(x) if x != ''
-0001b4e0: 2065 6c73 6520 3020 666f 7220 7820 696e   else 0 for x in
-0001b4f0: 206c 6973 7478 205d 2069 6620 6973 696e   listx ] if isin
-0001b500: 7374 616e 6365 286c 6973 7478 2c6c 6973  stance(listx,lis
-0001b510: 7429 2065 6c73 6520 5b30 2c30 5d29 0a20  t) else [0,0]). 
-0001b520: 2020 2020 2020 2020 2020 2064 6674 5b6e             dft[n
-0001b530: 6577 5f63 6f6c 5d20 3d20 7472 6169 6e78  ew_col] = trainx
-0001b540: 2e6d 6170 286c 616d 6264 6120 6c69 733a  .map(lambda lis:
-0001b550: 2072 6564 7563 6528 6c61 6d62 6461 2061   reduce(lambda a
-0001b560: 2c62 203a 2065 7661 6c28 2761 272b 7369  ,b : eval('a'+si
-0001b570: 676e 2b27 6227 292c 206c 6973 2920 6966  gn+'b'), lis) if
-0001b580: 2069 7369 6e73 7461 6e63 6528 6c69 732c   isinstance(lis,
-0001b590: 6c69 7374 2920 656c 7365 2030 292e 7661  list) else 0).va
-0001b5a0: 6c75 6573 0a20 2020 2020 2020 2065 7863  lues.        exc
-0001b5b0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-0001b5c0: 2070 7269 6e74 2827 2020 2020 4572 726f   print('    Erro
-0001b5d0: 723a 2072 6574 7572 6e69 6e67 2077 6974  r: returning wit
-0001b5e0: 686f 7574 2063 7265 6174 696e 6720 6e65  hout creating ne
-0001b5f0: 7720 636f 6c75 6d6e 2729 0a20 2020 2020  w column').     
-0001b600: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-0001b610: 740a 2020 2020 656c 6966 2061 6374 696f  t.    elif actio
-0001b620: 6e20 696e 205b 2763 6f6e 6361 7427 2c27  n in ['concat','
-0001b630: 636f 6e63 6174 656e 6174 6527 5d3a 0a20  concatenate']:. 
-0001b640: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0001b650: 2020 2020 2020 2020 6466 745b 6e65 775f          dft[new_
-0001b660: 636f 6c5d 203d 2064 6674 5b63 6f6c 5d2e  col] = dft[col].
-0001b670: 6d61 7028 6c61 6d62 6461 2078 3a20 2022  map(lambda x:  "
-0001b680: 2022 2069 6620 7820 6973 206e 702e 6e61   " if x is np.na
-0001b690: 6e20 656c 7365 2022 2022 2069 6620 7820  n else " " if x 
-0001b6a0: 3d3d 2027 2720 656c 7365 2078 2e73 706c  == '' else x.spl
-0001b6b0: 6974 2873 706c 6974 7465 7229 292e 6d61  it(splitter)).ma
-0001b6c0: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-0001b6d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001b6e0: 616d 6264 6120 6c69 7374 783a 206e 702e  ambda listx: np.
-0001b6f0: 636f 6e63 6174 656e 6174 6528 5b73 7472  concatenate([str
-0001b700: 2878 2920 6966 2078 2021 3d20 2727 2065  (x) if x != '' e
-0001b710: 6c73 6520 2220 2220 666f 7220 7820 696e  lse " " for x in
-0001b720: 206c 6973 7478 5d20 6966 2069 7369 6e73   listx] if isins
-0001b730: 7461 6e63 6528 6c69 7374 782c 6c69 7374  tance(listx,list
-0001b740: 2920 656c 7365 2022 2022 2929 2e76 616c  ) else " ")).val
-0001b750: 7565 730a 2020 2020 2020 2020 6578 6365  ues.        exce
-0001b760: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-0001b770: 7072 696e 7428 2720 2020 2045 7272 6f72  print('    Error
-0001b780: 3a20 7265 7475 726e 696e 6720 7769 7468  : returning with
-0001b790: 6f75 7420 6372 6561 7469 6e67 206e 6577  out creating new
-0001b7a0: 2063 6f6c 756d 6e27 290a 2020 2020 656c   column').    el
-0001b7b0: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
-0001b7c0: 7428 2743 6f75 6c64 206e 6f74 2070 6572  t('Could not per
-0001b7d0: 666f 726d 2061 6374 696f 6e2e 2050 6c65  form action. Ple
-0001b7e0: 6173 6520 6368 6563 6b20 796f 7572 2069  ase check your i
-0001b7f0: 6e70 7574 7320 616e 6420 7472 7920 6167  nputs and try ag
-0001b800: 6169 6e27 290a 2020 2020 2020 2020 7265  ain').        re
-0001b810: 7475 726e 2064 6674 0a20 2020 2072 6574  turn dft.    ret
-0001b820: 7572 6e20 6466 740a 2323 2323 2323 2323  urn dft.########
-0001b830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b1a0: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+0001b1b0: 2052 6574 7572 6e73 2061 2064 6174 6166   Returns a dataf
+0001b1c0: 7261 6d65 2077 6974 6820 6120 6e65 7720  rame with a new 
+0001b1d0: 636f 6c75 6d6e 2074 6861 7420 6973 2061  column that is a
+0001b1e0: 206d 6f64 6966 6963 6174 696f 6e20 6f66   modification of
+0001b1f0: 2074 6865 206f 6c64 2063 6f6c 756d 6e0a   the old column.
+0001b200: 2020 2020 2222 220a 2020 2020 6466 7420      """.    dft 
+0001b210: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
+0001b220: 6466 7429 0a20 2020 206e 6577 5f63 6f6c  dft).    new_col
+0001b230: 203d 2063 6f6c 202b 2027 5f73 706c 6974   = col + '_split
+0001b240: 5f61 7070 6c79 270a 2020 2020 7072 696e  _apply'.    prin
+0001b250: 7428 2743 7265 6174 696e 6720 636f 6c75  t('Creating colu
+0001b260: 6d6e 203d 2025 7320 7573 696e 6720 7370  mn = %s using sp
+0001b270: 6c69 745f 6164 6420 6665 6174 7572 6520  lit_add feature 
+0001b280: 656e 6769 6e65 6572 696e 672e 2e2e 2720  engineering...' 
+0001b290: 256e 6577 5f63 6f6c 290a 2020 2020 6966  %new_col).    if
+0001b2a0: 2061 6374 696f 6e20 696e 205b 272b 272c   action in ['+',
+0001b2b0: 272d 272c 272a 272c 272f 272c 2761 6464  '-','*','/','add
+0001b2c0: 272c 2773 7562 7472 6163 7427 2c27 6d75  ','subtract','mu
+0001b2d0: 6c74 6970 6c79 272c 2764 6976 6964 6527  ltiply','divide'
+0001b2e0: 5d3a 0a20 2020 2020 2020 2069 6620 6163  ]:.        if ac
+0001b2f0: 7469 6f6e 2069 6e20 5b27 6164 6427 2c27  tion in ['add','
+0001b300: 2b27 5d3a 0a20 2020 2020 2020 2020 2020  +']:.           
+0001b310: 2073 6967 6e20 3d20 272b 270a 2020 2020   sign = '+'.    
+0001b320: 2020 2020 656c 6966 2061 6374 696f 6e20      elif action 
+0001b330: 696e 205b 272d 272c 2027 7375 6274 7261  in ['-', 'subtra
+0001b340: 6374 275d 3a0a 2020 2020 2020 2020 2020  ct']:.          
+0001b350: 2020 7369 676e 203d 2027 2d27 0a20 2020    sign = '-'.   
+0001b360: 2020 2020 2065 6c69 6620 6163 7469 6f6e       elif action
+0001b370: 2069 6e20 5b27 2a27 2c20 276d 756c 7469   in ['*', 'multi
+0001b380: 706c 7927 5d3a 0a20 2020 2020 2020 2020  ply']:.         
+0001b390: 2020 2073 6967 6e20 3d20 272a 270a 2020     sign = '*'.  
+0001b3a0: 2020 2020 2020 656c 6966 2061 6374 696f        elif actio
+0001b3b0: 6e20 696e 205b 272f 272c 2027 6469 7669  n in ['/', 'divi
+0001b3c0: 6465 275d 3a0a 2020 2020 2020 2020 2020  de']:.          
+0001b3d0: 2020 7369 676e 203d 2027 2f27 0a20 2020    sign = '/'.   
+0001b3e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001b3f0: 2020 2020 2020 2073 6967 6e20 3d20 272b         sign = '+
+0001b400: 270a 2020 2020 2020 2020 2320 7573 696e  '.        # usin
+0001b410: 6720 7265 6475 6365 2074 6f20 636f 6d70  g reduce to comp
+0001b420: 7574 6520 7375 6d20 6f66 206c 6973 740a  ute sum of list.
+0001b430: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0001b440: 2020 2020 2020 2020 2074 7261 696e 7820           trainx 
+0001b450: 3d20 6466 745b 636f 6c5d 2e61 7374 7970  = dft[col].astyp
+0001b460: 6528 7374 7229 0a20 2020 2020 2020 2020  e(str).         
+0001b470: 2020 2074 7261 696e 7820 3d20 7472 6169     trainx = trai
+0001b480: 6e78 2e6d 6170 286c 616d 6264 6120 783a  nx.map(lambda x:
+0001b490: 2020 3020 6966 2078 2069 7320 6e70 2e6e    0 if x is np.n
+0001b4a0: 616e 2065 6c73 6520 3020 6966 2078 203d  an else 0 if x =
+0001b4b0: 3d20 2727 2065 6c73 6520 782e 7370 6c69  = '' else x.spli
+0001b4c0: 7428 7370 6c69 7474 6572 2929 2e6d 6170  t(splitter)).map
+0001b4d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4f0: 2020 6c61 6d62 6461 206c 6973 7478 3a20    lambda listx: 
+0001b500: 5b69 6e74 2878 2920 6966 2078 2021 3d20  [int(x) if x != 
+0001b510: 2727 2065 6c73 6520 3020 666f 7220 7820  '' else 0 for x 
+0001b520: 696e 206c 6973 7478 205d 2069 6620 6973  in listx ] if is
+0001b530: 696e 7374 616e 6365 286c 6973 7478 2c6c  instance(listx,l
+0001b540: 6973 7429 2065 6c73 6520 5b30 2c30 5d29  ist) else [0,0])
+0001b550: 0a20 2020 2020 2020 2020 2020 2064 6674  .            dft
+0001b560: 5b6e 6577 5f63 6f6c 5d20 3d20 7472 6169  [new_col] = trai
+0001b570: 6e78 2e6d 6170 286c 616d 6264 6120 6c69  nx.map(lambda li
+0001b580: 733a 2072 6564 7563 6528 6c61 6d62 6461  s: reduce(lambda
+0001b590: 2061 2c62 203a 2065 7661 6c28 2761 272b   a,b : eval('a'+
+0001b5a0: 7369 676e 2b27 6227 292c 206c 6973 2920  sign+'b'), lis) 
+0001b5b0: 6966 2069 7369 6e73 7461 6e63 6528 6c69  if isinstance(li
+0001b5c0: 732c 6c69 7374 2920 656c 7365 2030 292e  s,list) else 0).
+0001b5d0: 7661 6c75 6573 0a20 2020 2020 2020 2065  values.        e
+0001b5e0: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+0001b5f0: 2020 2070 7269 6e74 2827 2020 2020 4572     print('    Er
+0001b600: 726f 723a 2072 6574 7572 6e69 6e67 2077  ror: returning w
+0001b610: 6974 686f 7574 2063 7265 6174 696e 6720  ithout creating 
+0001b620: 6e65 7720 636f 6c75 6d6e 2729 0a20 2020  new column').   
+0001b630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001b640: 6466 740a 2020 2020 656c 6966 2061 6374  dft.    elif act
+0001b650: 696f 6e20 696e 205b 2763 6f6e 6361 7427  ion in ['concat'
+0001b660: 2c27 636f 6e63 6174 656e 6174 6527 5d3a  ,'concatenate']:
+0001b670: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0001b680: 2020 2020 2020 2020 2020 6466 745b 6e65            dft[ne
+0001b690: 775f 636f 6c5d 203d 2064 6674 5b63 6f6c  w_col] = dft[col
+0001b6a0: 5d2e 6d61 7028 6c61 6d62 6461 2078 3a20  ].map(lambda x: 
+0001b6b0: 2022 2022 2069 6620 7820 6973 206e 702e   " " if x is np.
+0001b6c0: 6e61 6e20 656c 7365 2022 2022 2069 6620  nan else " " if 
+0001b6d0: 7820 3d3d 2027 2720 656c 7365 2078 2e73  x == '' else x.s
+0001b6e0: 706c 6974 2873 706c 6974 7465 7229 292e  plit(splitter)).
+0001b6f0: 6d61 7028 0a20 2020 2020 2020 2020 2020  map(.           
+0001b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b710: 206c 616d 6264 6120 6c69 7374 783a 206e   lambda listx: n
+0001b720: 702e 636f 6e63 6174 656e 6174 6528 5b73  p.concatenate([s
+0001b730: 7472 2878 2920 6966 2078 2021 3d20 2727  tr(x) if x != ''
+0001b740: 2065 6c73 6520 2220 2220 666f 7220 7820   else " " for x 
+0001b750: 696e 206c 6973 7478 5d20 6966 2069 7369  in listx] if isi
+0001b760: 6e73 7461 6e63 6528 6c69 7374 782c 6c69  nstance(listx,li
+0001b770: 7374 2920 656c 7365 2022 2022 2929 2e76  st) else " ")).v
+0001b780: 616c 7565 730a 2020 2020 2020 2020 6578  alues.        ex
+0001b790: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0001b7a0: 2020 7072 696e 7428 2720 2020 2045 7272    print('    Err
+0001b7b0: 6f72 3a20 7265 7475 726e 696e 6720 7769  or: returning wi
+0001b7c0: 7468 6f75 7420 6372 6561 7469 6e67 206e  thout creating n
+0001b7d0: 6577 2063 6f6c 756d 6e27 290a 2020 2020  ew column').    
+0001b7e0: 656c 7365 3a0a 2020 2020 2020 2020 7072  else:.        pr
+0001b7f0: 696e 7428 2743 6f75 6c64 206e 6f74 2070  int('Could not p
+0001b800: 6572 666f 726d 2061 6374 696f 6e2e 2050  erform action. P
+0001b810: 6c65 6173 6520 6368 6563 6b20 796f 7572  lease check your
+0001b820: 2069 6e70 7574 7320 616e 6420 7472 7920   inputs and try 
+0001b830: 6167 6169 6e27 290a 2020 2020 2020 2020  again').        
+0001b840: 7265 7475 726e 2064 6674 0a20 2020 2072  return dft.    r
+0001b850: 6574 7572 6e20 6466 740a 2323 2323 2323  eturn dft.######
 0001b860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b870: 2323 2323 2323 2323 0a64 6566 2046 455f  ########.def FE_
-0001b880: 6164 645f 6167 655f 6279 5f64 6174 655f  add_age_by_date_
-0001b890: 636f 6c28 6466 742c 2064 6174 655f 636f  col(dft, date_co
-0001b8a0: 6c2c 2061 6765 5f66 6f72 6d61 7429 3a0a  l, age_format):.
-0001b8b0: 2020 2020 2222 220a 2020 2020 4645 206d      """.    FE m
-0001b8c0: 6561 6e73 2046 4541 5455 5245 2045 4e47  eans FEATURE ENG
-0001b8d0: 494e 4545 5249 4e47 202d 2054 6861 7420  INEERING - That 
-0001b8e0: 6d65 616e 7320 7468 6973 2066 756e 6374  means this funct
-0001b8f0: 696f 6e20 7769 6c6c 2063 7265 6174 6520  ion will create 
-0001b900: 6e65 7720 6665 6174 7572 6573 0a20 2020  new features.   
-0001b910: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-0001b920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b8a0: 2323 2323 2323 2323 2323 0a64 6566 2046  ##########.def F
+0001b8b0: 455f 6164 645f 6167 655f 6279 5f64 6174  E_add_age_by_dat
+0001b8c0: 655f 636f 6c28 6466 742c 2064 6174 655f  e_col(dft, date_
+0001b8d0: 636f 6c2c 2061 6765 5f66 6f72 6d61 7429  col, age_format)
+0001b8e0: 3a0a 2020 2020 2222 220a 2020 2020 4645  :.    """.    FE
+0001b8f0: 206d 6561 6e73 2046 4541 5455 5245 2045   means FEATURE E
+0001b900: 4e47 494e 4545 5249 4e47 202d 2054 6861  NGINEERING - Tha
+0001b910: 7420 6d65 616e 7320 7468 6973 2066 756e  t means this fun
+0001b920: 6374 696f 6e20 7769 6c6c 2063 7265 6174  ction will creat
+0001b930: 6520 6e65 7720 6665 6174 7572 6573 0a20  e new features. 
+0001b940: 2020 2023 2323 2323 2323 2323 2323 2323     #############
 0001b950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b960: 2323 2323 2323 230a 2020 2020 5468 6973  #######.    This
-0001b970: 2068 616e 6479 2066 756e 6374 696f 6e20   handy function 
-0001b980: 6765 7473 2079 6f75 2061 6765 2066 726f  gets you age fro
-0001b990: 6d20 7468 6520 6461 7465 5f63 6f6c 2074  m the date_col t
-0001b9a0: 6f20 746f 6461 792e 2049 7420 6361 6e20  o today. It can 
-0001b9b0: 6265 2063 6f75 6e74 6564 2069 6e20 6d6f  be counted in mo
-0001b9c0: 6e74 6873 206f 7220 7965 6172 7320 6f72  nths or years or
-0001b9d0: 2064 6179 732e 0a20 2020 2023 2323 2323   days..    #####
-0001b9e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b9f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ba00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b990: 2323 2323 2323 2323 230a 2020 2020 5468  #########.    Th
+0001b9a0: 6973 2068 616e 6479 2066 756e 6374 696f  is handy functio
+0001b9b0: 6e20 6765 7473 2079 6f75 2061 6765 2066  n gets you age f
+0001b9c0: 726f 6d20 7468 6520 6461 7465 5f63 6f6c  rom the date_col
+0001b9d0: 2074 6f20 746f 6461 792e 2049 7420 6361   to today. It ca
+0001b9e0: 6e20 6265 2063 6f75 6e74 6564 2069 6e20  n be counted in 
+0001b9f0: 6d6f 6e74 6873 206f 7220 7965 6172 7320  months or years 
+0001ba00: 6f72 2064 6179 732e 0a20 2020 2023 2323  or days..    ###
 0001ba10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001ba20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ba30: 230a 2020 2020 4974 2072 6574 7572 6e73  #.    It returns
-0001ba40: 2074 6865 2073 616d 6520 6461 7461 6672   the same datafr
-0001ba50: 616d 6520 7769 7468 2061 6e20 6578 7472  ame with an extr
-0001ba60: 6120 636f 6c75 6d6e 2061 6464 6564 2074  a column added t
-0001ba70: 6861 7420 6769 7665 7320 796f 7520 6167  hat gives you ag
-0001ba80: 650a 2020 2020 2222 220a 2020 2020 6966  e.    """.    if
-0001ba90: 206e 6f74 2061 6765 5f66 6f72 6d61 7420   not age_format 
-0001baa0: 696e 205b 274d 272c 2744 272c 2759 275d  in ['M','D','Y']
-0001bab0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-0001bac0: 2741 6765 2069 7320 6e6f 7420 6769 7665  'Age is not give
-0001bad0: 6e20 696e 2072 6967 6874 2066 6f72 6d61  n in right forma
-0001bae0: 742e 204d 7573 7420 6265 206f 6e65 206f  t. Must be one o
-0001baf0: 6620 442c 2059 206f 7220 4d27 290a 2020  f D, Y or M').  
-0001bb00: 2020 2020 2020 7265 7475 726e 2064 6674        return dft
-0001bb10: 0a20 2020 206e 6577 5f64 6174 655f 636f  .    new_date_co
-0001bb20: 6c20 3d20 276c 6173 745f 272b 6461 7465  l = 'last_'+date
-0001bb30: 5f63 6f6c 2b27 5f69 6e5f 6d6f 6e74 6873  _col+'_in_months
-0001bb40: 270a 2020 2020 7472 793a 0a20 2020 2020  '.    try:.     
-0001bb50: 2020 206e 6f77 203d 2070 642e 5469 6d65     now = pd.Time
-0001bb60: 7374 616d 7028 276e 6f77 2729 0a20 2020  stamp('now').   
-0001bb70: 2020 2020 2064 6674 5b64 6174 655f 636f       dft[date_co
-0001bb80: 6c5d 203d 2070 642e 746f 5f64 6174 6574  l] = pd.to_datet
-0001bb90: 696d 6528 6466 745b 6461 7465 5f63 6f6c  ime(dft[date_col
-0001bba0: 5d2c 2066 6f72 6d61 743d 2725 792d 256d  ], format='%y-%m
-0001bbb0: 2d25 6427 290a 2020 2020 2020 2020 6466  -%d').        df
-0001bbc0: 745b 6461 7465 5f63 6f6c 5d20 3d20 6466  t[date_col] = df
-0001bbd0: 745b 6461 7465 5f63 6f6c 5d2e 7768 6572  t[date_col].wher
-0001bbe0: 6528 6466 745b 6461 7465 5f63 6f6c 5d20  e(dft[date_col] 
-0001bbf0: 3c20 6e6f 772c 2064 6674 5b64 6174 655f  < now, dft[date_
-0001bc00: 636f 6c5d 202d 2020 6e70 2e74 696d 6564  col] -  np.timed
-0001bc10: 656c 7461 3634 2831 3030 2c20 6167 655f  elta64(100, age_
-0001bc20: 666f 726d 6174 2929 0a20 2020 2020 2020  format)).       
-0001bc30: 2069 6620 6167 655f 666f 726d 6174 203d   if age_format =
-0001bc40: 3d20 274d 273a 0a20 2020 2020 2020 2020  = 'M':.         
-0001bc50: 2020 2064 6674 5b6e 6577 5f64 6174 655f     dft[new_date_
-0001bc60: 636f 6c5d 203d 2028 6e6f 7720 2d20 6466  col] = (now - df
-0001bc70: 745b 6461 7465 5f63 6f6c 5d29 2e61 7374  t[date_col]).ast
-0001bc80: 7970 6528 273c 6d38 5b4d 5d27 290a 2020  ype('<m8[M]').  
-0001bc90: 2020 2020 2020 656c 6966 2061 6765 5f66        elif age_f
-0001bca0: 6f72 6d61 7420 3d3d 2027 5927 3a0a 2020  ormat == 'Y':.  
-0001bcb0: 2020 2020 2020 2020 2020 6466 745b 6e65            dft[ne
-0001bcc0: 775f 6461 7465 5f63 6f6c 5d20 3d20 286e  w_date_col] = (n
-0001bcd0: 6f77 202d 2064 6674 5b64 6174 655f 636f  ow - dft[date_co
-0001bce0: 6c5d 292e 6173 7479 7065 2827 3c6d 385b  l]).astype('<m8[
-0001bcf0: 595d 2729 0a20 2020 2020 2020 2065 6c69  Y]').        eli
-0001bd00: 6620 6167 655f 666f 726d 6174 203d 3d20  f age_format == 
-0001bd10: 2744 273a 0a20 2020 2020 2020 2020 2020  'D':.           
-0001bd20: 2064 6674 5b6e 6577 5f64 6174 655f 636f   dft[new_date_co
-0001bd30: 6c5d 203d 2028 6e6f 7720 2d20 6466 745b  l] = (now - dft[
-0001bd40: 6461 7465 5f63 6f6c 5d29 2e61 7374 7970  date_col]).astyp
-0001bd50: 6528 273c 6d38 5b44 5d27 290a 2020 2020  e('<m8[D]').    
-0001bd60: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-0001bd70: 7072 696e 7428 2720 2020 2045 7272 6f72  print('    Error
-0001bd80: 2069 6e20 6461 7465 2066 6f72 6d61 7474   in date formatt
-0001bd90: 696e 672e 2050 6c65 6173 6520 6368 6563  ing. Please chec
-0001bda0: 6b20 796f 7572 2069 6e70 7574 2061 6e64  k your input and
-0001bdb0: 2074 7279 2061 6761 696e 2729 0a20 2020   try again').   
-0001bdc0: 2072 6574 7572 6e20 6466 740a 2323 2323   return dft.####
-0001bdd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bde0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bdf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ba30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ba40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ba50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ba60: 2323 230a 2020 2020 4974 2072 6574 7572  ###.    It retur
+0001ba70: 6e73 2074 6865 2073 616d 6520 6461 7461  ns the same data
+0001ba80: 6672 616d 6520 7769 7468 2061 6e20 6578  frame with an ex
+0001ba90: 7472 6120 636f 6c75 6d6e 2061 6464 6564  tra column added
+0001baa0: 2074 6861 7420 6769 7665 7320 796f 7520   that gives you 
+0001bab0: 6167 650a 2020 2020 2222 220a 2020 2020  age.    """.    
+0001bac0: 6966 206e 6f74 2061 6765 5f66 6f72 6d61  if not age_forma
+0001bad0: 7420 696e 205b 274d 272c 2744 272c 2759  t in ['M','D','Y
+0001bae0: 275d 3a0a 2020 2020 2020 2020 7072 696e  ']:.        prin
+0001baf0: 7428 2741 6765 2069 7320 6e6f 7420 6769  t('Age is not gi
+0001bb00: 7665 6e20 696e 2072 6967 6874 2066 6f72  ven in right for
+0001bb10: 6d61 742e 204d 7573 7420 6265 206f 6e65  mat. Must be one
+0001bb20: 206f 6620 442c 2059 206f 7220 4d27 290a   of D, Y or M').
+0001bb30: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0001bb40: 6674 0a20 2020 206e 6577 5f64 6174 655f  ft.    new_date_
+0001bb50: 636f 6c20 3d20 276c 6173 745f 272b 6461  col = 'last_'+da
+0001bb60: 7465 5f63 6f6c 2b27 5f69 6e5f 6d6f 6e74  te_col+'_in_mont
+0001bb70: 6873 270a 2020 2020 7472 793a 0a20 2020  hs'.    try:.   
+0001bb80: 2020 2020 206e 6f77 203d 2070 642e 5469       now = pd.Ti
+0001bb90: 6d65 7374 616d 7028 276e 6f77 2729 0a20  mestamp('now'). 
+0001bba0: 2020 2020 2020 2064 6674 5b64 6174 655f         dft[date_
+0001bbb0: 636f 6c5d 203d 2070 642e 746f 5f64 6174  col] = pd.to_dat
+0001bbc0: 6574 696d 6528 6466 745b 6461 7465 5f63  etime(dft[date_c
+0001bbd0: 6f6c 5d2c 2066 6f72 6d61 743d 2725 792d  ol], format='%y-
+0001bbe0: 256d 2d25 6427 290a 2020 2020 2020 2020  %m-%d').        
+0001bbf0: 6466 745b 6461 7465 5f63 6f6c 5d20 3d20  dft[date_col] = 
+0001bc00: 6466 745b 6461 7465 5f63 6f6c 5d2e 7768  dft[date_col].wh
+0001bc10: 6572 6528 6466 745b 6461 7465 5f63 6f6c  ere(dft[date_col
+0001bc20: 5d20 3c20 6e6f 772c 2064 6674 5b64 6174  ] < now, dft[dat
+0001bc30: 655f 636f 6c5d 202d 2020 6e70 2e74 696d  e_col] -  np.tim
+0001bc40: 6564 656c 7461 3634 2831 3030 2c20 6167  edelta64(100, ag
+0001bc50: 655f 666f 726d 6174 2929 0a20 2020 2020  e_format)).     
+0001bc60: 2020 2069 6620 6167 655f 666f 726d 6174     if age_format
+0001bc70: 203d 3d20 274d 273a 0a20 2020 2020 2020   == 'M':.       
+0001bc80: 2020 2020 2064 6674 5b6e 6577 5f64 6174       dft[new_dat
+0001bc90: 655f 636f 6c5d 203d 2028 6e6f 7720 2d20  e_col] = (now - 
+0001bca0: 6466 745b 6461 7465 5f63 6f6c 5d29 2e61  dft[date_col]).a
+0001bcb0: 7374 7970 6528 273c 6d38 5b4d 5d27 290a  stype('<m8[M]').
+0001bcc0: 2020 2020 2020 2020 656c 6966 2061 6765          elif age
+0001bcd0: 5f66 6f72 6d61 7420 3d3d 2027 5927 3a0a  _format == 'Y':.
+0001bce0: 2020 2020 2020 2020 2020 2020 6466 745b              dft[
+0001bcf0: 6e65 775f 6461 7465 5f63 6f6c 5d20 3d20  new_date_col] = 
+0001bd00: 286e 6f77 202d 2064 6674 5b64 6174 655f  (now - dft[date_
+0001bd10: 636f 6c5d 292e 6173 7479 7065 2827 3c6d  col]).astype('<m
+0001bd20: 385b 595d 2729 0a20 2020 2020 2020 2065  8[Y]').        e
+0001bd30: 6c69 6620 6167 655f 666f 726d 6174 203d  lif age_format =
+0001bd40: 3d20 2744 273a 0a20 2020 2020 2020 2020  = 'D':.         
+0001bd50: 2020 2064 6674 5b6e 6577 5f64 6174 655f     dft[new_date_
+0001bd60: 636f 6c5d 203d 2028 6e6f 7720 2d20 6466  col] = (now - df
+0001bd70: 745b 6461 7465 5f63 6f6c 5d29 2e61 7374  t[date_col]).ast
+0001bd80: 7970 6528 273c 6d38 5b44 5d27 290a 2020  ype('<m8[D]').  
+0001bd90: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+0001bda0: 2020 7072 696e 7428 2720 2020 2045 7272    print('    Err
+0001bdb0: 6f72 2069 6e20 6461 7465 2066 6f72 6d61  or in date forma
+0001bdc0: 7474 696e 672e 2050 6c65 6173 6520 6368  tting. Please ch
+0001bdd0: 6563 6b20 796f 7572 2069 6e70 7574 2061  eck your input a
+0001bde0: 6e64 2074 7279 2061 6761 696e 2729 0a20  nd try again'). 
+0001bdf0: 2020 2072 6574 7572 6e20 6466 740a 2323     return dft.##
 0001be00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001be10: 2323 2323 2323 2323 2323 2323 230a 6465  #############.de
-0001be20: 6620 4645 5f63 6f75 6e74 5f72 6f77 735f  f FE_count_rows_
-0001be30: 666f 725f 616c 6c5f 636f 6c75 6d6e 735f  for_all_columns_
-0001be40: 6279 5f67 726f 7570 2864 6674 2c20 6964  by_group(dft, id
-0001be50: 5f63 6f6c 293a 0a20 2020 2022 2222 0a20  _col):.    """. 
-0001be60: 2020 2046 4520 6d65 616e 7320 4645 4154     FE means FEAT
-0001be70: 5552 4520 454e 4749 4e45 4552 494e 4720  URE ENGINEERING 
-0001be80: 2d20 5468 6174 206d 6561 6e73 2074 6869  - That means thi
-0001be90: 7320 6675 6e63 7469 6f6e 2077 696c 6c20  s function will 
-0001bea0: 6372 6561 7465 206e 6577 2066 6561 7475  create new featu
-0001beb0: 7265 730a 2020 2020 2323 2323 2323 2323  res.    ########
-0001bec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001be10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001be20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001be30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001be40: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+0001be50: 6465 6620 4645 5f63 6f75 6e74 5f72 6f77  def FE_count_row
+0001be60: 735f 666f 725f 616c 6c5f 636f 6c75 6d6e  s_for_all_column
+0001be70: 735f 6279 5f67 726f 7570 2864 6674 2c20  s_by_group(dft, 
+0001be80: 6964 5f63 6f6c 293a 0a20 2020 2022 2222  id_col):.    """
+0001be90: 0a20 2020 2046 4520 6d65 616e 7320 4645  .    FE means FE
+0001bea0: 4154 5552 4520 454e 4749 4e45 4552 494e  ATURE ENGINEERIN
+0001beb0: 4720 2d20 5468 6174 206d 6561 6e73 2074  G - That means t
+0001bec0: 6869 7320 6675 6e63 7469 6f6e 2077 696c  his function wil
+0001bed0: 6c20 6372 6561 7465 206e 6577 2066 6561  l create new fea
+0001bee0: 7475 7265 730a 2020 2020 2323 2323 2323  tures.    ######
 0001bef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bf00: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-0001bf10: 2020 2054 6869 7320 6861 6e64 7920 6675     This handy fu
-0001bf20: 6e63 7469 6f6e 2067 6976 6573 2079 6f75  nction gives you
-0001bf30: 2061 2063 6f75 6e74 206f 6620 616c 6c20   a count of all 
-0001bf40: 726f 7773 2062 7920 6772 6f75 7073 2062  rows by groups b
-0001bf50: 6173 6564 206f 6e20 6964 5f63 6f6c 2069  ased on id_col i
-0001bf60: 6e20 796f 7572 2064 6174 6166 7261 6d65  n your dataframe
-0001bf70: 2e0a 2020 2020 5265 6d65 6d62 6572 2074  ..    Remember t
-0001bf80: 6861 7420 6974 2063 6f75 6e74 7320 6f6e  hat it counts on
-0001bf90: 6c79 206e 6f6e 2d6e 756c 6c20 726f 7773  ly non-null rows
-0001bfa0: 2e20 4865 6e63 6520 6974 2069 7320 6120  . Hence it is a 
-0001bfb0: 6469 6666 6572 656e 7420 636f 756e 7420  different count 
-0001bfc0: 7468 616e 206f 7468 6572 2063 6f75 6e74  than other count
-0001bfd0: 2066 756e 6374 696f 6e2e 0a20 2020 2023   function..    #
-0001bfe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001bff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001bf00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001bf10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001bf20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001bf30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001bf40: 0a20 2020 2054 6869 7320 6861 6e64 7920  .    This handy 
+0001bf50: 6675 6e63 7469 6f6e 2067 6976 6573 2079  function gives y
+0001bf60: 6f75 2061 2063 6f75 6e74 206f 6620 616c  ou a count of al
+0001bf70: 6c20 726f 7773 2062 7920 6772 6f75 7073  l rows by groups
+0001bf80: 2062 6173 6564 206f 6e20 6964 5f63 6f6c   based on id_col
+0001bf90: 2069 6e20 796f 7572 2064 6174 6166 7261   in your datafra
+0001bfa0: 6d65 2e0a 2020 2020 5265 6d65 6d62 6572  me..    Remember
+0001bfb0: 2074 6861 7420 6974 2063 6f75 6e74 7320   that it counts 
+0001bfc0: 6f6e 6c79 206e 6f6e 2d6e 756c 6c20 726f  only non-null ro
+0001bfd0: 7773 2e20 4865 6e63 6520 6974 2069 7320  ws. Hence it is 
+0001bfe0: 6120 6469 6666 6572 656e 7420 636f 756e  a different coun
+0001bff0: 7420 7468 616e 206f 7468 6572 2063 6f75  t than other cou
+0001c000: 6e74 2066 756e 6374 696f 6e2e 0a20 2020  nt function..   
+0001c010: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
 0001c020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c030: 2323 2323 230a 2020 2020 4974 2072 6574  #####.    It ret
-0001c040: 7572 6e73 2061 2064 6174 6166 7261 6d65  urns a dataframe
-0001c050: 2077 6974 6820 6964 5f63 6f6c 2061 7320   with id_col as 
-0001c060: 7468 6520 696e 6465 7820 616e 6420 6120  the index and a 
-0001c070: 6275 6e63 6820 6f66 206e 6577 2063 6f6c  bunch of new col
-0001c080: 756d 6e73 2074 6861 7420 6769 7665 2079  umns that give y
-0001c090: 6f75 2063 6f75 6e74 7320 6f66 2067 726f  ou counts of gro
-0001c0a0: 7570 732e 0a20 2020 2022 2222 0a20 2020  ups..    """.   
-0001c0b0: 206e 6577 5f63 6f6c 203d 2027 726f 775f   new_col = 'row_
-0001c0c0: 636f 756e 745f 270a 2020 2020 6966 2069  count_'.    if i
-0001c0d0: 7369 6e73 7461 6e63 6528 6964 5f63 6f6c  sinstance(id_col
-0001c0e0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0001c0f0: 6772 6f75 7062 795f 636f 6c75 6d6e 7320  groupby_columns 
-0001c100: 3d20 205b 6964 5f63 6f6c 5d0a 2020 2020  =  [id_col].    
-0001c110: 656c 7365 3a0a 2020 2020 2020 2020 6772  else:.        gr
-0001c120: 6f75 7062 795f 636f 6c75 6d6e 7320 3d20  oupby_columns = 
-0001c130: 636f 7079 2e64 6565 7063 6f70 7928 6964  copy.deepcopy(id
-0001c140: 5f63 6f6c 290a 2020 2020 6772 6f75 7065  _col).    groupe
-0001c150: 645f 636f 756e 7420 3d20 6466 742e 6772  d_count = dft.gr
-0001c160: 6f75 7062 7928 6772 6f75 7062 795f 636f  oupby(groupby_co
-0001c170: 6c75 6d6e 7329 2e63 6f75 6e74 2829 2e61  lumns).count().a
-0001c180: 6464 5f70 7265 6669 7828 6e65 775f 636f  dd_prefix(new_co
-0001c190: 6c29 0a20 2020 2072 6574 7572 6e20 6772  l).    return gr
-0001c1a0: 6f75 7065 645f 636f 756e 740a 2323 2323  ouped_count.####
-0001c1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c060: 2323 2323 2323 230a 2020 2020 4974 2072  #######.    It r
+0001c070: 6574 7572 6e73 2061 2064 6174 6166 7261  eturns a datafra
+0001c080: 6d65 2077 6974 6820 6964 5f63 6f6c 2061  me with id_col a
+0001c090: 7320 7468 6520 696e 6465 7820 616e 6420  s the index and 
+0001c0a0: 6120 6275 6e63 6820 6f66 206e 6577 2063  a bunch of new c
+0001c0b0: 6f6c 756d 6e73 2074 6861 7420 6769 7665  olumns that give
+0001c0c0: 2079 6f75 2063 6f75 6e74 7320 6f66 2067   you counts of g
+0001c0d0: 726f 7570 732e 0a20 2020 2022 2222 0a20  roups..    """. 
+0001c0e0: 2020 206e 6577 5f63 6f6c 203d 2027 726f     new_col = 'ro
+0001c0f0: 775f 636f 756e 745f 270a 2020 2020 6966  w_count_'.    if
+0001c100: 2069 7369 6e73 7461 6e63 6528 6964 5f63   isinstance(id_c
+0001c110: 6f6c 2c20 7374 7229 3a0a 2020 2020 2020  ol, str):.      
+0001c120: 2020 6772 6f75 7062 795f 636f 6c75 6d6e    groupby_column
+0001c130: 7320 3d20 205b 6964 5f63 6f6c 5d0a 2020  s =  [id_col].  
+0001c140: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001c150: 6772 6f75 7062 795f 636f 6c75 6d6e 7320  groupby_columns 
+0001c160: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
+0001c170: 6964 5f63 6f6c 290a 2020 2020 6772 6f75  id_col).    grou
+0001c180: 7065 645f 636f 756e 7420 3d20 6466 742e  ped_count = dft.
+0001c190: 6772 6f75 7062 7928 6772 6f75 7062 795f  groupby(groupby_
+0001c1a0: 636f 6c75 6d6e 7329 2e63 6f75 6e74 2829  columns).count()
+0001c1b0: 2e61 6464 5f70 7265 6669 7828 6e65 775f  .add_prefix(new_
+0001c1c0: 636f 6c29 0a20 2020 2072 6574 7572 6e20  col).    return 
+0001c1d0: 6772 6f75 7065 645f 636f 756e 740a 2323  grouped_count.##
 0001c1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c1f0: 2323 2323 2323 2323 2323 2323 230a 6465  #############.de
-0001c200: 6620 636f 756e 745f 726f 7773 5f62 795f  f count_rows_by_
-0001c210: 6772 6f75 705f 696e 636c 5f6e 756c 6c73  group_incl_nulls
-0001c220: 2864 6674 2c20 6964 5f63 6f6c 293a 0a20  (dft, id_col):. 
-0001c230: 2020 2022 2222 0a20 2020 2023 2323 2323     """.    #####
-0001c240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c220: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+0001c230: 6465 6620 636f 756e 745f 726f 7773 5f62  def count_rows_b
+0001c240: 795f 6772 6f75 705f 696e 636c 5f6e 756c  y_group_incl_nul
+0001c250: 6c73 2864 6674 2c20 6964 5f63 6f6c 293a  ls(dft, id_col):
+0001c260: 0a20 2020 2022 2222 0a20 2020 2023 2323  .    """.    ###
 0001c270: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001c280: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c290: 230a 2020 2020 5468 6973 2066 756e 6374  #.    This funct
-0001c2a0: 696f 6e20 6769 7665 7320 796f 7520 7468  ion gives you th
-0001c2b0: 6520 636f 756e 7420 6f66 2061 6c6c 2074  e count of all t
-0001c2c0: 6865 2072 6f77 7320 696e 636c 7564 696e  he rows includin
-0001c2d0: 6720 6e75 6c6c 2072 6f77 7320 696e 2079  g null rows in y
-0001c2e0: 6f75 7220 6461 7461 2e0a 2020 2020 4974  our data..    It
-0001c2f0: 2072 6574 7572 6e73 2061 2064 6174 6166   returns a dataf
-0001c300: 7261 6d65 2077 6974 6820 6964 5f63 6f6c  rame with id_col
-0001c310: 2061 7320 7468 6520 696e 6465 7820 616e   as the index an
-0001c320: 6420 7468 6520 636f 756e 7473 206f 6620  d the counts of 
-0001c330: 726f 7773 2028 696e 636c 206e 756c 6c20  rows (incl null 
-0001c340: 726f 7773 2920 6173 2061 206e 6577 2063  rows) as a new c
-0001c350: 6f6c 756d 6e0a 2020 2020 2323 2323 2323  olumn.    ######
-0001c360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c290: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c2a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c2b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c2c0: 2323 230a 2020 2020 5468 6973 2066 756e  ###.    This fun
+0001c2d0: 6374 696f 6e20 6769 7665 7320 796f 7520  ction gives you 
+0001c2e0: 7468 6520 636f 756e 7420 6f66 2061 6c6c  the count of all
+0001c2f0: 2074 6865 2072 6f77 7320 696e 636c 7564   the rows includ
+0001c300: 696e 6720 6e75 6c6c 2072 6f77 7320 696e  ing null rows in
+0001c310: 2079 6f75 7220 6461 7461 2e0a 2020 2020   your data..    
+0001c320: 4974 2072 6574 7572 6e73 2061 2064 6174  It returns a dat
+0001c330: 6166 7261 6d65 2077 6974 6820 6964 5f63  aframe with id_c
+0001c340: 6f6c 2061 7320 7468 6520 696e 6465 7820  ol as the index 
+0001c350: 616e 6420 7468 6520 636f 756e 7473 206f  and the counts o
+0001c360: 6620 726f 7773 2028 696e 636c 206e 756c  f rows (incl nul
+0001c370: 6c20 726f 7773 2920 6173 2061 206e 6577  l rows) as a new
+0001c380: 2063 6f6c 756d 6e0a 2020 2020 2323 2323   column.    ####
 0001c390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001c3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c3b0: 0a20 2020 2022 2222 0a20 2020 206e 6577  .    """.    new
-0001c3c0: 5f63 6f6c 203d 2027 726f 775f 636f 756e  _col = 'row_coun
-0001c3d0: 745f 696e 636c 5f6e 756c 6c5f 726f 7773  t_incl_null_rows
-0001c3e0: 270a 2020 2020 6966 2069 7369 6e73 7461  '.    if isinsta
-0001c3f0: 6e63 6528 6964 5f63 6f6c 2c20 7374 7229  nce(id_col, str)
-0001c400: 3a0a 2020 2020 2020 2020 6772 6f75 7062  :.        groupb
-0001c410: 795f 636f 6c75 6d6e 7320 3d20 205b 6964  y_columns =  [id
-0001c420: 5f63 6f6c 5d0a 2020 2020 656c 7365 3a0a  _col].    else:.
-0001c430: 2020 2020 2020 2020 6772 6f75 7062 795f          groupby_
-0001c440: 636f 6c75 6d6e 7320 3d20 636f 7079 2e64  columns = copy.d
-0001c450: 6565 7063 6f70 7928 6964 5f63 6f6c 290a  eepcopy(id_col).
-0001c460: 2020 2020 2323 2320 6c65 6e20 6769 7665      ### len give
-0001c470: 7320 796f 7520 636f 756e 7420 6f66 2061  s you count of a
-0001c480: 6c6c 2074 6865 2072 6f77 7320 696e 636c  ll the rows incl
-0001c490: 7564 696e 6720 6e75 6c6c 2072 6f77 7320  uding null rows 
-0001c4a0: 696e 2079 6f75 7220 6461 7461 0a20 2020  in your data.   
-0001c4b0: 2067 726f 7570 6564 5f6c 656e 203d 2064   grouped_len = d
-0001c4c0: 6674 2e67 726f 7570 6279 2867 726f 7570  ft.groupby(group
-0001c4d0: 6279 5f63 6f6c 756d 6e73 292e 6170 706c  by_columns).appl
-0001c4e0: 7928 6c65 6e29 0a20 2020 2067 726f 7570  y(len).    group
-0001c4f0: 6564 5f76 616c 203d 2067 726f 7570 6564  ed_val = grouped
-0001c500: 5f6c 656e 2e76 616c 7565 730a 2020 2020  _len.values.    
-0001c510: 6772 6f75 7065 645f 6c65 6e20 3d20 7064  grouped_len = pd
-0001c520: 2e44 6174 6146 7261 6d65 2867 726f 7570  .DataFrame(group
-0001c530: 6564 5f76 616c 2c20 636f 6c75 6d6e 733d  ed_val, columns=
-0001c540: 5b6e 6577 5f63 6f6c 5d2c 696e 6465 783d  [new_col],index=
-0001c550: 6772 6f75 7065 645f 6c65 6e2e 696e 6465  grouped_len.inde
-0001c560: 7829 0a20 2020 2072 6574 7572 6e20 6772  x).    return gr
-0001c570: 6f75 7065 645f 6c65 6e0a 2323 2323 2323  ouped_len.######
-0001c580: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c5a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c3b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c3c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c3d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c3e0: 2323 0a20 2020 2022 2222 0a20 2020 206e  ##.    """.    n
+0001c3f0: 6577 5f63 6f6c 203d 2027 726f 775f 636f  ew_col = 'row_co
+0001c400: 756e 745f 696e 636c 5f6e 756c 6c5f 726f  unt_incl_null_ro
+0001c410: 7773 270a 2020 2020 6966 2069 7369 6e73  ws'.    if isins
+0001c420: 7461 6e63 6528 6964 5f63 6f6c 2c20 7374  tance(id_col, st
+0001c430: 7229 3a0a 2020 2020 2020 2020 6772 6f75  r):.        grou
+0001c440: 7062 795f 636f 6c75 6d6e 7320 3d20 205b  pby_columns =  [
+0001c450: 6964 5f63 6f6c 5d0a 2020 2020 656c 7365  id_col].    else
+0001c460: 3a0a 2020 2020 2020 2020 6772 6f75 7062  :.        groupb
+0001c470: 795f 636f 6c75 6d6e 7320 3d20 636f 7079  y_columns = copy
+0001c480: 2e64 6565 7063 6f70 7928 6964 5f63 6f6c  .deepcopy(id_col
+0001c490: 290a 2020 2020 2323 2320 6c65 6e20 6769  ).    ### len gi
+0001c4a0: 7665 7320 796f 7520 636f 756e 7420 6f66  ves you count of
+0001c4b0: 2061 6c6c 2074 6865 2072 6f77 7320 696e   all the rows in
+0001c4c0: 636c 7564 696e 6720 6e75 6c6c 2072 6f77  cluding null row
+0001c4d0: 7320 696e 2079 6f75 7220 6461 7461 0a20  s in your data. 
+0001c4e0: 2020 2067 726f 7570 6564 5f6c 656e 203d     grouped_len =
+0001c4f0: 2064 6674 2e67 726f 7570 6279 2867 726f   dft.groupby(gro
+0001c500: 7570 6279 5f63 6f6c 756d 6e73 292e 6170  upby_columns).ap
+0001c510: 706c 7928 6c65 6e29 0a20 2020 2067 726f  ply(len).    gro
+0001c520: 7570 6564 5f76 616c 203d 2067 726f 7570  uped_val = group
+0001c530: 6564 5f6c 656e 2e76 616c 7565 730a 2020  ed_len.values.  
+0001c540: 2020 6772 6f75 7065 645f 6c65 6e20 3d20    grouped_len = 
+0001c550: 7064 2e44 6174 6146 7261 6d65 2867 726f  pd.DataFrame(gro
+0001c560: 7570 6564 5f76 616c 2c20 636f 6c75 6d6e  uped_val, column
+0001c570: 733d 5b6e 6577 5f63 6f6c 5d2c 696e 6465  s=[new_col],inde
+0001c580: 783d 6772 6f75 7065 645f 6c65 6e2e 696e  x=grouped_len.in
+0001c590: 6465 7829 0a20 2020 2072 6574 7572 6e20  dex).    return 
+0001c5a0: 6772 6f75 7065 645f 6c65 6e0a 2323 2323  grouped_len.####
 0001c5b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c5c0: 2323 2323 2323 2323 2323 230a 2320 4361  ###########.# Ca
-0001c5d0: 6e20 7765 2073 6565 2069 6620 6120 6665  n we see if a fe
-0001c5e0: 6174 7572 6520 6f72 2066 6561 7475 7265  ature or feature
-0001c5f0: 7320 6861 7320 736f 6d65 206f 7574 6c69  s has some outli
-0001c600: 6572 7320 616e 6420 686f 7720 6361 6e20  ers and how can 
-0001c610: 7765 2063 6170 2074 6865 6d3f 0a66 726f  we cap them?.fro
-0001c620: 6d20 636f 6c6c 6563 7469 6f6e 7320 696d  m collections im
-0001c630: 706f 7274 2043 6f75 6e74 6572 0a64 6566  port Counter.def
-0001c640: 2046 455f 6361 7070 696e 675f 6f75 746c   FE_capping_outl
-0001c650: 6965 7273 5f62 6579 6f6e 645f 4951 525f  iers_beyond_IQR_
-0001c660: 5261 6e67 6528 6466 2c20 6665 6174 7572  Range(df, featur
-0001c670: 6573 2c20 6361 705f 6174 5f6e 7468 5f6c  es, cap_at_nth_l
-0001c680: 6172 6765 7374 3d35 2c20 4951 525f 6d75  argest=5, IQR_mu
-0001c690: 6c74 6970 6c69 6572 3d31 2e35 2c0a 2020  ltiplier=1.5,.  
-0001c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6c0: 2020 2020 2020 2064 726f 703d 4661 6c73         drop=Fals
-0001c6d0: 652c 2076 6572 626f 7365 3d46 616c 7365  e, verbose=False
-0001c6e0: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
-0001c6f0: 4520 6174 2074 6865 2062 6567 696e 6e69  E at the beginni
-0001c700: 6e67 206f 6620 6675 6e63 7469 6f6e 206e  ng of function n
-0001c710: 616d 6520 7374 616e 6473 2066 6f72 2046  ame stands for F
-0001c720: 6561 7475 7265 2045 6e67 696e 6565 7269  eature Engineeri
-0001c730: 6e67 2e20 4645 2066 756e 6374 696f 6e73  ng. FE functions
-0001c740: 2061 6464 206f 7220 6472 6f70 2066 6561   add or drop fea
-0001c750: 7475 7265 732e 0a20 2020 2023 2323 2323  tures..    #####
-0001c760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c5c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c5d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c5e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c5f0: 2323 2323 2323 2323 2323 2323 230a 2320  #############.# 
+0001c600: 4361 6e20 7765 2073 6565 2069 6620 6120  Can we see if a 
+0001c610: 6665 6174 7572 6520 6f72 2066 6561 7475  feature or featu
+0001c620: 7265 7320 6861 7320 736f 6d65 206f 7574  res has some out
+0001c630: 6c69 6572 7320 616e 6420 686f 7720 6361  liers and how ca
+0001c640: 6e20 7765 2063 6170 2074 6865 6d3f 0a66  n we cap them?.f
+0001c650: 726f 6d20 636f 6c6c 6563 7469 6f6e 7320  rom collections 
+0001c660: 696d 706f 7274 2043 6f75 6e74 6572 0a64  import Counter.d
+0001c670: 6566 2046 455f 6361 7070 696e 675f 6f75  ef FE_capping_ou
+0001c680: 746c 6965 7273 5f62 6579 6f6e 645f 4951  tliers_beyond_IQ
+0001c690: 525f 5261 6e67 6528 6466 2c20 6665 6174  R_Range(df, feat
+0001c6a0: 7572 6573 2c20 6361 705f 6174 5f6e 7468  ures, cap_at_nth
+0001c6b0: 5f6c 6172 6765 7374 3d35 2c20 4951 525f  _largest=5, IQR_
+0001c6c0: 6d75 6c74 6970 6c69 6572 3d31 2e35 2c0a  multiplier=1.5,.
+0001c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c6f0: 2020 2020 2020 2020 2064 726f 703d 4661           drop=Fa
+0001c700: 6c73 652c 2076 6572 626f 7365 3d46 616c  lse, verbose=Fal
+0001c710: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
+0001c720: 2046 4520 6174 2074 6865 2062 6567 696e   FE at the begin
+0001c730: 6e69 6e67 206f 6620 6675 6e63 7469 6f6e  ning of function
+0001c740: 206e 616d 6520 7374 616e 6473 2066 6f72   name stands for
+0001c750: 2046 6561 7475 7265 2045 6e67 696e 6565   Feature Enginee
+0001c760: 7269 6e67 2e20 4645 2066 756e 6374 696f  ring. FE functio
+0001c770: 6e73 2061 6464 206f 7220 6472 6f70 2066  ns add or drop f
+0001c780: 6561 7475 7265 732e 0a20 2020 2023 2323  eatures..    ###
 0001c790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001c7a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001c7b0: 2323 2323 0a20 2020 2054 7970 6963 616c  ####.    Typical
-0001c7c0: 6c79 2077 6520 7468 696e 6b20 6f66 206f  ly we think of o
-0001c7d0: 7574 6c69 6572 7320 6173 2062 6569 6e67  utliers as being
-0001c7e0: 206f 6273 6572 7661 7469 6f6e 7320 6265   observations be
-0001c7f0: 796f 6e64 2074 6865 2031 2e35 2049 6e74  yond the 1.5 Int
-0001c800: 6572 2051 7561 7274 696c 6520 5261 6e67  er Quartile Rang
-0001c810: 6520 2849 5152 290a 2020 2020 4275 7420  e (IQR).    But 
-0001c820: 7468 6973 2066 756e 6374 696f 6e20 7769  this function wi
-0001c830: 6c6c 2061 6c6c 6f77 2079 6f75 2074 6f20  ll allow you to 
-0001c840: 6361 7020 616e 7920 6f62 7365 7276 6174  cap any observat
-0001c850: 696f 6e20 7468 6174 2069 7320 6d75 6c74  ion that is mult
-0001c860: 6970 6c65 206f 6620 4951 5220 7261 6e67  iple of IQR rang
-0001c870: 652c 2073 7563 6820 6173 2031 2e35 2c20  e, such as 1.5, 
-0001c880: 322c 2065 7463 2e0a 2020 2020 496e 2061  2, etc..    In a
-0001c890: 6464 6974 696f 6e2c 2074 6869 7320 7574  ddition, this ut
-0001c8a0: 696c 6974 7920 6865 6c70 7320 796f 7520  ility helps you 
-0001c8b0: 7365 6c65 6374 2074 6865 2076 616c 7565  select the value
-0001c8c0: 2074 6f20 6361 7020 6974 2061 742e 0a20   to cap it at.. 
-0001c8d0: 2020 2054 6865 2076 616c 7565 2074 6f20     The value to 
-0001c8e0: 6265 2063 6170 7065 6420 6973 2062 6173  be capped is bas
-0001c8f0: 6564 206f 6e20 226e 2220 7468 6174 2079  ed on "n" that y
-0001c900: 6f75 2069 6e70 7574 2e0a 2020 2020 6e20  ou input..    n 
-0001c910: 7265 7072 6573 656e 7473 2074 6865 206e  represents the n
-0001c920: 7468 5f6c 6172 6765 7374 206e 756d 6265  th_largest numbe
-0001c930: 7220 6265 6c6f 7720 7468 6520 6d61 7869  r below the maxi
-0001c940: 6d75 6d20 7661 6c75 6520 746f 2063 6170  mum value to cap
-0001c950: 2061 7421 0a20 2020 204e 6f74 6963 6520   at!.    Notice 
-0001c960: 7468 6174 2069 7420 646f 6573 206e 6f74  that it does not
-0001c970: 2070 7574 2061 2066 6c6f 6f72 2075 6e64   put a floor und
-0001c980: 6572 206d 696e 696d 756d 732e 2059 6f75  er minimums. You
-0001c990: 2068 6176 6520 746f 2064 6f20 7468 6174   have to do that
-0001c9a0: 2079 6f75 7273 656c 662e 0a20 2020 2022   yourself..    "
-0001c9b0: 6361 705f 6174 5f6e 7468 5f6c 6172 6765  cap_at_nth_large
-0001c9c0: 7374 2220 7370 6563 6966 6965 7320 7468  st" specifies th
-0001c9d0: 6520 6d61 7820 6e75 6d62 6572 2062 656c  e max number bel
-0001c9e0: 6f77 2074 6865 206c 6172 6765 7374 2028  ow the largest (
-0001c9f0: 6d61 7829 206e 756d 6265 7220 696e 2079  max) number in y
-0001ca00: 6f75 7220 636f 6c75 6d6e 2074 6f20 6361  our column to ca
-0001ca10: 7020 7468 6174 2066 6561 7475 7265 2e0a  p that feature..
-0001ca20: 2020 2020 4f70 7469 6f6e 616c 6c79 2c20      Optionally, 
-0001ca30: 796f 7520 6361 6e20 6472 6f70 2063 6572  you can drop cer
-0001ca40: 7461 696e 206f 6273 6572 7661 7469 6f6e  tain observation
-0001ca50: 7320 7468 6174 2068 6176 6520 746f 6f20  s that have too 
-0001ca60: 6d61 6e79 206f 7574 6c69 6572 7320 696e  many outliers in
-0001ca70: 2061 7420 6c65 6173 7420 3320 636f 6c75   at least 3 colu
-0001ca80: 6d6e 732e 0a20 2020 2023 2323 2323 2323  mns..    #######
-0001ca90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001caa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001cab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c7b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c7c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c7d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001c7e0: 2323 2323 2323 0a20 2020 2054 7970 6963  ######.    Typic
+0001c7f0: 616c 6c79 2077 6520 7468 696e 6b20 6f66  ally we think of
+0001c800: 206f 7574 6c69 6572 7320 6173 2062 6569   outliers as bei
+0001c810: 6e67 206f 6273 6572 7661 7469 6f6e 7320  ng observations 
+0001c820: 6265 796f 6e64 2074 6865 2031 2e35 2049  beyond the 1.5 I
+0001c830: 6e74 6572 2051 7561 7274 696c 6520 5261  nter Quartile Ra
+0001c840: 6e67 6520 2849 5152 290a 2020 2020 4275  nge (IQR).    Bu
+0001c850: 7420 7468 6973 2066 756e 6374 696f 6e20  t this function 
+0001c860: 7769 6c6c 2061 6c6c 6f77 2079 6f75 2074  will allow you t
+0001c870: 6f20 6361 7020 616e 7920 6f62 7365 7276  o cap any observ
+0001c880: 6174 696f 6e20 7468 6174 2069 7320 6d75  ation that is mu
+0001c890: 6c74 6970 6c65 206f 6620 4951 5220 7261  ltiple of IQR ra
+0001c8a0: 6e67 652c 2073 7563 6820 6173 2031 2e35  nge, such as 1.5
+0001c8b0: 2c20 322c 2065 7463 2e0a 2020 2020 496e  , 2, etc..    In
+0001c8c0: 2061 6464 6974 696f 6e2c 2074 6869 7320   addition, this 
+0001c8d0: 7574 696c 6974 7920 6865 6c70 7320 796f  utility helps yo
+0001c8e0: 7520 7365 6c65 6374 2074 6865 2076 616c  u select the val
+0001c8f0: 7565 2074 6f20 6361 7020 6974 2061 742e  ue to cap it at.
+0001c900: 0a20 2020 2054 6865 2076 616c 7565 2074  .    The value t
+0001c910: 6f20 6265 2063 6170 7065 6420 6973 2062  o be capped is b
+0001c920: 6173 6564 206f 6e20 226e 2220 7468 6174  ased on "n" that
+0001c930: 2079 6f75 2069 6e70 7574 2e0a 2020 2020   you input..    
+0001c940: 6e20 7265 7072 6573 656e 7473 2074 6865  n represents the
+0001c950: 206e 7468 5f6c 6172 6765 7374 206e 756d   nth_largest num
+0001c960: 6265 7220 6265 6c6f 7720 7468 6520 6d61  ber below the ma
+0001c970: 7869 6d75 6d20 7661 6c75 6520 746f 2063  ximum value to c
+0001c980: 6170 2061 7421 0a20 2020 204e 6f74 6963  ap at!.    Notic
+0001c990: 6520 7468 6174 2069 7420 646f 6573 206e  e that it does n
+0001c9a0: 6f74 2070 7574 2061 2066 6c6f 6f72 2075  ot put a floor u
+0001c9b0: 6e64 6572 206d 696e 696d 756d 732e 2059  nder minimums. Y
+0001c9c0: 6f75 2068 6176 6520 746f 2064 6f20 7468  ou have to do th
+0001c9d0: 6174 2079 6f75 7273 656c 662e 0a20 2020  at yourself..   
+0001c9e0: 2022 6361 705f 6174 5f6e 7468 5f6c 6172   "cap_at_nth_lar
+0001c9f0: 6765 7374 2220 7370 6563 6966 6965 7320  gest" specifies 
+0001ca00: 7468 6520 6d61 7820 6e75 6d62 6572 2062  the max number b
+0001ca10: 656c 6f77 2074 6865 206c 6172 6765 7374  elow the largest
+0001ca20: 2028 6d61 7829 206e 756d 6265 7220 696e   (max) number in
+0001ca30: 2079 6f75 7220 636f 6c75 6d6e 2074 6f20   your column to 
+0001ca40: 6361 7020 7468 6174 2066 6561 7475 7265  cap that feature
+0001ca50: 2e0a 2020 2020 4f70 7469 6f6e 616c 6c79  ..    Optionally
+0001ca60: 2c20 796f 7520 6361 6e20 6472 6f70 2063  , you can drop c
+0001ca70: 6572 7461 696e 206f 6273 6572 7661 7469  ertain observati
+0001ca80: 6f6e 7320 7468 6174 2068 6176 6520 746f  ons that have to
+0001ca90: 6f20 6d61 6e79 206f 7574 6c69 6572 7320  o many outliers 
+0001caa0: 696e 2061 7420 6c65 6173 7420 3320 636f  in at least 3 co
+0001cab0: 6c75 6d6e 732e 0a20 2020 2023 2323 2323  lumns..    #####
 0001cac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001cad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001cae0: 2323 0a20 2020 2049 6e70 7574 733a 0a20  ##.    Inputs:. 
-0001caf0: 2020 2064 6620 3a20 7061 6e64 6173 2044     df : pandas D
-0001cb00: 6174 6146 7261 6d65 0a20 2020 2066 6561  ataFrame.    fea
-0001cb10: 7475 7265 733a 2061 2073 696e 676c 6520  tures: a single 
-0001cb20: 636f 6c75 6d6e 206f 7220 6120 6c69 7374  column or a list
-0001cb30: 206f 6620 636f 6c75 6d6e 7320 696e 2079   of columns in y
-0001cb40: 6f75 7220 4461 7461 4672 616d 650a 2020  our DataFrame.  
-0001cb50: 2020 6361 705f 6174 5f6e 7468 5f6c 6172    cap_at_nth_lar
-0001cb60: 6765 7374 3a20 6465 6661 756c 7420 6973  gest: default is
-0001cb70: 2035 203d 2079 6f75 2063 616e 2073 6574   5 = you can set
-0001cb80: 2069 7420 746f 2061 6e79 2069 6e74 6567   it to any integ
-0001cb90: 6572 2073 7563 6820 6173 2031 2c20 322c  er such as 1, 2,
-0001cba0: 2033 2c20 342c 2035 2c20 6574 632e 0a20   3, 4, 5, etc.. 
-0001cbb0: 2020 2049 5152 5f6d 756c 7469 706c 6965     IQR_multiplie
-0001cbc0: 723a 2064 6566 6175 6c74 2069 7320 312e  r: default is 1.
-0001cbd0: 3520 3d20 6275 7420 796f 7520 6361 6e20  5 = but you can 
-0001cbe0: 7365 7420 6974 2074 6f20 616e 7920 666c  set it to any fl
-0001cbf0: 6f61 7420 7661 6c75 6520 7375 6368 2061  oat value such a
-0001cc00: 7320 312c 2031 2e32 352e 2031 2e35 2c20  s 1, 1.25. 1.5, 
-0001cc10: 322e 302c 2065 7463 2e0a 0a20 2020 204f  2.0, etc...    O
-0001cc20: 7574 7075 7473 3a0a 2020 2020 6466 3a20  utputs:.    df: 
-0001cc30: 7061 6e64 6173 2044 6174 6146 7261 6d65  pandas DataFrame
-0001cc40: 0a20 2020 2049 7420 7265 7475 726e 7320  .    It returns 
-0001cc50: 7468 6520 7361 6d65 2064 6174 6166 7261  the same datafra
-0001cc60: 6d65 2061 7320 796f 7520 696e 7075 7420  me as you input 
-0001cc70: 756e 6c65 7373 2079 6f75 2063 6861 6e67  unless you chang
-0001cc80: 6520 6472 6f70 2074 6f20 5472 7565 2069  e drop to True i
-0001cc90: 6e20 7468 6520 696e 7075 7420 6172 6775  n the input argu
-0001cca0: 6d65 6e74 2e0a 0a20 2020 204f 7074 696f  ment...    Optio
-0001ccb0: 6e61 6c6c 792c 2069 7420 6361 6e20 6472  nally, it can dr
-0001ccc0: 6f70 2063 6572 7461 696e 2072 6f77 7320  op certain rows 
-0001ccd0: 7468 6174 2068 6176 6520 746f 6f20 6d61  that have too ma
-0001cce0: 6e79 206f 7574 6c69 6572 7320 696e 2061  ny outliers in a
-0001ccf0: 7420 6c65 6173 7420 3320 636f 6c75 6d6e  t least 3 column
-0001cd00: 7320 7369 6d75 6c74 616e 656f 7573 6c79  s simultaneously
-0001cd10: 2e0a 2020 2020 4966 2064 726f 703d 5472  ..    If drop=Tr
-0001cd20: 7565 2c20 6974 2077 696c 6c20 7265 7475  ue, it will retu
-0001cd30: 726e 2061 2073 6d61 6c6c 6572 206e 756d  rn a smaller num
-0001cd40: 6265 7220 6f66 2072 6f77 7320 696e 2079  ber of rows in y
-0001cd50: 6f75 7220 6461 7461 6672 616d 6520 7468  our dataframe th
-0001cd60: 616e 2077 6861 7420 796f 7520 7365 6e74  an what you sent
-0001cd70: 2069 6e2e 2042 6520 6361 7265 6675 6c21   in. Be careful!
-0001cd80: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-0001cd90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001cda0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001cdb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001cae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001caf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001cb00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001cb10: 2323 2323 0a20 2020 2049 6e70 7574 733a  ####.    Inputs:
+0001cb20: 0a20 2020 2064 6620 3a20 7061 6e64 6173  .    df : pandas
+0001cb30: 2044 6174 6146 7261 6d65 0a20 2020 2066   DataFrame.    f
+0001cb40: 6561 7475 7265 733a 2061 2073 696e 676c  eatures: a singl
+0001cb50: 6520 636f 6c75 6d6e 206f 7220 6120 6c69  e column or a li
+0001cb60: 7374 206f 6620 636f 6c75 6d6e 7320 696e  st of columns in
+0001cb70: 2079 6f75 7220 4461 7461 4672 616d 650a   your DataFrame.
+0001cb80: 2020 2020 6361 705f 6174 5f6e 7468 5f6c      cap_at_nth_l
+0001cb90: 6172 6765 7374 3a20 6465 6661 756c 7420  argest: default 
+0001cba0: 6973 2035 203d 2079 6f75 2063 616e 2073  is 5 = you can s
+0001cbb0: 6574 2069 7420 746f 2061 6e79 2069 6e74  et it to any int
+0001cbc0: 6567 6572 2073 7563 6820 6173 2031 2c20  eger such as 1, 
+0001cbd0: 322c 2033 2c20 342c 2035 2c20 6574 632e  2, 3, 4, 5, etc.
+0001cbe0: 0a20 2020 2049 5152 5f6d 756c 7469 706c  .    IQR_multipl
+0001cbf0: 6965 723a 2064 6566 6175 6c74 2069 7320  ier: default is 
+0001cc00: 312e 3520 3d20 6275 7420 796f 7520 6361  1.5 = but you ca
+0001cc10: 6e20 7365 7420 6974 2074 6f20 616e 7920  n set it to any 
+0001cc20: 666c 6f61 7420 7661 6c75 6520 7375 6368  float value such
+0001cc30: 2061 7320 312c 2031 2e32 352e 2031 2e35   as 1, 1.25. 1.5
+0001cc40: 2c20 322e 302c 2065 7463 2e0a 0a20 2020  , 2.0, etc...   
+0001cc50: 204f 7574 7075 7473 3a0a 2020 2020 6466   Outputs:.    df
+0001cc60: 3a20 7061 6e64 6173 2044 6174 6146 7261  : pandas DataFra
+0001cc70: 6d65 0a20 2020 2049 7420 7265 7475 726e  me.    It return
+0001cc80: 7320 7468 6520 7361 6d65 2064 6174 6166  s the same dataf
+0001cc90: 7261 6d65 2061 7320 796f 7520 696e 7075  rame as you inpu
+0001cca0: 7420 756e 6c65 7373 2079 6f75 2063 6861  t unless you cha
+0001ccb0: 6e67 6520 6472 6f70 2074 6f20 5472 7565  nge drop to True
+0001ccc0: 2069 6e20 7468 6520 696e 7075 7420 6172   in the input ar
+0001ccd0: 6775 6d65 6e74 2e0a 0a20 2020 204f 7074  gument...    Opt
+0001cce0: 696f 6e61 6c6c 792c 2069 7420 6361 6e20  ionally, it can 
+0001ccf0: 6472 6f70 2063 6572 7461 696e 2072 6f77  drop certain row
+0001cd00: 7320 7468 6174 2068 6176 6520 746f 6f20  s that have too 
+0001cd10: 6d61 6e79 206f 7574 6c69 6572 7320 696e  many outliers in
+0001cd20: 2061 7420 6c65 6173 7420 3320 636f 6c75   at least 3 colu
+0001cd30: 6d6e 7320 7369 6d75 6c74 616e 656f 7573  mns simultaneous
+0001cd40: 6c79 2e0a 2020 2020 4966 2064 726f 703d  ly..    If drop=
+0001cd50: 5472 7565 2c20 6974 2077 696c 6c20 7265  True, it will re
+0001cd60: 7475 726e 2061 2073 6d61 6c6c 6572 206e  turn a smaller n
+0001cd70: 756d 6265 7220 6f66 2072 6f77 7320 696e  umber of rows in
+0001cd80: 2079 6f75 7220 6461 7461 6672 616d 6520   your dataframe 
+0001cd90: 7468 616e 2077 6861 7420 796f 7520 7365  than what you se
+0001cda0: 6e74 2069 6e2e 2042 6520 6361 7265 6675  nt in. Be carefu
+0001cdb0: 6c21 0a20 2020 2023 2323 2323 2323 2323  l!.    #########
 0001cdc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001cdd0: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-0001cde0: 2020 2022 2222 0a20 2020 206f 7574 6c69     """.    outli
-0001cdf0: 6572 5f69 6e64 6963 6573 203d 205b 5d0a  er_indices = [].
-0001ce00: 2020 2020 6466 203d 2064 662e 636f 7079      df = df.copy
-0001ce10: 2864 6565 703d 5472 7565 290a 2020 2020  (deep=True).    
-0001ce20: 6966 2069 7369 6e73 7461 6e63 6528 6665  if isinstance(fe
-0001ce30: 6174 7572 6573 2c20 7374 7229 3a0a 2020  atures, str):.  
-0001ce40: 2020 2020 2020 6665 6174 7572 6573 203d        features =
-0001ce50: 205b 6665 6174 7572 6573 5d0a 2020 2020   [features].    
-0001ce60: 2320 6974 6572 6174 6520 6f76 6572 2066  # iterate over f
-0001ce70: 6561 7475 7265 7328 636f 6c75 6d6e 7329  eatures(columns)
-0001ce80: 0a20 2020 2066 6f72 2063 6f6c 2069 6e20  .    for col in 
-0001ce90: 6665 6174 7572 6573 3a0a 2020 2020 2020  features:.      
-0001cea0: 2020 2323 2320 7468 6973 2069 7320 686f    ### this is ho
-0001ceb0: 7720 7468 6520 636f 6c75 6d6e 206c 6f6f  w the column loo
-0001cec0: 6b73 206e 6f77 2062 6566 6f72 6520 6361  ks now before ca
-0001ced0: 7070 696e 6720 6f75 746c 6965 7273 0a20  pping outliers. 
-0001cee0: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-0001cef0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-0001cf00: 6967 2c20 2861 7831 2c61 7832 2920 3d20  ig, (ax1,ax2) = 
-0001cf10: 706c 742e 7375 6270 6c6f 7473 2831 2c32  plt.subplots(1,2
-0001cf20: 2c66 6967 7369 7a65 3d28 3132 2c35 2929  ,figsize=(12,5))
-0001cf30: 0a20 2020 2020 2020 2020 2020 2064 665b  .            df[
-0001cf40: 636f 6c5d 2e70 6c6f 7428 6b69 6e64 3d27  col].plot(kind='
-0001cf50: 626f 7827 2c20 7469 746c 6520 3d20 2725  box', title = '%
-0001cf60: 7320 6265 666f 7265 2063 6170 7069 6e67  s before capping
-0001cf70: 206f 7574 6c69 6572 7327 2025 636f 6c2c   outliers' %col,
-0001cf80: 2061 783d 6178 3129 0a20 2020 2020 2020   ax=ax1).       
-0001cf90: 2023 2031 7374 2071 7561 7274 696c 6520   # 1st quartile 
-0001cfa0: 2832 3525 290a 2020 2020 2020 2020 5131  (25%).        Q1
-0001cfb0: 203d 206e 702e 7065 7263 656e 7469 6c65   = np.percentile
-0001cfc0: 2864 665b 636f 6c5d 2c20 3235 290a 2020  (df[col], 25).  
-0001cfd0: 2020 2020 2020 2320 3372 6420 7175 6172        # 3rd quar
-0001cfe0: 7469 6c65 2028 3735 2529 0a20 2020 2020  tile (75%).     
-0001cff0: 2020 2051 3320 3d20 6e70 2e70 6572 6365     Q3 = np.perce
-0001d000: 6e74 696c 6528 6466 5b63 6f6c 5d2c 3735  ntile(df[col],75
-0001d010: 290a 2020 2020 2020 2020 2320 496e 7465  ).        # Inte
-0001d020: 7271 7561 7274 696c 6520 7261 6e67 6520  rquartile range 
-0001d030: 2849 5152 290a 2020 2020 2020 2020 4951  (IQR).        IQ
-0001d040: 5220 3d20 5133 202d 2051 310a 0a20 2020  R = Q3 - Q1..   
-0001d050: 2020 2020 2023 206f 7574 6c69 6572 2073       # outlier s
-0001d060: 7465 7020 7573 696e 6720 6d75 6c74 6970  tep using multip
-0001d070: 6c69 6572 0a20 2020 2020 2020 206f 7574  lier.        out
-0001d080: 6c69 6572 5f73 7465 7020 3d20 4951 525f  lier_step = IQR_
-0001d090: 6d75 6c74 6970 6c69 6572 202a 2049 5152  multiplier * IQR
-0001d0a0: 0a0a 2020 2020 2020 2020 6c6f 7765 725f  ..        lower_
-0001d0b0: 6c69 6d69 7420 3d20 5131 202d 206f 7574  limit = Q1 - out
-0001d0c0: 6c69 6572 5f73 7465 700a 2020 2020 2020  lier_step.      
-0001d0d0: 2020 7570 7065 725f 6c69 6d69 7420 3d20    upper_limit = 
-0001d0e0: 5133 202b 206f 7574 6c69 6572 5f73 7465  Q3 + outlier_ste
-0001d0f0: 700a 0a20 2020 2020 2020 2023 2044 6574  p..        # Det
-0001d100: 6572 6d69 6e65 2061 206c 6973 7420 6f66  ermine a list of
-0001d110: 2069 6e64 6963 6573 206f 6620 6f75 746c   indices of outl
-0001d120: 6965 7273 2066 6f72 2066 6561 7475 7265  iers for feature
-0001d130: 2063 6f6c 0a20 2020 2020 2020 206f 7574   col.        out
-0001d140: 6c69 6572 5f6c 6973 745f 636f 6c20 3d20  lier_list_col = 
-0001d150: 6466 5b28 6466 5b63 6f6c 5d20 3c20 6c6f  df[(df[col] < lo
-0001d160: 7765 725f 6c69 6d69 7429 207c 2028 6466  wer_limit) | (df
-0001d170: 5b63 6f6c 5d20 3e20 7570 7065 725f 6c69  [col] > upper_li
-0001d180: 6d69 7420 295d 2e69 6e64 6578 0a0a 2020  mit )].index..  
-0001d190: 2020 2020 2020 2323 2320 4361 7070 696e        ### Cappin
-0001d1a0: 6720 7573 696e 6720 7468 6520 6e20 6c61  g using the n la
-0001d1b0: 7267 6573 7420 7661 6c75 6520 6261 7365  rgest value base
-0001d1c0: 6420 6f6e 206e 2067 6976 656e 2069 6e20  d on n given in 
-0001d1d0: 696e 7075 742e 0a20 2020 2020 2020 206d  input..        m
-0001d1e0: 6178 7661 6c20 3d20 6466 5b63 6f6c 5d2e  axval = df[col].
-0001d1f0: 6d61 7828 2920 2023 2320 7768 6174 2069  max()  ## what i
-0001d200: 7320 7468 6520 6d61 7869 6d75 6d20 7661  s the maximum va
-0001d210: 6c75 6520 696e 2074 6869 7320 636f 6c75  lue in this colu
-0001d220: 6d6e 3f0a 2020 2020 2020 2020 6e75 6d5f  mn?.        num_
-0001d230: 6d61 7873 203d 2064 665b 6466 5b63 6f6c  maxs = df[df[col
-0001d240: 5d3d 3d6d 6178 7661 6c5d 2e73 6861 7065  ]==maxval].shape
-0001d250: 5b30 5d20 2323 206e 756d 6265 7220 6f66  [0] ## number of
-0001d260: 2072 6f77 7320 7468 6174 2068 6176 6520   rows that have 
-0001d270: 6d61 7820 7661 6c75 650a 2020 2020 2020  max value.      
-0001d280: 2020 2323 2320 6669 6e64 2074 6865 206e    ### find the n
-0001d290: 5f6c 6172 6765 7374 2076 616c 7565 7320  _largest values 
-0001d2a0: 6166 7465 7220 7468 6520 6d61 7869 6d75  after the maximu
-0001d2b0: 6d20 7661 6c75 6520 6261 7365 6420 6f6e  m value based on
-0001d2c0: 2067 6976 656e 2069 6e70 7574 206e 0a20   given input n. 
-0001d2d0: 2020 2020 2020 206e 756d 5f6c 6172 6765         num_large
-0001d2e0: 7374 5f61 6674 6572 5f6d 6178 203d 206e  st_after_max = n
-0001d2f0: 756d 5f6d 6178 7320 2b20 6361 705f 6174  um_maxs + cap_at
-0001d300: 5f6e 7468 5f6c 6172 6765 7374 0a20 2020  _nth_largest.   
-0001d310: 2020 2020 2063 6170 7065 645f 7661 6c75       capped_valu
-0001d320: 6520 3d20 6466 5b63 6f6c 5d2e 6e6c 6172  e = df[col].nlar
-0001d330: 6765 7374 286e 756d 5f6c 6172 6765 7374  gest(num_largest
-0001d340: 5f61 6674 6572 5f6d 6178 292e 696c 6f63  _after_max).iloc
-0001d350: 5b2d 315d 2023 2320 7468 6973 2069 7320  [-1] ## this is 
-0001d360: 7468 6520 7661 6c75 6520 7765 2063 6170  the value we cap
-0001d370: 2069 7420 6167 6169 6e73 740a 2020 2020   it against.    
-0001d380: 2020 2020 6466 2e6c 6f63 5b64 665b 636f      df.loc[df[co
-0001d390: 6c5d 3d3d 6d61 7876 616c 2c20 636f 6c5d  l]==maxval, col]
-0001d3a0: 203d 2020 6361 7070 6564 5f76 616c 7565   =  capped_value
-0001d3b0: 2023 2320 6d61 7869 6d75 6d20 7661 6c75   ## maximum valu
-0001d3c0: 6573 2061 7265 206e 6f77 2063 6170 7065  es are now cappe
-0001d3d0: 640a 2020 2020 2020 2020 2323 2320 796f  d.        ### yo
-0001d3e0: 7520 6172 6520 6e6f 7720 676f 6f64 2074  u are now good t
-0001d3f0: 6f20 676f 202d 2079 6f75 2063 616e 2073  o go - you can s
-0001d400: 686f 7720 686f 7720 7468 6579 2061 7265  how how they are
-0001d410: 2063 6170 7065 6420 7573 696e 6720 6265   capped using be
-0001d420: 666f 7265 2061 6e64 2061 6674 6572 2070  fore and after p
-0001d430: 6963 730a 2020 2020 2020 2020 6966 2076  ics.        if v
-0001d440: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-0001d450: 2020 2020 6466 5b63 6f6c 5d2e 706c 6f74      df[col].plot
-0001d460: 286b 696e 643d 2762 6f78 272c 2074 6974  (kind='box', tit
-0001d470: 6c65 203d 2027 2573 2061 6674 6572 2063  le = '%s after c
-0001d480: 6170 7069 6e67 206f 7574 6c69 6572 7327  apping outliers'
-0001d490: 2025 636f 6c2c 2061 783d 6178 3229 0a20   %col, ax=ax2). 
-0001d4a0: 2020 2020 2020 2020 2020 2070 6c74 2e73             plt.s
-0001d4b0: 686f 7728 290a 0a20 2020 2020 2020 2023  how()..        #
-0001d4c0: 204c 6574 2773 2073 6176 6520 7468 6520   Let's save the 
-0001d4d0: 6c69 7374 206f 6620 6f75 746c 6965 7273  list of outliers
-0001d4e0: 2061 6e64 2073 6565 2069 6620 7468 6572   and see if ther
-0001d4f0: 6520 6172 6520 736f 6d65 2077 6974 6820  e are some with 
-0001d500: 6f75 746c 6965 7273 2069 6e20 6d75 6c74  outliers in mult
-0001d510: 6970 6c65 2063 6f6c 756d 6e73 0a20 2020  iple columns.   
-0001d520: 2020 2020 206f 7574 6c69 6572 5f69 6e64       outlier_ind
-0001d530: 6963 6573 2e65 7874 656e 6428 6f75 746c  ices.extend(outl
-0001d540: 6965 725f 6c69 7374 5f63 6f6c 290a 0a20  ier_list_col).. 
-0001d550: 2020 2023 2073 656c 6563 7420 6365 7274     # select cert
-0001d560: 6169 6e20 6f62 7365 7276 6174 696f 6e73  ain observations
-0001d570: 2063 6f6e 7461 696e 696e 6720 6d6f 7265   containing more
-0001d580: 2074 6861 6e20 6f6e 6520 6f75 746c 6965   than one outlie
-0001d590: 7220 696e 2032 2063 6f6c 756d 6e73 206f  r in 2 columns o
-0001d5a0: 7220 6d6f 7265 2e20 5765 2063 616e 2064  r more. We can d
-0001d5b0: 726f 7020 7468 656d 210a 2020 2020 6f75  rop them!.    ou
-0001d5c0: 746c 6965 725f 696e 6469 6365 7320 3d20  tlier_indices = 
-0001d5d0: 436f 756e 7465 7228 6f75 746c 6965 725f  Counter(outlier_
-0001d5e0: 696e 6469 6365 7329 0a20 2020 206d 756c  indices).    mul
-0001d5f0: 7469 706c 655f 6f75 746c 6965 7273 203d  tiple_outliers =
-0001d600: 206c 6973 7428 206b 2066 6f72 206b 2c20   list( k for k, 
-0001d610: 7620 696e 206f 7574 6c69 6572 5f69 6e64  v in outlier_ind
-0001d620: 6963 6573 2e69 7465 6d73 2829 2069 6620  ices.items() if 
-0001d630: 7620 3e20 3320 290a 2020 2020 2323 2320  v > 3 ).    ### 
-0001d640: 6e6f 7720 6472 6f70 2074 6865 7365 2072  now drop these r
-0001d650: 6f77 7320 616c 746f 6765 7468 6572 2023  ows altogether #
-0001d660: 2323 230a 2020 2020 6966 2064 726f 703a  ###.    if drop:
-0001d670: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-0001d680: 5368 6170 6520 6f66 2064 6174 6166 7261  Shape of datafra
-0001d690: 6d65 2062 6566 6f72 6520 6f75 746c 6965  me before outlie
-0001d6a0: 7273 2062 6569 6e67 2064 726f 7070 6564  rs being dropped
-0001d6b0: 3a20 2573 2720 2528 6466 2e73 6861 7065  : %s' %(df.shape
-0001d6c0: 2c29 290a 2020 2020 2020 2020 6e75 6d62  ,)).        numb
-0001d6d0: 6572 5f6f 665f 726f 7773 203d 2064 662e  er_of_rows = df.
-0001d6e0: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
-0001d6f0: 2064 6620 3d20 6466 2e64 726f 7028 6d75   df = df.drop(mu
-0001d700: 6c74 6970 6c65 5f6f 7574 6c69 6572 732c  ltiple_outliers,
-0001d710: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-0001d720: 2070 7269 6e74 2827 5368 6170 6520 6f66   print('Shape of
-0001d730: 2064 6174 6166 7261 6d65 2061 6674 6572   dataframe after
-0001d740: 206f 7574 6c69 6572 7320 6265 696e 6720   outliers being 
-0001d750: 6472 6f70 7065 643a 2025 7327 2025 2864  dropped: %s' %(d
-0001d760: 662e 7368 6170 652c 2929 0a20 2020 2020  f.shape,)).     
-0001d770: 2020 2070 7269 6e74 2827 5c6e 4e75 6d62     print('\nNumb
-0001d780: 6572 5f6f 665f 726f 7773 2077 6974 6820  er_of_rows with 
-0001d790: 6d75 6c74 6970 6c65 206f 7574 6c69 6572  multiple outlier
-0001d7a0: 7320 696e 206d 6f72 6520 7468 616e 2033  s in more than 3
-0001d7b0: 2063 6f6c 756d 6e73 2077 6869 6368 2077   columns which w
-0001d7c0: 6572 6520 6472 6f70 7065 6420 3d20 2564  ere dropped = %d
-0001d7d0: 2720 2528 6e75 6d62 6572 5f6f 665f 726f  ' %(number_of_ro
-0001d7e0: 7773 2d64 662e 7368 6170 655b 305d 2929  ws-df.shape[0]))
-0001d7f0: 0a20 2020 2072 6574 7572 6e20 6466 0a23  .    return df.#
-0001d800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001cdd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001cde0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001cdf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ce00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ce10: 0a20 2020 2022 2222 0a20 2020 206f 7574  .    """.    out
+0001ce20: 6c69 6572 5f69 6e64 6963 6573 203d 205b  lier_indices = [
+0001ce30: 5d0a 2020 2020 6466 203d 2064 662e 636f  ].    df = df.co
+0001ce40: 7079 2864 6565 703d 5472 7565 290a 2020  py(deep=True).  
+0001ce50: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0001ce60: 6665 6174 7572 6573 2c20 7374 7229 3a0a  features, str):.
+0001ce70: 2020 2020 2020 2020 6665 6174 7572 6573          features
+0001ce80: 203d 205b 6665 6174 7572 6573 5d0a 2020   = [features].  
+0001ce90: 2020 2320 6974 6572 6174 6520 6f76 6572    # iterate over
+0001cea0: 2066 6561 7475 7265 7328 636f 6c75 6d6e   features(column
+0001ceb0: 7329 0a20 2020 2066 6f72 2063 6f6c 2069  s).    for col i
+0001cec0: 6e20 6665 6174 7572 6573 3a0a 2020 2020  n features:.    
+0001ced0: 2020 2020 2323 2320 7468 6973 2069 7320      ### this is 
+0001cee0: 686f 7720 7468 6520 636f 6c75 6d6e 206c  how the column l
+0001cef0: 6f6f 6b73 206e 6f77 2062 6566 6f72 6520  ooks now before 
+0001cf00: 6361 7070 696e 6720 6f75 746c 6965 7273  capping outliers
+0001cf10: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+0001cf20: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+0001cf30: 2066 6967 2c20 2861 7831 2c61 7832 2920   fig, (ax1,ax2) 
+0001cf40: 3d20 706c 742e 7375 6270 6c6f 7473 2831  = plt.subplots(1
+0001cf50: 2c32 2c66 6967 7369 7a65 3d28 3132 2c35  ,2,figsize=(12,5
+0001cf60: 2929 0a20 2020 2020 2020 2020 2020 2064  )).            d
+0001cf70: 665b 636f 6c5d 2e70 6c6f 7428 6b69 6e64  f[col].plot(kind
+0001cf80: 3d27 626f 7827 2c20 7469 746c 6520 3d20  ='box', title = 
+0001cf90: 2725 7320 6265 666f 7265 2063 6170 7069  '%s before cappi
+0001cfa0: 6e67 206f 7574 6c69 6572 7327 2025 636f  ng outliers' %co
+0001cfb0: 6c2c 2061 783d 6178 3129 0a20 2020 2020  l, ax=ax1).     
+0001cfc0: 2020 2023 2031 7374 2071 7561 7274 696c     # 1st quartil
+0001cfd0: 6520 2832 3525 290a 2020 2020 2020 2020  e (25%).        
+0001cfe0: 5131 203d 206e 702e 7065 7263 656e 7469  Q1 = np.percenti
+0001cff0: 6c65 2864 665b 636f 6c5d 2c20 3235 290a  le(df[col], 25).
+0001d000: 2020 2020 2020 2020 2320 3372 6420 7175          # 3rd qu
+0001d010: 6172 7469 6c65 2028 3735 2529 0a20 2020  artile (75%).   
+0001d020: 2020 2020 2051 3320 3d20 6e70 2e70 6572       Q3 = np.per
+0001d030: 6365 6e74 696c 6528 6466 5b63 6f6c 5d2c  centile(df[col],
+0001d040: 3735 290a 2020 2020 2020 2020 2320 496e  75).        # In
+0001d050: 7465 7271 7561 7274 696c 6520 7261 6e67  terquartile rang
+0001d060: 6520 2849 5152 290a 2020 2020 2020 2020  e (IQR).        
+0001d070: 4951 5220 3d20 5133 202d 2051 310a 0a20  IQR = Q3 - Q1.. 
+0001d080: 2020 2020 2020 2023 206f 7574 6c69 6572         # outlier
+0001d090: 2073 7465 7020 7573 696e 6720 6d75 6c74   step using mult
+0001d0a0: 6970 6c69 6572 0a20 2020 2020 2020 206f  iplier.        o
+0001d0b0: 7574 6c69 6572 5f73 7465 7020 3d20 4951  utlier_step = IQ
+0001d0c0: 525f 6d75 6c74 6970 6c69 6572 202a 2049  R_multiplier * I
+0001d0d0: 5152 0a0a 2020 2020 2020 2020 6c6f 7765  QR..        lowe
+0001d0e0: 725f 6c69 6d69 7420 3d20 5131 202d 206f  r_limit = Q1 - o
+0001d0f0: 7574 6c69 6572 5f73 7465 700a 2020 2020  utlier_step.    
+0001d100: 2020 2020 7570 7065 725f 6c69 6d69 7420      upper_limit 
+0001d110: 3d20 5133 202b 206f 7574 6c69 6572 5f73  = Q3 + outlier_s
+0001d120: 7465 700a 0a20 2020 2020 2020 2023 2044  tep..        # D
+0001d130: 6574 6572 6d69 6e65 2061 206c 6973 7420  etermine a list 
+0001d140: 6f66 2069 6e64 6963 6573 206f 6620 6f75  of indices of ou
+0001d150: 746c 6965 7273 2066 6f72 2066 6561 7475  tliers for featu
+0001d160: 7265 2063 6f6c 0a20 2020 2020 2020 206f  re col.        o
+0001d170: 7574 6c69 6572 5f6c 6973 745f 636f 6c20  utlier_list_col 
+0001d180: 3d20 6466 5b28 6466 5b63 6f6c 5d20 3c20  = df[(df[col] < 
+0001d190: 6c6f 7765 725f 6c69 6d69 7429 207c 2028  lower_limit) | (
+0001d1a0: 6466 5b63 6f6c 5d20 3e20 7570 7065 725f  df[col] > upper_
+0001d1b0: 6c69 6d69 7420 295d 2e69 6e64 6578 0a0a  limit )].index..
+0001d1c0: 2020 2020 2020 2020 2323 2320 4361 7070          ### Capp
+0001d1d0: 696e 6720 7573 696e 6720 7468 6520 6e20  ing using the n 
+0001d1e0: 6c61 7267 6573 7420 7661 6c75 6520 6261  largest value ba
+0001d1f0: 7365 6420 6f6e 206e 2067 6976 656e 2069  sed on n given i
+0001d200: 6e20 696e 7075 742e 0a20 2020 2020 2020  n input..       
+0001d210: 206d 6178 7661 6c20 3d20 6466 5b63 6f6c   maxval = df[col
+0001d220: 5d2e 6d61 7828 2920 2023 2320 7768 6174  ].max()  ## what
+0001d230: 2069 7320 7468 6520 6d61 7869 6d75 6d20   is the maximum 
+0001d240: 7661 6c75 6520 696e 2074 6869 7320 636f  value in this co
+0001d250: 6c75 6d6e 3f0a 2020 2020 2020 2020 6e75  lumn?.        nu
+0001d260: 6d5f 6d61 7873 203d 2064 665b 6466 5b63  m_maxs = df[df[c
+0001d270: 6f6c 5d3d 3d6d 6178 7661 6c5d 2e73 6861  ol]==maxval].sha
+0001d280: 7065 5b30 5d20 2323 206e 756d 6265 7220  pe[0] ## number 
+0001d290: 6f66 2072 6f77 7320 7468 6174 2068 6176  of rows that hav
+0001d2a0: 6520 6d61 7820 7661 6c75 650a 2020 2020  e max value.    
+0001d2b0: 2020 2020 2323 2320 6669 6e64 2074 6865      ### find the
+0001d2c0: 206e 5f6c 6172 6765 7374 2076 616c 7565   n_largest value
+0001d2d0: 7320 6166 7465 7220 7468 6520 6d61 7869  s after the maxi
+0001d2e0: 6d75 6d20 7661 6c75 6520 6261 7365 6420  mum value based 
+0001d2f0: 6f6e 2067 6976 656e 2069 6e70 7574 206e  on given input n
+0001d300: 0a20 2020 2020 2020 206e 756d 5f6c 6172  .        num_lar
+0001d310: 6765 7374 5f61 6674 6572 5f6d 6178 203d  gest_after_max =
+0001d320: 206e 756d 5f6d 6178 7320 2b20 6361 705f   num_maxs + cap_
+0001d330: 6174 5f6e 7468 5f6c 6172 6765 7374 0a20  at_nth_largest. 
+0001d340: 2020 2020 2020 2063 6170 7065 645f 7661         capped_va
+0001d350: 6c75 6520 3d20 6466 5b63 6f6c 5d2e 6e6c  lue = df[col].nl
+0001d360: 6172 6765 7374 286e 756d 5f6c 6172 6765  argest(num_large
+0001d370: 7374 5f61 6674 6572 5f6d 6178 292e 696c  st_after_max).il
+0001d380: 6f63 5b2d 315d 2023 2320 7468 6973 2069  oc[-1] ## this i
+0001d390: 7320 7468 6520 7661 6c75 6520 7765 2063  s the value we c
+0001d3a0: 6170 2069 7420 6167 6169 6e73 740a 2020  ap it against.  
+0001d3b0: 2020 2020 2020 6466 2e6c 6f63 5b64 665b        df.loc[df[
+0001d3c0: 636f 6c5d 3d3d 6d61 7876 616c 2c20 636f  col]==maxval, co
+0001d3d0: 6c5d 203d 2020 6361 7070 6564 5f76 616c  l] =  capped_val
+0001d3e0: 7565 2023 2320 6d61 7869 6d75 6d20 7661  ue ## maximum va
+0001d3f0: 6c75 6573 2061 7265 206e 6f77 2063 6170  lues are now cap
+0001d400: 7065 640a 2020 2020 2020 2020 2323 2320  ped.        ### 
+0001d410: 796f 7520 6172 6520 6e6f 7720 676f 6f64  you are now good
+0001d420: 2074 6f20 676f 202d 2079 6f75 2063 616e   to go - you can
+0001d430: 2073 686f 7720 686f 7720 7468 6579 2061   show how they a
+0001d440: 7265 2063 6170 7065 6420 7573 696e 6720  re capped using 
+0001d450: 6265 666f 7265 2061 6e64 2061 6674 6572  before and after
+0001d460: 2070 6963 730a 2020 2020 2020 2020 6966   pics.        if
+0001d470: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+0001d480: 2020 2020 2020 6466 5b63 6f6c 5d2e 706c        df[col].pl
+0001d490: 6f74 286b 696e 643d 2762 6f78 272c 2074  ot(kind='box', t
+0001d4a0: 6974 6c65 203d 2027 2573 2061 6674 6572  itle = '%s after
+0001d4b0: 2063 6170 7069 6e67 206f 7574 6c69 6572   capping outlier
+0001d4c0: 7327 2025 636f 6c2c 2061 783d 6178 3229  s' %col, ax=ax2)
+0001d4d0: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
+0001d4e0: 2e73 686f 7728 290a 0a20 2020 2020 2020  .show()..       
+0001d4f0: 2023 204c 6574 2773 2073 6176 6520 7468   # Let's save th
+0001d500: 6520 6c69 7374 206f 6620 6f75 746c 6965  e list of outlie
+0001d510: 7273 2061 6e64 2073 6565 2069 6620 7468  rs and see if th
+0001d520: 6572 6520 6172 6520 736f 6d65 2077 6974  ere are some wit
+0001d530: 6820 6f75 746c 6965 7273 2069 6e20 6d75  h outliers in mu
+0001d540: 6c74 6970 6c65 2063 6f6c 756d 6e73 0a20  ltiple columns. 
+0001d550: 2020 2020 2020 206f 7574 6c69 6572 5f69         outlier_i
+0001d560: 6e64 6963 6573 2e65 7874 656e 6428 6f75  ndices.extend(ou
+0001d570: 746c 6965 725f 6c69 7374 5f63 6f6c 290a  tlier_list_col).
+0001d580: 0a20 2020 2023 2073 656c 6563 7420 6365  .    # select ce
+0001d590: 7274 6169 6e20 6f62 7365 7276 6174 696f  rtain observatio
+0001d5a0: 6e73 2063 6f6e 7461 696e 696e 6720 6d6f  ns containing mo
+0001d5b0: 7265 2074 6861 6e20 6f6e 6520 6f75 746c  re than one outl
+0001d5c0: 6965 7220 696e 2032 2063 6f6c 756d 6e73  ier in 2 columns
+0001d5d0: 206f 7220 6d6f 7265 2e20 5765 2063 616e   or more. We can
+0001d5e0: 2064 726f 7020 7468 656d 210a 2020 2020   drop them!.    
+0001d5f0: 6f75 746c 6965 725f 696e 6469 6365 7320  outlier_indices 
+0001d600: 3d20 436f 756e 7465 7228 6f75 746c 6965  = Counter(outlie
+0001d610: 725f 696e 6469 6365 7329 0a20 2020 206d  r_indices).    m
+0001d620: 756c 7469 706c 655f 6f75 746c 6965 7273  ultiple_outliers
+0001d630: 203d 206c 6973 7428 206b 2066 6f72 206b   = list( k for k
+0001d640: 2c20 7620 696e 206f 7574 6c69 6572 5f69  , v in outlier_i
+0001d650: 6e64 6963 6573 2e69 7465 6d73 2829 2069  ndices.items() i
+0001d660: 6620 7620 3e20 3320 290a 2020 2020 2323  f v > 3 ).    ##
+0001d670: 2320 6e6f 7720 6472 6f70 2074 6865 7365  # now drop these
+0001d680: 2072 6f77 7320 616c 746f 6765 7468 6572   rows altogether
+0001d690: 2023 2323 230a 2020 2020 6966 2064 726f   ####.    if dro
+0001d6a0: 703a 0a20 2020 2020 2020 2070 7269 6e74  p:.        print
+0001d6b0: 2827 5368 6170 6520 6f66 2064 6174 6166  ('Shape of dataf
+0001d6c0: 7261 6d65 2062 6566 6f72 6520 6f75 746c  rame before outl
+0001d6d0: 6965 7273 2062 6569 6e67 2064 726f 7070  iers being dropp
+0001d6e0: 6564 3a20 2573 2720 2528 6466 2e73 6861  ed: %s' %(df.sha
+0001d6f0: 7065 2c29 290a 2020 2020 2020 2020 6e75  pe,)).        nu
+0001d700: 6d62 6572 5f6f 665f 726f 7773 203d 2064  mber_of_rows = d
+0001d710: 662e 7368 6170 655b 305d 0a20 2020 2020  f.shape[0].     
+0001d720: 2020 2064 6620 3d20 6466 2e64 726f 7028     df = df.drop(
+0001d730: 6d75 6c74 6970 6c65 5f6f 7574 6c69 6572  multiple_outlier
+0001d740: 732c 2061 7869 733d 3029 0a20 2020 2020  s, axis=0).     
+0001d750: 2020 2070 7269 6e74 2827 5368 6170 6520     print('Shape 
+0001d760: 6f66 2064 6174 6166 7261 6d65 2061 6674  of dataframe aft
+0001d770: 6572 206f 7574 6c69 6572 7320 6265 696e  er outliers bein
+0001d780: 6720 6472 6f70 7065 643a 2025 7327 2025  g dropped: %s' %
+0001d790: 2864 662e 7368 6170 652c 2929 0a20 2020  (df.shape,)).   
+0001d7a0: 2020 2020 2070 7269 6e74 2827 5c6e 4e75       print('\nNu
+0001d7b0: 6d62 6572 5f6f 665f 726f 7773 2077 6974  mber_of_rows wit
+0001d7c0: 6820 6d75 6c74 6970 6c65 206f 7574 6c69  h multiple outli
+0001d7d0: 6572 7320 696e 206d 6f72 6520 7468 616e  ers in more than
+0001d7e0: 2033 2063 6f6c 756d 6e73 2077 6869 6368   3 columns which
+0001d7f0: 2077 6572 6520 6472 6f70 7065 6420 3d20   were dropped = 
+0001d800: 2564 2720 2528 6e75 6d62 6572 5f6f 665f  %d' %(number_of_
+0001d810: 726f 7773 2d64 662e 7368 6170 655b 305d  rows-df.shape[0]
+0001d820: 2929 0a20 2020 2072 6574 7572 6e20 6466  )).    return df
+0001d830: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
 0001d840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d850: 0a64 6566 2045 4441 5f63 6c61 7373 6966  .def EDA_classif
-0001d860: 795f 616e 645f 7265 7475 726e 5f63 6f6c  y_and_return_col
-0001d870: 735f 6279 5f74 7970 6528 6466 3129 3a0a  s_by_type(df1):.
-0001d880: 2020 2020 2222 220a 2020 2020 4544 4120      """.    EDA 
-0001d890: 7374 616e 6473 2066 6f72 2045 7870 6c6f  stands for Explo
-0001d8a0: 7261 746f 7279 2064 6174 6120 616e 616c  ratory data anal
-0001d8b0: 7973 6973 2e20 5468 6973 2066 756e 6374  ysis. This funct
-0001d8c0: 696f 6e20 7065 7266 6f72 6d73 2045 4441  ion performs EDA
-0001d8d0: 202d 2068 656e 6365 2074 6865 206e 616d   - hence the nam
-0001d8e0: 650a 2020 2020 2323 2323 2323 2323 2323  e.    ##########
-0001d8f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d900: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d880: 2323 0a64 6566 2045 4441 5f63 6c61 7373  ##.def EDA_class
+0001d890: 6966 795f 616e 645f 7265 7475 726e 5f63  ify_and_return_c
+0001d8a0: 6f6c 735f 6279 5f74 7970 6528 6466 3129  ols_by_type(df1)
+0001d8b0: 3a0a 2020 2020 2222 220a 2020 2020 4544  :.    """.    ED
+0001d8c0: 4120 7374 616e 6473 2066 6f72 2045 7870  A stands for Exp
+0001d8d0: 6c6f 7261 746f 7279 2064 6174 6120 616e  loratory data an
+0001d8e0: 616c 7973 6973 2e20 5468 6973 2066 756e  alysis. This fun
+0001d8f0: 6374 696f 6e20 7065 7266 6f72 6d73 2045  ction performs E
+0001d900: 4441 202d 2068 656e 6365 2074 6865 206e  DA - hence the n
+0001d910: 616d 650a 2020 2020 2323 2323 2323 2323  ame.    ########
 0001d920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001d930: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-0001d940: 2020 2054 6869 7320 6861 6e64 7920 6675     This handy fu
-0001d950: 6e63 7469 6f6e 2063 6c61 7373 6966 6965  nction classifie
-0001d960: 7320 796f 7572 2063 6f6c 756d 6e73 2069  s your columns i
-0001d970: 6e74 6f20 6469 6666 6572 656e 7420 7479  nto different ty
-0001d980: 7065 7320 3a20 6d61 6b65 2073 7572 6520  pes : make sure 
-0001d990: 796f 7520 7365 6e64 206f 6e6c 7920 7072  you send only pr
-0001d9a0: 6564 6963 746f 7273 2e0a 2020 2020 4265  edictors..    Be
-0001d9b0: 7761 7265 2073 656e 6469 6e67 2074 6172  ware sending tar
-0001d9c0: 6765 7420 636f 6c75 6d6e 2069 6e74 6f20  get column into 
-0001d9d0: 7468 6520 6461 7461 6672 616d 652e 2059  the dataframe. Y
-0001d9e0: 6f75 2064 6f6e 2774 2077 616e 7420 746f  ou don't want to
-0001d9f0: 2073 7461 7274 206d 6f64 6966 7969 6e67   start modifying
-0001da00: 2069 742e 0a20 2020 2023 2323 2323 2323   it..    #######
-0001da10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001da20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001da30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001d970: 0a20 2020 2054 6869 7320 6861 6e64 7920  .    This handy 
+0001d980: 6675 6e63 7469 6f6e 2063 6c61 7373 6966  function classif
+0001d990: 6965 7320 796f 7572 2063 6f6c 756d 6e73  ies your columns
+0001d9a0: 2069 6e74 6f20 6469 6666 6572 656e 7420   into different 
+0001d9b0: 7479 7065 7320 3a20 6d61 6b65 2073 7572  types : make sur
+0001d9c0: 6520 796f 7520 7365 6e64 206f 6e6c 7920  e you send only 
+0001d9d0: 7072 6564 6963 746f 7273 2e0a 2020 2020  predictors..    
+0001d9e0: 4265 7761 7265 2073 656e 6469 6e67 2074  Beware sending t
+0001d9f0: 6172 6765 7420 636f 6c75 6d6e 2069 6e74  arget column int
+0001da00: 6f20 7468 6520 6461 7461 6672 616d 652e  o the dataframe.
+0001da10: 2059 6f75 2064 6f6e 2774 2077 616e 7420   You don't want 
+0001da20: 746f 2073 7461 7274 206d 6f64 6966 7969  to start modifyi
+0001da30: 6e67 2069 742e 0a20 2020 2023 2323 2323  ng it..    #####
 0001da40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001da50: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-0001da60: 2020 2049 7420 7265 7475 726e 7320 6120     It returns a 
-0001da70: 6c69 7374 206f 6620 6361 7465 676f 7269  list of categori
-0001da80: 6361 6c20 636f 6c75 6d6e 732c 2069 6e74  cal columns, int
-0001da90: 6567 6572 2063 6f6c 7320 616e 6420 666c  eger cols and fl
-0001daa0: 6f61 7420 636f 6c75 6d6e 7320 696e 2074  oat columns in t
-0001dab0: 6861 7420 6f72 6465 722e 0a20 2020 2022  hat order..    "
-0001dac0: 2222 0a20 2020 2023 2323 204c 6574 2773  "".    ### Let's
-0001dad0: 2066 696e 6420 616c 6c20 7468 6520 6361   find all the ca
-0001dae0: 7465 676f 7269 6361 6c20 6578 636c 7564  tegorical exclud
-0001daf0: 696e 6720 696e 7465 6765 7220 636f 6c75  ing integer colu
-0001db00: 6d6e 7320 696e 2064 6174 6173 6574 3a20  mns in dataset: 
-0001db10: 756e 666f 7274 756e 6174 656c 7920 6e6f  unfortunately no
-0001db20: 7420 616c 6c20 696e 7465 6765 7273 2061  t all integers a
-0001db30: 7265 2063 6174 6567 6f72 6963 616c 210a  re categorical!.
-0001db40: 2020 2020 6361 7463 6f6c 7320 3d20 6466      catcols = df
-0001db50: 312e 7365 6c65 6374 5f64 7479 7065 7328  1.select_dtypes(
-0001db60: 696e 636c 7564 653d 276f 626a 6563 7427  include='object'
-0001db70: 292e 636f 6c75 6d6e 732e 746f 6c69 7374  ).columns.tolist
-0001db80: 2829 202b 2064 6631 2e73 656c 6563 745f  () + df1.select_
-0001db90: 6474 7970 6573 2869 6e63 6c75 6465 3d27  dtypes(include='
-0001dba0: 6361 7465 676f 7279 2729 2e63 6f6c 756d  category').colum
-0001dbb0: 6e73 2e74 6f6c 6973 7428 290a 2020 2020  ns.tolist().    
-0001dbc0: 6361 7473 203d 2063 6f70 792e 6465 6570  cats = copy.deep
-0001dbd0: 636f 7079 2863 6174 636f 6c73 290a 2020  copy(catcols).  
-0001dbe0: 2020 6e6c 7063 6f6c 7320 3d20 5b5d 0a20    nlpcols = []. 
-0001dbf0: 2020 2066 6f72 2065 6163 685f 6361 7420     for each_cat 
-0001dc00: 696e 2063 6174 733a 0a20 2020 2020 2020  in cats:.       
-0001dc10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0001dc20: 2020 6966 2064 6631 5b5b 6561 6368 5f63    if df1[[each_c
-0001dc30: 6174 5d5d 2e66 696c 6c6e 6128 276d 6973  at]].fillna('mis
-0001dc40: 7369 6e67 2729 2e6d 6170 286c 656e 292e  sing').map(len).
-0001dc50: 6d65 616e 2829 203e 3d20 3430 3a0a 2020  mean() >= 40:.  
-0001dc60: 2020 2020 2020 2020 2020 2020 2020 6e6c                nl
-0001dc70: 7063 6f6c 732e 6170 7065 6e64 2865 6163  pcols.append(eac
-0001dc80: 685f 6361 7429 0a20 2020 2020 2020 2020  h_cat).         
-0001dc90: 2020 2020 2020 2063 6174 636f 6c73 2e72         catcols.r
-0001dca0: 656d 6f76 6528 6561 6368 5f63 6174 290a  emove(each_cat).
-0001dcb0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-0001dcc0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0001dcd0: 696e 7565 0a20 2020 2069 6e74 636f 6c73  inue.    intcols
-0001dce0: 203d 2064 6631 2e73 656c 6563 745f 6474   = df1.select_dt
-0001dcf0: 7970 6573 2869 6e63 6c75 6465 3d27 696e  ypes(include='in
-0001dd00: 7465 6765 7227 292e 636f 6c75 6d6e 732e  teger').columns.
-0001dd10: 746f 6c69 7374 2829 0a20 2020 2023 206c  tolist().    # l
-0001dd20: 6574 2773 2066 696e 6420 616c 6c20 7468  et's find all th
-0001dd30: 6520 666c 6f61 7420 6e75 6d65 7269 6320  e float numeric 
-0001dd40: 636f 6c75 6d6e 7320 696e 2064 6174 610a  columns in data.
-0001dd50: 2020 2020 666c 6f61 7463 6f6c 7320 3d20      floatcols = 
-0001dd60: 6466 312e 7365 6c65 6374 5f64 7479 7065  df1.select_dtype
-0001dd70: 7328 696e 636c 7564 653d 2766 6c6f 6174  s(include='float
-0001dd80: 2729 2e63 6f6c 756d 6e73 2e74 6f6c 6973  ').columns.tolis
-0001dd90: 7428 290a 2020 2020 7265 7475 726e 2063  t().    return c
-0001dda0: 6174 636f 6c73 2c20 696e 7463 6f6c 732c  atcols, intcols,
-0001ddb0: 2066 6c6f 6174 636f 6c73 2c20 6e6c 7063   floatcols, nlpc
-0001ddc0: 6f6c 730a 2323 2323 2323 2323 2323 2323  ols.############
-0001ddd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001dde0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ddf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001da50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001da60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001da70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001da80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001da90: 0a20 2020 2049 7420 7265 7475 726e 7320  .    It returns 
+0001daa0: 6120 6c69 7374 206f 6620 6361 7465 676f  a list of catego
+0001dab0: 7269 6361 6c20 636f 6c75 6d6e 732c 2069  rical columns, i
+0001dac0: 6e74 6567 6572 2063 6f6c 7320 616e 6420  nteger cols and 
+0001dad0: 666c 6f61 7420 636f 6c75 6d6e 7320 696e  float columns in
+0001dae0: 2074 6861 7420 6f72 6465 722e 0a20 2020   that order..   
+0001daf0: 2022 2222 0a20 2020 2023 2323 204c 6574   """.    ### Let
+0001db00: 2773 2066 696e 6420 616c 6c20 7468 6520  's find all the 
+0001db10: 6361 7465 676f 7269 6361 6c20 6578 636c  categorical excl
+0001db20: 7564 696e 6720 696e 7465 6765 7220 636f  uding integer co
+0001db30: 6c75 6d6e 7320 696e 2064 6174 6173 6574  lumns in dataset
+0001db40: 3a20 756e 666f 7274 756e 6174 656c 7920  : unfortunately 
+0001db50: 6e6f 7420 616c 6c20 696e 7465 6765 7273  not all integers
+0001db60: 2061 7265 2063 6174 6567 6f72 6963 616c   are categorical
+0001db70: 210a 2020 2020 6361 7463 6f6c 7320 3d20  !.    catcols = 
+0001db80: 6466 312e 7365 6c65 6374 5f64 7479 7065  df1.select_dtype
+0001db90: 7328 696e 636c 7564 653d 276f 626a 6563  s(include='objec
+0001dba0: 7427 292e 636f 6c75 6d6e 732e 746f 6c69  t').columns.toli
+0001dbb0: 7374 2829 202b 2064 6631 2e73 656c 6563  st() + df1.selec
+0001dbc0: 745f 6474 7970 6573 2869 6e63 6c75 6465  t_dtypes(include
+0001dbd0: 3d27 6361 7465 676f 7279 2729 2e63 6f6c  ='category').col
+0001dbe0: 756d 6e73 2e74 6f6c 6973 7428 290a 2020  umns.tolist().  
+0001dbf0: 2020 6361 7473 203d 2063 6f70 792e 6465    cats = copy.de
+0001dc00: 6570 636f 7079 2863 6174 636f 6c73 290a  epcopy(catcols).
+0001dc10: 2020 2020 6e6c 7063 6f6c 7320 3d20 5b5d      nlpcols = []
+0001dc20: 0a20 2020 2066 6f72 2065 6163 685f 6361  .    for each_ca
+0001dc30: 7420 696e 2063 6174 733a 0a20 2020 2020  t in cats:.     
+0001dc40: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001dc50: 2020 2020 6966 2064 6631 5b5b 6561 6368      if df1[[each
+0001dc60: 5f63 6174 5d5d 2e66 696c 6c6e 6128 276d  _cat]].fillna('m
+0001dc70: 6973 7369 6e67 2729 2e6d 6170 286c 656e  issing').map(len
+0001dc80: 292e 6d65 616e 2829 203e 3d20 3430 3a0a  ).mean() >= 40:.
+0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dca0: 6e6c 7063 6f6c 732e 6170 7065 6e64 2865  nlpcols.append(e
+0001dcb0: 6163 685f 6361 7429 0a20 2020 2020 2020  ach_cat).       
+0001dcc0: 2020 2020 2020 2020 2063 6174 636f 6c73           catcols
+0001dcd0: 2e72 656d 6f76 6528 6561 6368 5f63 6174  .remove(each_cat
+0001dce0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+0001dcf0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+0001dd00: 6e74 696e 7565 0a20 2020 2069 6e74 636f  ntinue.    intco
+0001dd10: 6c73 203d 2064 6631 2e73 656c 6563 745f  ls = df1.select_
+0001dd20: 6474 7970 6573 2869 6e63 6c75 6465 3d27  dtypes(include='
+0001dd30: 696e 7465 6765 7227 292e 636f 6c75 6d6e  integer').column
+0001dd40: 732e 746f 6c69 7374 2829 0a20 2020 2023  s.tolist().    #
+0001dd50: 206c 6574 2773 2066 696e 6420 616c 6c20   let's find all 
+0001dd60: 7468 6520 666c 6f61 7420 6e75 6d65 7269  the float numeri
+0001dd70: 6320 636f 6c75 6d6e 7320 696e 2064 6174  c columns in dat
+0001dd80: 610a 2020 2020 666c 6f61 7463 6f6c 7320  a.    floatcols 
+0001dd90: 3d20 6466 312e 7365 6c65 6374 5f64 7479  = df1.select_dty
+0001dda0: 7065 7328 696e 636c 7564 653d 2766 6c6f  pes(include='flo
+0001ddb0: 6174 2729 2e63 6f6c 756d 6e73 2e74 6f6c  at').columns.tol
+0001ddc0: 6973 7428 290a 2020 2020 7265 7475 726e  ist().    return
+0001ddd0: 2063 6174 636f 6c73 2c20 696e 7463 6f6c   catcols, intcol
+0001dde0: 732c 2066 6c6f 6174 636f 6c73 2c20 6e6c  s, floatcols, nl
+0001ddf0: 7063 6f6c 730a 2323 2323 2323 2323 2323  pcols.##########
 0001de00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001de10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001de20: 0a64 6566 2045 4441 5f63 6c61 7373 6966  .def EDA_classif
-0001de30: 795f 6665 6174 7572 6573 5f66 6f72 5f64  y_features_for_d
-0001de40: 6565 705f 6c65 6172 6e69 6e67 2874 7261  eep_learning(tra
-0001de50: 696e 2c20 7461 7267 6574 2c20 6964 636f  in, target, idco
-0001de60: 6c73 293a 0a20 2020 2022 2222 0a20 2020  ls):.    """.   
-0001de70: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-0001de80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001de90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001dea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001de20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001de30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001de40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001de50: 2323 0a64 6566 2045 4441 5f63 6c61 7373  ##.def EDA_class
+0001de60: 6966 795f 6665 6174 7572 6573 5f66 6f72  ify_features_for
+0001de70: 5f64 6565 705f 6c65 6172 6e69 6e67 2874  _deep_learning(t
+0001de80: 7261 696e 2c20 7461 7267 6574 2c20 6964  rain, target, id
+0001de90: 636f 6c73 293a 0a20 2020 2022 2222 0a20  cols):.    """. 
+0001dea0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
 0001deb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001dec0: 2323 2323 2323 230a 2020 2020 5468 6973  #######.    This
-0001ded0: 2069 7320 6120 7369 6d70 6c65 206d 6574   is a simple met
-0001dee0: 686f 6420 6f66 2063 6c61 7373 6966 7969  hod of classifyi
-0001def0: 6e67 2066 6561 7475 7265 7320 696e 746f  ng features into
-0001df00: 2034 2074 7970 6573 3a20 6361 7473 2c20   4 types: cats, 
-0001df10: 696e 7465 6765 7273 2c20 666c 6f61 7473  integers, floats
-0001df20: 2061 6e64 204e 4c50 730a 2020 2020 5468   and NLPs.    Th
-0001df30: 6973 2069 7320 6e65 6564 6564 2066 6f72  is is needed for
-0001df40: 2064 6565 7020 6c65 6172 6e69 6e67 2070   deep learning p
-0001df50: 726f 626c 656d 7320 7768 6572 6520 7765  roblems where we
-0001df60: 206e 6565 6420 6665 7765 7220 7479 7065   need fewer type
-0001df70: 7320 6f66 2076 6172 6961 626c 6573 2074  s of variables t
-0001df80: 6f20 7472 616e 7366 6f72 6d2e 0a20 2020  o transform..   
-0001df90: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-0001dfa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001dfb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001dfc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001dec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ded0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001dee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001def0: 2323 2323 2323 2323 230a 2020 2020 5468  #########.    Th
+0001df00: 6973 2069 7320 6120 7369 6d70 6c65 206d  is is a simple m
+0001df10: 6574 686f 6420 6f66 2063 6c61 7373 6966  ethod of classif
+0001df20: 7969 6e67 2066 6561 7475 7265 7320 696e  ying features in
+0001df30: 746f 2034 2074 7970 6573 3a20 6361 7473  to 4 types: cats
+0001df40: 2c20 696e 7465 6765 7273 2c20 666c 6f61  , integers, floa
+0001df50: 7473 2061 6e64 204e 4c50 730a 2020 2020  ts and NLPs.    
+0001df60: 5468 6973 2069 7320 6e65 6564 6564 2066  This is needed f
+0001df70: 6f72 2064 6565 7020 6c65 6172 6e69 6e67  or deep learning
+0001df80: 2070 726f 626c 656d 7320 7768 6572 6520   problems where 
+0001df90: 7765 206e 6565 6420 6665 7765 7220 7479  we need fewer ty
+0001dfa0: 7065 7320 6f66 2076 6172 6961 626c 6573  pes of variables
+0001dfb0: 2074 6f20 7472 616e 7366 6f72 6d2e 0a20   to transform.. 
+0001dfc0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
 0001dfd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001dfe0: 2323 2323 2323 230a 2020 2020 2222 220a  #######.    """.
-0001dff0: 2020 2020 2323 2320 5465 7374 204c 6162      ### Test Lab
-0001e000: 656c 6572 2069 7320 6120 7665 7279 2069  eler is a very i
-0001e010: 6d70 6f72 7461 6e74 2064 6963 7469 6f6e  mportant diction
-0001e020: 6172 7920 7468 6174 2077 696c 6c20 6865  ary that will he
-0001e030: 6c70 2074 7261 6e73 666f 726d 2074 6573  lp transform tes
-0001e040: 7420 6461 7461 2073 616d 6520 6173 2074  t data same as t
-0001e050: 7261 696e 2023 2323 230a 2020 2020 7465  rain ####.    te
-0001e060: 7374 5f6c 6162 656c 6572 203d 2064 6566  st_labeler = def
-0001e070: 6175 6c74 6469 6374 286c 6973 7429 0a0a  aultdict(list)..
-0001e080: 2020 2020 2323 2323 2061 6c6c 2063 6f6c      #### all col
-0001e090: 756d 6e73 2061 7265 2066 6561 7475 7265  umns are feature
-0001e0a0: 7320 6578 6365 7074 2074 6865 2074 6172  s except the tar
-0001e0b0: 6765 7420 636f 6c75 6d6e 2061 6e64 2074  get column and t
-0001e0c0: 6865 2066 6f6c 6473 2063 6f6c 756d 6e20  he folds column 
-0001e0d0: 2323 230a 2020 2020 6966 2069 7369 6e73  ###.    if isins
-0001e0e0: 7461 6e63 6528 7461 7267 6574 2c20 7374  tance(target, st
-0001e0f0: 7229 3a0a 2020 2020 2020 2020 6665 6174  r):.        feat
-0001e100: 7572 6573 203d 205b 7820 666f 7220 7820  ures = [x for x 
-0001e110: 696e 206c 6973 7428 7472 6169 6e29 2069  in list(train) i
-0001e120: 6620 7820 6e6f 7420 696e 205b 7461 7267  f x not in [targ
-0001e130: 6574 5d2b 6964 636f 6c73 5d0a 2020 2020  et]+idcols].    
-0001e140: 656c 7365 3a0a 2020 2020 2020 2020 2323  else:.        ##
-0001e150: 2320 696e 2074 6869 7320 6361 7365 2074  # in this case t
-0001e160: 6172 6765 7420 6973 2061 206c 6973 7420  arget is a list 
-0001e170: 616e 6420 6865 6e63 6520 6361 6e20 6265  and hence can be
-0001e180: 2061 6464 6564 2074 6f20 6964 636f 6c73   added to idcols
-0001e190: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
-0001e1a0: 7320 3d20 5b78 2066 6f72 2078 2069 6e20  s = [x for x in 
-0001e1b0: 6c69 7374 2874 7261 696e 2920 6966 2078  list(train) if x
-0001e1c0: 206e 6f74 2069 6e20 7461 7267 6574 2b69   not in target+i
-0001e1d0: 6463 6f6c 735d 0a0a 2020 2020 2323 2320  dcols]..    ### 
-0001e1e0: 6669 7273 7420 6669 6e64 2061 6c6c 2074  first find all t
-0001e1f0: 6865 2074 7970 6573 206f 6620 636f 6c75  he types of colu
-0001e200: 6d6e 7320 696e 2079 6f75 7220 6461 7461  mns in your data
-0001e210: 2073 6574 2023 2323 230a 2020 2020 6361   set ####.    ca
-0001e220: 7473 2c20 696e 7473 2c20 666c 6f61 7473  ts, ints, floats
-0001e230: 2c20 6e6c 7073 203d 2045 4441 5f63 6c61  , nlps = EDA_cla
-0001e240: 7373 6966 795f 616e 645f 7265 7475 726e  ssify_and_return
-0001e250: 5f63 6f6c 735f 6279 5f74 7970 6528 7472  _cols_by_type(tr
-0001e260: 6169 6e5b 6665 6174 7572 6573 5d29 0a0a  ain[features])..
-0001e270: 2020 2020 6e75 6d65 7269 635f 6665 6174      numeric_feat
-0001e280: 7572 6573 203d 2069 6e74 7320 2b20 666c  ures = ints + fl
-0001e290: 6f61 7473 0a20 2020 2063 6174 6567 6f72  oats.    categor
-0001e2a0: 6963 616c 735f 6665 6174 7572 6573 203d  icals_features =
-0001e2b0: 2063 6f70 792e 6465 6570 636f 7079 2863   copy.deepcopy(c
-0001e2c0: 6174 7329 0a20 2020 206e 6c70 5f66 6561  ats).    nlp_fea
-0001e2d0: 7475 7265 7320 3d20 636f 7079 2e64 6565  tures = copy.dee
-0001e2e0: 7063 6f70 7928 6e6c 7073 290a 0a20 2020  pcopy(nlps)..   
-0001e2f0: 2074 6573 745f 6c61 6265 6c65 725b 2763   test_labeler['c
-0001e300: 6174 6567 6f72 6963 616c 735f 6665 6174  ategoricals_feat
-0001e310: 7572 6573 275d 203d 2063 6174 6567 6f72  ures'] = categor
-0001e320: 6963 616c 735f 6665 6174 7572 6573 0a20  icals_features. 
-0001e330: 2020 2074 6573 745f 6c61 6265 6c65 725b     test_labeler[
-0001e340: 276e 756d 6572 6963 5f66 6561 7475 7265  'numeric_feature
-0001e350: 7327 5d20 3d20 6e75 6d65 7269 635f 6665  s'] = numeric_fe
-0001e360: 6174 7572 6573 0a20 2020 2074 6573 745f  atures.    test_
-0001e370: 6c61 6265 6c65 725b 276e 6c70 5f66 6561  labeler['nlp_fea
-0001e380: 7475 7265 7327 5d20 3d20 6e6c 705f 6665  tures'] = nlp_fe
-0001e390: 6174 7572 6573 0a0a 2020 2020 7265 7475  atures..    retu
-0001e3a0: 726e 2063 6174 732c 2069 6e74 732c 2066  rn cats, ints, f
-0001e3b0: 6c6f 6174 732c 206e 6c70 730a 2323 2323  loats, nlps.####
-0001e3c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e3d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e3e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001dfe0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001dff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e010: 2323 2323 2323 2323 230a 2020 2020 2222  #########.    ""
+0001e020: 220a 2020 2020 2323 2320 5465 7374 204c  ".    ### Test L
+0001e030: 6162 656c 6572 2069 7320 6120 7665 7279  abeler is a very
+0001e040: 2069 6d70 6f72 7461 6e74 2064 6963 7469   important dicti
+0001e050: 6f6e 6172 7920 7468 6174 2077 696c 6c20  onary that will 
+0001e060: 6865 6c70 2074 7261 6e73 666f 726d 2074  help transform t
+0001e070: 6573 7420 6461 7461 2073 616d 6520 6173  est data same as
+0001e080: 2074 7261 696e 2023 2323 230a 2020 2020   train ####.    
+0001e090: 7465 7374 5f6c 6162 656c 6572 203d 2064  test_labeler = d
+0001e0a0: 6566 6175 6c74 6469 6374 286c 6973 7429  efaultdict(list)
+0001e0b0: 0a0a 2020 2020 2323 2323 2061 6c6c 2063  ..    #### all c
+0001e0c0: 6f6c 756d 6e73 2061 7265 2066 6561 7475  olumns are featu
+0001e0d0: 7265 7320 6578 6365 7074 2074 6865 2074  res except the t
+0001e0e0: 6172 6765 7420 636f 6c75 6d6e 2061 6e64  arget column and
+0001e0f0: 2074 6865 2066 6f6c 6473 2063 6f6c 756d   the folds colum
+0001e100: 6e20 2323 230a 2020 2020 6966 2069 7369  n ###.    if isi
+0001e110: 6e73 7461 6e63 6528 7461 7267 6574 2c20  nstance(target, 
+0001e120: 7374 7229 3a0a 2020 2020 2020 2020 6665  str):.        fe
+0001e130: 6174 7572 6573 203d 205b 7820 666f 7220  atures = [x for 
+0001e140: 7820 696e 206c 6973 7428 7472 6169 6e29  x in list(train)
+0001e150: 2069 6620 7820 6e6f 7420 696e 205b 7461   if x not in [ta
+0001e160: 7267 6574 5d2b 6964 636f 6c73 5d0a 2020  rget]+idcols].  
+0001e170: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001e180: 2323 2320 696e 2074 6869 7320 6361 7365  ### in this case
+0001e190: 2074 6172 6765 7420 6973 2061 206c 6973   target is a lis
+0001e1a0: 7420 616e 6420 6865 6e63 6520 6361 6e20  t and hence can 
+0001e1b0: 6265 2061 6464 6564 2074 6f20 6964 636f  be added to idco
+0001e1c0: 6c73 0a20 2020 2020 2020 2066 6561 7475  ls.        featu
+0001e1d0: 7265 7320 3d20 5b78 2066 6f72 2078 2069  res = [x for x i
+0001e1e0: 6e20 6c69 7374 2874 7261 696e 2920 6966  n list(train) if
+0001e1f0: 2078 206e 6f74 2069 6e20 7461 7267 6574   x not in target
+0001e200: 2b69 6463 6f6c 735d 0a0a 2020 2020 2323  +idcols]..    ##
+0001e210: 2320 6669 7273 7420 6669 6e64 2061 6c6c  # first find all
+0001e220: 2074 6865 2074 7970 6573 206f 6620 636f   the types of co
+0001e230: 6c75 6d6e 7320 696e 2079 6f75 7220 6461  lumns in your da
+0001e240: 7461 2073 6574 2023 2323 230a 2020 2020  ta set ####.    
+0001e250: 6361 7473 2c20 696e 7473 2c20 666c 6f61  cats, ints, floa
+0001e260: 7473 2c20 6e6c 7073 203d 2045 4441 5f63  ts, nlps = EDA_c
+0001e270: 6c61 7373 6966 795f 616e 645f 7265 7475  lassify_and_retu
+0001e280: 726e 5f63 6f6c 735f 6279 5f74 7970 6528  rn_cols_by_type(
+0001e290: 7472 6169 6e5b 6665 6174 7572 6573 5d29  train[features])
+0001e2a0: 0a0a 2020 2020 6e75 6d65 7269 635f 6665  ..    numeric_fe
+0001e2b0: 6174 7572 6573 203d 2069 6e74 7320 2b20  atures = ints + 
+0001e2c0: 666c 6f61 7473 0a20 2020 2063 6174 6567  floats.    categ
+0001e2d0: 6f72 6963 616c 735f 6665 6174 7572 6573  oricals_features
+0001e2e0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+0001e2f0: 2863 6174 7329 0a20 2020 206e 6c70 5f66  (cats).    nlp_f
+0001e300: 6561 7475 7265 7320 3d20 636f 7079 2e64  eatures = copy.d
+0001e310: 6565 7063 6f70 7928 6e6c 7073 290a 0a20  eepcopy(nlps).. 
+0001e320: 2020 2074 6573 745f 6c61 6265 6c65 725b     test_labeler[
+0001e330: 2763 6174 6567 6f72 6963 616c 735f 6665  'categoricals_fe
+0001e340: 6174 7572 6573 275d 203d 2063 6174 6567  atures'] = categ
+0001e350: 6f72 6963 616c 735f 6665 6174 7572 6573  oricals_features
+0001e360: 0a20 2020 2074 6573 745f 6c61 6265 6c65  .    test_labele
+0001e370: 725b 276e 756d 6572 6963 5f66 6561 7475  r['numeric_featu
+0001e380: 7265 7327 5d20 3d20 6e75 6d65 7269 635f  res'] = numeric_
+0001e390: 6665 6174 7572 6573 0a20 2020 2074 6573  features.    tes
+0001e3a0: 745f 6c61 6265 6c65 725b 276e 6c70 5f66  t_labeler['nlp_f
+0001e3b0: 6561 7475 7265 7327 5d20 3d20 6e6c 705f  eatures'] = nlp_
+0001e3c0: 6665 6174 7572 6573 0a0a 2020 2020 7265  features..    re
+0001e3d0: 7475 726e 2063 6174 732c 2069 6e74 732c  turn cats, ints,
+0001e3e0: 2066 6c6f 6174 732c 206e 6c70 730a 2323   floats, nlps.##
 0001e3f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e410: 2323 2323 2323 2323 230a 6672 6f6d 2069  #########.from i
-0001e420: 7465 7274 6f6f 6c73 2069 6d70 6f72 7420  tertools import 
-0001e430: 636f 6d62 696e 6174 696f 6e73 0a64 6566  combinations.def
-0001e440: 2046 455f 6372 6561 7465 5f63 6174 6567   FE_create_categ
-0001e450: 6f72 6963 616c 5f66 6561 7475 7265 5f63  orical_feature_c
-0001e460: 726f 7373 6573 2864 6663 2c20 6361 7473  rosses(dfc, cats
-0001e470: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
-0001e480: 4520 6d65 616e 7320 4645 4154 5552 4520  E means FEATURE 
-0001e490: 454e 4749 4e45 4552 494e 4720 2d20 5468  ENGINEERING - Th
-0001e4a0: 6174 206d 6561 6e73 2074 6869 7320 6675  at means this fu
-0001e4b0: 6e63 7469 6f6e 2077 696c 6c20 6372 6561  nction will crea
-0001e4c0: 7465 206e 6577 2066 6561 7475 7265 730a  te new features.
-0001e4d0: 2020 2020 2323 2323 2323 2323 2323 2323      ############
-0001e4e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e4f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e440: 2323 2323 2323 2323 2323 230a 6672 6f6d  ###########.from
+0001e450: 2069 7465 7274 6f6f 6c73 2069 6d70 6f72   itertools impor
+0001e460: 7420 636f 6d62 696e 6174 696f 6e73 0a64  t combinations.d
+0001e470: 6566 2046 455f 6372 6561 7465 5f63 6174  ef FE_create_cat
+0001e480: 6567 6f72 6963 616c 5f66 6561 7475 7265  egorical_feature
+0001e490: 5f63 726f 7373 6573 2864 6663 2c20 6361  _crosses(dfc, ca
+0001e4a0: 7473 293a 0a20 2020 2022 2222 0a20 2020  ts):.    """.   
+0001e4b0: 2046 4520 6d65 616e 7320 4645 4154 5552   FE means FEATUR
+0001e4c0: 4520 454e 4749 4e45 4552 494e 4720 2d20  E ENGINEERING - 
+0001e4d0: 5468 6174 206d 6561 6e73 2074 6869 7320  That means this 
+0001e4e0: 6675 6e63 7469 6f6e 2077 696c 6c20 6372  function will cr
+0001e4f0: 6561 7465 206e 6577 2066 6561 7475 7265  eate new feature
+0001e500: 730a 2020 2020 2323 2323 2323 2323 2323  s.    ##########
 0001e510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e520: 2323 2323 2323 2323 2323 0a20 2020 2054  ##########.    T
-0001e530: 6869 7320 6372 6561 7465 7320 6665 6174  his creates feat
-0001e540: 7572 6520 6372 6f73 7365 7320 666f 7220  ure crosses for 
-0001e550: 6561 6368 2070 6169 7220 6f66 2063 6174  each pair of cat
-0001e560: 6567 6f72 6963 616c 2076 6172 6961 626c  egorical variabl
-0001e570: 6573 2069 6e20 6361 7473 2e0a 2020 2020  es in cats..    
-0001e580: 5468 6520 6e75 6d62 6572 206f 6620 6665  The number of fe
-0001e590: 6174 7572 6573 2063 7265 6174 6564 2077  atures created w
-0001e5a0: 696c 6c20 6265 206e 2a28 6e2d 3129 2f32  ill be n*(n-1)/2
-0001e5b0: 2077 6869 6368 206d 6561 6e73 2033 2063   which means 3 c
-0001e5c0: 6174 2066 6561 7475 7265 7320 7769 6c6c  at features will
-0001e5d0: 2063 7265 6174 650a 2020 2020 332a 322f   create.    3*2/
-0001e5e0: 3220 3d20 3320 6e65 7720 6665 6174 7572  2 = 3 new featur
-0001e5f0: 6573 2e20 596f 7520 6d75 7374 2062 6520  es. You must be 
-0001e600: 6361 7265 6675 6c20 7769 7468 2074 6869  careful with thi
-0001e610: 7320 6675 6e63 7469 6f6e 2073 6f20 6974  s function so it
-0001e620: 2064 6f65 736e 2774 2063 7265 6174 6520   doesn't create 
-0001e630: 746f 6f20 6d61 6e79 2e0a 0a20 2020 2049  too many...    I
-0001e640: 6e70 7574 733a 0a20 2020 2064 6663 203a  nputs:.    dfc :
-0001e650: 2064 6174 6166 7261 6d65 2063 6f6e 7461   dataframe conta
-0001e660: 696e 696e 6720 616c 6c20 7468 6520 6665  ining all the fe
-0001e670: 6174 7572 6573 0a20 2020 2063 6174 733a  atures.    cats:
-0001e680: 2061 206c 6973 7420 6f66 2063 6174 6567   a list of categ
-0001e690: 6f72 6963 616c 2066 6561 7475 7265 7320  orical features 
-0001e6a0: 696e 2074 6865 2064 6174 6166 7261 6d65  in the dataframe
-0001e6b0: 2061 626f 7665 2028 6466 6329 0a0a 2020   above (dfc)..  
-0001e6c0: 2020 4f75 7470 7574 733a 0a20 2020 2064    Outputs:.    d
-0001e6d0: 6663 3a20 7265 7475 726e 7320 7468 6520  fc: returns the 
-0001e6e0: 6461 7461 6672 616d 6520 7769 7468 206e  dataframe with n
-0001e6f0: 6577 6c79 2061 6464 6564 2066 6561 7475  ewly added featu
-0001e700: 7265 732e 204f 7269 6769 6e61 6c20 6665  res. Original fe
-0001e710: 6174 7572 6573 2061 7265 2075 6e74 6f75  atures are untou
-0001e720: 6368 6564 2e0a 0a20 2020 2023 2323 2323  ched...    #####
-0001e730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e550: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+0001e560: 2054 6869 7320 6372 6561 7465 7320 6665   This creates fe
+0001e570: 6174 7572 6520 6372 6f73 7365 7320 666f  ature crosses fo
+0001e580: 7220 6561 6368 2070 6169 7220 6f66 2063  r each pair of c
+0001e590: 6174 6567 6f72 6963 616c 2076 6172 6961  ategorical varia
+0001e5a0: 626c 6573 2069 6e20 6361 7473 2e0a 2020  bles in cats..  
+0001e5b0: 2020 5468 6520 6e75 6d62 6572 206f 6620    The number of 
+0001e5c0: 6665 6174 7572 6573 2063 7265 6174 6564  features created
+0001e5d0: 2077 696c 6c20 6265 206e 2a28 6e2d 3129   will be n*(n-1)
+0001e5e0: 2f32 2077 6869 6368 206d 6561 6e73 2033  /2 which means 3
+0001e5f0: 2063 6174 2066 6561 7475 7265 7320 7769   cat features wi
+0001e600: 6c6c 2063 7265 6174 650a 2020 2020 332a  ll create.    3*
+0001e610: 322f 3220 3d20 3320 6e65 7720 6665 6174  2/2 = 3 new feat
+0001e620: 7572 6573 2e20 596f 7520 6d75 7374 2062  ures. You must b
+0001e630: 6520 6361 7265 6675 6c20 7769 7468 2074  e careful with t
+0001e640: 6869 7320 6675 6e63 7469 6f6e 2073 6f20  his function so 
+0001e650: 6974 2064 6f65 736e 2774 2063 7265 6174  it doesn't creat
+0001e660: 6520 746f 6f20 6d61 6e79 2e0a 0a20 2020  e too many...   
+0001e670: 2049 6e70 7574 733a 0a20 2020 2064 6663   Inputs:.    dfc
+0001e680: 203a 2064 6174 6166 7261 6d65 2063 6f6e   : dataframe con
+0001e690: 7461 696e 696e 6720 616c 6c20 7468 6520  taining all the 
+0001e6a0: 6665 6174 7572 6573 0a20 2020 2063 6174  features.    cat
+0001e6b0: 733a 2061 206c 6973 7420 6f66 2063 6174  s: a list of cat
+0001e6c0: 6567 6f72 6963 616c 2066 6561 7475 7265  egorical feature
+0001e6d0: 7320 696e 2074 6865 2064 6174 6166 7261  s in the datafra
+0001e6e0: 6d65 2061 626f 7665 2028 6466 6329 0a0a  me above (dfc)..
+0001e6f0: 2020 2020 4f75 7470 7574 733a 0a20 2020      Outputs:.   
+0001e700: 2064 6663 3a20 7265 7475 726e 7320 7468   dfc: returns th
+0001e710: 6520 6461 7461 6672 616d 6520 7769 7468  e dataframe with
+0001e720: 206e 6577 6c79 2061 6464 6564 2066 6561   newly added fea
+0001e730: 7475 7265 732e 204f 7269 6769 6e61 6c20  tures. Original 
+0001e740: 6665 6174 7572 6573 2061 7265 2075 6e74  features are unt
+0001e750: 6f75 6368 6564 2e0a 0a20 2020 2023 2323  ouched...    ###
 0001e760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e780: 230a 2020 2020 5573 6167 653a 0a20 2020  #.    Usage:.   
-0001e790: 2064 6663 203d 2046 455f 6372 6561 7465   dfc = FE_create
-0001e7a0: 5f66 6561 7475 7265 5f63 726f 7373 6573  _feature_crosses
-0001e7b0: 2864 6663 2c20 6361 7473 290a 2020 2020  (dfc, cats).    
-0001e7c0: 2222 220a 2020 2020 6466 6320 3d20 636f  """.    dfc = co
-0001e7d0: 7079 2e64 6565 7063 6f70 7928 6466 6329  py.deepcopy(dfc)
-0001e7e0: 0a20 2020 2063 6f6d 626f 7320 3d20 6c69  .    combos = li
-0001e7f0: 7374 2863 6f6d 6269 6e61 7469 6f6e 7328  st(combinations(
-0001e800: 6361 7473 2c20 3229 290a 2020 2020 666f  cats, 2)).    fo
-0001e810: 7220 6361 7431 2c20 6361 7432 2069 6e20  r cat1, cat2 in 
-0001e820: 636f 6d62 6f73 3a0a 2020 2020 2020 2020  combos:.        
-0001e830: 6466 632e 6c6f 635b 3a2c 6361 7431 2b27  dfc.loc[:,cat1+'
-0001e840: 5f63 726f 7373 5f27 2b63 6174 325d 203d  _cross_'+cat2] =
-0001e850: 2064 6663 5b63 6174 315d 2e61 7374 7970   dfc[cat1].astyp
-0001e860: 6528 7374 7229 2b22 2022 2b64 6663 5b63  e(str)+" "+dfc[c
-0001e870: 6174 325d 2e61 7374 7970 6528 7374 7229  at2].astype(str)
-0001e880: 0a20 2020 2072 6574 7572 6e20 6466 630a  .    return dfc.
-0001e890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e8a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e8b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e8c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e7a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e7b0: 2323 230a 2020 2020 5573 6167 653a 0a20  ###.    Usage:. 
+0001e7c0: 2020 2064 6663 203d 2046 455f 6372 6561     dfc = FE_crea
+0001e7d0: 7465 5f66 6561 7475 7265 5f63 726f 7373  te_feature_cross
+0001e7e0: 6573 2864 6663 2c20 6361 7473 290a 2020  es(dfc, cats).  
+0001e7f0: 2020 2222 220a 2020 2020 6466 6320 3d20    """.    dfc = 
+0001e800: 636f 7079 2e64 6565 7063 6f70 7928 6466  copy.deepcopy(df
+0001e810: 6329 0a20 2020 2063 6f6d 626f 7320 3d20  c).    combos = 
+0001e820: 6c69 7374 2863 6f6d 6269 6e61 7469 6f6e  list(combination
+0001e830: 7328 6361 7473 2c20 3229 290a 2020 2020  s(cats, 2)).    
+0001e840: 666f 7220 6361 7431 2c20 6361 7432 2069  for cat1, cat2 i
+0001e850: 6e20 636f 6d62 6f73 3a0a 2020 2020 2020  n combos:.      
+0001e860: 2020 6466 632e 6c6f 635b 3a2c 6361 7431    dfc.loc[:,cat1
+0001e870: 2b27 5f63 726f 7373 5f27 2b63 6174 325d  +'_cross_'+cat2]
+0001e880: 203d 2064 6663 5b63 6174 315d 2e61 7374   = dfc[cat1].ast
+0001e890: 7970 6528 7374 7229 2b22 2022 2b64 6663  ype(str)+" "+dfc
+0001e8a0: 5b63 6174 325d 2e61 7374 7970 6528 7374  [cat2].astype(st
+0001e8b0: 7229 0a20 2020 2072 6574 7572 6e20 6466  r).    return df
+0001e8c0: 630a 2323 2323 2323 2323 2323 2323 2323  c.##############
 0001e8d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e8e0: 2323 2323 2323 2323 2323 2323 230a 6672  #############.fr
-0001e8f0: 6f6d 2073 6369 7079 2e73 7461 7473 2069  om scipy.stats i
-0001e900: 6d70 6f72 7420 7072 6f62 706c 6f74 2c73  mport probplot,s
-0001e910: 6b65 770a 6465 6620 4544 415f 6669 6e64  kew.def EDA_find
-0001e920: 5f73 6b65 7765 645f 7661 7269 6162 6c65  _skewed_variable
-0001e930: 7328 6466 742c 2073 6b65 775f 6c69 6d69  s(dft, skew_limi
-0001e940: 743d 312e 3129 3a0a 2020 2020 2222 220a  t=1.1):.    """.
-0001e950: 2020 2020 4544 4120 7374 616e 6473 2066      EDA stands f
-0001e960: 6f72 2045 7870 6c6f 7261 746f 7279 2044  or Exploratory D
-0001e970: 6174 6120 416e 616c 7973 6973 203a 2074  ata Analysis : t
-0001e980: 6869 7320 6675 6e63 7469 6f6e 2070 6572  his function per
-0001e990: 666f 726d 7320 4544 410a 2020 2020 2323  forms EDA.    ##
-0001e9a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e9b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e9c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e8e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e8f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e900: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e910: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+0001e920: 6672 6f6d 2073 6369 7079 2e73 7461 7473  from scipy.stats
+0001e930: 2069 6d70 6f72 7420 7072 6f62 706c 6f74   import probplot
+0001e940: 2c73 6b65 770a 6465 6620 4544 415f 6669  ,skew.def EDA_fi
+0001e950: 6e64 5f73 6b65 7765 645f 7661 7269 6162  nd_skewed_variab
+0001e960: 6c65 7328 6466 742c 2073 6b65 775f 6c69  les(dft, skew_li
+0001e970: 6d69 743d 312e 3129 3a0a 2020 2020 2222  mit=1.1):.    ""
+0001e980: 220a 2020 2020 4544 4120 7374 616e 6473  ".    EDA stands
+0001e990: 2066 6f72 2045 7870 6c6f 7261 746f 7279   for Exploratory
+0001e9a0: 2044 6174 6120 416e 616c 7973 6973 203a   Data Analysis :
+0001e9b0: 2074 6869 7320 6675 6e63 7469 6f6e 2070   this function p
+0001e9c0: 6572 666f 726d 7320 4544 410a 2020 2020  erforms EDA.    
 0001e9d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001e9e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001e9f0: 2323 2323 0a20 2020 2054 6869 7320 6675  ####.    This fu
-0001ea00: 6e63 7469 6f6e 2066 696e 6473 2061 6c6c  nction finds all
-0001ea10: 2074 6865 2068 6967 686c 7920 736b 6577   the highly skew
-0001ea20: 6564 2066 6c6f 6174 2028 636f 6e74 696e  ed float (contin
-0001ea30: 756f 7573 2920 7661 7269 6162 6c65 7320  uous) variables 
-0001ea40: 696e 2079 6f75 7220 4461 7461 4672 616d  in your DataFram
-0001ea50: 650a 2020 2020 4974 2073 656c 6563 7473  e.    It selects
-0001ea60: 2074 6865 6d20 6261 7365 6420 6f6e 2074   them based on t
-0001ea70: 6865 2073 6b65 775f 6c69 6d69 7420 796f  he skew_limit yo
-0001ea80: 7520 7365 743a 2061 6e79 7468 696e 6720  u set: anything 
-0001ea90: 6f76 6572 2073 6b65 7720 312e 3120 6973  over skew 1.1 is
-0001eaa0: 2074 6865 2064 6566 6175 6c74 2073 6574   the default set
-0001eab0: 7469 6e67 2e0a 2020 2020 2323 2323 2323  ting..    ######
-0001eac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ead0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001eae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001e9f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ea00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ea10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ea20: 2323 2323 2323 0a20 2020 2054 6869 7320  ######.    This 
+0001ea30: 6675 6e63 7469 6f6e 2066 696e 6473 2061  function finds a
+0001ea40: 6c6c 2074 6865 2068 6967 686c 7920 736b  ll the highly sk
+0001ea50: 6577 6564 2066 6c6f 6174 2028 636f 6e74  ewed float (cont
+0001ea60: 696e 756f 7573 2920 7661 7269 6162 6c65  inuous) variable
+0001ea70: 7320 696e 2079 6f75 7220 4461 7461 4672  s in your DataFr
+0001ea80: 616d 650a 2020 2020 4974 2073 656c 6563  ame.    It selec
+0001ea90: 7473 2074 6865 6d20 6261 7365 6420 6f6e  ts them based on
+0001eaa0: 2074 6865 2073 6b65 775f 6c69 6d69 7420   the skew_limit 
+0001eab0: 796f 7520 7365 743a 2061 6e79 7468 696e  you set: anythin
+0001eac0: 6720 6f76 6572 2073 6b65 7720 312e 3120  g over skew 1.1 
+0001ead0: 6973 2074 6865 2064 6566 6175 6c74 2073  is the default s
+0001eae0: 6574 7469 6e67 2e0a 2020 2020 2323 2323  etting..    ####
 0001eaf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001eb00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001eb10: 0a20 2020 2049 6e70 7574 733a 0a20 2020  .    Inputs:.   
-0001eb20: 2064 663a 2070 616e 6461 7320 4461 7461   df: pandas Data
-0001eb30: 4672 616d 650a 2020 2020 736b 6577 5f6c  Frame.    skew_l
-0001eb40: 696d 6974 3a20 6465 6661 756c 7420 312e  imit: default 1.
-0001eb50: 3120 3d20 616e 7974 6869 6e67 206f 7665  1 = anything ove
-0001eb60: 7220 7468 6973 206c 696d 6974 2061 6e64  r this limit and
-0001eb70: 2069 7420 6465 7465 6374 7320 6974 2061   it detects it a
-0001eb80: 7320 6120 6869 6768 6c79 2073 6b65 7765  s a highly skewe
-0001eb90: 6420 7661 722e 0a0a 2020 2020 4f75 7470  d var...    Outp
-0001eba0: 7574 733a 0a20 2020 206c 6973 7420 6f66  uts:.    list of
-0001ebb0: 2061 2076 6172 6961 626c 6573 2066 6f75   a variables fou
-0001ebc0: 6e64 2074 6861 7420 6861 7665 2068 6967  nd that have hig
-0001ebd0: 6820 736b 6577 2069 6e20 6461 7461 2073  h skew in data s
-0001ebe0: 6574 2e0a 2020 2020 2323 2323 2323 2323  et..    ########
-0001ebf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ec00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ec10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001eb10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001eb20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001eb30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001eb40: 2323 0a20 2020 2049 6e70 7574 733a 0a20  ##.    Inputs:. 
+0001eb50: 2020 2064 663a 2070 616e 6461 7320 4461     df: pandas Da
+0001eb60: 7461 4672 616d 650a 2020 2020 736b 6577  taFrame.    skew
+0001eb70: 5f6c 696d 6974 3a20 6465 6661 756c 7420  _limit: default 
+0001eb80: 312e 3120 3d20 616e 7974 6869 6e67 206f  1.1 = anything o
+0001eb90: 7665 7220 7468 6973 206c 696d 6974 2061  ver this limit a
+0001eba0: 6e64 2069 7420 6465 7465 6374 7320 6974  nd it detects it
+0001ebb0: 2061 7320 6120 6869 6768 6c79 2073 6b65   as a highly ske
+0001ebc0: 7765 6420 7661 722e 0a0a 2020 2020 4f75  wed var...    Ou
+0001ebd0: 7470 7574 733a 0a20 2020 206c 6973 7420  tputs:.    list 
+0001ebe0: 6f66 2061 2076 6172 6961 626c 6573 2066  of a variables f
+0001ebf0: 6f75 6e64 2074 6861 7420 6861 7665 2068  ound that have h
+0001ec00: 6967 6820 736b 6577 2069 6e20 6461 7461  igh skew in data
+0001ec10: 2073 6574 2e0a 2020 2020 2323 2323 2323   set..    ######
 0001ec20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ec30: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-0001ec40: 2020 2059 6f75 2063 616e 2075 7365 2046     You can use F
-0001ec50: 455f 6361 7070 696e 675f 6f75 746c 6965  E_capping_outlie
-0001ec60: 7273 5f62 6579 6f6e 645f 4951 525f 5261  rs_beyond_IQR_Ra
-0001ec70: 6e67 6528 2920 6675 6e63 7469 6f6e 2074  nge() function t
-0001ec80: 6f20 6361 7020 6f75 746c 6965 7273 2069  o cap outliers i
-0001ec90: 6e20 7468 6573 6520 7661 7269 6162 6c65  n these variable
-0001eca0: 732e 0a20 2020 2022 2222 0a20 2020 2073  s..    """.    s
-0001ecb0: 6b65 7765 645f 7661 7273 203d 205b 5d0a  kewed_vars = [].
-0001ecc0: 2020 2020 636f 6e74 6920 3d20 6466 742e      conti = dft.
-0001ecd0: 7365 6c65 6374 5f64 7479 7065 7328 696e  select_dtypes(in
-0001ece0: 636c 7564 653d 2766 6c6f 6174 2729 2e63  clude='float').c
-0001ecf0: 6f6c 756d 6e73 2e74 6f6c 6973 7428 290a  olumns.tolist().
-0001ed00: 2020 2020 666f 7220 6561 6368 5f63 6f6e      for each_con
-0001ed10: 7469 2069 6e20 636f 6e74 693a 0a20 2020  ti in conti:.   
-0001ed20: 2020 2020 2073 6b65 775f 7661 6c3d 726f       skew_val=ro
-0001ed30: 756e 6428 6466 745b 6561 6368 5f63 6f6e  und(dft[each_con
-0001ed40: 7469 5d2e 736b 6577 2829 2c20 3129 0a20  ti].skew(), 1). 
-0001ed50: 2020 2020 2020 2069 6620 736b 6577 5f76         if skew_v
-0001ed60: 616c 203e 3d20 736b 6577 5f6c 696d 6974  al >= skew_limit
-0001ed70: 3a0a 2020 2020 2020 2020 2020 2020 736b  :.            sk
-0001ed80: 6577 6564 5f76 6172 732e 6170 7065 6e64  ewed_vars.append
-0001ed90: 2865 6163 685f 636f 6e74 6929 0a20 2020  (each_conti).   
-0001eda0: 2070 7269 6e74 2827 466f 756e 6420 2564   print('Found %d
-0001edb0: 2073 6b65 7765 6420 7661 7269 6162 6c65   skewed variable
-0001edc0: 7320 696e 2064 6174 6120 6261 7365 6420  s in data based 
-0001edd0: 6f6e 2073 6b65 775f 6c69 6d69 7420 3e3d  on skew_limit >=
-0001ede0: 2025 7327 2025 286c 656e 2873 6b65 7765   %s' %(len(skewe
-0001edf0: 645f 7661 7273 292c 736b 6577 5f6c 696d  d_vars),skew_lim
-0001ee00: 6974 2929 0a20 2020 2072 6574 7572 6e20  it)).    return 
-0001ee10: 736b 6577 6564 5f76 6172 730a 2323 2323  skewed_vars.####
-0001ee20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ee30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ee40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ec30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ec40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ec50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ec60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ec70: 0a20 2020 2059 6f75 2063 616e 2075 7365  .    You can use
+0001ec80: 2046 455f 6361 7070 696e 675f 6f75 746c   FE_capping_outl
+0001ec90: 6965 7273 5f62 6579 6f6e 645f 4951 525f  iers_beyond_IQR_
+0001eca0: 5261 6e67 6528 2920 6675 6e63 7469 6f6e  Range() function
+0001ecb0: 2074 6f20 6361 7020 6f75 746c 6965 7273   to cap outliers
+0001ecc0: 2069 6e20 7468 6573 6520 7661 7269 6162   in these variab
+0001ecd0: 6c65 732e 0a20 2020 2022 2222 0a20 2020  les..    """.   
+0001ece0: 2073 6b65 7765 645f 7661 7273 203d 205b   skewed_vars = [
+0001ecf0: 5d0a 2020 2020 636f 6e74 6920 3d20 6466  ].    conti = df
+0001ed00: 742e 7365 6c65 6374 5f64 7479 7065 7328  t.select_dtypes(
+0001ed10: 696e 636c 7564 653d 2766 6c6f 6174 2729  include='float')
+0001ed20: 2e63 6f6c 756d 6e73 2e74 6f6c 6973 7428  .columns.tolist(
+0001ed30: 290a 2020 2020 666f 7220 6561 6368 5f63  ).    for each_c
+0001ed40: 6f6e 7469 2069 6e20 636f 6e74 693a 0a20  onti in conti:. 
+0001ed50: 2020 2020 2020 2073 6b65 775f 7661 6c3d         skew_val=
+0001ed60: 726f 756e 6428 6466 745b 6561 6368 5f63  round(dft[each_c
+0001ed70: 6f6e 7469 5d2e 736b 6577 2829 2c20 3129  onti].skew(), 1)
+0001ed80: 0a20 2020 2020 2020 2069 6620 736b 6577  .        if skew
+0001ed90: 5f76 616c 203e 3d20 736b 6577 5f6c 696d  _val >= skew_lim
+0001eda0: 6974 3a0a 2020 2020 2020 2020 2020 2020  it:.            
+0001edb0: 736b 6577 6564 5f76 6172 732e 6170 7065  skewed_vars.appe
+0001edc0: 6e64 2865 6163 685f 636f 6e74 6929 0a20  nd(each_conti). 
+0001edd0: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
+0001ede0: 2564 2073 6b65 7765 6420 7661 7269 6162  %d skewed variab
+0001edf0: 6c65 7320 696e 2064 6174 6120 6261 7365  les in data base
+0001ee00: 6420 6f6e 2073 6b65 775f 6c69 6d69 7420  d on skew_limit 
+0001ee10: 3e3d 2025 7327 2025 286c 656e 2873 6b65  >= %s' %(len(ske
+0001ee20: 7765 645f 7661 7273 292c 736b 6577 5f6c  wed_vars),skew_l
+0001ee30: 696d 6974 2929 0a20 2020 2072 6574 7572  imit)).    retur
+0001ee40: 6e20 736b 6577 6564 5f76 6172 730a 2323  n skewed_vars.##
 0001ee50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001ee60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001ee70: 2323 2323 2323 2323 230a 6465 6620 6973  #########.def is
-0001ee80: 5f6f 7574 6c69 6572 2864 6174 6166 7261  _outlier(datafra
-0001ee90: 6d65 2c20 7468 7265 7368 3d33 2e35 293a  me, thresh=3.5):
-0001eea0: 0a20 2020 2069 6620 6c65 6e28 6461 7461  .    if len(data
-0001eeb0: 6672 616d 652e 7368 6170 6529 203d 3d20  frame.shape) == 
-0001eec0: 313a 0a20 2020 2020 2020 2064 6174 6166  1:.        dataf
-0001eed0: 7261 6d65 203d 2064 6174 6166 7261 6d65  rame = dataframe
-0001eee0: 5b3a 2c4e 6f6e 655d 0a20 2020 206d 6564  [:,None].    med
-0001eef0: 6961 6e20 3d20 6e70 2e6d 6564 6961 6e28  ian = np.median(
-0001ef00: 6461 7461 6672 616d 652c 2061 7869 733d  dataframe, axis=
-0001ef10: 3029 0a20 2020 2064 6966 6620 3d20 6e70  0).    diff = np
-0001ef20: 2e73 756d 2828 6461 7461 6672 616d 6520  .sum((dataframe 
-0001ef30: 2d20 6d65 6469 616e 292a 2a32 2c20 6178  - median)**2, ax
-0001ef40: 6973 3d2d 3129 0a20 2020 2064 6966 6620  is=-1).    diff 
-0001ef50: 3d20 6e70 2e73 7172 7428 6469 6666 290a  = np.sqrt(diff).
-0001ef60: 2020 2020 6d65 645f 6162 735f 6465 7669      med_abs_devi
-0001ef70: 6174 696f 6e20 3d20 6e70 2e6d 6564 6961  ation = np.media
-0001ef80: 6e28 6469 6666 290a 0a20 2020 206d 6f64  n(diff)..    mod
-0001ef90: 6966 6965 645f 7a5f 7363 6f72 6520 3d20  ified_z_score = 
-0001efa0: 302e 3637 3435 202a 2064 6966 6620 2f20  0.6745 * diff / 
-0001efb0: 6d65 645f 6162 735f 6465 7669 6174 696f  med_abs_deviatio
-0001efc0: 6e0a 2020 2020 7265 7475 726e 206d 6f64  n.    return mod
-0001efd0: 6966 6965 645f 7a5f 7363 6f72 6520 3e20  ified_z_score > 
-0001efe0: 7468 7265 7368 0a0a 6465 6620 4544 415f  thresh..def EDA_
-0001eff0: 6669 6e64 5f6f 7574 6c69 6572 7328 6466  find_outliers(df
-0001f000: 2c20 636f 6c2c 2074 6872 6573 683d 3529  , col, thresh=5)
-0001f010: 3a0a 2020 2020 2222 220a 2020 2020 2222  :.    """.    ""
-0001f020: 220a 2020 2020 2323 2323 2323 2320 4669  ".    ####### Fi
-0001f030: 6e64 7320 4f75 746c 6965 7273 2061 6e64  nds Outliers and
-0001f040: 206d 6172 6b73 2074 6865 6d20 6173 2027   marks them as '
-0001f050: 5472 7565 2720 6966 2074 6865 7920 6172  True' if they ar
-0001f060: 6520 6f75 746c 6965 7273 0a20 2020 2023  e outliers.    #
-0001f070: 2323 2323 2323 2044 6174 6166 7261 6d65  ###### Dataframe
-0001f080: 2072 6566 6572 7320 746f 2074 6865 2069   refers to the i
-0001f090: 6e70 7574 2064 6174 6166 7261 6d65 2061  nput dataframe a
-0001f0a0: 6e64 2074 6872 6573 686f 6c64 2072 6566  nd threshold ref
-0001f0b0: 6572 7320 746f 2068 6f77 2066 6172 2066  ers to how far f
-0001f0c0: 726f 6d20 7468 6520 6d65 6469 616e 2061  rom the median a
-0001f0d0: 2076 616c 7565 2069 730a 2020 2020 2323   value is.    ##
-0001f0e0: 2323 2323 2320 4920 616d 2075 7369 6e67  ##### I am using
-0001f0f0: 2074 6865 204d 6564 6961 6e20 4162 736f   the Median Abso
-0001f100: 6c75 7465 2044 6576 6961 7469 6f6e 204d  lute Deviation M
-0001f110: 6574 686f 6420 284d 4144 4429 2074 6f20  ethod (MADD) to 
-0001f120: 6669 6e64 204f 7574 6c69 6572 7320 6865  find Outliers he
-0001f130: 7265 0a20 2020 206d 6173 6b5f 6f75 746c  re.    mask_outl
-0001f140: 6965 7273 203d 2069 735f 6f75 746c 6965  iers = is_outlie
-0001f150: 7228 6466 5b63 6f6c 5d2c 7468 7265 7368  r(df[col],thresh
-0001f160: 3d74 6872 6573 6829 2e61 7374 7970 6528  =thresh).astype(
-0001f170: 696e 7429 0a20 2020 2072 6574 7572 6e20  int).    return 
-0001f180: 6466 2e69 6c6f 635b 6e70 2e77 6865 7265  df.iloc[np.where
-0001f190: 286d 6173 6b5f 6f75 746c 6965 7273 3e30  (mask_outliers>0
-0001f1a0: 295d 0a23 2323 2323 2323 2323 2323 2323  )].#############
-0001f1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ee70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ee80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001ee90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001eea0: 2323 2323 2323 2323 2323 230a 6465 6620  ###########.def 
+0001eeb0: 6973 5f6f 7574 6c69 6572 2864 6174 6166  is_outlier(dataf
+0001eec0: 7261 6d65 2c20 7468 7265 7368 3d33 2e35  rame, thresh=3.5
+0001eed0: 293a 0a20 2020 2069 6620 6c65 6e28 6461  ):.    if len(da
+0001eee0: 7461 6672 616d 652e 7368 6170 6529 203d  taframe.shape) =
+0001eef0: 3d20 313a 0a20 2020 2020 2020 2064 6174  = 1:.        dat
+0001ef00: 6166 7261 6d65 203d 2064 6174 6166 7261  aframe = datafra
+0001ef10: 6d65 5b3a 2c4e 6f6e 655d 0a20 2020 206d  me[:,None].    m
+0001ef20: 6564 6961 6e20 3d20 6e70 2e6d 6564 6961  edian = np.media
+0001ef30: 6e28 6461 7461 6672 616d 652c 2061 7869  n(dataframe, axi
+0001ef40: 733d 3029 0a20 2020 2064 6966 6620 3d20  s=0).    diff = 
+0001ef50: 6e70 2e73 756d 2828 6461 7461 6672 616d  np.sum((datafram
+0001ef60: 6520 2d20 6d65 6469 616e 292a 2a32 2c20  e - median)**2, 
+0001ef70: 6178 6973 3d2d 3129 0a20 2020 2064 6966  axis=-1).    dif
+0001ef80: 6620 3d20 6e70 2e73 7172 7428 6469 6666  f = np.sqrt(diff
+0001ef90: 290a 2020 2020 6d65 645f 6162 735f 6465  ).    med_abs_de
+0001efa0: 7669 6174 696f 6e20 3d20 6e70 2e6d 6564  viation = np.med
+0001efb0: 6961 6e28 6469 6666 290a 0a20 2020 206d  ian(diff)..    m
+0001efc0: 6f64 6966 6965 645f 7a5f 7363 6f72 6520  odified_z_score 
+0001efd0: 3d20 302e 3637 3435 202a 2064 6966 6620  = 0.6745 * diff 
+0001efe0: 2f20 6d65 645f 6162 735f 6465 7669 6174  / med_abs_deviat
+0001eff0: 696f 6e0a 2020 2020 7265 7475 726e 206d  ion.    return m
+0001f000: 6f64 6966 6965 645f 7a5f 7363 6f72 6520  odified_z_score 
+0001f010: 3e20 7468 7265 7368 0a0a 6465 6620 4544  > thresh..def ED
+0001f020: 415f 6669 6e64 5f6f 7574 6c69 6572 7328  A_find_outliers(
+0001f030: 6466 2c20 636f 6c2c 2074 6872 6573 683d  df, col, thresh=
+0001f040: 3529 3a0a 2020 2020 2222 220a 2020 2020  5):.    """.    
+0001f050: 2222 220a 2020 2020 2323 2323 2323 2320  """.    ####### 
+0001f060: 4669 6e64 7320 4f75 746c 6965 7273 2061  Finds Outliers a
+0001f070: 6e64 206d 6172 6b73 2074 6865 6d20 6173  nd marks them as
+0001f080: 2027 5472 7565 2720 6966 2074 6865 7920   'True' if they 
+0001f090: 6172 6520 6f75 746c 6965 7273 0a20 2020  are outliers.   
+0001f0a0: 2023 2323 2323 2323 2044 6174 6166 7261   ####### Datafra
+0001f0b0: 6d65 2072 6566 6572 7320 746f 2074 6865  me refers to the
+0001f0c0: 2069 6e70 7574 2064 6174 6166 7261 6d65   input dataframe
+0001f0d0: 2061 6e64 2074 6872 6573 686f 6c64 2072   and threshold r
+0001f0e0: 6566 6572 7320 746f 2068 6f77 2066 6172  efers to how far
+0001f0f0: 2066 726f 6d20 7468 6520 6d65 6469 616e   from the median
+0001f100: 2061 2076 616c 7565 2069 730a 2020 2020   a value is.    
+0001f110: 2323 2323 2323 2320 4920 616d 2075 7369  ####### I am usi
+0001f120: 6e67 2074 6865 204d 6564 6961 6e20 4162  ng the Median Ab
+0001f130: 736f 6c75 7465 2044 6576 6961 7469 6f6e  solute Deviation
+0001f140: 204d 6574 686f 6420 284d 4144 4429 2074   Method (MADD) t
+0001f150: 6f20 6669 6e64 204f 7574 6c69 6572 7320  o find Outliers 
+0001f160: 6865 7265 0a20 2020 206d 6173 6b5f 6f75  here.    mask_ou
+0001f170: 746c 6965 7273 203d 2069 735f 6f75 746c  tliers = is_outl
+0001f180: 6965 7228 6466 5b63 6f6c 5d2c 7468 7265  ier(df[col],thre
+0001f190: 7368 3d74 6872 6573 6829 2e61 7374 7970  sh=thresh).astyp
+0001f1a0: 6528 696e 7429 0a20 2020 2072 6574 7572  e(int).    retur
+0001f1b0: 6e20 6466 2e69 6c6f 635b 6e70 2e77 6865  n df.iloc[np.whe
+0001f1c0: 7265 286d 6173 6b5f 6f75 746c 6965 7273  re(mask_outliers
+0001f1d0: 3e30 295d 0a23 2323 2323 2323 2323 2323  >0)].###########
 0001f1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f1f0: 2323 2323 2323 0a64 6566 206f 7574 6c69  ######.def outli
-0001f200: 6572 5f64 6574 6572 6d69 6e65 5f74 6872  er_determine_thr
-0001f210: 6573 686f 6c64 2864 662c 2063 6f6c 293a  eshold(df, col):
-0001f220: 0a20 2020 2022 2222 0a20 2020 2054 6869  .    """.    Thi
-0001f230: 7320 6675 6e63 7469 6f6e 2061 7574 6f6d  s function autom
-0001f240: 6174 6963 616c 6c79 2064 6574 6572 6d69  atically determi
-0001f250: 6e65 7320 7468 6520 7269 6768 7420 7468  nes the right th
-0001f260: 7265 7368 6f6c 6420 666f 7220 7468 6520  reshold for the 
-0001f270: 6461 7461 6672 616d 6520 616e 6420 636f  dataframe and co
-0001f280: 6c75 6d6e 2e0a 2020 2020 5468 7265 7368  lumn..    Thresh
-0001f290: 6f6c 6420 6973 2075 7365 6420 746f 2064  old is used to d
-0001f2a0: 6574 6572 6d69 6e65 2068 6f77 206d 616e  etermine how man
-0001f2b0: 7920 6f75 746c 6965 7273 2077 6520 7368  y outliers we sh
-0001f2c0: 6f75 6c64 2064 6574 6563 7420 696e 2074  ould detect in t
-0001f2d0: 6865 2073 6572 6965 732e 0a20 2020 2041  he series..    A
-0001f2e0: 206c 6f77 2074 6872 6573 686f 6c64 2077   low threshold w
-0001f2f0: 696c 6c20 7265 7375 6c74 2069 6e20 746f  ill result in to
-0001f300: 6f20 6d61 6e79 206f 7574 6c69 6572 7320  o many outliers 
-0001f310: 616e 6420 6120 7665 7279 2068 6967 6820  and a very high 
-0001f320: 7468 7265 7368 6f6c 6420 7769 6c6c 206e  threshold will n
-0001f330: 6f74 2066 696e 6420 616e 792e 0a20 2020  ot find any..   
-0001f340: 2054 6869 7320 6c6f 6f70 7320 756e 7469   This loops unti
-0001f350: 6c20 6974 2066 696e 6473 206c 6573 7320  l it finds less 
-0001f360: 7468 616e 2031 3020 7469 6d65 7320 6f72  than 10 times or
-0001f370: 206d 6178 696d 756d 2031 2520 6f66 2064   maximum 1% of d
-0001f380: 6174 6120 6265 696e 6720 6f75 746c 6965  ata being outlie
-0001f390: 7273 2e0a 2020 2020 2222 220a 2020 2020  rs..    """.    
-0001f3a0: 6466 203d 2064 662e 636f 7079 2864 6565  df = df.copy(dee
-0001f3b0: 703d 5472 7565 290a 2020 2020 6b65 6570  p=True).    keep
-0001f3c0: 5f6c 6f6f 7069 6e67 203d 2054 7275 650a  _looping = True.
-0001f3d0: 2020 2020 6e75 6d62 6572 5f6f 665f 6c6f      number_of_lo
-0001f3e0: 6f70 7320 3d20 310a 2020 2020 7468 7265  ops = 1.    thre
-0001f3f0: 7368 203d 2035 0a20 2020 2077 6869 6c65  sh = 5.    while
-0001f400: 206b 6565 705f 6c6f 6f70 696e 673a 0a20   keep_looping:. 
-0001f410: 2020 2020 2020 2069 6620 6e75 6d62 6572         if number
-0001f420: 5f6f 665f 6c6f 6f70 7320 3e3d 2031 303a  _of_loops >= 10:
-0001f430: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
-0001f440: 616b 0a20 2020 2020 2020 206d 6173 6b5f  ak.        mask_
-0001f450: 6f75 746c 6965 7273 203d 2069 735f 6f75  outliers = is_ou
-0001f460: 746c 6965 7228 6466 5b63 6f6c 5d2c 2074  tlier(df[col], t
-0001f470: 6872 6573 683d 7468 7265 7368 292e 6173  hresh=thresh).as
-0001f480: 7479 7065 2869 6e74 290a 2020 2020 2020  type(int).      
-0001f490: 2020 6466 6f75 745f 696e 6465 7820 3d20    dfout_index = 
-0001f4a0: 6466 2e69 6c6f 635b 6e70 2e77 6865 7265  df.iloc[np.where
-0001f4b0: 286d 6173 6b5f 6f75 746c 6965 7273 3e30  (mask_outliers>0
-0001f4c0: 295d 2e69 6e64 6578 0a20 2020 2020 2020  )].index.       
-0001f4d0: 2070 6374 5f6f 7574 6c69 6572 7320 3d20   pct_outliers = 
-0001f4e0: 6c65 6e28 6466 6f75 745f 696e 6465 7829  len(dfout_index)
-0001f4f0: 2f6c 656e 2864 6629 0a20 2020 2020 2020  /len(df).       
-0001f500: 2069 6620 7063 745f 6f75 746c 6965 7273   if pct_outliers
-0001f510: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0001f520: 2020 2069 6620 7468 7265 7368 203e 2035     if thresh > 5
-0001f530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001f540: 2020 7468 7265 7368 203d 2074 6872 6573    thresh = thres
-0001f550: 6820 2d20 350a 2020 2020 2020 2020 2020  h - 5.          
-0001f560: 2020 656c 6966 2074 6872 6573 6820 3d3d    elif thresh ==
-0001f570: 2035 3a0a 2020 2020 2020 2020 2020 2020   5:.            
-0001f580: 2020 2020 7265 7475 726e 2074 6872 6573      return thres
-0001f590: 680a 2020 2020 2020 2020 2020 2020 656c  h.            el
-0001f5a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001f5b0: 2020 2020 7468 7265 7368 203d 2074 6872      thresh = thr
-0001f5c0: 6573 6820 2d20 310a 2020 2020 2020 2020  esh - 1.        
-0001f5d0: 656c 6966 2020 7063 745f 6f75 746c 6965  elif  pct_outlie
-0001f5e0: 7273 203c 3d20 302e 3031 3a0a 2020 2020  rs <= 0.01:.    
-0001f5f0: 2020 2020 2020 2020 6b65 6570 5f6c 6f6f          keep_loo
-0001f600: 7069 6e67 203d 2046 616c 7365 0a20 2020  ping = False.   
-0001f610: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001f620: 2020 2020 2020 2074 6872 6573 685f 6d75         thresh_mu
-0001f630: 6c74 6970 6c69 6572 203d 2069 6e74 2828  ltiplier = int((
-0001f640: 7063 745f 6f75 746c 6965 7273 2f30 2e30  pct_outliers/0.0
-0001f650: 3129 2a30 2e35 290a 2020 2020 2020 2020  1)*0.5).        
-0001f660: 2020 2020 7468 7265 7368 203d 2074 6872      thresh = thr
-0001f670: 6573 682a 7468 7265 7368 5f6d 756c 7469  esh*thresh_multi
-0001f680: 706c 6965 720a 2020 2020 2020 2020 6e75  plier.        nu
-0001f690: 6d62 6572 5f6f 665f 6c6f 6f70 7320 2b3d  mber_of_loops +=
-0001f6a0: 2031 0a20 2020 2070 7269 6e74 2827 2020   1.    print('  
-0001f6b0: 2020 2573 204f 7574 6c69 6572 2074 6872    %s Outlier thr
-0001f6c0: 6573 686f 6c64 203d 2025 6427 2025 2863  eshold = %d' %(c
-0001f6d0: 6f6c 2c20 7468 7265 7368 2929 0a20 2020  ol, thresh)).   
-0001f6e0: 2072 6574 7572 6e20 7468 7265 7368 0a0a   return thresh..
-0001f6f0: 6672 6f6d 2063 6f6c 6c65 6374 696f 6e73  from collections
-0001f700: 2069 6d70 6f72 7420 436f 756e 7465 720a   import Counter.
-0001f710: 6465 6620 4645 5f66 696e 645f 616e 645f  def FE_find_and_
-0001f720: 6361 705f 6f75 746c 6965 7273 2864 662c  cap_outliers(df,
-0001f730: 2066 6561 7475 7265 732c 2064 726f 703d   features, drop=
-0001f740: 4661 6c73 652c 2076 6572 626f 7365 3d46  False, verbose=F
-0001f750: 616c 7365 293a 0a20 2020 2022 2222 0a20  alse):.    """. 
-0001f760: 2020 2046 4520 6174 2074 6865 2062 6567     FE at the beg
-0001f770: 696e 6e69 6e67 206f 6620 6675 6e63 7469  inning of functi
-0001f780: 6f6e 206e 616d 6520 7374 616e 6473 2066  on name stands f
-0001f790: 6f72 2046 6561 7475 7265 2045 6e67 696e  or Feature Engin
-0001f7a0: 6565 7269 6e67 2e20 4645 2066 756e 6374  eering. FE funct
-0001f7b0: 696f 6e73 2061 6464 206f 7220 6472 6f70  ions add or drop
-0001f7c0: 2066 6561 7475 7265 732e 0a20 2020 2023   features..    #
-0001f7d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f7e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f7f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f220: 2323 2323 2323 2323 0a64 6566 206f 7574  ########.def out
+0001f230: 6c69 6572 5f64 6574 6572 6d69 6e65 5f74  lier_determine_t
+0001f240: 6872 6573 686f 6c64 2864 662c 2063 6f6c  hreshold(df, col
+0001f250: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+0001f260: 6869 7320 6675 6e63 7469 6f6e 2061 7574  his function aut
+0001f270: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
+0001f280: 6d69 6e65 7320 7468 6520 7269 6768 7420  mines the right 
+0001f290: 7468 7265 7368 6f6c 6420 666f 7220 7468  threshold for th
+0001f2a0: 6520 6461 7461 6672 616d 6520 616e 6420  e dataframe and 
+0001f2b0: 636f 6c75 6d6e 2e0a 2020 2020 5468 7265  column..    Thre
+0001f2c0: 7368 6f6c 6420 6973 2075 7365 6420 746f  shold is used to
+0001f2d0: 2064 6574 6572 6d69 6e65 2068 6f77 206d   determine how m
+0001f2e0: 616e 7920 6f75 746c 6965 7273 2077 6520  any outliers we 
+0001f2f0: 7368 6f75 6c64 2064 6574 6563 7420 696e  should detect in
+0001f300: 2074 6865 2073 6572 6965 732e 0a20 2020   the series..   
+0001f310: 2041 206c 6f77 2074 6872 6573 686f 6c64   A low threshold
+0001f320: 2077 696c 6c20 7265 7375 6c74 2069 6e20   will result in 
+0001f330: 746f 6f20 6d61 6e79 206f 7574 6c69 6572  too many outlier
+0001f340: 7320 616e 6420 6120 7665 7279 2068 6967  s and a very hig
+0001f350: 6820 7468 7265 7368 6f6c 6420 7769 6c6c  h threshold will
+0001f360: 206e 6f74 2066 696e 6420 616e 792e 0a20   not find any.. 
+0001f370: 2020 2054 6869 7320 6c6f 6f70 7320 756e     This loops un
+0001f380: 7469 6c20 6974 2066 696e 6473 206c 6573  til it finds les
+0001f390: 7320 7468 616e 2031 3020 7469 6d65 7320  s than 10 times 
+0001f3a0: 6f72 206d 6178 696d 756d 2031 2520 6f66  or maximum 1% of
+0001f3b0: 2064 6174 6120 6265 696e 6720 6f75 746c   data being outl
+0001f3c0: 6965 7273 2e0a 2020 2020 2222 220a 2020  iers..    """.  
+0001f3d0: 2020 6466 203d 2064 662e 636f 7079 2864    df = df.copy(d
+0001f3e0: 6565 703d 5472 7565 290a 2020 2020 6b65  eep=True).    ke
+0001f3f0: 6570 5f6c 6f6f 7069 6e67 203d 2054 7275  ep_looping = Tru
+0001f400: 650a 2020 2020 6e75 6d62 6572 5f6f 665f  e.    number_of_
+0001f410: 6c6f 6f70 7320 3d20 310a 2020 2020 7468  loops = 1.    th
+0001f420: 7265 7368 203d 2035 0a20 2020 2077 6869  resh = 5.    whi
+0001f430: 6c65 206b 6565 705f 6c6f 6f70 696e 673a  le keep_looping:
+0001f440: 0a20 2020 2020 2020 2069 6620 6e75 6d62  .        if numb
+0001f450: 6572 5f6f 665f 6c6f 6f70 7320 3e3d 2031  er_of_loops >= 1
+0001f460: 303a 0a20 2020 2020 2020 2020 2020 2062  0:.            b
+0001f470: 7265 616b 0a20 2020 2020 2020 206d 6173  reak.        mas
+0001f480: 6b5f 6f75 746c 6965 7273 203d 2069 735f  k_outliers = is_
+0001f490: 6f75 746c 6965 7228 6466 5b63 6f6c 5d2c  outlier(df[col],
+0001f4a0: 2074 6872 6573 683d 7468 7265 7368 292e   thresh=thresh).
+0001f4b0: 6173 7479 7065 2869 6e74 290a 2020 2020  astype(int).    
+0001f4c0: 2020 2020 6466 6f75 745f 696e 6465 7820      dfout_index 
+0001f4d0: 3d20 6466 2e69 6c6f 635b 6e70 2e77 6865  = df.iloc[np.whe
+0001f4e0: 7265 286d 6173 6b5f 6f75 746c 6965 7273  re(mask_outliers
+0001f4f0: 3e30 295d 2e69 6e64 6578 0a20 2020 2020  >0)].index.     
+0001f500: 2020 2070 6374 5f6f 7574 6c69 6572 7320     pct_outliers 
+0001f510: 3d20 6c65 6e28 6466 6f75 745f 696e 6465  = len(dfout_inde
+0001f520: 7829 2f6c 656e 2864 6629 0a20 2020 2020  x)/len(df).     
+0001f530: 2020 2069 6620 7063 745f 6f75 746c 6965     if pct_outlie
+0001f540: 7273 203d 3d20 303a 0a20 2020 2020 2020  rs == 0:.       
+0001f550: 2020 2020 2069 6620 7468 7265 7368 203e       if thresh >
+0001f560: 2035 3a0a 2020 2020 2020 2020 2020 2020   5:.            
+0001f570: 2020 2020 7468 7265 7368 203d 2074 6872      thresh = thr
+0001f580: 6573 6820 2d20 350a 2020 2020 2020 2020  esh - 5.        
+0001f590: 2020 2020 656c 6966 2074 6872 6573 6820      elif thresh 
+0001f5a0: 3d3d 2035 3a0a 2020 2020 2020 2020 2020  == 5:.          
+0001f5b0: 2020 2020 2020 7265 7475 726e 2074 6872        return thr
+0001f5c0: 6573 680a 2020 2020 2020 2020 2020 2020  esh.            
+0001f5d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001f5e0: 2020 2020 2020 7468 7265 7368 203d 2074        thresh = t
+0001f5f0: 6872 6573 6820 2d20 310a 2020 2020 2020  hresh - 1.      
+0001f600: 2020 656c 6966 2020 7063 745f 6f75 746c    elif  pct_outl
+0001f610: 6965 7273 203c 3d20 302e 3031 3a0a 2020  iers <= 0.01:.  
+0001f620: 2020 2020 2020 2020 2020 6b65 6570 5f6c            keep_l
+0001f630: 6f6f 7069 6e67 203d 2046 616c 7365 0a20  ooping = False. 
+0001f640: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001f650: 2020 2020 2020 2020 2074 6872 6573 685f           thresh_
+0001f660: 6d75 6c74 6970 6c69 6572 203d 2069 6e74  multiplier = int
+0001f670: 2828 7063 745f 6f75 746c 6965 7273 2f30  ((pct_outliers/0
+0001f680: 2e30 3129 2a30 2e35 290a 2020 2020 2020  .01)*0.5).      
+0001f690: 2020 2020 2020 7468 7265 7368 203d 2074        thresh = t
+0001f6a0: 6872 6573 682a 7468 7265 7368 5f6d 756c  hresh*thresh_mul
+0001f6b0: 7469 706c 6965 720a 2020 2020 2020 2020  tiplier.        
+0001f6c0: 6e75 6d62 6572 5f6f 665f 6c6f 6f70 7320  number_of_loops 
+0001f6d0: 2b3d 2031 0a20 2020 2070 7269 6e74 2827  += 1.    print('
+0001f6e0: 2020 2020 2573 204f 7574 6c69 6572 2074      %s Outlier t
+0001f6f0: 6872 6573 686f 6c64 203d 2025 6427 2025  hreshold = %d' %
+0001f700: 2863 6f6c 2c20 7468 7265 7368 2929 0a20  (col, thresh)). 
+0001f710: 2020 2072 6574 7572 6e20 7468 7265 7368     return thresh
+0001f720: 0a0a 6672 6f6d 2063 6f6c 6c65 6374 696f  ..from collectio
+0001f730: 6e73 2069 6d70 6f72 7420 436f 756e 7465  ns import Counte
+0001f740: 720a 6465 6620 4645 5f66 696e 645f 616e  r.def FE_find_an
+0001f750: 645f 6361 705f 6f75 746c 6965 7273 2864  d_cap_outliers(d
+0001f760: 662c 2066 6561 7475 7265 732c 2064 726f  f, features, dro
+0001f770: 703d 4661 6c73 652c 2076 6572 626f 7365  p=False, verbose
+0001f780: 3d46 616c 7365 293a 0a20 2020 2022 2222  =False):.    """
+0001f790: 0a20 2020 2046 4520 6174 2074 6865 2062  .    FE at the b
+0001f7a0: 6567 696e 6e69 6e67 206f 6620 6675 6e63  eginning of func
+0001f7b0: 7469 6f6e 206e 616d 6520 7374 616e 6473  tion name stands
+0001f7c0: 2066 6f72 2046 6561 7475 7265 2045 6e67   for Feature Eng
+0001f7d0: 696e 6565 7269 6e67 2e20 4645 2066 756e  ineering. FE fun
+0001f7e0: 6374 696f 6e73 2061 6464 206f 7220 6472  ctions add or dr
+0001f7f0: 6f70 2066 6561 7475 7265 732e 0a20 2020  op features..   
+0001f800: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
 0001f810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001f820: 2323 2323 2323 2323 0a20 2020 2054 7970  ########.    Typ
-0001f830: 6963 616c 6c79 2077 6520 7468 696e 6b20  ically we think 
-0001f840: 6f66 206f 7574 6c69 6572 7320 6173 2062  of outliers as b
-0001f850: 6569 6e67 206f 6273 6572 7661 7469 6f6e  eing observation
-0001f860: 7320 6265 796f 6e64 2074 6865 2031 2e35  s beyond the 1.5
-0001f870: 2049 6e74 6572 2051 7561 7274 696c 6520   Inter Quartile 
-0001f880: 5261 6e67 6520 2849 5152 290a 2020 2020  Range (IQR).    
-0001f890: 4275 7420 7468 6973 2066 756e 6374 696f  But this functio
-0001f8a0: 6e20 7769 6c6c 2061 6c6c 6f77 2079 6f75  n will allow you
-0001f8b0: 2074 6f20 6361 7020 616e 7920 6f62 7365   to cap any obse
-0001f8c0: 7276 6174 696f 6e20 7573 696e 6720 4d41  rvation using MA
-0001f8d0: 4444 206d 6574 686f 643a 0a20 2020 2020  DD method:.     
-0001f8e0: 2020 204d 4144 443a 204d 6564 6961 6e20     MADD: Median 
-0001f8f0: 4162 736f 6c75 7465 2044 6576 6961 7469  Absolute Deviati
-0001f900: 6f6e 204d 6574 686f 6420 2d20 6974 2773  on Method - it's
-0001f910: 2061 2066 6173 7420 616e 6420 6561 7379   a fast and easy
-0001f920: 206d 6574 686f 6420 746f 2066 696e 6420   method to find 
-0001f930: 6f75 746c 6965 7273 2e0a 2020 2020 496e  outliers..    In
-0001f940: 2061 6464 6974 696f 6e2c 2074 6869 7320   addition, this 
-0001f950: 7574 696c 6974 7920 6175 746f 6d61 7469  utility automati
-0001f960: 6361 6c6c 7920 7365 6c65 6374 7320 7468  cally selects th
-0001f970: 6520 7661 6c75 6520 746f 2063 6170 2069  e value to cap i
-0001f980: 7420 6174 2e0a 2020 2020 2020 2020 202d  t at..         -
-0001f990: 2d20 5468 6520 7661 6c75 6520 746f 2062  - The value to b
-0001f9a0: 6520 6361 7070 6564 2069 7320 6261 7365  e capped is base
-0001f9b0: 6420 6f6e 206d 6178 696d 756d 2031 2520  d on maximum 1% 
-0001f9c0: 6f66 2064 6174 6120 6265 696e 6720 6f75  of data being ou
-0001f9d0: 746c 6965 7273 2e0a 2020 2020 4974 2061  tliers..    It a
-0001f9e0: 7574 6f6d 6174 6963 616c 6c79 2064 6574  utomatically det
-0001f9f0: 6572 6d69 6e65 7320 686f 7720 6661 7220  ermines how far 
-0001fa00: 6177 6179 2066 726f 6d20 6d65 6469 616e  away from median
-0001fa10: 2074 6865 2064 6174 6120 706f 696e 7420   the data point 
-0001fa20: 6e65 6564 7320 746f 2062 6520 666f 7220  needs to be for 
-0001fa30: 6974 2074 6f20 6361 6c6c 6564 2061 6e20  it to called an 
-0001fa40: 6f75 746c 6965 722e 0a20 2020 2020 2020  outlier..       
-0001fa50: 2020 2d2d 2069 7420 7573 6573 2061 2074    -- it uses a t
-0001fa60: 6872 6573 6820 6e75 6d62 6572 3a20 7468  hresh number: th
-0001fa70: 6520 6c6f 7765 7220 6974 2069 732c 206d  e lower it is, m
-0001fa80: 6f72 6520 6f75 746c 6965 7273 2e20 4974  ore outliers. It
-0001fa90: 2073 7461 7274 7320 6174 2035 206f 7220   starts at 5 or 
-0001faa0: 6869 6768 6572 2061 7320 7468 7265 7368  higher as thresh
-0001fab0: 6f6c 6420 7661 6c75 652e 0a20 2020 204e  old value..    N
-0001fac0: 6f74 6963 6520 7468 6174 2069 7420 646f  otice that it do
-0001fad0: 6573 206e 6f74 2075 7365 2061 206c 6f77  es not use a low
-0001fae0: 6572 2062 6f75 6e64 2074 6f20 6669 6e64  er bound to find
-0001faf0: 2074 6f6f 206c 6f77 206f 7574 6c69 6572   too low outlier
-0001fb00: 732e 2054 6861 7420 796f 7520 6861 7665  s. That you have
-0001fb10: 2074 6f20 646f 2074 6861 7420 796f 7572   to do that your
-0001fb20: 7365 6c66 2e0a 2020 2020 2323 2323 2323  self..    ######
-0001fb30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001fb40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001fb50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001f850: 2323 2323 2323 2323 2323 0a20 2020 2054  ##########.    T
+0001f860: 7970 6963 616c 6c79 2077 6520 7468 696e  ypically we thin
+0001f870: 6b20 6f66 206f 7574 6c69 6572 7320 6173  k of outliers as
+0001f880: 2062 6569 6e67 206f 6273 6572 7661 7469   being observati
+0001f890: 6f6e 7320 6265 796f 6e64 2074 6865 2031  ons beyond the 1
+0001f8a0: 2e35 2049 6e74 6572 2051 7561 7274 696c  .5 Inter Quartil
+0001f8b0: 6520 5261 6e67 6520 2849 5152 290a 2020  e Range (IQR).  
+0001f8c0: 2020 4275 7420 7468 6973 2066 756e 6374    But this funct
+0001f8d0: 696f 6e20 7769 6c6c 2061 6c6c 6f77 2079  ion will allow y
+0001f8e0: 6f75 2074 6f20 6361 7020 616e 7920 6f62  ou to cap any ob
+0001f8f0: 7365 7276 6174 696f 6e20 7573 696e 6720  servation using 
+0001f900: 4d41 4444 206d 6574 686f 643a 0a20 2020  MADD method:.   
+0001f910: 2020 2020 204d 4144 443a 204d 6564 6961       MADD: Media
+0001f920: 6e20 4162 736f 6c75 7465 2044 6576 6961  n Absolute Devia
+0001f930: 7469 6f6e 204d 6574 686f 6420 2d20 6974  tion Method - it
+0001f940: 2773 2061 2066 6173 7420 616e 6420 6561  's a fast and ea
+0001f950: 7379 206d 6574 686f 6420 746f 2066 696e  sy method to fin
+0001f960: 6420 6f75 746c 6965 7273 2e0a 2020 2020  d outliers..    
+0001f970: 496e 2061 6464 6974 696f 6e2c 2074 6869  In addition, thi
+0001f980: 7320 7574 696c 6974 7920 6175 746f 6d61  s utility automa
+0001f990: 7469 6361 6c6c 7920 7365 6c65 6374 7320  tically selects 
+0001f9a0: 7468 6520 7661 6c75 6520 746f 2063 6170  the value to cap
+0001f9b0: 2069 7420 6174 2e0a 2020 2020 2020 2020   it at..        
+0001f9c0: 202d 2d20 5468 6520 7661 6c75 6520 746f   -- The value to
+0001f9d0: 2062 6520 6361 7070 6564 2069 7320 6261   be capped is ba
+0001f9e0: 7365 6420 6f6e 206d 6178 696d 756d 2031  sed on maximum 1
+0001f9f0: 2520 6f66 2064 6174 6120 6265 696e 6720  % of data being 
+0001fa00: 6f75 746c 6965 7273 2e0a 2020 2020 4974  outliers..    It
+0001fa10: 2061 7574 6f6d 6174 6963 616c 6c79 2064   automatically d
+0001fa20: 6574 6572 6d69 6e65 7320 686f 7720 6661  etermines how fa
+0001fa30: 7220 6177 6179 2066 726f 6d20 6d65 6469  r away from medi
+0001fa40: 616e 2074 6865 2064 6174 6120 706f 696e  an the data poin
+0001fa50: 7420 6e65 6564 7320 746f 2062 6520 666f  t needs to be fo
+0001fa60: 7220 6974 2074 6f20 6361 6c6c 6564 2061  r it to called a
+0001fa70: 6e20 6f75 746c 6965 722e 0a20 2020 2020  n outlier..     
+0001fa80: 2020 2020 2d2d 2069 7420 7573 6573 2061      -- it uses a
+0001fa90: 2074 6872 6573 6820 6e75 6d62 6572 3a20   thresh number: 
+0001faa0: 7468 6520 6c6f 7765 7220 6974 2069 732c  the lower it is,
+0001fab0: 206d 6f72 6520 6f75 746c 6965 7273 2e20   more outliers. 
+0001fac0: 4974 2073 7461 7274 7320 6174 2035 206f  It starts at 5 o
+0001fad0: 7220 6869 6768 6572 2061 7320 7468 7265  r higher as thre
+0001fae0: 7368 6f6c 6420 7661 6c75 652e 0a20 2020  shold value..   
+0001faf0: 204e 6f74 6963 6520 7468 6174 2069 7420   Notice that it 
+0001fb00: 646f 6573 206e 6f74 2075 7365 2061 206c  does not use a l
+0001fb10: 6f77 6572 2062 6f75 6e64 2074 6f20 6669  ower bound to fi
+0001fb20: 6e64 2074 6f6f 206c 6f77 206f 7574 6c69  nd too low outli
+0001fb30: 6572 732e 2054 6861 7420 796f 7520 6861  ers. That you ha
+0001fb40: 7665 2074 6f20 646f 2074 6861 7420 796f  ve to do that yo
+0001fb50: 7572 7365 6c66 2e0a 2020 2020 2323 2323  urself..    ####
 0001fb60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001fb70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001fb80: 2323 230a 2020 2020 496e 7075 7473 3a0a  ###.    Inputs:.
-0001fb90: 2020 2020 6466 203a 2070 616e 6461 7320      df : pandas 
-0001fba0: 4461 7461 4672 616d 650a 2020 2020 6665  DataFrame.    fe
-0001fbb0: 6174 7572 6573 3a20 6120 7369 6e67 6c65  atures: a single
-0001fbc0: 2063 6f6c 756d 6e20 6f72 2061 206c 6973   column or a lis
-0001fbd0: 7420 6f66 2063 6f6c 756d 6e73 2069 6e20  t of columns in 
-0001fbe0: 796f 7572 2044 6174 6146 7261 6d65 0a20  your DataFrame. 
-0001fbf0: 2020 2063 6170 5f61 745f 6e74 685f 6c61     cap_at_nth_la
-0001fc00: 7267 6573 743a 2064 6566 6175 6c74 2069  rgest: default i
-0001fc10: 7320 3520 3d20 796f 7520 6361 6e20 7365  s 5 = you can se
-0001fc20: 7420 6974 2074 6f20 616e 7920 696e 7465  t it to any inte
-0001fc30: 6765 7220 7375 6368 2061 7320 312c 2032  ger such as 1, 2
-0001fc40: 2c20 332c 2034 2c20 352c 2065 7463 2e0a  , 3, 4, 5, etc..
-0001fc50: 0a20 2020 204f 7574 7075 7473 3a0a 2020  .    Outputs:.  
-0001fc60: 2020 6466 3a20 7061 6e64 6173 2044 6174    df: pandas Dat
-0001fc70: 6146 7261 6d65 0a20 2020 2049 7420 7265  aFrame.    It re
-0001fc80: 7475 726e 7320 7468 6520 7361 6d65 2064  turns the same d
-0001fc90: 6174 6166 7261 6d65 2061 7320 796f 7520  ataframe as you 
-0001fca0: 696e 7075 7420 756e 6c65 7373 2079 6f75  input unless you
-0001fcb0: 2063 6861 6e67 6520 6472 6f70 2074 6f20   change drop to 
-0001fcc0: 5472 7565 2069 6e20 7468 6520 696e 7075  True in the inpu
-0001fcd0: 7420 6172 6775 6d65 6e74 2e0a 0a20 2020  t argument...   
-0001fce0: 204f 7074 696f 6e61 6c6c 792c 2069 7420   Optionally, it 
-0001fcf0: 6361 6e20 6472 6f70 2063 6572 7461 696e  can drop certain
-0001fd00: 2072 6f77 7320 7468 6174 2068 6176 6520   rows that have 
-0001fd10: 746f 6f20 6d61 6e79 206f 7574 6c69 6572  too many outlier
-0001fd20: 7320 696e 2061 7420 6c65 6173 7420 3320  s in at least 3 
-0001fd30: 636f 6c75 6d6e 7320 7369 6d75 6c74 616e  columns simultan
-0001fd40: 656f 7573 6c79 2e0a 2020 2020 4966 2064  eously..    If d
-0001fd50: 726f 703d 5472 7565 2c20 6974 2077 696c  rop=True, it wil
-0001fd60: 6c20 7265 7475 726e 2061 2073 6d61 6c6c  l return a small
-0001fd70: 6572 206e 756d 6265 7220 6f66 2072 6f77  er number of row
-0001fd80: 7320 696e 2079 6f75 7220 6461 7461 6672  s in your datafr
-0001fd90: 616d 6520 7468 616e 2077 6861 7420 796f  ame than what yo
-0001fda0: 7520 7365 6e74 2069 6e2e 2042 6520 6361  u sent in. Be ca
-0001fdb0: 7265 6675 6c21 0a20 2020 2023 2323 2323  reful!.    #####
-0001fdc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001fdd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001fde0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fb80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fb90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fbb0: 2323 2323 230a 2020 2020 496e 7075 7473  #####.    Inputs
+0001fbc0: 3a0a 2020 2020 6466 203a 2070 616e 6461  :.    df : panda
+0001fbd0: 7320 4461 7461 4672 616d 650a 2020 2020  s DataFrame.    
+0001fbe0: 6665 6174 7572 6573 3a20 6120 7369 6e67  features: a sing
+0001fbf0: 6c65 2063 6f6c 756d 6e20 6f72 2061 206c  le column or a l
+0001fc00: 6973 7420 6f66 2063 6f6c 756d 6e73 2069  ist of columns i
+0001fc10: 6e20 796f 7572 2044 6174 6146 7261 6d65  n your DataFrame
+0001fc20: 0a20 2020 2063 6170 5f61 745f 6e74 685f  .    cap_at_nth_
+0001fc30: 6c61 7267 6573 743a 2064 6566 6175 6c74  largest: default
+0001fc40: 2069 7320 3520 3d20 796f 7520 6361 6e20   is 5 = you can 
+0001fc50: 7365 7420 6974 2074 6f20 616e 7920 696e  set it to any in
+0001fc60: 7465 6765 7220 7375 6368 2061 7320 312c  teger such as 1,
+0001fc70: 2032 2c20 332c 2034 2c20 352c 2065 7463   2, 3, 4, 5, etc
+0001fc80: 2e0a 0a20 2020 204f 7574 7075 7473 3a0a  ...    Outputs:.
+0001fc90: 2020 2020 6466 3a20 7061 6e64 6173 2044      df: pandas D
+0001fca0: 6174 6146 7261 6d65 0a20 2020 2049 7420  ataFrame.    It 
+0001fcb0: 7265 7475 726e 7320 7468 6520 7361 6d65  returns the same
+0001fcc0: 2064 6174 6166 7261 6d65 2061 7320 796f   dataframe as yo
+0001fcd0: 7520 696e 7075 7420 756e 6c65 7373 2079  u input unless y
+0001fce0: 6f75 2063 6861 6e67 6520 6472 6f70 2074  ou change drop t
+0001fcf0: 6f20 5472 7565 2069 6e20 7468 6520 696e  o True in the in
+0001fd00: 7075 7420 6172 6775 6d65 6e74 2e0a 0a20  put argument... 
+0001fd10: 2020 204f 7074 696f 6e61 6c6c 792c 2069     Optionally, i
+0001fd20: 7420 6361 6e20 6472 6f70 2063 6572 7461  t can drop certa
+0001fd30: 696e 2072 6f77 7320 7468 6174 2068 6176  in rows that hav
+0001fd40: 6520 746f 6f20 6d61 6e79 206f 7574 6c69  e too many outli
+0001fd50: 6572 7320 696e 2061 7420 6c65 6173 7420  ers in at least 
+0001fd60: 3320 636f 6c75 6d6e 7320 7369 6d75 6c74  3 columns simult
+0001fd70: 616e 656f 7573 6c79 2e0a 2020 2020 4966  aneously..    If
+0001fd80: 2064 726f 703d 5472 7565 2c20 6974 2077   drop=True, it w
+0001fd90: 696c 6c20 7265 7475 726e 2061 2073 6d61  ill return a sma
+0001fda0: 6c6c 6572 206e 756d 6265 7220 6f66 2072  ller number of r
+0001fdb0: 6f77 7320 696e 2079 6f75 7220 6461 7461  ows in your data
+0001fdc0: 6672 616d 6520 7468 616e 2077 6861 7420  frame than what 
+0001fdd0: 796f 7520 7365 6e74 2069 6e2e 2042 6520  you sent in. Be 
+0001fde0: 6361 7265 6675 6c21 0a20 2020 2023 2323  careful!.    ###
 0001fdf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001fe00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001fe10: 2323 2323 0a20 2020 2022 2222 0a20 2020  ####.    """.   
-0001fe20: 2064 6620 3d20 6466 2e63 6f70 7928 6465   df = df.copy(de
-0001fe30: 6570 3d54 7275 6529 0a20 2020 206f 7574  ep=True).    out
-0001fe40: 6c69 6572 5f69 6e64 6963 6573 203d 205b  lier_indices = [
-0001fe50: 5d0a 2020 2020 6964 636f 6c20 3d20 2769  ].    idcol = 'i
-0001fe60: 6463 6f6c 270a 2020 2020 6466 5b69 6463  dcol'.    df[idc
-0001fe70: 6f6c 5d20 3d20 7261 6e67 6528 6c65 6e28  ol] = range(len(
-0001fe80: 6466 2929 0a20 2020 2069 6620 6973 696e  df)).    if isin
-0001fe90: 7374 616e 6365 2866 6561 7475 7265 732c  stance(features,
-0001fea0: 2073 7472 293a 0a20 2020 2020 2020 2066   str):.        f
-0001feb0: 6561 7475 7265 7320 3d20 5b66 6561 7475  eatures = [featu
-0001fec0: 7265 735d 0a20 2020 2023 2069 7465 7261  res].    # itera
-0001fed0: 7465 206f 7665 7220 6665 6174 7572 6573  te over features
-0001fee0: 2863 6f6c 756d 6e73 290a 2020 2020 666f  (columns).    fo
-0001fef0: 7220 636f 6c20 696e 2066 6561 7475 7265  r col in feature
-0001ff00: 733a 0a20 2020 2020 2020 2023 2044 6574  s:.        # Det
-0001ff10: 6572 6d69 6e65 2061 206c 6973 7420 6f66  ermine a list of
-0001ff20: 2069 6e64 6963 6573 206f 6620 6f75 746c   indices of outl
-0001ff30: 6965 7273 2066 6f72 2066 6561 7475 7265  iers for feature
-0001ff40: 2063 6f6c 0a20 2020 2020 2020 2074 6872   col.        thr
-0001ff50: 6573 6820 3d20 6f75 746c 6965 725f 6465  esh = outlier_de
-0001ff60: 7465 726d 696e 655f 7468 7265 7368 6f6c  termine_threshol
-0001ff70: 6428 6466 2c20 636f 6c29 0a20 2020 2020  d(df, col).     
-0001ff80: 2020 206d 6173 6b5f 6f75 746c 6965 7273     mask_outliers
-0001ff90: 203d 2069 735f 6f75 746c 6965 7228 6466   = is_outlier(df
-0001ffa0: 5b63 6f6c 5d2c 2074 6872 6573 683d 7468  [col], thresh=th
-0001ffb0: 7265 7368 292e 6173 7479 7065 2869 6e74  resh).astype(int
-0001ffc0: 290a 2020 2020 2020 2020 6466 6f75 745f  ).        dfout_
-0001ffd0: 696e 6465 7820 3d20 6466 2e69 6c6f 635b  index = df.iloc[
-0001ffe0: 6e70 2e77 6865 7265 286d 6173 6b5f 6f75  np.where(mask_ou
-0001fff0: 746c 6965 7273 3e30 295d 2e69 6e64 6578  tliers>0)].index
-00020000: 0a0a 2020 2020 2020 2020 6466 5b27 616e  ..        df['an
-00020010: 6f6d 616c 7931 275d 203d 2030 0a20 2020  omaly1'] = 0.   
-00020020: 2020 2020 2064 662e 6c6f 635b 6466 6f75       df.loc[dfou
-00020030: 745f 696e 6465 7820 2c27 616e 6f6d 616c  t_index ,'anomal
-00020040: 7931 275d 203d 2031 0a0a 2020 2020 2020  y1'] = 1..      
-00020050: 2020 2323 2320 7468 6973 2069 7320 686f    ### this is ho
-00020060: 7720 7468 6520 636f 6c75 6d6e 206c 6f6f  w the column loo
-00020070: 6b73 206e 6f77 2062 6566 6f72 6520 6361  ks now before ca
-00020080: 7070 696e 6720 6f75 746c 6965 7273 0a20  pping outliers. 
-00020090: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-000200a0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-000200b0: 6967 2c20 2861 7831 2c61 7832 2920 3d20  ig, (ax1,ax2) = 
-000200c0: 706c 742e 7375 6270 6c6f 7473 2831 2c32  plt.subplots(1,2
-000200d0: 2c66 6967 7369 7a65 3d28 3132 2c35 2929  ,figsize=(12,5))
-000200e0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-000200f0: 6f72 7320 3d20 7b30 3a27 626c 7565 272c  ors = {0:'blue',
-00020100: 2031 3a27 7265 6427 7d0a 2020 2020 2020   1:'red'}.      
-00020110: 2020 2020 2020 6178 312e 7363 6174 7465        ax1.scatte
-00020120: 7228 6466 5b69 6463 6f6c 5d2c 2064 665b  r(df[idcol], df[
-00020130: 636f 6c5d 2c20 633d 6466 5b22 616e 6f6d  col], c=df["anom
-00020140: 616c 7931 225d 2e61 7070 6c79 286c 616d  aly1"].apply(lam
-00020150: 6264 6120 783a 2063 6f6c 6f72 735b 785d  bda x: colors[x]
-00020160: 2929 0a20 2020 2020 2020 2020 2020 2061  )).            a
-00020170: 7831 2e73 6574 5f78 6c61 6265 6c28 2752  x1.set_xlabel('R
-00020180: 6f77 2049 4427 290a 2020 2020 2020 2020  ow ID').        
-00020190: 2020 2020 6178 312e 7365 745f 796c 6162      ax1.set_ylab
-000201a0: 656c 2827 5461 7267 6574 2076 616c 7565  el('Target value
-000201b0: 7327 290a 2020 2020 2020 2020 2020 2020  s').            
-000201c0: 6178 312e 7365 745f 7469 746c 6528 2725  ax1.set_title('%
-000201d0: 7320 6265 666f 7265 2063 6170 7069 6e67  s before capping
-000201e0: 206f 7574 6c69 6572 7327 2025 636f 6c29   outliers' %col)
-000201f0: 0a0a 2020 2020 2020 2020 6361 7070 6564  ..        capped
-00020200: 5f76 616c 7565 203d 2064 662e 6c6f 635b  _value = df.loc[
-00020210: 6466 6f75 745f 696e 6465 782c 2063 6f6c  dfout_index, col
-00020220: 5d2e 6d69 6e28 2920 2323 2074 6869 7320  ].min() ## this 
-00020230: 6973 2074 6865 2076 616c 7565 2077 6520  is the value we 
-00020240: 6361 7020 6974 2061 6761 696e 7374 0a20  cap it against. 
-00020250: 2020 2020 2020 2064 662e 6c6f 635b 6466         df.loc[df
-00020260: 6f75 745f 696e 6465 782c 2063 6f6c 5d20  out_index, col] 
-00020270: 3d20 2063 6170 7065 645f 7661 6c75 6520  =  capped_value 
-00020280: 2323 206d 6178 696d 756d 2076 616c 7565  ## maximum value
-00020290: 7320 6172 6520 6e6f 7720 6361 7070 6564  s are now capped
-000202a0: 0a20 2020 2020 2020 2023 2323 2079 6f75  .        ### you
-000202b0: 2061 7265 206e 6f77 2067 6f6f 6420 746f   are now good to
-000202c0: 2067 6f20 2d20 796f 7520 6361 6e20 7368   go - you can sh
-000202d0: 6f77 2068 6f77 2074 6865 7920 6172 6520  ow how they are 
-000202e0: 6361 7070 6564 2075 7369 6e67 2062 6566  capped using bef
-000202f0: 6f72 6520 616e 6420 6166 7465 7220 7069  ore and after pi
-00020300: 6373 0a20 2020 2020 2020 2069 6620 7665  cs.        if ve
-00020310: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-00020320: 2020 2063 6f6c 6f72 7320 3d20 7b30 3a27     colors = {0:'
-00020330: 626c 7565 272c 2031 3a27 7265 6427 7d0a  blue', 1:'red'}.
-00020340: 2020 2020 2020 2020 2020 2020 6178 322e              ax2.
-00020350: 7363 6174 7465 7228 6466 5b69 6463 6f6c  scatter(df[idcol
-00020360: 5d2c 2064 665b 636f 6c5d 2c20 633d 6466  ], df[col], c=df
-00020370: 5b22 616e 6f6d 616c 7931 225d 2e61 7070  ["anomaly1"].app
-00020380: 6c79 286c 616d 6264 6120 783a 2063 6f6c  ly(lambda x: col
-00020390: 6f72 735b 785d 2929 0a20 2020 2020 2020  ors[x])).       
-000203a0: 2020 2020 2061 7832 2e73 6574 5f78 6c61       ax2.set_xla
-000203b0: 6265 6c28 2752 6f77 2049 4427 290a 2020  bel('Row ID').  
-000203c0: 2020 2020 2020 2020 2020 6178 322e 7365            ax2.se
-000203d0: 745f 796c 6162 656c 2827 5461 7267 6574  t_ylabel('Target
-000203e0: 2076 616c 7565 7327 290a 2020 2020 2020   values').      
-000203f0: 2020 2020 2020 6178 322e 7365 745f 7469        ax2.set_ti
-00020400: 746c 6528 2725 7320 6166 7465 7220 6361  tle('%s after ca
-00020410: 7070 696e 6720 6f75 746c 6965 7273 2720  pping outliers' 
-00020420: 2563 6f6c 290a 0a20 2020 2020 2020 2023  %col)..        #
-00020430: 204c 6574 2773 2073 6176 6520 7468 6520   Let's save the 
-00020440: 6c69 7374 206f 6620 6f75 746c 6965 7273  list of outliers
-00020450: 2061 6e64 2073 6565 2069 6620 7468 6572   and see if ther
-00020460: 6520 6172 6520 736f 6d65 2077 6974 6820  e are some with 
-00020470: 6f75 746c 6965 7273 2069 6e20 6d75 6c74  outliers in mult
-00020480: 6970 6c65 2063 6f6c 756d 6e73 0a20 2020  iple columns.   
-00020490: 2020 2020 206f 7574 6c69 6572 5f69 6e64       outlier_ind
-000204a0: 6963 6573 2e65 7874 656e 6428 6466 6f75  ices.extend(dfou
-000204b0: 745f 696e 6465 7829 0a0a 2020 2020 2320  t_index)..    # 
-000204c0: 7365 6c65 6374 2063 6572 7461 696e 206f  select certain o
-000204d0: 6273 6572 7661 7469 6f6e 7320 636f 6e74  bservations cont
-000204e0: 6169 6e69 6e67 206d 6f72 6520 7468 616e  aining more than
-000204f0: 206f 6e65 206f 7574 6c69 6572 2069 6e20   one outlier in 
-00020500: 3220 636f 6c75 6d6e 7320 6f72 206d 6f72  2 columns or mor
-00020510: 652e 2057 6520 6361 6e20 6472 6f70 2074  e. We can drop t
-00020520: 6865 6d21 0a20 2020 206f 7574 6c69 6572  hem!.    outlier
-00020530: 5f69 6e64 6963 6573 203d 2043 6f75 6e74  _indices = Count
-00020540: 6572 286f 7574 6c69 6572 5f69 6e64 6963  er(outlier_indic
-00020550: 6573 290a 2020 2020 6d75 6c74 6970 6c65  es).    multiple
-00020560: 5f6f 7574 6c69 6572 7320 3d20 6c69 7374  _outliers = list
-00020570: 2820 6b20 666f 7220 6b2c 2076 2069 6e20  ( k for k, v in 
-00020580: 6f75 746c 6965 725f 696e 6469 6365 732e  outlier_indices.
-00020590: 6974 656d 7328 2920 6966 2076 203e 2033  items() if v > 3
-000205a0: 2029 0a20 2020 2023 2323 206e 6f77 2064   ).    ### now d
-000205b0: 726f 7020 7468 6573 6520 726f 7773 2061  rop these rows a
-000205c0: 6c74 6f67 6574 6865 7220 2323 2323 0a20  ltogether ####. 
-000205d0: 2020 2064 6620 3d20 6466 2e64 726f 7028     df = df.drop(
-000205e0: 5b69 6463 6f6c 2c27 616e 6f6d 616c 7931  [idcol,'anomaly1
-000205f0: 275d 2c20 6178 6973 3d31 290a 2020 2020  '], axis=1).    
-00020600: 6966 2064 726f 703a 0a20 2020 2020 2020  if drop:.       
-00020610: 2070 7269 6e74 2827 5368 6170 6520 6f66   print('Shape of
-00020620: 2064 6174 6166 7261 6d65 2062 6566 6f72   dataframe befor
-00020630: 6520 6f75 746c 6965 7273 2062 6569 6e67  e outliers being
-00020640: 2064 726f 7070 6564 3a20 2573 2720 2528   dropped: %s' %(
-00020650: 6466 2e73 6861 7065 2c29 290a 2020 2020  df.shape,)).    
-00020660: 2020 2020 6e75 6d62 6572 5f6f 665f 726f      number_of_ro
-00020670: 7773 203d 2064 662e 7368 6170 655b 305d  ws = df.shape[0]
-00020680: 0a20 2020 2020 2020 2064 6620 3d20 6466  .        df = df
-00020690: 2e64 726f 7028 6d75 6c74 6970 6c65 5f6f  .drop(multiple_o
-000206a0: 7574 6c69 6572 732c 2061 7869 733d 3029  utliers, axis=0)
-000206b0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-000206c0: 5368 6170 6520 6f66 2064 6174 6166 7261  Shape of datafra
-000206d0: 6d65 2061 6674 6572 206f 7574 6c69 6572  me after outlier
-000206e0: 7320 6265 696e 6720 6472 6f70 7065 643a  s being dropped:
-000206f0: 2025 7327 2025 2864 662e 7368 6170 652c   %s' %(df.shape,
-00020700: 2929 0a20 2020 2020 2020 2070 7269 6e74  )).        print
-00020710: 2827 5c6e 4e75 6d62 6572 5f6f 665f 726f  ('\nNumber_of_ro
-00020720: 7773 2077 6974 6820 6d75 6c74 6970 6c65  ws with multiple
-00020730: 206f 7574 6c69 6572 7320 696e 206d 6f72   outliers in mor
-00020740: 6520 7468 616e 2033 2063 6f6c 756d 6e73  e than 3 columns
-00020750: 2077 6869 6368 2077 6572 6520 6472 6f70   which were drop
-00020760: 7065 6420 3d20 2564 2720 2528 6e75 6d62  ped = %d' %(numb
-00020770: 6572 5f6f 665f 726f 7773 2d64 662e 7368  er_of_rows-df.sh
-00020780: 6170 655b 305d 2929 0a20 2020 2072 6574  ape[0])).    ret
-00020790: 7572 6e20 6466 0a23 2323 2323 2323 2323  urn df.#########
-000207a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000207b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000207c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fe10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fe20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fe30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001fe40: 2323 2323 2323 0a20 2020 2022 2222 0a20  ######.    """. 
+0001fe50: 2020 2064 6620 3d20 6466 2e63 6f70 7928     df = df.copy(
+0001fe60: 6465 6570 3d54 7275 6529 0a20 2020 206f  deep=True).    o
+0001fe70: 7574 6c69 6572 5f69 6e64 6963 6573 203d  utlier_indices =
+0001fe80: 205b 5d0a 2020 2020 6964 636f 6c20 3d20   [].    idcol = 
+0001fe90: 2769 6463 6f6c 270a 2020 2020 6466 5b69  'idcol'.    df[i
+0001fea0: 6463 6f6c 5d20 3d20 7261 6e67 6528 6c65  dcol] = range(le
+0001feb0: 6e28 6466 2929 0a20 2020 2069 6620 6973  n(df)).    if is
+0001fec0: 696e 7374 616e 6365 2866 6561 7475 7265  instance(feature
+0001fed0: 732c 2073 7472 293a 0a20 2020 2020 2020  s, str):.       
+0001fee0: 2066 6561 7475 7265 7320 3d20 5b66 6561   features = [fea
+0001fef0: 7475 7265 735d 0a20 2020 2023 2069 7465  tures].    # ite
+0001ff00: 7261 7465 206f 7665 7220 6665 6174 7572  rate over featur
+0001ff10: 6573 2863 6f6c 756d 6e73 290a 2020 2020  es(columns).    
+0001ff20: 666f 7220 636f 6c20 696e 2066 6561 7475  for col in featu
+0001ff30: 7265 733a 0a20 2020 2020 2020 2023 2044  res:.        # D
+0001ff40: 6574 6572 6d69 6e65 2061 206c 6973 7420  etermine a list 
+0001ff50: 6f66 2069 6e64 6963 6573 206f 6620 6f75  of indices of ou
+0001ff60: 746c 6965 7273 2066 6f72 2066 6561 7475  tliers for featu
+0001ff70: 7265 2063 6f6c 0a20 2020 2020 2020 2074  re col.        t
+0001ff80: 6872 6573 6820 3d20 6f75 746c 6965 725f  hresh = outlier_
+0001ff90: 6465 7465 726d 696e 655f 7468 7265 7368  determine_thresh
+0001ffa0: 6f6c 6428 6466 2c20 636f 6c29 0a20 2020  old(df, col).   
+0001ffb0: 2020 2020 206d 6173 6b5f 6f75 746c 6965       mask_outlie
+0001ffc0: 7273 203d 2069 735f 6f75 746c 6965 7228  rs = is_outlier(
+0001ffd0: 6466 5b63 6f6c 5d2c 2074 6872 6573 683d  df[col], thresh=
+0001ffe0: 7468 7265 7368 292e 6173 7479 7065 2869  thresh).astype(i
+0001fff0: 6e74 290a 2020 2020 2020 2020 6466 6f75  nt).        dfou
+00020000: 745f 696e 6465 7820 3d20 6466 2e69 6c6f  t_index = df.ilo
+00020010: 635b 6e70 2e77 6865 7265 286d 6173 6b5f  c[np.where(mask_
+00020020: 6f75 746c 6965 7273 3e30 295d 2e69 6e64  outliers>0)].ind
+00020030: 6578 0a0a 2020 2020 2020 2020 6466 5b27  ex..        df['
+00020040: 616e 6f6d 616c 7931 275d 203d 2030 0a20  anomaly1'] = 0. 
+00020050: 2020 2020 2020 2064 662e 6c6f 635b 6466         df.loc[df
+00020060: 6f75 745f 696e 6465 7820 2c27 616e 6f6d  out_index ,'anom
+00020070: 616c 7931 275d 203d 2031 0a0a 2020 2020  aly1'] = 1..    
+00020080: 2020 2020 2323 2320 7468 6973 2069 7320      ### this is 
+00020090: 686f 7720 7468 6520 636f 6c75 6d6e 206c  how the column l
+000200a0: 6f6f 6b73 206e 6f77 2062 6566 6f72 6520  ooks now before 
+000200b0: 6361 7070 696e 6720 6f75 746c 6965 7273  capping outliers
+000200c0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+000200d0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+000200e0: 2066 6967 2c20 2861 7831 2c61 7832 2920   fig, (ax1,ax2) 
+000200f0: 3d20 706c 742e 7375 6270 6c6f 7473 2831  = plt.subplots(1
+00020100: 2c32 2c66 6967 7369 7a65 3d28 3132 2c35  ,2,figsize=(12,5
+00020110: 2929 0a20 2020 2020 2020 2020 2020 2063  )).            c
+00020120: 6f6c 6f72 7320 3d20 7b30 3a27 626c 7565  olors = {0:'blue
+00020130: 272c 2031 3a27 7265 6427 7d0a 2020 2020  ', 1:'red'}.    
+00020140: 2020 2020 2020 2020 6178 312e 7363 6174          ax1.scat
+00020150: 7465 7228 6466 5b69 6463 6f6c 5d2c 2064  ter(df[idcol], d
+00020160: 665b 636f 6c5d 2c20 633d 6466 5b22 616e  f[col], c=df["an
+00020170: 6f6d 616c 7931 225d 2e61 7070 6c79 286c  omaly1"].apply(l
+00020180: 616d 6264 6120 783a 2063 6f6c 6f72 735b  ambda x: colors[
+00020190: 785d 2929 0a20 2020 2020 2020 2020 2020  x])).           
+000201a0: 2061 7831 2e73 6574 5f78 6c61 6265 6c28   ax1.set_xlabel(
+000201b0: 2752 6f77 2049 4427 290a 2020 2020 2020  'Row ID').      
+000201c0: 2020 2020 2020 6178 312e 7365 745f 796c        ax1.set_yl
+000201d0: 6162 656c 2827 5461 7267 6574 2076 616c  abel('Target val
+000201e0: 7565 7327 290a 2020 2020 2020 2020 2020  ues').          
+000201f0: 2020 6178 312e 7365 745f 7469 746c 6528    ax1.set_title(
+00020200: 2725 7320 6265 666f 7265 2063 6170 7069  '%s before cappi
+00020210: 6e67 206f 7574 6c69 6572 7327 2025 636f  ng outliers' %co
+00020220: 6c29 0a0a 2020 2020 2020 2020 6361 7070  l)..        capp
+00020230: 6564 5f76 616c 7565 203d 2064 662e 6c6f  ed_value = df.lo
+00020240: 635b 6466 6f75 745f 696e 6465 782c 2063  c[dfout_index, c
+00020250: 6f6c 5d2e 6d69 6e28 2920 2323 2074 6869  ol].min() ## thi
+00020260: 7320 6973 2074 6865 2076 616c 7565 2077  s is the value w
+00020270: 6520 6361 7020 6974 2061 6761 696e 7374  e cap it against
+00020280: 0a20 2020 2020 2020 2064 662e 6c6f 635b  .        df.loc[
+00020290: 6466 6f75 745f 696e 6465 782c 2063 6f6c  dfout_index, col
+000202a0: 5d20 3d20 2063 6170 7065 645f 7661 6c75  ] =  capped_valu
+000202b0: 6520 2323 206d 6178 696d 756d 2076 616c  e ## maximum val
+000202c0: 7565 7320 6172 6520 6e6f 7720 6361 7070  ues are now capp
+000202d0: 6564 0a20 2020 2020 2020 2023 2323 2079  ed.        ### y
+000202e0: 6f75 2061 7265 206e 6f77 2067 6f6f 6420  ou are now good 
+000202f0: 746f 2067 6f20 2d20 796f 7520 6361 6e20  to go - you can 
+00020300: 7368 6f77 2068 6f77 2074 6865 7920 6172  show how they ar
+00020310: 6520 6361 7070 6564 2075 7369 6e67 2062  e capped using b
+00020320: 6566 6f72 6520 616e 6420 6166 7465 7220  efore and after 
+00020330: 7069 6373 0a20 2020 2020 2020 2069 6620  pics.        if 
+00020340: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+00020350: 2020 2020 2063 6f6c 6f72 7320 3d20 7b30       colors = {0
+00020360: 3a27 626c 7565 272c 2031 3a27 7265 6427  :'blue', 1:'red'
+00020370: 7d0a 2020 2020 2020 2020 2020 2020 6178  }.            ax
+00020380: 322e 7363 6174 7465 7228 6466 5b69 6463  2.scatter(df[idc
+00020390: 6f6c 5d2c 2064 665b 636f 6c5d 2c20 633d  ol], df[col], c=
+000203a0: 6466 5b22 616e 6f6d 616c 7931 225d 2e61  df["anomaly1"].a
+000203b0: 7070 6c79 286c 616d 6264 6120 783a 2063  pply(lambda x: c
+000203c0: 6f6c 6f72 735b 785d 2929 0a20 2020 2020  olors[x])).     
+000203d0: 2020 2020 2020 2061 7832 2e73 6574 5f78         ax2.set_x
+000203e0: 6c61 6265 6c28 2752 6f77 2049 4427 290a  label('Row ID').
+000203f0: 2020 2020 2020 2020 2020 2020 6178 322e              ax2.
+00020400: 7365 745f 796c 6162 656c 2827 5461 7267  set_ylabel('Targ
+00020410: 6574 2076 616c 7565 7327 290a 2020 2020  et values').    
+00020420: 2020 2020 2020 2020 6178 322e 7365 745f          ax2.set_
+00020430: 7469 746c 6528 2725 7320 6166 7465 7220  title('%s after 
+00020440: 6361 7070 696e 6720 6f75 746c 6965 7273  capping outliers
+00020450: 2720 2563 6f6c 290a 0a20 2020 2020 2020  ' %col)..       
+00020460: 2023 204c 6574 2773 2073 6176 6520 7468   # Let's save th
+00020470: 6520 6c69 7374 206f 6620 6f75 746c 6965  e list of outlie
+00020480: 7273 2061 6e64 2073 6565 2069 6620 7468  rs and see if th
+00020490: 6572 6520 6172 6520 736f 6d65 2077 6974  ere are some wit
+000204a0: 6820 6f75 746c 6965 7273 2069 6e20 6d75  h outliers in mu
+000204b0: 6c74 6970 6c65 2063 6f6c 756d 6e73 0a20  ltiple columns. 
+000204c0: 2020 2020 2020 206f 7574 6c69 6572 5f69         outlier_i
+000204d0: 6e64 6963 6573 2e65 7874 656e 6428 6466  ndices.extend(df
+000204e0: 6f75 745f 696e 6465 7829 0a0a 2020 2020  out_index)..    
+000204f0: 2320 7365 6c65 6374 2063 6572 7461 696e  # select certain
+00020500: 206f 6273 6572 7661 7469 6f6e 7320 636f   observations co
+00020510: 6e74 6169 6e69 6e67 206d 6f72 6520 7468  ntaining more th
+00020520: 616e 206f 6e65 206f 7574 6c69 6572 2069  an one outlier i
+00020530: 6e20 3220 636f 6c75 6d6e 7320 6f72 206d  n 2 columns or m
+00020540: 6f72 652e 2057 6520 6361 6e20 6472 6f70  ore. We can drop
+00020550: 2074 6865 6d21 0a20 2020 206f 7574 6c69   them!.    outli
+00020560: 6572 5f69 6e64 6963 6573 203d 2043 6f75  er_indices = Cou
+00020570: 6e74 6572 286f 7574 6c69 6572 5f69 6e64  nter(outlier_ind
+00020580: 6963 6573 290a 2020 2020 6d75 6c74 6970  ices).    multip
+00020590: 6c65 5f6f 7574 6c69 6572 7320 3d20 6c69  le_outliers = li
+000205a0: 7374 2820 6b20 666f 7220 6b2c 2076 2069  st( k for k, v i
+000205b0: 6e20 6f75 746c 6965 725f 696e 6469 6365  n outlier_indice
+000205c0: 732e 6974 656d 7328 2920 6966 2076 203e  s.items() if v >
+000205d0: 2033 2029 0a20 2020 2023 2323 206e 6f77   3 ).    ### now
+000205e0: 2064 726f 7020 7468 6573 6520 726f 7773   drop these rows
+000205f0: 2061 6c74 6f67 6574 6865 7220 2323 2323   altogether ####
+00020600: 0a20 2020 2064 6620 3d20 6466 2e64 726f  .    df = df.dro
+00020610: 7028 5b69 6463 6f6c 2c27 616e 6f6d 616c  p([idcol,'anomal
+00020620: 7931 275d 2c20 6178 6973 3d31 290a 2020  y1'], axis=1).  
+00020630: 2020 6966 2064 726f 703a 0a20 2020 2020    if drop:.     
+00020640: 2020 2070 7269 6e74 2827 5368 6170 6520     print('Shape 
+00020650: 6f66 2064 6174 6166 7261 6d65 2062 6566  of dataframe bef
+00020660: 6f72 6520 6f75 746c 6965 7273 2062 6569  ore outliers bei
+00020670: 6e67 2064 726f 7070 6564 3a20 2573 2720  ng dropped: %s' 
+00020680: 2528 6466 2e73 6861 7065 2c29 290a 2020  %(df.shape,)).  
+00020690: 2020 2020 2020 6e75 6d62 6572 5f6f 665f        number_of_
+000206a0: 726f 7773 203d 2064 662e 7368 6170 655b  rows = df.shape[
+000206b0: 305d 0a20 2020 2020 2020 2064 6620 3d20  0].        df = 
+000206c0: 6466 2e64 726f 7028 6d75 6c74 6970 6c65  df.drop(multiple
+000206d0: 5f6f 7574 6c69 6572 732c 2061 7869 733d  _outliers, axis=
+000206e0: 3029 0a20 2020 2020 2020 2070 7269 6e74  0).        print
+000206f0: 2827 5368 6170 6520 6f66 2064 6174 6166  ('Shape of dataf
+00020700: 7261 6d65 2061 6674 6572 206f 7574 6c69  rame after outli
+00020710: 6572 7320 6265 696e 6720 6472 6f70 7065  ers being droppe
+00020720: 643a 2025 7327 2025 2864 662e 7368 6170  d: %s' %(df.shap
+00020730: 652c 2929 0a20 2020 2020 2020 2070 7269  e,)).        pri
+00020740: 6e74 2827 5c6e 4e75 6d62 6572 5f6f 665f  nt('\nNumber_of_
+00020750: 726f 7773 2077 6974 6820 6d75 6c74 6970  rows with multip
+00020760: 6c65 206f 7574 6c69 6572 7320 696e 206d  le outliers in m
+00020770: 6f72 6520 7468 616e 2033 2063 6f6c 756d  ore than 3 colum
+00020780: 6e73 2077 6869 6368 2077 6572 6520 6472  ns which were dr
+00020790: 6f70 7065 6420 3d20 2564 2720 2528 6e75  opped = %d' %(nu
+000207a0: 6d62 6572 5f6f 665f 726f 7773 2d64 662e  mber_of_rows-df.
+000207b0: 7368 6170 655b 305d 2929 0a20 2020 2072  shape[0])).    r
+000207c0: 6574 7572 6e20 6466 0a23 2323 2323 2323  eturn df.#######
 000207d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000207e0: 2323 2323 2323 2323 0a69 6d70 6f72 7420  ########.import 
-000207f0: 7061 6e64 6173 2061 7320 7064 0a69 6d70  pandas as pd.imp
-00020800: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00020810: 696d 706f 7274 2070 6462 0a66 726f 6d20  import pdb.from 
-00020820: 736b 6c65 6172 6e2e 7574 696c 732e 7661  sklearn.utils.va
-00020830: 6c69 6461 7469 6f6e 2069 6d70 6f72 7420  lidation import 
-00020840: 6368 6563 6b5f 585f 792c 2063 6865 636b  check_X_y, check
-00020850: 5f69 735f 6669 7474 6564 0a66 726f 6d20  _is_fitted.from 
-00020860: 736b 6c65 6172 6e2e 7072 6570 726f 6365  sklearn.preproce
-00020870: 7373 696e 6720 696d 706f 7274 204c 6162  ssing import Lab
-00020880: 656c 456e 636f 6465 720a 6672 6f6d 2063  elEncoder.from c
-00020890: 6f6c 6c65 6374 696f 6e73 2069 6d70 6f72  ollections impor
-000208a0: 7420 436f 756e 7465 722c 2064 6566 6175  t Counter, defau
-000208b0: 6c74 6469 6374 0a66 726f 6d20 736b 6c65  ltdict.from skle
-000208c0: 6172 6e2e 6261 7365 2069 6d70 6f72 7420  arn.base import 
-000208d0: 4261 7365 4573 7469 6d61 746f 722c 2043  BaseEstimator, C
-000208e0: 6c61 7373 6966 6965 724d 6978 696e 2c20  lassifierMixin, 
-000208f0: 5472 616e 7366 6f72 6d65 724d 6978 696e  TransformerMixin
-00020900: 0a0a 6672 6f6d 2069 6d62 6c65 6172 6e2e  ..from imblearn.
-00020910: 6f76 6572 5f73 616d 706c 696e 6720 696d  over_sampling im
-00020920: 706f 7274 2053 4d4f 5445 2c20 5356 4d53  port SMOTE, SVMS
-00020930: 4d4f 5445 0a66 726f 6d20 696d 626c 6561  MOTE.from imblea
-00020940: 726e 2e6f 7665 725f 7361 6d70 6c69 6e67  rn.over_sampling
-00020950: 2069 6d70 6f72 7420 4144 4153 594e 2c20   import ADASYN, 
-00020960: 534d 4f54 454e 430a 0a69 6d70 6f72 7420  SMOTENC..import 
-00020970: 7061 6e64 6173 2061 7320 7064 0a69 6d70  pandas as pd.imp
-00020980: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00020990: 6672 6f6d 2063 6f6c 6c65 6374 696f 6e73  from collections
-000209a0: 2069 6d70 6f72 7420 436f 756e 7465 720a   import Counter.
-000209b0: 696d 706f 7274 2077 6172 6e69 6e67 730a  import warnings.
-000209c0: 7761 726e 696e 6773 2e66 696c 7465 7277  warnings.filterw
-000209d0: 6172 6e69 6e67 7328 2269 676e 6f72 6522  arnings("ignore"
-000209e0: 290a 2323 2323 2323 2323 2323 2323 2323  ).##############
-000209f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00020a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00020a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000207e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000207f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00020800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00020810: 2323 2323 2323 2323 2323 0a69 6d70 6f72  ##########.impor
+00020820: 7420 7061 6e64 6173 2061 7320 7064 0a69  t pandas as pd.i
+00020830: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+00020840: 700a 696d 706f 7274 2070 6462 0a66 726f  p.import pdb.fro
+00020850: 6d20 736b 6c65 6172 6e2e 7574 696c 732e  m sklearn.utils.
+00020860: 7661 6c69 6461 7469 6f6e 2069 6d70 6f72  validation impor
+00020870: 7420 6368 6563 6b5f 585f 792c 2063 6865  t check_X_y, che
+00020880: 636b 5f69 735f 6669 7474 6564 0a66 726f  ck_is_fitted.fro
+00020890: 6d20 736b 6c65 6172 6e2e 7072 6570 726f  m sklearn.prepro
+000208a0: 6365 7373 696e 6720 696d 706f 7274 204c  cessing import L
+000208b0: 6162 656c 456e 636f 6465 720a 6672 6f6d  abelEncoder.from
+000208c0: 2063 6f6c 6c65 6374 696f 6e73 2069 6d70   collections imp
+000208d0: 6f72 7420 436f 756e 7465 722c 2064 6566  ort Counter, def
+000208e0: 6175 6c74 6469 6374 0a66 726f 6d20 736b  aultdict.from sk
+000208f0: 6c65 6172 6e2e 6261 7365 2069 6d70 6f72  learn.base impor
+00020900: 7420 4261 7365 4573 7469 6d61 746f 722c  t BaseEstimator,
+00020910: 2043 6c61 7373 6966 6965 724d 6978 696e   ClassifierMixin
+00020920: 2c20 5472 616e 7366 6f72 6d65 724d 6978  , TransformerMix
+00020930: 696e 0a0a 6672 6f6d 2069 6d62 6c65 6172  in..from imblear
+00020940: 6e2e 6f76 6572 5f73 616d 706c 696e 6720  n.over_sampling 
+00020950: 696d 706f 7274 2053 4d4f 5445 2c20 5356  import SMOTE, SV
+00020960: 4d53 4d4f 5445 0a66 726f 6d20 696d 626c  MSMOTE.from imbl
+00020970: 6561 726e 2e6f 7665 725f 7361 6d70 6c69  earn.over_sampli
+00020980: 6e67 2069 6d70 6f72 7420 4144 4153 594e  ng import ADASYN
+00020990: 2c20 534d 4f54 454e 430a 0a69 6d70 6f72  , SMOTENC..impor
+000209a0: 7420 7061 6e64 6173 2061 7320 7064 0a69  t pandas as pd.i
+000209b0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+000209c0: 700a 6672 6f6d 2063 6f6c 6c65 6374 696f  p.from collectio
+000209d0: 6e73 2069 6d70 6f72 7420 436f 756e 7465  ns import Counte
+000209e0: 720a 696d 706f 7274 2077 6172 6e69 6e67  r.import warning
+000209f0: 730a 7761 726e 696e 6773 2e66 696c 7465  s.warnings.filte
+00020a00: 7277 6172 6e69 6e67 7328 2269 676e 6f72  rwarnings("ignor
+00020a10: 6522 290a 2323 2323 2323 2323 2323 2323  e").############
 00020a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00020a30: 2323 230a 696d 706f 7274 2063 6f70 790a  ###.import copy.
-00020a40: 6672 6f6d 2073 6b6c 6561 726e 2e63 6c75  from sklearn.clu
-00020a50: 7374 6572 2069 6d70 6f72 7420 4b4d 6561  ster import KMea
-00020a60: 6e73 0a64 6566 2046 455f 6b6d 6561 6e73  ns.def FE_kmeans
-00020a70: 5f72 6573 616d 706c 6572 2878 5f74 7261  _resampler(x_tra
-00020a80: 696e 2c20 795f 7472 6169 6e2c 2074 6172  in, y_train, tar
-00020a90: 6765 742c 2073 6d6f 7465 3d22 222c 2076  get, smote="", v
-00020aa0: 6572 626f 7365 3d30 293a 0a20 2020 2022  erbose=0):.    "
-00020ab0: 2222 0a20 2020 2054 6869 7320 6675 6e63  "".    This func
-00020ac0: 7469 6f6e 2063 6f6e 7665 7274 7320 6120  tion converts a 
-00020ad0: 5265 6772 6573 7369 6f6e 2070 726f 626c  Regression probl
-00020ae0: 656d 2069 6e74 6f20 6120 436c 6173 7369  em into a Classi
-00020af0: 6669 6361 7469 6f6e 2070 726f 626c 656d  fication problem
-00020b00: 2074 6f20 656e 6162 6c65 2053 4d4f 5445   to enable SMOTE
-00020b10: 210a 2020 2020 4974 2069 7320 6120 7665  !.    It is a ve
-00020b20: 7279 2073 696d 706c 6520 7761 7920 746f  ry simple way to
-00020b30: 2073 656e 6420 796f 7572 2078 5f74 7261   send your x_tra
-00020b40: 696e 2c20 795f 7472 6169 6e20 696e 2061  in, y_train in a
-00020b50: 6e64 2067 6574 2062 6163 6b20 616e 206f  nd get back an o
-00020b60: 7665 7273 616d 706c 6564 2078 5f74 7261  versampled x_tra
-00020b70: 696e 2c20 795f 7472 6169 6e2e 0a20 2020  in, y_train..   
-00020b80: 2057 6879 2069 7320 7468 6973 206e 6565   Why is this nee
-00020b90: 6465 6420 696e 204d 6163 6869 6e65 204c  ded in Machine L
-00020ba0: 6561 726e 696e 6720 7072 6f62 6c65 6d73  earning problems
-00020bb0: 3f0a 2020 2020 2020 2020 2049 6e20 496d  ?.         In Im
-00020bc0: 6261 6c61 6e63 6564 2064 6174 6173 6574  balanced dataset
-00020bd0: 732c 2065 7370 2e20 736b 6577 6564 2072  s, esp. skewed r
-00020be0: 6567 7265 7373 696f 6e20 7072 6f62 6c65  egression proble
-00020bf0: 6d73 2077 6865 7265 2074 6865 2074 6172  ms where the tar
-00020c00: 6765 7420 7661 7269 6162 6c65 2069 7320  get variable is 
-00020c10: 736b 6577 6564 2c20 7468 6973 2069 7320  skewed, this is 
-00020c20: 6e65 6564 6564 2e0a 2020 2020 5472 7920  needed..    Try 
-00020c30: 7468 6973 206f 6e20 796f 7572 2073 6b65  this on your ske
-00020c40: 7765 6420 5265 6772 6573 7369 6f6e 2070  wed Regression p
-00020c50: 726f 626c 656d 7320 616e 6420 7365 6520  roblems and see 
-00020c60: 7768 6174 2072 6573 756c 7473 2079 6f75  what results you
-00020c70: 2067 6574 2e20 4974 2073 686f 756c 6420   get. It should 
-00020c80: 6265 2062 6574 7465 722e 0a20 2020 202d  be better..    -
-00020c90: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 496e  ---------.    In
-00020ca0: 7075 7473 0a20 2020 202d 2d2d 2d2d 2d2d  puts.    -------
-00020cb0: 2d2d 2d0a 2020 2020 785f 7472 6169 6e20  ---.    x_train 
-00020cc0: 3a20 7061 6e64 6173 2064 6174 6166 7261  : pandas datafra
-00020cd0: 6d65 3a20 796f 7520 6d75 7374 2073 656e  me: you must sen
-00020ce0: 6420 696e 2074 6865 2064 6174 6120 7769  d in the data wi
-00020cf0: 7468 2070 7265 6469 6374 6f72 7320 6f6e  th predictors on
-00020d00: 6c79 2e0a 2020 2020 6d69 6e5f 6e5f 7361  ly..    min_n_sa
-00020d10: 6d70 6c65 7320 3a20 696e 742c 2064 6566  mples : int, def
-00020d20: 6175 6c74 3d35 3a20 6d69 6e20 6e75 6d62  ault=5: min numb
-00020d30: 6572 206f 6620 7361 6d70 6c65 7320 6265  er of samples be
-00020d40: 6c6f 7720 7768 6963 6820 796f 7520 636f  low which you co
-00020d50: 6d62 696e 6520 6269 6e73 0a20 2020 2062  mbine bins.    b
-00020d60: 696e 7320 3a20 696e 742c 2064 6566 6175  ins : int, defau
-00020d70: 6c74 3d33 3a20 686f 7720 6d61 6e79 2062  lt=3: how many b
-00020d80: 696e 7320 796f 7520 7761 6e74 2074 6f20  ins you want to 
-00020d90: 7370 6c69 7420 7461 7267 6574 2069 6e74  split target int
-00020da0: 6f0a 0a20 2020 204f 7574 7075 7473 0a20  o..    Outputs. 
-00020db0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00020dc0: 2020 6e5f 6665 6174 7572 6573 5f20 3a20    n_features_ : 
-00020dd0: 696e 740a 2020 2020 2020 2020 5468 6520  int.        The 
-00020de0: 6e75 6d62 6572 206f 6620 6665 6174 7572  number of featur
-00020df0: 6573 206f 6620 7468 6520 6461 7461 2070  es of the data p
-00020e00: 6173 7365 6420 746f 203a 6d65 7468 3a60  assed to :meth:`
-00020e10: 6669 7460 2e0a 2020 2020 2222 220a 2020  fit`..    """.  
-00020e20: 2020 785f 7472 6169 6e5f 6320 3d20 636f    x_train_c = co
-00020e30: 7079 2e64 6565 7063 6f70 7928 785f 7472  py.deepcopy(x_tr
-00020e40: 6169 6e29 0a20 2020 2078 5f74 7261 696e  ain).    x_train
-00020e50: 5f63 5b74 6172 6765 745d 203d 2079 5f74  _c[target] = y_t
-00020e60: 7261 696e 2e76 616c 7565 730a 0a20 2020  rain.values..   
-00020e70: 2023 2052 6567 7265 7373 696f 6e20 7072   # Regression pr
-00020e80: 6f62 6c65 6d20 7475 726e 6564 2069 6e74  oblem turned int
-00020e90: 6f20 436c 6173 7369 6669 6361 7469 6f6e  o Classification
-00020ea0: 2070 726f 626c 656d 0a20 2020 206e 5f63   problem.    n_c
-00020eb0: 6c75 7374 6572 7320 3d20 6d61 7828 332c  lusters = max(3,
-00020ec0: 2069 6e74 286e 702e 6c6f 6731 3028 6c65   int(np.log10(le
-00020ed0: 6e28 795f 7472 6169 6e29 2929 202b 2031  n(y_train))) + 1
-00020ee0: 290a 2020 2020 2320 5573 6520 4b4d 6561  ).    # Use KMea
-00020ef0: 6e73 2074 6f20 6669 6e64 206e 6174 7572  ns to find natur
-00020f00: 616c 2063 6c75 7374 6572 7320 696e 2079  al clusters in y
-00020f10: 6f75 7220 6461 7461 0a20 2020 206b 6d5f  our data.    km_
-00020f20: 6d6f 6465 6c20 3d20 4b4d 6561 6e73 286e  model = KMeans(n
-00020f30: 5f63 6c75 7374 6572 733d 6e5f 636c 7573  _clusters=n_clus
-00020f40: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
-00020f50: 2020 2020 2020 2020 2020 2020 6e5f 696e              n_in
-00020f60: 6974 3d35 2c0a 2020 2020 2020 2020 2020  it=5,.          
-00020f70: 2020 2020 2020 2020 2020 2020 7261 6e64              rand
-00020f80: 6f6d 5f73 7461 7465 3d39 3929 0a20 2020  om_state=99).   
-00020f90: 2023 2323 2320 7265 6d65 6d62 6572 2079   #### remember y
-00020fa0: 6f75 206d 7573 7420 7072 6564 6963 7420  ou must predict 
-00020fb0: 7573 696e 6720 6f6e 6c79 2070 7265 6469  using only predi
-00020fc0: 6374 6f72 2076 6172 6961 626c 6573 210a  ctor variables!.
-00020fd0: 2020 2020 795f 7472 6169 6e5f 6320 3d20      y_train_c = 
-00020fe0: 6b6d 5f6d 6f64 656c 2e66 6974 5f70 7265  km_model.fit_pre
-00020ff0: 6469 6374 2878 5f74 7261 696e 290a 0a20  dict(x_train).. 
-00021000: 2020 2069 6620 7665 7262 6f73 6520 3e3d     if verbose >=
-00021010: 2031 3a0a 2020 2020 2020 2020 7072 696e   1:.        prin
-00021020: 7428 274e 756d 6265 7220 6f66 2063 6c75  t('Number of clu
-00021030: 7374 6572 7320 6372 6561 7465 6420 3d20  sters created = 
-00021040: 2564 2720 256e 5f63 6c75 7374 6572 7329  %d' %n_clusters)
-00021050: 0a0a 2020 2020 2323 2323 2047 656e 6572  ..    #### Gener
-00021060: 6174 6520 7468 6520 6f76 6572 2d73 616d  ate the over-sam
-00021070: 706c 6564 2064 6174 610a 2020 2020 2323  pled data.    ##
-00021080: 2323 2041 4441 5359 4e20 2f20 534d 4f54  ## ADASYN / SMOT
-00021090: 4520 6f76 6572 7361 6d70 6c69 6e67 2023  E oversampling #
-000210a0: 2323 2323 0a20 2020 2069 6620 6973 696e  ####.    if isin
-000210b0: 7374 616e 6365 2873 6d6f 7465 2c20 7374  stance(smote, st
-000210c0: 7229 3a0a 2020 2020 2020 2020 785f 7472  r):.        x_tr
-000210d0: 6169 6e5f 6578 742c 205f 203d 206f 7665  ain_ext, _ = ove
-000210e0: 7273 616d 706c 655f 534d 4f54 4528 785f  rsample_SMOTE(x_
-000210f0: 7472 6169 6e5f 632c 2079 5f74 7261 696e  train_c, y_train
-00021100: 5f63 290a 2020 2020 656c 7365 3a0a 2020  _c).    else:.  
-00021110: 2020 2020 2020 785f 7472 6169 6e5f 6578        x_train_ex
-00021120: 742c 205f 203d 2073 6d6f 7465 2e66 6974  t, _ = smote.fit
-00021130: 5f72 6573 616d 706c 6528 785f 7472 6169  _resample(x_trai
-00021140: 6e5f 632c 2079 5f74 7261 696e 5f63 290a  n_c, y_train_c).
-00021150: 2020 2020 795f 7472 6169 6e5f 6578 7420      y_train_ext 
-00021160: 3d20 785f 7472 6169 6e5f 6578 745b 7461  = x_train_ext[ta
-00021170: 7267 6574 5d2e 7661 6c75 6573 0a20 2020  rget].values.   
-00021180: 2078 5f74 7261 696e 5f65 7874 203d 2078   x_train_ext = x
-00021190: 5f74 7261 696e 5f65 7874 2e64 726f 7028  _train_ext.drop(
-000211a0: 7461 7267 6574 2c20 6178 6973 3d31 290a  target, axis=1).
-000211b0: 2020 2020 7265 7475 726e 2028 785f 7472      return (x_tr
-000211c0: 6169 6e5f 6578 742c 2079 5f74 7261 696e  ain_ext, y_train
-000211d0: 5f65 7874 290a 0a23 2323 2323 2323 2323  _ext)..#########
-000211e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000211f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00020a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00020a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00020a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00020a60: 2323 2323 230a 696d 706f 7274 2063 6f70  #####.import cop
+00020a70: 790a 6672 6f6d 2073 6b6c 6561 726e 2e63  y.from sklearn.c
+00020a80: 6c75 7374 6572 2069 6d70 6f72 7420 4b4d  luster import KM
+00020a90: 6561 6e73 0a64 6566 2046 455f 6b6d 6561  eans.def FE_kmea
+00020aa0: 6e73 5f72 6573 616d 706c 6572 2878 5f74  ns_resampler(x_t
+00020ab0: 7261 696e 2c20 795f 7472 6169 6e2c 2074  rain, y_train, t
+00020ac0: 6172 6765 742c 2073 6d6f 7465 3d22 222c  arget, smote="",
+00020ad0: 2076 6572 626f 7365 3d30 293a 0a20 2020   verbose=0):.   
+00020ae0: 2022 2222 0a20 2020 2054 6869 7320 6675   """.    This fu
+00020af0: 6e63 7469 6f6e 2063 6f6e 7665 7274 7320  nction converts 
+00020b00: 6120 5265 6772 6573 7369 6f6e 2070 726f  a Regression pro
+00020b10: 626c 656d 2069 6e74 6f20 6120 436c 6173  blem into a Clas
+00020b20: 7369 6669 6361 7469 6f6e 2070 726f 626c  sification probl
+00020b30: 656d 2074 6f20 656e 6162 6c65 2053 4d4f  em to enable SMO
+00020b40: 5445 210a 2020 2020 4974 2069 7320 6120  TE!.    It is a 
+00020b50: 7665 7279 2073 696d 706c 6520 7761 7920  very simple way 
+00020b60: 746f 2073 656e 6420 796f 7572 2078 5f74  to send your x_t
+00020b70: 7261 696e 2c20 795f 7472 6169 6e20 696e  rain, y_train in
+00020b80: 2061 6e64 2067 6574 2062 6163 6b20 616e   and get back an
+00020b90: 206f 7665 7273 616d 706c 6564 2078 5f74   oversampled x_t
+00020ba0: 7261 696e 2c20 795f 7472 6169 6e2e 0a20  rain, y_train.. 
+00020bb0: 2020 2057 6879 2069 7320 7468 6973 206e     Why is this n
+00020bc0: 6565 6465 6420 696e 204d 6163 6869 6e65  eeded in Machine
+00020bd0: 204c 6561 726e 696e 6720 7072 6f62 6c65   Learning proble
+00020be0: 6d73 3f0a 2020 2020 2020 2020 2049 6e20  ms?.         In 
+00020bf0: 496d 6261 6c61 6e63 6564 2064 6174 6173  Imbalanced datas
+00020c00: 6574 732c 2065 7370 2e20 736b 6577 6564  ets, esp. skewed
+00020c10: 2072 6567 7265 7373 696f 6e20 7072 6f62   regression prob
+00020c20: 6c65 6d73 2077 6865 7265 2074 6865 2074  lems where the t
+00020c30: 6172 6765 7420 7661 7269 6162 6c65 2069  arget variable i
+00020c40: 7320 736b 6577 6564 2c20 7468 6973 2069  s skewed, this i
+00020c50: 7320 6e65 6564 6564 2e0a 2020 2020 5472  s needed..    Tr
+00020c60: 7920 7468 6973 206f 6e20 796f 7572 2073  y this on your s
+00020c70: 6b65 7765 6420 5265 6772 6573 7369 6f6e  kewed Regression
+00020c80: 2070 726f 626c 656d 7320 616e 6420 7365   problems and se
+00020c90: 6520 7768 6174 2072 6573 756c 7473 2079  e what results y
+00020ca0: 6f75 2067 6574 2e20 4974 2073 686f 756c  ou get. It shoul
+00020cb0: 6420 6265 2062 6574 7465 722e 0a20 2020  d be better..   
+00020cc0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00020cd0: 496e 7075 7473 0a20 2020 202d 2d2d 2d2d  Inputs.    -----
+00020ce0: 2d2d 2d2d 2d0a 2020 2020 785f 7472 6169  -----.    x_trai
+00020cf0: 6e20 3a20 7061 6e64 6173 2064 6174 6166  n : pandas dataf
+00020d00: 7261 6d65 3a20 796f 7520 6d75 7374 2073  rame: you must s
+00020d10: 656e 6420 696e 2074 6865 2064 6174 6120  end in the data 
+00020d20: 7769 7468 2070 7265 6469 6374 6f72 7320  with predictors 
+00020d30: 6f6e 6c79 2e0a 2020 2020 6d69 6e5f 6e5f  only..    min_n_
+00020d40: 7361 6d70 6c65 7320 3a20 696e 742c 2064  samples : int, d
+00020d50: 6566 6175 6c74 3d35 3a20 6d69 6e20 6e75  efault=5: min nu
+00020d60: 6d62 6572 206f 6620 7361 6d70 6c65 7320  mber of samples 
+00020d70: 6265 6c6f 7720 7768 6963 6820 796f 7520  below which you 
+00020d80: 636f 6d62 696e 6520 6269 6e73 0a20 2020  combine bins.   
+00020d90: 2062 696e 7320 3a20 696e 742c 2064 6566   bins : int, def
+00020da0: 6175 6c74 3d33 3a20 686f 7720 6d61 6e79  ault=3: how many
+00020db0: 2062 696e 7320 796f 7520 7761 6e74 2074   bins you want t
+00020dc0: 6f20 7370 6c69 7420 7461 7267 6574 2069  o split target i
+00020dd0: 6e74 6f0a 0a20 2020 204f 7574 7075 7473  nto..    Outputs
+00020de0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00020df0: 2020 2020 6e5f 6665 6174 7572 6573 5f20      n_features_ 
+00020e00: 3a20 696e 740a 2020 2020 2020 2020 5468  : int.        Th
+00020e10: 6520 6e75 6d62 6572 206f 6620 6665 6174  e number of feat
+00020e20: 7572 6573 206f 6620 7468 6520 6461 7461  ures of the data
+00020e30: 2070 6173 7365 6420 746f 203a 6d65 7468   passed to :meth
+00020e40: 3a60 6669 7460 2e0a 2020 2020 2222 220a  :`fit`..    """.
+00020e50: 2020 2020 785f 7472 6169 6e5f 6320 3d20      x_train_c = 
+00020e60: 636f 7079 2e64 6565 7063 6f70 7928 785f  copy.deepcopy(x_
+00020e70: 7472 6169 6e29 0a20 2020 2078 5f74 7261  train).    x_tra
+00020e80: 696e 5f63 5b74 6172 6765 745d 203d 2079  in_c[target] = y
+00020e90: 5f74 7261 696e 2e76 616c 7565 730a 0a20  _train.values.. 
+00020ea0: 2020 2023 2052 6567 7265 7373 696f 6e20     # Regression 
+00020eb0: 7072 6f62 6c65 6d20 7475 726e 6564 2069  problem turned i
+00020ec0: 6e74 6f20 436c 6173 7369 6669 6361 7469  nto Classificati
+00020ed0: 6f6e 2070 726f 626c 656d 0a20 2020 206e  on problem.    n
+00020ee0: 5f63 6c75 7374 6572 7320 3d20 6d61 7828  _clusters = max(
+00020ef0: 332c 2069 6e74 286e 702e 6c6f 6731 3028  3, int(np.log10(
+00020f00: 6c65 6e28 795f 7472 6169 6e29 2929 202b  len(y_train))) +
+00020f10: 2031 290a 2020 2020 2320 5573 6520 4b4d   1).    # Use KM
+00020f20: 6561 6e73 2074 6f20 6669 6e64 206e 6174  eans to find nat
+00020f30: 7572 616c 2063 6c75 7374 6572 7320 696e  ural clusters in
+00020f40: 2079 6f75 7220 6461 7461 0a20 2020 206b   your data.    k
+00020f50: 6d5f 6d6f 6465 6c20 3d20 4b4d 6561 6e73  m_model = KMeans
+00020f60: 286e 5f63 6c75 7374 6572 733d 6e5f 636c  (n_clusters=n_cl
+00020f70: 7573 7465 7273 2c0a 2020 2020 2020 2020  usters,.        
+00020f80: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+00020f90: 696e 6974 3d35 2c0a 2020 2020 2020 2020  init=5,.        
+00020fa0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00020fb0: 6e64 6f6d 5f73 7461 7465 3d39 3929 0a20  ndom_state=99). 
+00020fc0: 2020 2023 2323 2320 7265 6d65 6d62 6572     #### remember
+00020fd0: 2079 6f75 206d 7573 7420 7072 6564 6963   you must predic
+00020fe0: 7420 7573 696e 6720 6f6e 6c79 2070 7265  t using only pre
+00020ff0: 6469 6374 6f72 2076 6172 6961 626c 6573  dictor variables
+00021000: 210a 2020 2020 795f 7472 6169 6e5f 6320  !.    y_train_c 
+00021010: 3d20 6b6d 5f6d 6f64 656c 2e66 6974 5f70  = km_model.fit_p
+00021020: 7265 6469 6374 2878 5f74 7261 696e 290a  redict(x_train).
+00021030: 0a20 2020 2069 6620 7665 7262 6f73 6520  .    if verbose 
+00021040: 3e3d 2031 3a0a 2020 2020 2020 2020 7072  >= 1:.        pr
+00021050: 696e 7428 274e 756d 6265 7220 6f66 2063  int('Number of c
+00021060: 6c75 7374 6572 7320 6372 6561 7465 6420  lusters created 
+00021070: 3d20 2564 2720 256e 5f63 6c75 7374 6572  = %d' %n_cluster
+00021080: 7329 0a0a 2020 2020 2323 2323 2047 656e  s)..    #### Gen
+00021090: 6572 6174 6520 7468 6520 6f76 6572 2d73  erate the over-s
+000210a0: 616d 706c 6564 2064 6174 610a 2020 2020  ampled data.    
+000210b0: 2323 2323 2041 4441 5359 4e20 2f20 534d  #### ADASYN / SM
+000210c0: 4f54 4520 6f76 6572 7361 6d70 6c69 6e67  OTE oversampling
+000210d0: 2023 2323 2323 0a20 2020 2069 6620 6973   #####.    if is
+000210e0: 696e 7374 616e 6365 2873 6d6f 7465 2c20  instance(smote, 
+000210f0: 7374 7229 3a0a 2020 2020 2020 2020 785f  str):.        x_
+00021100: 7472 6169 6e5f 6578 742c 205f 203d 206f  train_ext, _ = o
+00021110: 7665 7273 616d 706c 655f 534d 4f54 4528  versample_SMOTE(
+00021120: 785f 7472 6169 6e5f 632c 2079 5f74 7261  x_train_c, y_tra
+00021130: 696e 5f63 290a 2020 2020 656c 7365 3a0a  in_c).    else:.
+00021140: 2020 2020 2020 2020 785f 7472 6169 6e5f          x_train_
+00021150: 6578 742c 205f 203d 2073 6d6f 7465 2e66  ext, _ = smote.f
+00021160: 6974 5f72 6573 616d 706c 6528 785f 7472  it_resample(x_tr
+00021170: 6169 6e5f 632c 2079 5f74 7261 696e 5f63  ain_c, y_train_c
+00021180: 290a 2020 2020 795f 7472 6169 6e5f 6578  ).    y_train_ex
+00021190: 7420 3d20 785f 7472 6169 6e5f 6578 745b  t = x_train_ext[
+000211a0: 7461 7267 6574 5d2e 7661 6c75 6573 0a20  target].values. 
+000211b0: 2020 2078 5f74 7261 696e 5f65 7874 203d     x_train_ext =
+000211c0: 2078 5f74 7261 696e 5f65 7874 2e64 726f   x_train_ext.dro
+000211d0: 7028 7461 7267 6574 2c20 6178 6973 3d31  p(target, axis=1
+000211e0: 290a 2020 2020 7265 7475 726e 2028 785f  ).    return (x_
+000211f0: 7472 6169 6e5f 6578 742c 2079 5f74 7261  train_ext, y_tra
+00021200: 696e 5f65 7874 290a 0a23 2323 2323 2323  in_ext)..#######
 00021210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00021220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021230: 2323 2323 2323 2323 2323 0a23 2043 616c  ##########.# Cal
-00021240: 6375 6c61 7465 2063 6c61 7373 2077 6569  culate class wei
-00021250: 6768 740a 696d 706f 7274 2063 6f70 790a  ght.import copy.
-00021260: 6672 6f6d 2063 6f6c 6c65 6374 696f 6e73  from collections
-00021270: 2069 6d70 6f72 7420 436f 756e 7465 720a   import Counter.
-00021280: 6672 6f6d 2073 6b6c 6561 726e 2e75 7469  from sklearn.uti
-00021290: 6c73 2e63 6c61 7373 5f77 6569 6768 7420  ls.class_weight 
-000212a0: 696d 706f 7274 2063 6f6d 7075 7465 5f63  import compute_c
-000212b0: 6c61 7373 5f77 6569 6768 740a 6465 6620  lass_weight.def 
-000212c0: 6765 745f 636c 6173 735f 6469 7374 7269  get_class_distri
-000212d0: 6275 7469 6f6e 2879 5f69 6e70 7574 2c20  bution(y_input, 
-000212e0: 7665 7262 6f73 653d 3029 3a0a 2020 2020  verbose=0):.    
-000212f0: 795f 696e 7075 7420 3d20 636f 7079 2e64  y_input = copy.d
-00021300: 6565 7063 6f70 7928 795f 696e 7075 7429  eepcopy(y_input)
-00021310: 0a20 2020 2063 6c61 7373 6573 203d 206e  .    classes = n
-00021320: 702e 756e 6971 7565 2879 5f69 6e70 7574  p.unique(y_input
-00021330: 290a 2020 2020 7870 203d 2043 6f75 6e74  ).    xp = Count
-00021340: 6572 2879 5f69 6e70 7574 290a 2020 2020  er(y_input).    
-00021350: 636c 6173 735f 7765 6967 6874 7320 3d20  class_weights = 
-00021360: 636f 6d70 7574 655f 636c 6173 735f 7765  compute_class_we
-00021370: 6967 6874 2827 6261 6c61 6e63 6564 272c  ight('balanced',
-00021380: 2063 6c61 7373 6573 3d6e 702e 756e 6971   classes=np.uniq
-00021390: 7565 2879 5f69 6e70 7574 292c 2079 3d79  ue(y_input), y=y
-000213a0: 5f69 6e70 7574 290a 2020 2020 6966 206c  _input).    if l
-000213b0: 656e 2863 6c61 7373 5f77 6569 6768 7473  en(class_weights
-000213c0: 5b28 636c 6173 735f 7765 6967 6874 733e  [(class_weights>
-000213d0: 2031 3029 5d29 203e 2030 3a0a 2020 2020   10)]) > 0:.    
-000213e0: 2020 2020 636c 6173 735f 7765 6967 6874      class_weight
-000213f0: 7320 3d20 2863 6c61 7373 5f77 6569 6768  s = (class_weigh
-00021400: 7473 2f31 3029 0a20 2020 2065 6c73 653a  ts/10).    else:
-00021410: 0a20 2020 2020 2020 2063 6c61 7373 5f77  .        class_w
-00021420: 6569 6768 7473 203d 2028 636c 6173 735f  eights = (class_
-00021430: 7765 6967 6874 7329 0a20 2020 2023 7072  weights).    #pr
-00021440: 696e 7428 2720 2020 2063 6c61 7373 5f77  int('    class_w
-00021450: 6569 6768 7473 203d 2025 7327 2025 636c  eights = %s' %cl
-00021460: 6173 735f 7765 6967 6874 7329 0a20 2020  ass_weights).   
-00021470: 2063 6c61 7373 5f77 6569 6768 7473 5b28   class_weights[(
-00021480: 636c 6173 735f 7765 6967 6874 733c 3129  class_weights<1)
-00021490: 5d3d 310a 2020 2020 636c 6173 735f 726f  ]=1.    class_ro
-000214a0: 7773 203d 2063 6c61 7373 5f77 6569 6768  ws = class_weigh
-000214b0: 7473 2a5b 7870 5b78 5d20 666f 7220 7820  ts*[xp[x] for x 
-000214c0: 696e 2063 6c61 7373 6573 5d0a 2020 2020  in classes].    
-000214d0: 636c 6173 735f 726f 7773 203d 2063 6c61  class_rows = cla
-000214e0: 7373 5f72 6f77 732e 6173 7479 7065 2869  ss_rows.astype(i
-000214f0: 6e74 290a 2020 2020 636c 6173 735f 7765  nt).    class_we
-00021500: 6967 6874 6564 5f72 6f77 7320 3d20 6469  ighted_rows = di
-00021510: 6374 287a 6970 2863 6c61 7373 6573 2c63  ct(zip(classes,c
-00021520: 6c61 7373 5f72 6f77 7329 290a 2020 2020  lass_rows)).    
-00021530: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-00021540: 2020 2020 7072 696e 7428 2720 2020 2063      print('    c
-00021550: 6c61 7373 5f77 6569 6768 7465 645f 726f  lass_weighted_ro
-00021560: 7773 203d 2025 7327 2025 636c 6173 735f  ws = %s' %class_
-00021570: 7765 6967 6874 6564 5f72 6f77 7329 0a20  weighted_rows). 
-00021580: 2020 2072 6574 7572 6e20 636c 6173 735f     return class_
-00021590: 7765 6967 6874 6564 5f72 6f77 730a 0a0a  weighted_rows...
-000215a0: 6465 6620 6f76 6572 7361 6d70 6c65 5f53  def oversample_S
-000215b0: 4d4f 5445 2858 2c79 293a 0a20 2020 2023  MOTE(X,y):.    #
-000215c0: 696e 7075 7420 4461 7461 4672 616d 650a  input DataFrame.
-000215d0: 2020 2020 2358 20e2 8692 496e 6465 7065      #X ...Indepe
-000215e0: 6e64 656e 7420 5661 7269 6162 6c65 2069  ndent Variable i
-000215f0: 6e20 4461 7461 4672 616d 655c 0a20 2020  n DataFrame\.   
-00021600: 2023 7920 e286 9264 6570 656e 6465 6e74   #y ...dependent
-00021610: 2056 6172 6961 626c 6520 696e 2050 616e   Variable in Pan
-00021620: 6461 7320 4461 7461 4672 616d 6520 666f  das DataFrame fo
-00021630: 726d 6174 0a20 2020 2023 2047 6574 2074  rmat.    # Get t
-00021640: 6865 2063 6c61 7373 2064 6973 7472 6975  he class distriu
-00021650: 6274 696f 6e20 666f 7220 7065 7266 6f6d  btion for perfom
-00021660: 696e 6720 7265 6c61 7469 7665 2073 616d  ing relative sam
-00021670: 706c 696e 6720 696e 2074 6865 206e 6578  pling in the nex
-00021680: 7420 6c69 6e65 0a20 2020 2063 6c61 7373  t line.    class
-00021690: 5f77 6569 6768 7465 645f 726f 7773 203d  _weighted_rows =
-000216a0: 2067 6574 5f63 6c61 7373 5f64 6973 7472   get_class_distr
-000216b0: 6962 7574 696f 6e28 7929 0a20 2020 2073  ibution(y).    s
-000216c0: 6d6f 7465 203d 2053 564d 534d 4f54 4528  mote = SVMSMOTE(
-000216d0: 2072 616e 646f 6d5f 7374 6174 653d 3237   random_state=27
-000216e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000216f0: 2020 2020 7361 6d70 6c69 6e67 5f73 7472      sampling_str
-00021700: 6174 6567 793d 636c 6173 735f 7765 6967  ategy=class_weig
-00021710: 6874 6564 5f72 6f77 7329 0a20 2020 2058  hted_rows).    X
-00021720: 2c20 7920 3d20 736d 6f74 652e 6669 745f  , y = smote.fit_
-00021730: 7265 7361 6d70 6c65 2858 2c20 7929 0a20  resample(X, y). 
-00021740: 2020 2072 6574 7572 6e28 582c 7929 0a0a     return(X,y)..
-00021750: 6465 6620 6f76 6572 7361 6d70 6c65 5f41  def oversample_A
-00021760: 4441 5359 4e28 582c 7929 3a0a 2020 2020  DASYN(X,y):.    
-00021770: 2369 6e70 7574 2044 6174 6146 7261 6d65  #input DataFrame
-00021780: 0a20 2020 2023 5820 e286 9249 6e64 6570  .    #X ...Indep
-00021790: 656e 6465 6e74 2056 6172 6961 626c 6520  endent Variable 
-000217a0: 696e 2044 6174 6146 7261 6d65 5c0a 2020  in DataFrame\.  
-000217b0: 2020 2379 20e2 8692 6465 7065 6e64 656e    #y ...dependen
-000217c0: 7420 5661 7269 6162 6c65 2069 6e20 5061  t Variable in Pa
-000217d0: 6e64 6173 2044 6174 6146 7261 6d65 2066  ndas DataFrame f
-000217e0: 6f72 6d61 740a 2020 2020 2320 4765 7420  ormat.    # Get 
-000217f0: 7468 6520 636c 6173 7320 6469 7374 7269  the class distri
-00021800: 7562 7469 6f6e 2066 6f72 2070 6572 666f  ubtion for perfo
-00021810: 6d69 6e67 2072 656c 6174 6976 6520 7361  ming relative sa
-00021820: 6d70 6c69 6e67 2069 6e20 7468 6520 6e65  mpling in the ne
-00021830: 7874 206c 696e 650a 2020 2020 636c 6173  xt line.    clas
-00021840: 735f 7765 6967 6874 6564 5f72 6f77 7320  s_weighted_rows 
-00021850: 3d20 6765 745f 636c 6173 735f 6469 7374  = get_class_dist
-00021860: 7269 6275 7469 6f6e 2879 290a 2020 2020  ribution(y).    
-00021870: 2320 596f 7572 2066 6176 6f75 7269 7465  # Your favourite
-00021880: 206f 7665 7273 616d 706c 6572 0a20 2020   oversampler.   
-00021890: 2073 6d6f 7465 203d 2041 4441 5359 4e28   smote = ADASYN(
-000218a0: 7261 6e64 6f6d 5f73 7461 7465 3d32 372c  random_state=27,
-000218b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000218c0: 2020 2020 7361 6d70 6c69 6e67 5f73 7472      sampling_str
-000218d0: 6174 6567 793d 636c 6173 735f 7765 6967  ategy=class_weig
-000218e0: 6874 6564 5f72 6f77 7329 0a20 2020 2058  hted_rows).    X
-000218f0: 2c20 7920 3d20 736d 6f74 652e 6669 745f  , y = smote.fit_
-00021900: 7265 7361 6d70 6c65 2858 2c20 7929 0a20  resample(X, y). 
-00021910: 2020 2072 6574 7572 6e28 582c 7929 0a23     return(X,y).#
-00021920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021960: 2323 2323 2323 2323 2323 2323 0a69 6d70  ############.imp
-00021970: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00021980: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-00021990: 2070 640a 6672 6f6d 2073 6b6c 6561 726e   pd.from sklearn
-000219a0: 2e6d 6f64 656c 5f73 656c 6563 7469 6f6e  .model_selection
-000219b0: 2069 6d70 6f72 7420 7472 6169 6e5f 7465   import train_te
-000219c0: 7374 5f73 706c 6974 0a64 6566 2073 706c  st_split.def spl
-000219d0: 6974 5f64 6174 615f 6e5f 7761 7973 2864  it_data_n_ways(d
-000219e0: 662c 2074 6172 6765 742c 206e 5f73 706c  f, target, n_spl
-000219f0: 6974 732c 2074 6573 745f 7369 7a65 3d30  its, test_size=0
-00021a00: 2e32 2c20 6d6f 6465 6c74 7970 653d 4e6f  .2, modeltype=No
-00021a10: 6e65 2c2a 2a6b 7761 7267 7329 3a0a 2020  ne,**kwargs):.  
-00021a20: 2020 2222 220a 2020 2020 496e 7075 7473    """.    Inputs
-00021a30: 3a0a 2020 2020 6466 3a20 6461 7461 6672  :.    df: datafr
-00021a40: 616d 6520 7468 6174 2079 6f75 2077 616e  ame that you wan
-00021a50: 7420 746f 2073 706c 6974 0a20 2020 2074  t to split.    t
-00021a60: 6172 6765 743a 2074 6865 2074 6172 6765  arget: the targe
-00021a70: 7420 7661 7269 6162 6c65 2069 6e20 6461  t variable in da
-00021a80: 7461 2066 7261 6d65 2028 6466 290a 2020  ta frame (df).  
-00021a90: 2020 6e5f 7370 6c69 7473 3a20 6e75 6d62    n_splits: numb
-00021aa0: 6572 206f 6620 7761 7973 2069 6e20 7768  er of ways in wh
-00021ab0: 6963 6820 796f 7520 7761 6e74 2074 6f20  ich you want to 
-00021ac0: 7370 6c69 7420 7468 6520 6461 7461 2066  split the data f
-00021ad0: 7261 6d65 2028 6465 6661 756c 743d 3329  rame (default=3)
-00021ae0: 0a20 2020 2074 6573 745f 7369 7a65 3a20  .    test_size: 
-00021af0: 7369 7a65 206f 6620 7468 6520 7465 7374  size of the test
-00021b00: 2064 6174 6173 6574 3a20 6465 6661 756c   dataset: defaul
-00021b10: 7420 6973 2030 2e32 2042 7574 2069 7420  t is 0.2 But it 
-00021b20: 7370 6c69 7473 2074 6869 7320 7465 7374  splits this test
-00021b30: 2069 6e74 6f20 7661 6c69 6420 616e 6420   into valid and 
-00021b40: 7465 7374 2068 616c 662e 0a20 2020 2048  test half..    H
-00021b50: 656e 6365 2079 6f75 2077 696c 6c20 6765  ence you will ge
-00021b60: 7420 3130 2520 6f66 2064 6620 6173 2074  t 10% of df as t
-00021b70: 6573 7420 616e 6420 3130 2520 6f66 2064  est and 10% of d
-00021b80: 6620 6173 2076 616c 6964 2061 6e64 2072  f as valid and r
-00021b90: 656d 6169 6e69 6e67 2038 3025 2061 7320  emaining 80% as 
-00021ba0: 7472 6169 6e0a 2020 2020 2323 2323 2323  train.    ######
-00021bb0: 2323 2323 2323 2323 2323 2020 2068 6f77  ##########   how
-00021bc0: 2069 7420 776f 726b 7320 2323 2323 2323   it works ######
-00021bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00021bf0: 2323 2323 2323 2323 2323 0a20 2020 2059  ##########.    Y
-00021c00: 6f75 2063 616e 2073 706c 6974 2061 2064  ou can split a d
-00021c10: 6174 6166 7261 6d65 2074 6872 6565 2077  ataframe three w
-00021c20: 6179 7320 6f72 2073 6978 2077 6179 7320  ays or six ways 
-00021c30: 6465 7065 6e64 696e 6720 6f6e 2079 6f75  depending on you
-00021c40: 7220 6e65 6564 2e20 5468 7265 6520 7761  r need. Three wa
-00021c50: 7973 2069 733a 0a20 2020 2074 7261 696e  ys is:.    train
-00021c60: 2c20 7661 6c69 642c 2074 6573 740a 2020  , valid, test.  
-00021c70: 2020 5369 7820 7761 7973 2063 616e 2062    Six ways can b
-00021c80: 653a 0a20 2020 2058 5f74 7261 696e 2c79  e:.    X_train,y
-00021c90: 5f74 7261 696e 2c20 585f 7661 6c69 642c  _train, X_valid,
-00021ca0: 2079 5f76 616c 6964 2c20 585f 7465 7374   y_valid, X_test
-00021cb0: 2c20 795f 7465 7374 0a20 2020 2059 6f75  , y_test.    You
-00021cc0: 2077 696c 6c20 6765 7420 6120 6c69 7374   will get a list
-00021cd0: 2063 6f6e 7461 696e 696e 6720 7468 6573   containing thes
-00021ce0: 6520 6461 7461 6672 616d 6573 2e2e 2e64  e dataframes...d
-00021cf0: 6570 656e 6469 6e67 206f 6e20 7768 6174  epending on what
-00021d00: 2079 6f75 2065 6e74 6572 6564 2061 7320   you entered as 
-00021d10: 6e75 6d62 6572 206f 6620 7370 6c69 7473  number of splits
-00021d20: 0a20 2020 204f 7574 7075 743a 204c 6973  .    Output: Lis
-00021d30: 7420 6f66 2064 6174 6166 7261 6d65 730a  t of dataframes.
-00021d40: 2020 2020 2222 220a 2020 2020 6966 206b      """.    if k
-00021d50: 7761 7267 733a 0a20 2020 2020 2020 2066  wargs:.        f
-00021d60: 6f72 206b 6579 2c20 7661 6c20 696e 206b  or key, val in k
-00021d70: 7761 7267 733a 0a20 2020 2020 2020 2020  wargs:.         
-00021d80: 2020 2069 6620 6b65 7920 3d3d 2027 6d6f     if key == 'mo
-00021d90: 6465 6c74 7970 6527 3a0a 2020 2020 2020  deltype':.      
-00021da0: 2020 2020 2020 2020 2020 6b65 7920 3d20            key = 
-00021db0: 7661 6c0a 2020 2020 2020 2020 2020 2020  val.            
-00021dc0: 6966 206b 6579 203d 3d20 2774 6573 745f  if key == 'test_
-00021dd0: 7369 7a65 273a 0a20 2020 2020 2020 2020  size':.         
-00021de0: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
-00021df0: 203d 2076 616c 0a20 2020 2069 6620 6d6f   = val.    if mo
-00021e00: 6465 6c74 7970 6520 6973 204e 6f6e 653a  deltype is None:
-00021e10: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00021e20: 7374 616e 6365 2874 6172 6765 742c 2073  stance(target, s
-00021e30: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00021e40: 2069 6620 6466 5b74 6172 6765 745d 2e64   if df[target].d
-00021e50: 7479 7065 203d 3d20 666c 6f61 743a 0a20  type == float:. 
-00021e60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00021e70: 6f64 656c 7479 7065 203d 2027 5265 6772  odeltype = 'Regr
-00021e80: 6573 7369 6f6e 270a 2020 2020 2020 2020  ession'.        
-00021e90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00021ea0: 2020 2020 2020 2020 2020 6d6f 6465 6c74            modelt
-00021eb0: 7970 6520 3d20 2743 6c61 7373 6966 6963  ype = 'Classific
-00021ec0: 6174 696f 6e27 0a20 2020 2020 2020 2020  ation'.         
-00021ed0: 2020 2074 6172 6765 7420 3d20 5b74 6172     target = [tar
-00021ee0: 6765 745d 0a20 2020 2020 2020 2065 6c73  get].        els
-00021ef0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00021f00: 6620 6466 5b74 6172 6765 745b 305d 5d2e  f df[target[0]].
-00021f10: 6474 7970 6520 3d3d 2066 6c6f 6174 3a0a  dtype == float:.
-00021f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f30: 6d6f 6465 6c74 7970 6520 3d20 2752 6567  modeltype = 'Reg
-00021f40: 7265 7373 696f 6e27 0a20 2020 2020 2020  ression'.       
-00021f50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00021f60: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00021f70: 6c74 7970 6520 3d20 2743 6c61 7373 6966  ltype = 'Classif
-00021f80: 6963 6174 696f 6e27 0a20 2020 2070 7265  ication'.    pre
-00021f90: 6473 203d 205b 7820 666f 7220 7820 696e  ds = [x for x in
-00021fa0: 206c 6973 7428 6466 2920 6966 2078 206e   list(df) if x n
-00021fb0: 6f74 2069 6e20 7461 7267 6574 5d0a 2020  ot in target].  
-00021fc0: 2020 7072 696e 7428 274e 756d 6265 7220    print('Number 
-00021fd0: 6f66 2070 7265 6469 6374 6f72 7320 696e  of predictors in
-00021fe0: 2064 6174 6173 6574 3a20 2564 2720 256c   dataset: %d' %l
-00021ff0: 656e 2870 7265 6473 2929 0a20 2020 206c  en(preds)).    l
-00022000: 6973 745f 6f66 5f64 6673 203d 205b 5d0a  ist_of_dfs = [].
-00022010: 2020 2020 6966 206d 6f64 656c 7479 7065      if modeltype
-00022020: 203d 3d20 2752 6567 7265 7373 696f 6e27   == 'Regression'
-00022030: 3a0a 2020 2020 2020 2020 6e75 6d73 203d  :.        nums =
-00022040: 2069 6e74 2828 312d 7465 7374 5f73 697a   int((1-test_siz
-00022050: 6529 2a64 662e 7368 6170 655b 305d 290a  e)*df.shape[0]).
-00022060: 2020 2020 2020 2020 7472 6169 6e2c 2074          train, t
-00022070: 6573 746c 6172 6765 203d 2064 665b 3a6e  estlarge = df[:n
-00022080: 756d 735d 2c20 6466 5b6e 756d 733a 5d0a  ums], df[nums:].
-00022090: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000220a0: 2020 7472 6169 6e2c 2074 6573 746c 6172    train, testlar
-000220b0: 6765 203d 2074 7261 696e 5f74 6573 745f  ge = train_test_
-000220c0: 7370 6c69 7428 6466 2c20 7465 7374 5f73  split(df, test_s
-000220d0: 697a 653d 7465 7374 5f73 697a 652c 2072  ize=test_size, r
-000220e0: 616e 646f 6d5f 7374 6174 653d 3432 290a  andom_state=42).
-000220f0: 2020 2020 6c69 7374 5f6f 665f 6466 732e      list_of_dfs.
-00022100: 6170 7065 6e64 2874 7261 696e 290a 2020  append(train).  
-00022110: 2020 6966 206e 5f73 706c 6974 7320 3d3d    if n_splits ==
-00022120: 2032 3a0a 2020 2020 2020 2020 7072 696e   2:.        prin
-00022130: 7428 2752 6574 7572 6e69 6e67 2061 2054  t('Returning a T
-00022140: 7570 6c65 2077 6974 6820 7477 6f20 6461  uple with two da
-00022150: 7461 6672 616d 6573 2061 6e64 2073 6861  taframes and sha
-00022160: 7065 733a 2028 2573 2c25 7329 2720 2528  pes: (%s,%s)' %(
-00022170: 7472 6169 6e2e 7368 6170 652c 2074 6573  train.shape, tes
-00022180: 746c 6172 6765 2e73 6861 7065 2929 0a20  tlarge.shape)). 
-00022190: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-000221a0: 6169 6e2c 2074 6573 746c 6172 6765 0a20  ain, testlarge. 
-000221b0: 2020 2065 6c69 6620 6d6f 6465 6c74 7970     elif modeltyp
-000221c0: 6520 3d3d 2027 5265 6772 6573 7369 6f6e  e == 'Regression
-000221d0: 2720 616e 6420 6e5f 7370 6c69 7473 203d  ' and n_splits =
-000221e0: 3d20 333a 0a20 2020 2020 2020 206e 756d  = 3:.        num
-000221f0: 7332 203d 2069 6e74 2830 2e35 2a28 7465  s2 = int(0.5*(te
-00022200: 7374 6c61 7267 652e 7368 6170 655b 305d  stlarge.shape[0]
-00022210: 2929 0a20 2020 2020 2020 2076 616c 6964  )).        valid
-00022220: 2c20 7465 7374 203d 2074 6573 746c 6172  , test = testlar
-00022230: 6765 5b3a 6e75 6d73 325d 2c20 7465 7374  ge[:nums2], test
-00022240: 6c61 7267 655b 6e75 6d73 323a 5d0a 2020  large[nums2:].  
-00022250: 2020 2020 2020 7072 696e 7428 2752 6574        print('Ret
-00022260: 7572 6e69 6e67 2061 2054 7570 6c65 2077  urning a Tuple w
-00022270: 6974 6820 7468 7265 6520 6461 7461 6672  ith three datafr
-00022280: 616d 6573 2061 6e64 2073 6861 7065 733a  ames and shapes:
-00022290: 2028 2573 2c25 732c 2573 2927 2025 2874   (%s,%s,%s)' %(t
-000222a0: 7261 696e 2e73 6861 7065 2c20 7661 6c69  rain.shape, vali
-000222b0: 642e 7368 6170 652c 2074 6573 742e 7368  d.shape, test.sh
-000222c0: 6170 6529 290a 2020 2020 2020 2020 7265  ape)).        re
-000222d0: 7475 726e 2074 7261 696e 2c20 7661 6c69  turn train, vali
-000222e0: 642c 2074 6573 740a 2020 2020 656c 6966  d, test.    elif
-000222f0: 206d 6f64 656c 7479 7065 203d 3d20 2743   modeltype == 'C
-00022300: 6c61 7373 6966 6963 6174 696f 6e27 2061  lassification' a
-00022310: 6e64 206e 5f73 706c 6974 7320 3d3d 2033  nd n_splits == 3
-00022320: 3a0a 2020 2020 2020 2020 7661 6c69 642c  :.        valid,
-00022330: 2074 6573 7420 3d20 7472 6169 6e5f 7465   test = train_te
-00022340: 7374 5f73 706c 6974 2874 6573 746c 6172  st_split(testlar
-00022350: 6765 2c20 7465 7374 5f73 697a 653d 302e  ge, test_size=0.
-00022360: 352c 2072 616e 646f 6d5f 7374 6174 653d  5, random_state=
-00022370: 3939 290a 2020 2020 2020 2020 7072 696e  99).        prin
-00022380: 7428 2752 6574 7572 6e69 6e67 2061 2054  t('Returning a T
-00022390: 7570 6c65 2077 6974 6820 7468 7265 6520  uple with three 
-000223a0: 6461 7461 6672 616d 6573 2061 6e64 2073  dataframes and s
-000223b0: 6861 7065 733a 2028 2573 2c25 732c 2573  hapes: (%s,%s,%s
-000223c0: 2927 2025 2874 7261 696e 2e73 6861 7065  )' %(train.shape
-000223d0: 2c20 7661 6c69 642e 7368 6170 652c 2074  , valid.shape, t
-000223e0: 6573 742e 7368 6170 6529 290a 2020 2020  est.shape)).    
-000223f0: 2020 2020 7265 7475 726e 2074 7261 696e      return train
-00022400: 2c20 7661 6c69 642c 2074 6573 740a 2020  , valid, test.  
-00022410: 2020 2323 2323 2043 6f6e 7469 6e75 6520    #### Continue 
-00022420: 6f6e 6c79 2069 6620 796f 7520 6e65 6564  only if you need
-00022430: 206d 6f72 6520 7468 616e 2033 2073 706c   more than 3 spl
-00022440: 6974 7320 2323 2323 2323 0a20 2020 2069  its ######.    i
-00022450: 6620 6d6f 6465 6c74 7970 6520 3d3d 2027  f modeltype == '
-00022460: 5265 6772 6573 7369 6f6e 273a 0a20 2020  Regression':.   
-00022470: 2020 2020 206e 756d 7332 203d 2069 6e74       nums2 = int
-00022480: 2830 2e35 2a28 6466 2e73 6861 7065 5b30  (0.5*(df.shape[0
-00022490: 5d20 2d20 6e75 6d73 2929 0a20 2020 2020  ] - nums)).     
-000224a0: 2020 2076 616c 6964 2c20 7465 7374 203d     valid, test =
-000224b0: 2074 6573 746c 6172 6765 5b3a 6e75 6d73   testlarge[:nums
-000224c0: 325d 2c20 7465 7374 6c61 7267 655b 6e75  2], testlarge[nu
-000224d0: 6d73 323a 5d0a 2020 2020 2020 2020 6966  ms2:].        if
-000224e0: 206e 5f73 706c 6974 7320 3d3d 2034 3a0a   n_splits == 4:.
-000224f0: 2020 2020 2020 2020 2020 2020 585f 7472              X_tr
-00022500: 6169 6e2c 2079 5f74 7261 696e 2c20 585f  ain, y_train, X_
-00022510: 7465 7374 2c20 795f 7465 7374 203d 2074  test, y_test = t
-00022520: 7261 696e 5b70 7265 6473 5d2c 2074 7261  rain[preds], tra
-00022530: 696e 5b74 6172 6765 745d 2c20 7465 7374  in[target], test
-00022540: 6c61 7267 655b 7072 6564 735d 2c20 7465  large[preds], te
-00022550: 7374 6c61 7267 655b 7461 7267 6574 5d0a  stlarge[target].
-00022560: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00022570: 5f6f 665f 6466 7320 3d20 5b58 5f74 7261  _of_dfs = [X_tra
-00022580: 696e 2c79 5f74 7261 696e 2c20 585f 7465  in,y_train, X_te
-00022590: 7374 2c20 795f 7465 7374 5d0a 2020 2020  st, y_test].    
-000225a0: 2020 2020 2020 2020 7072 696e 7428 2752          print('R
-000225b0: 6574 7572 6e69 6e67 2061 2054 7570 6c65  eturning a Tuple
-000225c0: 2077 6974 6820 3420 6461 7461 6672 616d   with 4 datafram
-000225d0: 6573 3a20 2825 7320 2573 2025 7320 2573  es: (%s %s %s %s
-000225e0: 2927 2025 2858 5f74 7261 696e 2e73 6861  )' %(X_train.sha
-000225f0: 7065 2c79 5f74 7261 696e 2e73 6861 7065  pe,y_train.shape
-00022600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00022610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022620: 2020 585f 7465 7374 2e73 6861 7065 2c79    X_test.shape,y
-00022630: 5f74 6573 742e 7368 6170 6529 290a 2020  _test.shape)).  
-00022640: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00022650: 206c 6973 745f 6f66 5f64 6673 0a20 2020   list_of_dfs.   
-00022660: 2020 2020 2065 6c69 6620 6e5f 7370 6c69       elif n_spli
-00022670: 7473 203d 3d20 363a 0a20 2020 2020 2020  ts == 6:.       
-00022680: 2020 2020 2058 5f74 7261 696e 2c20 795f       X_train, y_
-00022690: 7472 6169 6e2c 2058 5f76 616c 6964 2c20  train, X_valid, 
-000226a0: 795f 7661 6c69 642c 2058 5f74 6573 742c  y_valid, X_test,
-000226b0: 2079 5f74 6573 7420 3d20 7472 6169 6e5b   y_test = train[
-000226c0: 7072 6564 735d 2c20 7472 6169 6e5b 7461  preds], train[ta
-000226d0: 7267 6574 5d2c 2076 616c 6964 5b0a 2020  rget], valid[.  
-000226e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000226f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022700: 2020 7072 6564 735d 2c20 7661 6c69 645b    preds], valid[
-00022710: 7461 7267 6574 5d2c 2074 6573 745b 7072  target], test[pr
-00022720: 6564 735d 2c20 7465 7374 5b74 6172 6765  eds], test[targe
-00022730: 745d 0a20 2020 2020 2020 2020 2020 206c  t].            l
-00022740: 6973 745f 6f66 5f64 6673 203d 205b 585f  ist_of_dfs = [X_
-00022750: 7472 6169 6e2c 795f 7472 6169 6e2c 2058  train,y_train, X
-00022760: 5f76 616c 6964 2c20 795f 7661 6c69 642c  _valid, y_valid,
-00022770: 2058 5f74 6573 742c 2079 5f74 6573 745d   X_test, y_test]
-00022780: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00022790: 6e74 2827 5265 7475 726e 696e 6720 6120  nt('Returning a 
-000227a0: 5475 706c 6520 7769 7468 2073 6978 2064  Tuple with six d
-000227b0: 6174 6166 7261 6d65 7320 616e 6420 7368  ataframes and sh
-000227c0: 6170 6573 3a20 2825 7320 2573 2025 7320  apes: (%s %s %s 
-000227d0: 2573 2c25 732c 2573 2927 2025 280a 2020  %s,%s,%s)' %(.  
-000227e0: 2020 2020 2020 2020 2020 2020 2020 585f                X_
-000227f0: 7472 6169 6e2e 7368 6170 652c 795f 7472  train.shape,y_tr
-00022800: 6169 6e2e 7368 6170 652c 2058 5f76 616c  ain.shape, X_val
-00022810: 6964 2e73 6861 7065 2c79 5f76 616c 6964  id.shape,y_valid
-00022820: 2e73 6861 7065 2c58 5f74 6573 742e 7368  .shape,X_test.sh
-00022830: 6170 652c 795f 7465 7374 2e73 6861 7065  ape,y_test.shape
-00022840: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-00022850: 6574 7572 6e20 6c69 7374 5f6f 665f 6466  eturn list_of_df
-00022860: 730a 2020 2020 2020 2020 656c 7365 3a0a  s.        else:.
-00022870: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00022880: 7428 274e 756d 6265 7220 6f66 2073 706c  t('Number of spl
-00022890: 6974 7320 6d75 7374 2062 6520 322c 2033  its must be 2, 3
-000228a0: 2c20 3420 6f72 2036 2729 0a20 2020 2020  , 4 or 6').     
-000228b0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-000228c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000228d0: 6966 206e 5f73 706c 6974 7320 3d3d 2034  if n_splits == 4
-000228e0: 3a0a 2020 2020 2020 2020 2020 2020 585f  :.            X_
-000228f0: 7472 6169 6e2c 2079 5f74 7261 696e 2c20  train, y_train, 
-00022900: 585f 7465 7374 2c20 795f 7465 7374 203d  X_test, y_test =
-00022910: 2074 7261 696e 5b70 7265 6473 5d2c 2074   train[preds], t
-00022920: 7261 696e 5b74 6172 6765 745d 2c20 7465  rain[target], te
-00022930: 7374 6c61 7267 655b 7072 6564 735d 2c20  stlarge[preds], 
-00022940: 7465 7374 6c61 7267 655b 7461 7267 6574  testlarge[target
-00022950: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
-00022960: 7374 5f6f 665f 6466 7320 3d20 5b58 5f74  st_of_dfs = [X_t
-00022970: 7261 696e 2c79 5f74 7261 696e 2c20 585f  rain,y_train, X_
-00022980: 7465 7374 2c20 795f 7465 7374 5d0a 2020  test, y_test].  
-00022990: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000229a0: 2752 6574 7572 6e69 6e67 2061 2054 7570  'Returning a Tup
-000229b0: 6c65 2077 6974 6820 3420 6461 7461 6672  le with 4 datafr
-000229c0: 616d 6573 3a20 2825 7320 2573 2025 7320  ames: (%s %s %s 
-000229d0: 2573 2927 2025 2858 5f74 7261 696e 2e73  %s)' %(X_train.s
-000229e0: 6861 7065 2c79 5f74 7261 696e 2e73 6861  hape,y_train.sha
-000229f0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00022a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a10: 2020 2020 585f 7465 7374 2e73 6861 7065      X_test.shape
-00022a20: 2c79 5f74 6573 742e 7368 6170 6529 290a  ,y_test.shape)).
-00022a30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00022a40: 726e 206c 6973 745f 6f66 5f64 6673 0a20  rn list_of_dfs. 
-00022a50: 2020 2020 2020 2065 6c69 6620 6e5f 7370         elif n_sp
-00022a60: 6c69 7473 203d 3d20 363a 0a20 2020 2020  lits == 6:.     
-00022a70: 2020 2020 2020 2058 5f74 7261 696e 2c20         X_train, 
-00022a80: 795f 7472 6169 6e2c 2058 5f76 616c 6964  y_train, X_valid
-00022a90: 2c20 795f 7661 6c69 642c 2058 5f74 6573  , y_valid, X_tes
-00022aa0: 742c 2079 5f74 6573 7420 3d20 7472 6169  t, y_test = trai
-00022ab0: 6e5b 7072 6564 735d 2c20 7472 6169 6e5b  n[preds], train[
-00022ac0: 7461 7267 6574 5d2c 2076 616c 6964 5b0a  target], valid[.
-00022ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022af0: 2020 2020 7072 6564 735d 2c20 7661 6c69      preds], vali
-00022b00: 645b 7461 7267 6574 5d2c 2074 6573 745b  d[target], test[
-00022b10: 7072 6564 735d 2c20 7465 7374 5b74 6172  preds], test[tar
-00022b20: 6765 745d 0a20 2020 2020 2020 2020 2020  get].           
-00022b30: 2070 7269 6e74 2827 5265 7475 726e 696e   print('Returnin
-00022b40: 6720 3420 6461 7461 6672 616d 6573 3a27  g 4 dataframes:'
-00022b50: 2c20 585f 7472 6169 6e2e 7368 6170 652c  , X_train.shape,
-00022b60: 2079 5f74 7261 696e 2e73 6861 7065 2c20   y_train.shape, 
-00022b70: 585f 7465 7374 2e73 6861 7065 2c20 795f  X_test.shape, y_
-00022b80: 7465 7374 2e73 6861 7065 290a 2020 2020  test.shape).    
-00022b90: 2020 2020 2020 2020 6c69 7374 5f6f 665f          list_of_
-00022ba0: 6466 7320 3d20 5b58 5f74 7261 696e 2c79  dfs = [X_train,y
-00022bb0: 5f74 7261 696e 2c20 585f 7661 6c69 642c  _train, X_valid,
-00022bc0: 2079 5f76 616c 6964 2c20 585f 7465 7374   y_valid, X_test
-00022bd0: 2c20 795f 7465 7374 5d0a 2020 2020 2020  , y_test].      
-00022be0: 2020 2020 2020 7072 696e 7428 2752 6574        print('Ret
-00022bf0: 7572 6e69 6e67 2061 2054 7570 6c65 2077  urning a Tuple w
-00022c00: 6974 6820 7369 7820 6461 7461 6672 616d  ith six datafram
-00022c10: 6573 2061 6e64 2073 6861 7065 733a 2028  es and shapes: (
-00022c20: 2573 2025 7320 2573 2025 732c 2573 2c25  %s %s %s %s,%s,%
-00022c30: 7329 2720 2528 0a20 2020 2020 2020 2020  s)' %(.         
-00022c40: 2020 2020 2020 2058 5f74 7261 696e 2e73         X_train.s
-00022c50: 6861 7065 2c79 5f74 7261 696e 2e73 6861  hape,y_train.sha
-00022c60: 7065 2c20 585f 7661 6c69 642e 7368 6170  pe, X_valid.shap
-00022c70: 652c 795f 7661 6c69 642e 7368 6170 652c  e,y_valid.shape,
-00022c80: 585f 7465 7374 2e73 6861 7065 2c79 5f74  X_test.shape,y_t
-00022c90: 6573 742e 7368 6170 6529 290a 2020 2020  est.shape)).    
-00022ca0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00022cb0: 6973 745f 6f66 5f64 6673 0a20 2020 2020  ist_of_dfs.     
-00022cc0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00022cd0: 2020 2020 2070 7269 6e74 2827 4e75 6d62       print('Numb
-00022ce0: 6572 206f 6620 7370 6c69 7473 206d 7573  er of splits mus
-00022cf0: 7420 6265 2032 2c20 332c 2034 206f 7220  t be 2, 3, 4 or 
-00022d00: 3627 290a 2020 2020 2020 2020 2020 2020  6').            
-00022d10: 7265 7475 726e 0a23 2323 2323 2323 2323  return.#########
-00022d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022d40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021260: 2323 2323 2323 2323 2323 2323 0a23 2043  ############.# C
+00021270: 616c 6375 6c61 7465 2063 6c61 7373 2077  alculate class w
+00021280: 6569 6768 740a 696d 706f 7274 2063 6f70  eight.import cop
+00021290: 790a 6672 6f6d 2063 6f6c 6c65 6374 696f  y.from collectio
+000212a0: 6e73 2069 6d70 6f72 7420 436f 756e 7465  ns import Counte
+000212b0: 720a 6672 6f6d 2073 6b6c 6561 726e 2e75  r.from sklearn.u
+000212c0: 7469 6c73 2e63 6c61 7373 5f77 6569 6768  tils.class_weigh
+000212d0: 7420 696d 706f 7274 2063 6f6d 7075 7465  t import compute
+000212e0: 5f63 6c61 7373 5f77 6569 6768 740a 6465  _class_weight.de
+000212f0: 6620 6765 745f 636c 6173 735f 6469 7374  f get_class_dist
+00021300: 7269 6275 7469 6f6e 2879 5f69 6e70 7574  ribution(y_input
+00021310: 2c20 7665 7262 6f73 653d 3029 3a0a 2020  , verbose=0):.  
+00021320: 2020 795f 696e 7075 7420 3d20 636f 7079    y_input = copy
+00021330: 2e64 6565 7063 6f70 7928 795f 696e 7075  .deepcopy(y_inpu
+00021340: 7429 0a20 2020 2063 6c61 7373 6573 203d  t).    classes =
+00021350: 206e 702e 756e 6971 7565 2879 5f69 6e70   np.unique(y_inp
+00021360: 7574 290a 2020 2020 7870 203d 2043 6f75  ut).    xp = Cou
+00021370: 6e74 6572 2879 5f69 6e70 7574 290a 2020  nter(y_input).  
+00021380: 2020 636c 6173 735f 7765 6967 6874 7320    class_weights 
+00021390: 3d20 636f 6d70 7574 655f 636c 6173 735f  = compute_class_
+000213a0: 7765 6967 6874 2827 6261 6c61 6e63 6564  weight('balanced
+000213b0: 272c 2063 6c61 7373 6573 3d6e 702e 756e  ', classes=np.un
+000213c0: 6971 7565 2879 5f69 6e70 7574 292c 2079  ique(y_input), y
+000213d0: 3d79 5f69 6e70 7574 290a 2020 2020 6966  =y_input).    if
+000213e0: 206c 656e 2863 6c61 7373 5f77 6569 6768   len(class_weigh
+000213f0: 7473 5b28 636c 6173 735f 7765 6967 6874  ts[(class_weight
+00021400: 733e 2031 3029 5d29 203e 2030 3a0a 2020  s> 10)]) > 0:.  
+00021410: 2020 2020 2020 636c 6173 735f 7765 6967        class_weig
+00021420: 6874 7320 3d20 2863 6c61 7373 5f77 6569  hts = (class_wei
+00021430: 6768 7473 2f31 3029 0a20 2020 2065 6c73  ghts/10).    els
+00021440: 653a 0a20 2020 2020 2020 2063 6c61 7373  e:.        class
+00021450: 5f77 6569 6768 7473 203d 2028 636c 6173  _weights = (clas
+00021460: 735f 7765 6967 6874 7329 0a20 2020 2023  s_weights).    #
+00021470: 7072 696e 7428 2720 2020 2063 6c61 7373  print('    class
+00021480: 5f77 6569 6768 7473 203d 2025 7327 2025  _weights = %s' %
+00021490: 636c 6173 735f 7765 6967 6874 7329 0a20  class_weights). 
+000214a0: 2020 2063 6c61 7373 5f77 6569 6768 7473     class_weights
+000214b0: 5b28 636c 6173 735f 7765 6967 6874 733c  [(class_weights<
+000214c0: 3129 5d3d 310a 2020 2020 636c 6173 735f  1)]=1.    class_
+000214d0: 726f 7773 203d 2063 6c61 7373 5f77 6569  rows = class_wei
+000214e0: 6768 7473 2a5b 7870 5b78 5d20 666f 7220  ghts*[xp[x] for 
+000214f0: 7820 696e 2063 6c61 7373 6573 5d0a 2020  x in classes].  
+00021500: 2020 636c 6173 735f 726f 7773 203d 2063    class_rows = c
+00021510: 6c61 7373 5f72 6f77 732e 6173 7479 7065  lass_rows.astype
+00021520: 2869 6e74 290a 2020 2020 636c 6173 735f  (int).    class_
+00021530: 7765 6967 6874 6564 5f72 6f77 7320 3d20  weighted_rows = 
+00021540: 6469 6374 287a 6970 2863 6c61 7373 6573  dict(zip(classes
+00021550: 2c63 6c61 7373 5f72 6f77 7329 290a 2020  ,class_rows)).  
+00021560: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+00021570: 2020 2020 2020 7072 696e 7428 2720 2020        print('   
+00021580: 2063 6c61 7373 5f77 6569 6768 7465 645f   class_weighted_
+00021590: 726f 7773 203d 2025 7327 2025 636c 6173  rows = %s' %clas
+000215a0: 735f 7765 6967 6874 6564 5f72 6f77 7329  s_weighted_rows)
+000215b0: 0a20 2020 2072 6574 7572 6e20 636c 6173  .    return clas
+000215c0: 735f 7765 6967 6874 6564 5f72 6f77 730a  s_weighted_rows.
+000215d0: 0a0a 6465 6620 6f76 6572 7361 6d70 6c65  ..def oversample
+000215e0: 5f53 4d4f 5445 2858 2c79 293a 0a20 2020  _SMOTE(X,y):.   
+000215f0: 2023 696e 7075 7420 4461 7461 4672 616d   #input DataFram
+00021600: 650a 2020 2020 2358 20e2 8692 496e 6465  e.    #X ...Inde
+00021610: 7065 6e64 656e 7420 5661 7269 6162 6c65  pendent Variable
+00021620: 2069 6e20 4461 7461 4672 616d 655c 0a20   in DataFrame\. 
+00021630: 2020 2023 7920 e286 9264 6570 656e 6465     #y ...depende
+00021640: 6e74 2056 6172 6961 626c 6520 696e 2050  nt Variable in P
+00021650: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
+00021660: 666f 726d 6174 0a20 2020 2023 2047 6574  format.    # Get
+00021670: 2074 6865 2063 6c61 7373 2064 6973 7472   the class distr
+00021680: 6975 6274 696f 6e20 666f 7220 7065 7266  iubtion for perf
+00021690: 6f6d 696e 6720 7265 6c61 7469 7665 2073  oming relative s
+000216a0: 616d 706c 696e 6720 696e 2074 6865 206e  ampling in the n
+000216b0: 6578 7420 6c69 6e65 0a20 2020 2063 6c61  ext line.    cla
+000216c0: 7373 5f77 6569 6768 7465 645f 726f 7773  ss_weighted_rows
+000216d0: 203d 2067 6574 5f63 6c61 7373 5f64 6973   = get_class_dis
+000216e0: 7472 6962 7574 696f 6e28 7929 0a20 2020  tribution(y).   
+000216f0: 2073 6d6f 7465 203d 2053 564d 534d 4f54   smote = SVMSMOT
+00021700: 4528 2072 616e 646f 6d5f 7374 6174 653d  E( random_state=
+00021710: 3237 2c0a 2020 2020 2020 2020 2020 2020  27,.            
+00021720: 2020 2020 2020 7361 6d70 6c69 6e67 5f73        sampling_s
+00021730: 7472 6174 6567 793d 636c 6173 735f 7765  trategy=class_we
+00021740: 6967 6874 6564 5f72 6f77 7329 0a20 2020  ighted_rows).   
+00021750: 2058 2c20 7920 3d20 736d 6f74 652e 6669   X, y = smote.fi
+00021760: 745f 7265 7361 6d70 6c65 2858 2c20 7929  t_resample(X, y)
+00021770: 0a20 2020 2072 6574 7572 6e28 582c 7929  .    return(X,y)
+00021780: 0a0a 6465 6620 6f76 6572 7361 6d70 6c65  ..def oversample
+00021790: 5f41 4441 5359 4e28 582c 7929 3a0a 2020  _ADASYN(X,y):.  
+000217a0: 2020 2369 6e70 7574 2044 6174 6146 7261    #input DataFra
+000217b0: 6d65 0a20 2020 2023 5820 e286 9249 6e64  me.    #X ...Ind
+000217c0: 6570 656e 6465 6e74 2056 6172 6961 626c  ependent Variabl
+000217d0: 6520 696e 2044 6174 6146 7261 6d65 5c0a  e in DataFrame\.
+000217e0: 2020 2020 2379 20e2 8692 6465 7065 6e64      #y ...depend
+000217f0: 656e 7420 5661 7269 6162 6c65 2069 6e20  ent Variable in 
+00021800: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
+00021810: 2066 6f72 6d61 740a 2020 2020 2320 4765   format.    # Ge
+00021820: 7420 7468 6520 636c 6173 7320 6469 7374  t the class dist
+00021830: 7269 7562 7469 6f6e 2066 6f72 2070 6572  riubtion for per
+00021840: 666f 6d69 6e67 2072 656c 6174 6976 6520  foming relative 
+00021850: 7361 6d70 6c69 6e67 2069 6e20 7468 6520  sampling in the 
+00021860: 6e65 7874 206c 696e 650a 2020 2020 636c  next line.    cl
+00021870: 6173 735f 7765 6967 6874 6564 5f72 6f77  ass_weighted_row
+00021880: 7320 3d20 6765 745f 636c 6173 735f 6469  s = get_class_di
+00021890: 7374 7269 6275 7469 6f6e 2879 290a 2020  stribution(y).  
+000218a0: 2020 2320 596f 7572 2066 6176 6f75 7269    # Your favouri
+000218b0: 7465 206f 7665 7273 616d 706c 6572 0a20  te oversampler. 
+000218c0: 2020 2073 6d6f 7465 203d 2041 4441 5359     smote = ADASY
+000218d0: 4e28 7261 6e64 6f6d 5f73 7461 7465 3d32  N(random_state=2
+000218e0: 372c 0a20 2020 2020 2020 2020 2020 2020  7,.             
+000218f0: 2020 2020 2020 7361 6d70 6c69 6e67 5f73        sampling_s
+00021900: 7472 6174 6567 793d 636c 6173 735f 7765  trategy=class_we
+00021910: 6967 6874 6564 5f72 6f77 7329 0a20 2020  ighted_rows).   
+00021920: 2058 2c20 7920 3d20 736d 6f74 652e 6669   X, y = smote.fi
+00021930: 745f 7265 7361 6d70 6c65 2858 2c20 7929  t_resample(X, y)
+00021940: 0a20 2020 2072 6574 7572 6e28 582c 7929  .    return(X,y)
+00021950: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00021960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021990: 2323 2323 2323 2323 2323 2323 2323 0a69  ##############.i
+000219a0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+000219b0: 700a 696d 706f 7274 2070 616e 6461 7320  p.import pandas 
+000219c0: 6173 2070 640a 6672 6f6d 2073 6b6c 6561  as pd.from sklea
+000219d0: 726e 2e6d 6f64 656c 5f73 656c 6563 7469  rn.model_selecti
+000219e0: 6f6e 2069 6d70 6f72 7420 7472 6169 6e5f  on import train_
+000219f0: 7465 7374 5f73 706c 6974 0a64 6566 2073  test_split.def s
+00021a00: 706c 6974 5f64 6174 615f 6e5f 7761 7973  plit_data_n_ways
+00021a10: 2864 662c 2074 6172 6765 742c 206e 5f73  (df, target, n_s
+00021a20: 706c 6974 732c 2074 6573 745f 7369 7a65  plits, test_size
+00021a30: 3d30 2e32 2c20 6d6f 6465 6c74 7970 653d  =0.2, modeltype=
+00021a40: 4e6f 6e65 2c2a 2a6b 7761 7267 7329 3a0a  None,**kwargs):.
+00021a50: 2020 2020 2222 220a 2020 2020 496e 7075      """.    Inpu
+00021a60: 7473 3a0a 2020 2020 6466 3a20 6461 7461  ts:.    df: data
+00021a70: 6672 616d 6520 7468 6174 2079 6f75 2077  frame that you w
+00021a80: 616e 7420 746f 2073 706c 6974 0a20 2020  ant to split.   
+00021a90: 2074 6172 6765 743a 2074 6865 2074 6172   target: the tar
+00021aa0: 6765 7420 7661 7269 6162 6c65 2069 6e20  get variable in 
+00021ab0: 6461 7461 2066 7261 6d65 2028 6466 290a  data frame (df).
+00021ac0: 2020 2020 6e5f 7370 6c69 7473 3a20 6e75      n_splits: nu
+00021ad0: 6d62 6572 206f 6620 7761 7973 2069 6e20  mber of ways in 
+00021ae0: 7768 6963 6820 796f 7520 7761 6e74 2074  which you want t
+00021af0: 6f20 7370 6c69 7420 7468 6520 6461 7461  o split the data
+00021b00: 2066 7261 6d65 2028 6465 6661 756c 743d   frame (default=
+00021b10: 3329 0a20 2020 2074 6573 745f 7369 7a65  3).    test_size
+00021b20: 3a20 7369 7a65 206f 6620 7468 6520 7465  : size of the te
+00021b30: 7374 2064 6174 6173 6574 3a20 6465 6661  st dataset: defa
+00021b40: 756c 7420 6973 2030 2e32 2042 7574 2069  ult is 0.2 But i
+00021b50: 7420 7370 6c69 7473 2074 6869 7320 7465  t splits this te
+00021b60: 7374 2069 6e74 6f20 7661 6c69 6420 616e  st into valid an
+00021b70: 6420 7465 7374 2068 616c 662e 0a20 2020  d test half..   
+00021b80: 2048 656e 6365 2079 6f75 2077 696c 6c20   Hence you will 
+00021b90: 6765 7420 3130 2520 6f66 2064 6620 6173  get 10% of df as
+00021ba0: 2074 6573 7420 616e 6420 3130 2520 6f66   test and 10% of
+00021bb0: 2064 6620 6173 2076 616c 6964 2061 6e64   df as valid and
+00021bc0: 2072 656d 6169 6e69 6e67 2038 3025 2061   remaining 80% a
+00021bd0: 7320 7472 6169 6e0a 2020 2020 2323 2323  s train.    ####
+00021be0: 2323 2323 2323 2323 2323 2323 2020 2068  ############   h
+00021bf0: 6f77 2069 7420 776f 726b 7320 2323 2323  ow it works ####
+00021c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021c10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00021c20: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+00021c30: 2059 6f75 2063 616e 2073 706c 6974 2061   You can split a
+00021c40: 2064 6174 6166 7261 6d65 2074 6872 6565   dataframe three
+00021c50: 2077 6179 7320 6f72 2073 6978 2077 6179   ways or six way
+00021c60: 7320 6465 7065 6e64 696e 6720 6f6e 2079  s depending on y
+00021c70: 6f75 7220 6e65 6564 2e20 5468 7265 6520  our need. Three 
+00021c80: 7761 7973 2069 733a 0a20 2020 2074 7261  ways is:.    tra
+00021c90: 696e 2c20 7661 6c69 642c 2074 6573 740a  in, valid, test.
+00021ca0: 2020 2020 5369 7820 7761 7973 2063 616e      Six ways can
+00021cb0: 2062 653a 0a20 2020 2058 5f74 7261 696e   be:.    X_train
+00021cc0: 2c79 5f74 7261 696e 2c20 585f 7661 6c69  ,y_train, X_vali
+00021cd0: 642c 2079 5f76 616c 6964 2c20 585f 7465  d, y_valid, X_te
+00021ce0: 7374 2c20 795f 7465 7374 0a20 2020 2059  st, y_test.    Y
+00021cf0: 6f75 2077 696c 6c20 6765 7420 6120 6c69  ou will get a li
+00021d00: 7374 2063 6f6e 7461 696e 696e 6720 7468  st containing th
+00021d10: 6573 6520 6461 7461 6672 616d 6573 2e2e  ese dataframes..
+00021d20: 2e64 6570 656e 6469 6e67 206f 6e20 7768  .depending on wh
+00021d30: 6174 2079 6f75 2065 6e74 6572 6564 2061  at you entered a
+00021d40: 7320 6e75 6d62 6572 206f 6620 7370 6c69  s number of spli
+00021d50: 7473 0a20 2020 204f 7574 7075 743a 204c  ts.    Output: L
+00021d60: 6973 7420 6f66 2064 6174 6166 7261 6d65  ist of dataframe
+00021d70: 730a 2020 2020 2222 220a 2020 2020 6966  s.    """.    if
+00021d80: 206b 7761 7267 733a 0a20 2020 2020 2020   kwargs:.       
+00021d90: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
+00021da0: 206b 7761 7267 733a 0a20 2020 2020 2020   kwargs:.       
+00021db0: 2020 2020 2069 6620 6b65 7920 3d3d 2027       if key == '
+00021dc0: 6d6f 6465 6c74 7970 6527 3a0a 2020 2020  modeltype':.    
+00021dd0: 2020 2020 2020 2020 2020 2020 6b65 7920              key 
+00021de0: 3d20 7661 6c0a 2020 2020 2020 2020 2020  = val.          
+00021df0: 2020 6966 206b 6579 203d 3d20 2774 6573    if key == 'tes
+00021e00: 745f 7369 7a65 273a 0a20 2020 2020 2020  t_size':.       
+00021e10: 2020 2020 2020 2020 2074 6573 745f 7369           test_si
+00021e20: 7a65 203d 2076 616c 0a20 2020 2069 6620  ze = val.    if 
+00021e30: 6d6f 6465 6c74 7970 6520 6973 204e 6f6e  modeltype is Non
+00021e40: 653a 0a20 2020 2020 2020 2069 6620 6973  e:.        if is
+00021e50: 696e 7374 616e 6365 2874 6172 6765 742c  instance(target,
+00021e60: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+00021e70: 2020 2069 6620 6466 5b74 6172 6765 745d     if df[target]
+00021e80: 2e64 7479 7065 203d 3d20 666c 6f61 743a  .dtype == float:
+00021e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021ea0: 206d 6f64 656c 7479 7065 203d 2027 5265   modeltype = 'Re
+00021eb0: 6772 6573 7369 6f6e 270a 2020 2020 2020  gression'.      
+00021ec0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00021ed0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00021ee0: 6c74 7970 6520 3d20 2743 6c61 7373 6966  ltype = 'Classif
+00021ef0: 6963 6174 696f 6e27 0a20 2020 2020 2020  ication'.       
+00021f00: 2020 2020 2074 6172 6765 7420 3d20 5b74       target = [t
+00021f10: 6172 6765 745d 0a20 2020 2020 2020 2065  arget].        e
+00021f20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00021f30: 2069 6620 6466 5b74 6172 6765 745b 305d   if df[target[0]
+00021f40: 5d2e 6474 7970 6520 3d3d 2066 6c6f 6174  ].dtype == float
+00021f50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021f60: 2020 6d6f 6465 6c74 7970 6520 3d20 2752    modeltype = 'R
+00021f70: 6567 7265 7373 696f 6e27 0a20 2020 2020  egression'.     
+00021f80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00021f90: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00021fa0: 6465 6c74 7970 6520 3d20 2743 6c61 7373  deltype = 'Class
+00021fb0: 6966 6963 6174 696f 6e27 0a20 2020 2070  ification'.    p
+00021fc0: 7265 6473 203d 205b 7820 666f 7220 7820  reds = [x for x 
+00021fd0: 696e 206c 6973 7428 6466 2920 6966 2078  in list(df) if x
+00021fe0: 206e 6f74 2069 6e20 7461 7267 6574 5d0a   not in target].
+00021ff0: 2020 2020 7072 696e 7428 274e 756d 6265      print('Numbe
+00022000: 7220 6f66 2070 7265 6469 6374 6f72 7320  r of predictors 
+00022010: 696e 2064 6174 6173 6574 3a20 2564 2720  in dataset: %d' 
+00022020: 256c 656e 2870 7265 6473 2929 0a20 2020  %len(preds)).   
+00022030: 206c 6973 745f 6f66 5f64 6673 203d 205b   list_of_dfs = [
+00022040: 5d0a 2020 2020 6966 206d 6f64 656c 7479  ].    if modelty
+00022050: 7065 203d 3d20 2752 6567 7265 7373 696f  pe == 'Regressio
+00022060: 6e27 3a0a 2020 2020 2020 2020 6e75 6d73  n':.        nums
+00022070: 203d 2069 6e74 2828 312d 7465 7374 5f73   = int((1-test_s
+00022080: 697a 6529 2a64 662e 7368 6170 655b 305d  ize)*df.shape[0]
+00022090: 290a 2020 2020 2020 2020 7472 6169 6e2c  ).        train,
+000220a0: 2074 6573 746c 6172 6765 203d 2064 665b   testlarge = df[
+000220b0: 3a6e 756d 735d 2c20 6466 5b6e 756d 733a  :nums], df[nums:
+000220c0: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
+000220d0: 2020 2020 7472 6169 6e2c 2074 6573 746c      train, testl
+000220e0: 6172 6765 203d 2074 7261 696e 5f74 6573  arge = train_tes
+000220f0: 745f 7370 6c69 7428 6466 2c20 7465 7374  t_split(df, test
+00022100: 5f73 697a 653d 7465 7374 5f73 697a 652c  _size=test_size,
+00022110: 2072 616e 646f 6d5f 7374 6174 653d 3432   random_state=42
+00022120: 290a 2020 2020 6c69 7374 5f6f 665f 6466  ).    list_of_df
+00022130: 732e 6170 7065 6e64 2874 7261 696e 290a  s.append(train).
+00022140: 2020 2020 6966 206e 5f73 706c 6974 7320      if n_splits 
+00022150: 3d3d 2032 3a0a 2020 2020 2020 2020 7072  == 2:.        pr
+00022160: 696e 7428 2752 6574 7572 6e69 6e67 2061  int('Returning a
+00022170: 2054 7570 6c65 2077 6974 6820 7477 6f20   Tuple with two 
+00022180: 6461 7461 6672 616d 6573 2061 6e64 2073  dataframes and s
+00022190: 6861 7065 733a 2028 2573 2c25 7329 2720  hapes: (%s,%s)' 
+000221a0: 2528 7472 6169 6e2e 7368 6170 652c 2074  %(train.shape, t
+000221b0: 6573 746c 6172 6765 2e73 6861 7065 2929  estlarge.shape))
+000221c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000221d0: 7472 6169 6e2c 2074 6573 746c 6172 6765  train, testlarge
+000221e0: 0a20 2020 2065 6c69 6620 6d6f 6465 6c74  .    elif modelt
+000221f0: 7970 6520 3d3d 2027 5265 6772 6573 7369  ype == 'Regressi
+00022200: 6f6e 2720 616e 6420 6e5f 7370 6c69 7473  on' and n_splits
+00022210: 203d 3d20 333a 0a20 2020 2020 2020 206e   == 3:.        n
+00022220: 756d 7332 203d 2069 6e74 2830 2e35 2a28  ums2 = int(0.5*(
+00022230: 7465 7374 6c61 7267 652e 7368 6170 655b  testlarge.shape[
+00022240: 305d 2929 0a20 2020 2020 2020 2076 616c  0])).        val
+00022250: 6964 2c20 7465 7374 203d 2074 6573 746c  id, test = testl
+00022260: 6172 6765 5b3a 6e75 6d73 325d 2c20 7465  arge[:nums2], te
+00022270: 7374 6c61 7267 655b 6e75 6d73 323a 5d0a  stlarge[nums2:].
+00022280: 2020 2020 2020 2020 7072 696e 7428 2752          print('R
+00022290: 6574 7572 6e69 6e67 2061 2054 7570 6c65  eturning a Tuple
+000222a0: 2077 6974 6820 7468 7265 6520 6461 7461   with three data
+000222b0: 6672 616d 6573 2061 6e64 2073 6861 7065  frames and shape
+000222c0: 733a 2028 2573 2c25 732c 2573 2927 2025  s: (%s,%s,%s)' %
+000222d0: 2874 7261 696e 2e73 6861 7065 2c20 7661  (train.shape, va
+000222e0: 6c69 642e 7368 6170 652c 2074 6573 742e  lid.shape, test.
+000222f0: 7368 6170 6529 290a 2020 2020 2020 2020  shape)).        
+00022300: 7265 7475 726e 2074 7261 696e 2c20 7661  return train, va
+00022310: 6c69 642c 2074 6573 740a 2020 2020 656c  lid, test.    el
+00022320: 6966 206d 6f64 656c 7479 7065 203d 3d20  if modeltype == 
+00022330: 2743 6c61 7373 6966 6963 6174 696f 6e27  'Classification'
+00022340: 2061 6e64 206e 5f73 706c 6974 7320 3d3d   and n_splits ==
+00022350: 2033 3a0a 2020 2020 2020 2020 7661 6c69   3:.        vali
+00022360: 642c 2074 6573 7420 3d20 7472 6169 6e5f  d, test = train_
+00022370: 7465 7374 5f73 706c 6974 2874 6573 746c  test_split(testl
+00022380: 6172 6765 2c20 7465 7374 5f73 697a 653d  arge, test_size=
+00022390: 302e 352c 2072 616e 646f 6d5f 7374 6174  0.5, random_stat
+000223a0: 653d 3939 290a 2020 2020 2020 2020 7072  e=99).        pr
+000223b0: 696e 7428 2752 6574 7572 6e69 6e67 2061  int('Returning a
+000223c0: 2054 7570 6c65 2077 6974 6820 7468 7265   Tuple with thre
+000223d0: 6520 6461 7461 6672 616d 6573 2061 6e64  e dataframes and
+000223e0: 2073 6861 7065 733a 2028 2573 2c25 732c   shapes: (%s,%s,
+000223f0: 2573 2927 2025 2874 7261 696e 2e73 6861  %s)' %(train.sha
+00022400: 7065 2c20 7661 6c69 642e 7368 6170 652c  pe, valid.shape,
+00022410: 2074 6573 742e 7368 6170 6529 290a 2020   test.shape)).  
+00022420: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
+00022430: 696e 2c20 7661 6c69 642c 2074 6573 740a  in, valid, test.
+00022440: 2020 2020 2323 2323 2043 6f6e 7469 6e75      #### Continu
+00022450: 6520 6f6e 6c79 2069 6620 796f 7520 6e65  e only if you ne
+00022460: 6564 206d 6f72 6520 7468 616e 2033 2073  ed more than 3 s
+00022470: 706c 6974 7320 2323 2323 2323 0a20 2020  plits ######.   
+00022480: 2069 6620 6d6f 6465 6c74 7970 6520 3d3d   if modeltype ==
+00022490: 2027 5265 6772 6573 7369 6f6e 273a 0a20   'Regression':. 
+000224a0: 2020 2020 2020 206e 756d 7332 203d 2069         nums2 = i
+000224b0: 6e74 2830 2e35 2a28 6466 2e73 6861 7065  nt(0.5*(df.shape
+000224c0: 5b30 5d20 2d20 6e75 6d73 2929 0a20 2020  [0] - nums)).   
+000224d0: 2020 2020 2076 616c 6964 2c20 7465 7374       valid, test
+000224e0: 203d 2074 6573 746c 6172 6765 5b3a 6e75   = testlarge[:nu
+000224f0: 6d73 325d 2c20 7465 7374 6c61 7267 655b  ms2], testlarge[
+00022500: 6e75 6d73 323a 5d0a 2020 2020 2020 2020  nums2:].        
+00022510: 6966 206e 5f73 706c 6974 7320 3d3d 2034  if n_splits == 4
+00022520: 3a0a 2020 2020 2020 2020 2020 2020 585f  :.            X_
+00022530: 7472 6169 6e2c 2079 5f74 7261 696e 2c20  train, y_train, 
+00022540: 585f 7465 7374 2c20 795f 7465 7374 203d  X_test, y_test =
+00022550: 2074 7261 696e 5b70 7265 6473 5d2c 2074   train[preds], t
+00022560: 7261 696e 5b74 6172 6765 745d 2c20 7465  rain[target], te
+00022570: 7374 6c61 7267 655b 7072 6564 735d 2c20  stlarge[preds], 
+00022580: 7465 7374 6c61 7267 655b 7461 7267 6574  testlarge[target
+00022590: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
+000225a0: 7374 5f6f 665f 6466 7320 3d20 5b58 5f74  st_of_dfs = [X_t
+000225b0: 7261 696e 2c79 5f74 7261 696e 2c20 585f  rain,y_train, X_
+000225c0: 7465 7374 2c20 795f 7465 7374 5d0a 2020  test, y_test].  
+000225d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000225e0: 2752 6574 7572 6e69 6e67 2061 2054 7570  'Returning a Tup
+000225f0: 6c65 2077 6974 6820 3420 6461 7461 6672  le with 4 datafr
+00022600: 616d 6573 3a20 2825 7320 2573 2025 7320  ames: (%s %s %s 
+00022610: 2573 2927 2025 2858 5f74 7261 696e 2e73  %s)' %(X_train.s
+00022620: 6861 7065 2c79 5f74 7261 696e 2e73 6861  hape,y_train.sha
+00022630: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+00022640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022650: 2020 2020 585f 7465 7374 2e73 6861 7065      X_test.shape
+00022660: 2c79 5f74 6573 742e 7368 6170 6529 290a  ,y_test.shape)).
+00022670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00022680: 726e 206c 6973 745f 6f66 5f64 6673 0a20  rn list_of_dfs. 
+00022690: 2020 2020 2020 2065 6c69 6620 6e5f 7370         elif n_sp
+000226a0: 6c69 7473 203d 3d20 363a 0a20 2020 2020  lits == 6:.     
+000226b0: 2020 2020 2020 2058 5f74 7261 696e 2c20         X_train, 
+000226c0: 795f 7472 6169 6e2c 2058 5f76 616c 6964  y_train, X_valid
+000226d0: 2c20 795f 7661 6c69 642c 2058 5f74 6573  , y_valid, X_tes
+000226e0: 742c 2079 5f74 6573 7420 3d20 7472 6169  t, y_test = trai
+000226f0: 6e5b 7072 6564 735d 2c20 7472 6169 6e5b  n[preds], train[
+00022700: 7461 7267 6574 5d2c 2076 616c 6964 5b0a  target], valid[.
+00022710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022730: 2020 2020 7072 6564 735d 2c20 7661 6c69      preds], vali
+00022740: 645b 7461 7267 6574 5d2c 2074 6573 745b  d[target], test[
+00022750: 7072 6564 735d 2c20 7465 7374 5b74 6172  preds], test[tar
+00022760: 6765 745d 0a20 2020 2020 2020 2020 2020  get].           
+00022770: 206c 6973 745f 6f66 5f64 6673 203d 205b   list_of_dfs = [
+00022780: 585f 7472 6169 6e2c 795f 7472 6169 6e2c  X_train,y_train,
+00022790: 2058 5f76 616c 6964 2c20 795f 7661 6c69   X_valid, y_vali
+000227a0: 642c 2058 5f74 6573 742c 2079 5f74 6573  d, X_test, y_tes
+000227b0: 745d 0a20 2020 2020 2020 2020 2020 2070  t].            p
+000227c0: 7269 6e74 2827 5265 7475 726e 696e 6720  rint('Returning 
+000227d0: 6120 5475 706c 6520 7769 7468 2073 6978  a Tuple with six
+000227e0: 2064 6174 6166 7261 6d65 7320 616e 6420   dataframes and 
+000227f0: 7368 6170 6573 3a20 2825 7320 2573 2025  shapes: (%s %s %
+00022800: 7320 2573 2c25 732c 2573 2927 2025 280a  s %s,%s,%s)' %(.
+00022810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022820: 585f 7472 6169 6e2e 7368 6170 652c 795f  X_train.shape,y_
+00022830: 7472 6169 6e2e 7368 6170 652c 2058 5f76  train.shape, X_v
+00022840: 616c 6964 2e73 6861 7065 2c79 5f76 616c  alid.shape,y_val
+00022850: 6964 2e73 6861 7065 2c58 5f74 6573 742e  id.shape,X_test.
+00022860: 7368 6170 652c 795f 7465 7374 2e73 6861  shape,y_test.sha
+00022870: 7065 2929 0a20 2020 2020 2020 2020 2020  pe)).           
+00022880: 2072 6574 7572 6e20 6c69 7374 5f6f 665f   return list_of_
+00022890: 6466 730a 2020 2020 2020 2020 656c 7365  dfs.        else
+000228a0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000228b0: 696e 7428 274e 756d 6265 7220 6f66 2073  int('Number of s
+000228c0: 706c 6974 7320 6d75 7374 2062 6520 322c  plits must be 2,
+000228d0: 2033 2c20 3420 6f72 2036 2729 0a20 2020   3, 4 or 6').   
+000228e0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000228f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00022900: 2020 6966 206e 5f73 706c 6974 7320 3d3d    if n_splits ==
+00022910: 2034 3a0a 2020 2020 2020 2020 2020 2020   4:.            
+00022920: 585f 7472 6169 6e2c 2079 5f74 7261 696e  X_train, y_train
+00022930: 2c20 585f 7465 7374 2c20 795f 7465 7374  , X_test, y_test
+00022940: 203d 2074 7261 696e 5b70 7265 6473 5d2c   = train[preds],
+00022950: 2074 7261 696e 5b74 6172 6765 745d 2c20   train[target], 
+00022960: 7465 7374 6c61 7267 655b 7072 6564 735d  testlarge[preds]
+00022970: 2c20 7465 7374 6c61 7267 655b 7461 7267  , testlarge[targ
+00022980: 6574 5d0a 2020 2020 2020 2020 2020 2020  et].            
+00022990: 6c69 7374 5f6f 665f 6466 7320 3d20 5b58  list_of_dfs = [X
+000229a0: 5f74 7261 696e 2c79 5f74 7261 696e 2c20  _train,y_train, 
+000229b0: 585f 7465 7374 2c20 795f 7465 7374 5d0a  X_test, y_test].
+000229c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000229d0: 7428 2752 6574 7572 6e69 6e67 2061 2054  t('Returning a T
+000229e0: 7570 6c65 2077 6974 6820 3420 6461 7461  uple with 4 data
+000229f0: 6672 616d 6573 3a20 2825 7320 2573 2025  frames: (%s %s %
+00022a00: 7320 2573 2927 2025 2858 5f74 7261 696e  s %s)' %(X_train
+00022a10: 2e73 6861 7065 2c79 5f74 7261 696e 2e73  .shape,y_train.s
+00022a20: 6861 7065 2c0a 2020 2020 2020 2020 2020  hape,.          
+00022a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a40: 2020 2020 2020 585f 7465 7374 2e73 6861        X_test.sha
+00022a50: 7065 2c79 5f74 6573 742e 7368 6170 6529  pe,y_test.shape)
+00022a60: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00022a70: 7475 726e 206c 6973 745f 6f66 5f64 6673  turn list_of_dfs
+00022a80: 0a20 2020 2020 2020 2065 6c69 6620 6e5f  .        elif n_
+00022a90: 7370 6c69 7473 203d 3d20 363a 0a20 2020  splits == 6:.   
+00022aa0: 2020 2020 2020 2020 2058 5f74 7261 696e           X_train
+00022ab0: 2c20 795f 7472 6169 6e2c 2058 5f76 616c  , y_train, X_val
+00022ac0: 6964 2c20 795f 7661 6c69 642c 2058 5f74  id, y_valid, X_t
+00022ad0: 6573 742c 2079 5f74 6573 7420 3d20 7472  est, y_test = tr
+00022ae0: 6169 6e5b 7072 6564 735d 2c20 7472 6169  ain[preds], trai
+00022af0: 6e5b 7461 7267 6574 5d2c 2076 616c 6964  n[target], valid
+00022b00: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00022b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b20: 2020 2020 2020 7072 6564 735d 2c20 7661        preds], va
+00022b30: 6c69 645b 7461 7267 6574 5d2c 2074 6573  lid[target], tes
+00022b40: 745b 7072 6564 735d 2c20 7465 7374 5b74  t[preds], test[t
+00022b50: 6172 6765 745d 0a20 2020 2020 2020 2020  arget].         
+00022b60: 2020 2070 7269 6e74 2827 5265 7475 726e     print('Return
+00022b70: 696e 6720 3420 6461 7461 6672 616d 6573  ing 4 dataframes
+00022b80: 3a27 2c20 585f 7472 6169 6e2e 7368 6170  :', X_train.shap
+00022b90: 652c 2079 5f74 7261 696e 2e73 6861 7065  e, y_train.shape
+00022ba0: 2c20 585f 7465 7374 2e73 6861 7065 2c20  , X_test.shape, 
+00022bb0: 795f 7465 7374 2e73 6861 7065 290a 2020  y_test.shape).  
+00022bc0: 2020 2020 2020 2020 2020 6c69 7374 5f6f            list_o
+00022bd0: 665f 6466 7320 3d20 5b58 5f74 7261 696e  f_dfs = [X_train
+00022be0: 2c79 5f74 7261 696e 2c20 585f 7661 6c69  ,y_train, X_vali
+00022bf0: 642c 2079 5f76 616c 6964 2c20 585f 7465  d, y_valid, X_te
+00022c00: 7374 2c20 795f 7465 7374 5d0a 2020 2020  st, y_test].    
+00022c10: 2020 2020 2020 2020 7072 696e 7428 2752          print('R
+00022c20: 6574 7572 6e69 6e67 2061 2054 7570 6c65  eturning a Tuple
+00022c30: 2077 6974 6820 7369 7820 6461 7461 6672   with six datafr
+00022c40: 616d 6573 2061 6e64 2073 6861 7065 733a  ames and shapes:
+00022c50: 2028 2573 2025 7320 2573 2025 732c 2573   (%s %s %s %s,%s
+00022c60: 2c25 7329 2720 2528 0a20 2020 2020 2020  ,%s)' %(.       
+00022c70: 2020 2020 2020 2020 2058 5f74 7261 696e           X_train
+00022c80: 2e73 6861 7065 2c79 5f74 7261 696e 2e73  .shape,y_train.s
+00022c90: 6861 7065 2c20 585f 7661 6c69 642e 7368  hape, X_valid.sh
+00022ca0: 6170 652c 795f 7661 6c69 642e 7368 6170  ape,y_valid.shap
+00022cb0: 652c 585f 7465 7374 2e73 6861 7065 2c79  e,X_test.shape,y
+00022cc0: 5f74 6573 742e 7368 6170 6529 290a 2020  _test.shape)).  
+00022cd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00022ce0: 206c 6973 745f 6f66 5f64 6673 0a20 2020   list_of_dfs.   
+00022cf0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00022d00: 2020 2020 2020 2070 7269 6e74 2827 4e75         print('Nu
+00022d10: 6d62 6572 206f 6620 7370 6c69 7473 206d  mber of splits m
+00022d20: 7573 7420 6265 2032 2c20 332c 2034 206f  ust be 2, 3, 4 o
+00022d30: 7220 3627 290a 2020 2020 2020 2020 2020  r 6').          
+00022d40: 2020 7265 7475 726e 0a23 2323 2323 2323    return.#######
 00022d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00022d60: 2323 2323 2323 2323 230a 6465 6620 4645  #########.def FE
-00022d70: 5f63 6f6e 6361 7465 6e61 7465 5f6d 756c  _concatenate_mul
-00022d80: 7469 706c 655f 636f 6c75 6d6e 7328 6466  tiple_columns(df
-00022d90: 2c20 636f 6c73 2c20 6669 6c6c 6572 3d22  , cols, filler="
-00022da0: 2022 2c20 6472 6f70 3d54 7275 6529 3a0a   ", drop=True):.
-00022db0: 2020 2020 2222 220a 2020 2020 5468 6973      """.    This
-00022dc0: 2068 616e 6479 2066 756e 6374 696f 6e20   handy function 
-00022dd0: 636f 6d62 696e 6573 206d 756c 7469 706c  combines multipl
-00022de0: 6520 7374 7269 6e67 2063 6f6c 756d 6e73  e string columns
-00022df0: 2069 6e74 6f20 6120 7369 6e67 6c65 204e   into a single N
-00022e00: 4c50 2074 6578 7420 636f 6c75 6d6e 2e0a  LP text column..
-00022e10: 2020 2020 596f 7520 6361 6e20 646f 2066      You can do f
-00022e20: 7572 7468 6572 2070 7265 2d70 726f 6365  urther pre-proce
-00022e30: 7373 696e 6720 6f6e 2073 7563 6820 6120  ssing on such a 
-00022e40: 636f 6d62 696e 6564 2063 6f6c 756d 6e20  combined column 
-00022e50: 7769 7468 2054 4649 4446 206f 7220 4245  with TFIDF or BE
-00022e60: 5254 2073 7479 6c65 2065 6d62 6564 6469  RT style embeddi
-00022e70: 6e67 2e0a 0a20 2020 2049 6e70 7574 730a  ng...    Inputs.
-00022e80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d0a 2020      ---------.  
-00022e90: 2020 2020 2020 6466 3a20 7061 6e64 6173        df: pandas
-00022ea0: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
-00022eb0: 2020 2063 6f6c 733a 2073 7472 696e 6720     cols: string 
-00022ec0: 636f 6c75 6d6e 7320 7468 6174 2079 6f75  columns that you
-00022ed0: 2077 616e 7420 746f 2063 6f6e 6361 7465   want to concate
-00022ee0: 6e61 7465 2069 6e74 6f20 6120 7369 6e67  nate into a sing
-00022ef0: 6c65 2063 6f6d 6269 6e65 6420 636f 6c75  le combined colu
-00022f00: 6d6e 0a20 2020 2020 2020 2066 696c 6c65  mn.        fille
-00022f10: 723a 2073 7472 696e 6720 2864 6566 6175  r: string (defau
-00022f20: 6c74 3a20 2220 2229 3a20 796f 7520 6361  lt: " "): you ca
-00022f30: 6e20 696e 7075 7420 616e 7920 7374 7269  n input any stri
-00022f40: 6e67 2074 6861 7420 796f 7520 7761 6e74  ng that you want
-00022f50: 2074 6f20 636f 6d62 696e 6520 7468 656d   to combine them
-00022f60: 2077 6974 682e 0a20 2020 2020 2020 2064   with..        d
-00022f70: 726f 703a 2064 6566 6175 6c74 2054 7275  rop: default Tru
-00022f80: 652e 2049 6620 5472 7565 2c20 6472 6f70  e. If True, drop
-00022f90: 2074 6865 2063 6f6c 756d 6e73 2069 6e70   the columns inp
-00022fa0: 7574 2e20 4966 2046 616c 7365 2c20 6b65  ut. If False, ke
-00022fb0: 6570 2074 6865 2063 6f6c 756d 6e73 2e0a  ep the columns..
-00022fc0: 0a20 2020 204f 7574 7075 7473 3a0a 2020  .    Outputs:.  
-00022fd0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00022fe0: 2020 2020 2064 663a 2074 6865 7265 2077       df: there w
-00022ff0: 696c 6c20 6265 2061 206e 6577 2063 6f6c  ill be a new col
-00023000: 756d 6e20 6361 6c6c 6564 205b 2763 6f6d  umn called ['com
-00023010: 6269 6e65 6427 5d20 7468 6174 2077 696c  bined'] that wil
-00023020: 6c20 6265 2061 6464 6564 2074 6f20 796f  l be added to yo
-00023030: 7572 2064 6174 6166 7261 6d65 2e0a 2020  ur dataframe..  
-00023040: 2020 2222 220a 2020 2020 6466 203d 2064    """.    df = d
-00023050: 662e 636f 7079 2864 6565 703d 5472 7565  f.copy(deep=True
-00023060: 290a 2020 2020 6466 5b27 636f 6d62 696e  ).    df['combin
-00023070: 6564 275d 203d 2064 665b 636f 6c73 5d2e  ed'] = df[cols].
-00023080: 6170 706c 7928 6c61 6d62 6461 2072 6f77  apply(lambda row
-00023090: 3a20 6669 6c6c 6572 2e6a 6f69 6e28 726f  : filler.join(ro
-000230a0: 772e 7661 6c75 6573 2e61 7374 7970 6528  w.values.astype(
-000230b0: 7374 7229 292c 2061 7869 733d 3129 0a20  str)), axis=1). 
-000230c0: 2020 2069 6620 6472 6f70 3a0a 2020 2020     if drop:.    
-000230d0: 2020 2020 6466 203d 2064 662e 6472 6f70      df = df.drop
-000230e0: 2863 6f6c 732c 2061 7869 733d 3129 0a20  (cols, axis=1). 
-000230f0: 2020 2072 6574 7572 6e20 6466 0a23 2323     return df.###
-00023100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00022d90: 2323 2323 2323 2323 2323 230a 6465 6620  ###########.def 
+00022da0: 4645 5f63 6f6e 6361 7465 6e61 7465 5f6d  FE_concatenate_m
+00022db0: 756c 7469 706c 655f 636f 6c75 6d6e 7328  ultiple_columns(
+00022dc0: 6466 2c20 636f 6c73 2c20 6669 6c6c 6572  df, cols, filler
+00022dd0: 3d22 2022 2c20 6472 6f70 3d54 7275 6529  =" ", drop=True)
+00022de0: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+00022df0: 6973 2068 616e 6479 2066 756e 6374 696f  is handy functio
+00022e00: 6e20 636f 6d62 696e 6573 206d 756c 7469  n combines multi
+00022e10: 706c 6520 7374 7269 6e67 2063 6f6c 756d  ple string colum
+00022e20: 6e73 2069 6e74 6f20 6120 7369 6e67 6c65  ns into a single
+00022e30: 204e 4c50 2074 6578 7420 636f 6c75 6d6e   NLP text column
+00022e40: 2e0a 2020 2020 596f 7520 6361 6e20 646f  ..    You can do
+00022e50: 2066 7572 7468 6572 2070 7265 2d70 726f   further pre-pro
+00022e60: 6365 7373 696e 6720 6f6e 2073 7563 6820  cessing on such 
+00022e70: 6120 636f 6d62 696e 6564 2063 6f6c 756d  a combined colum
+00022e80: 6e20 7769 7468 2054 4649 4446 206f 7220  n with TFIDF or 
+00022e90: 4245 5254 2073 7479 6c65 2065 6d62 6564  BERT style embed
+00022ea0: 6469 6e67 2e0a 0a20 2020 2049 6e70 7574  ding...    Input
+00022eb0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d0a  s.    ---------.
+00022ec0: 2020 2020 2020 2020 6466 3a20 7061 6e64          df: pand
+00022ed0: 6173 2064 6174 6166 7261 6d65 0a20 2020  as dataframe.   
+00022ee0: 2020 2020 2063 6f6c 733a 2073 7472 696e       cols: strin
+00022ef0: 6720 636f 6c75 6d6e 7320 7468 6174 2079  g columns that y
+00022f00: 6f75 2077 616e 7420 746f 2063 6f6e 6361  ou want to conca
+00022f10: 7465 6e61 7465 2069 6e74 6f20 6120 7369  tenate into a si
+00022f20: 6e67 6c65 2063 6f6d 6269 6e65 6420 636f  ngle combined co
+00022f30: 6c75 6d6e 0a20 2020 2020 2020 2066 696c  lumn.        fil
+00022f40: 6c65 723a 2073 7472 696e 6720 2864 6566  ler: string (def
+00022f50: 6175 6c74 3a20 2220 2229 3a20 796f 7520  ault: " "): you 
+00022f60: 6361 6e20 696e 7075 7420 616e 7920 7374  can input any st
+00022f70: 7269 6e67 2074 6861 7420 796f 7520 7761  ring that you wa
+00022f80: 6e74 2074 6f20 636f 6d62 696e 6520 7468  nt to combine th
+00022f90: 656d 2077 6974 682e 0a20 2020 2020 2020  em with..       
+00022fa0: 2064 726f 703a 2064 6566 6175 6c74 2054   drop: default T
+00022fb0: 7275 652e 2049 6620 5472 7565 2c20 6472  rue. If True, dr
+00022fc0: 6f70 2074 6865 2063 6f6c 756d 6e73 2069  op the columns i
+00022fd0: 6e70 7574 2e20 4966 2046 616c 7365 2c20  nput. If False, 
+00022fe0: 6b65 6570 2074 6865 2063 6f6c 756d 6e73  keep the columns
+00022ff0: 2e0a 0a20 2020 204f 7574 7075 7473 3a0a  ...    Outputs:.
+00023000: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00023010: 2020 2020 2020 2064 663a 2074 6865 7265         df: there
+00023020: 2077 696c 6c20 6265 2061 206e 6577 2063   will be a new c
+00023030: 6f6c 756d 6e20 6361 6c6c 6564 205b 2763  olumn called ['c
+00023040: 6f6d 6269 6e65 6427 5d20 7468 6174 2077  ombined'] that w
+00023050: 696c 6c20 6265 2061 6464 6564 2074 6f20  ill be added to 
+00023060: 796f 7572 2064 6174 6166 7261 6d65 2e0a  your dataframe..
+00023070: 2020 2020 2222 220a 2020 2020 6466 203d      """.    df =
+00023080: 2064 662e 636f 7079 2864 6565 703d 5472   df.copy(deep=Tr
+00023090: 7565 290a 2020 2020 6466 5b27 636f 6d62  ue).    df['comb
+000230a0: 696e 6564 275d 203d 2064 665b 636f 6c73  ined'] = df[cols
+000230b0: 5d2e 6170 706c 7928 6c61 6d62 6461 2072  ].apply(lambda r
+000230c0: 6f77 3a20 6669 6c6c 6572 2e6a 6f69 6e28  ow: filler.join(
+000230d0: 726f 772e 7661 6c75 6573 2e61 7374 7970  row.values.astyp
+000230e0: 6528 7374 7229 292c 2061 7869 733d 3129  e(str)), axis=1)
+000230f0: 0a20 2020 2069 6620 6472 6f70 3a0a 2020  .    if drop:.  
+00023100: 2020 2020 2020 6466 203d 2064 662e 6472        df = df.dr
+00023110: 6f70 2863 6f6c 732c 2061 7869 733d 3129  op(cols, axis=1)
+00023120: 0a20 2020 2072 6574 7572 6e20 6466 0a23  .    return df.#
 00023130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023140: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00023150: 6672 6f6d 2073 6b6c 6561 726e 2e70 7265  from sklearn.pre
-00023160: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
-00023170: 7420 4b42 696e 7344 6973 6372 6574 697a  t KBinsDiscretiz
-00023180: 6572 0a66 726f 6d20 736b 6c65 6172 6e2e  er.from sklearn.
-00023190: 6d69 7874 7572 6520 696d 706f 7274 2047  mixture import G
-000231a0: 6175 7373 6961 6e4d 6978 7475 7265 0a0a  aussianMixture..
-000231b0: 6465 6620 4645 5f64 6973 6372 6574 697a  def FE_discretiz
-000231c0: 655f 6e75 6d65 7269 635f 7661 7269 6162  e_numeric_variab
-000231d0: 6c65 7328 7472 6169 6e2c 2062 696e 5f64  les(train, bin_d
-000231e0: 6963 742c 2074 6573 743d 2727 2c20 7374  ict, test='', st
-000231f0: 7261 7465 6779 3d27 6b6d 6561 6e73 272c  rategy='kmeans',
-00023200: 7665 7262 6f73 653d 3029 3a0a 2020 2020  verbose=0):.    
-00023210: 2222 220a 2020 2020 5468 6973 2068 616e  """.    This han
-00023220: 6479 2066 756e 6374 696f 6e20 6469 7363  dy function disc
-00023230: 7265 7469 7a65 7320 6e75 6d65 7269 6320  retizes numeric 
-00023240: 7661 7269 6162 6c65 7320 696e 746f 2062  variables into b
-00023250: 696e 6e65 6420 7661 7269 6162 6c65 7320  inned variables 
-00023260: 7573 696e 6720 6b6d 6561 6e73 2061 6c67  using kmeans alg
-00023270: 6f72 6974 686d 2e0a 2020 2020 596f 7520  orithm..    You 
-00023280: 6e65 6564 2074 6f20 7072 6f76 6964 6520  need to provide 
-00023290: 7468 6520 6e61 6d65 7320 6f66 2074 6865  the names of the
-000232a0: 2076 6172 6961 626c 6573 2061 6e64 2074   variables and t
-000232b0: 6865 206e 756d 6265 7273 206f 6620 6269  he numbers of bi
-000232c0: 6e73 2066 6f72 2065 6163 6820 7661 7269  ns for each vari
-000232d0: 6162 6c65 2069 6e20 6120 6469 6374 696f  able in a dictio
-000232e0: 6e61 7279 2e0a 2020 2020 4974 2077 696c  nary..    It wil
-000232f0: 6c20 7265 7475 726e 2074 6865 2073 616d  l return the sam
-00023300: 6520 6461 7461 6672 616d 6520 7769 7468  e dataframe with
-00023310: 206e 6577 2062 696e 6e65 6420 7661 7269   new binned vari
-00023320: 6162 6c65 7320 7468 6174 2069 7420 6861  ables that it ha
-00023330: 7320 6372 6561 7465 642e 0a0a 2020 2020  s created...    
-00023340: 496e 7075 7473 3a0a 2020 2020 2d2d 2d2d  Inputs:.    ----
-00023350: 2d2d 2d2d 2d2d 0a20 2020 2064 6620 3a20  ------.    df : 
-00023360: 7061 6e64 6173 2064 6174 6166 7261 6d65  pandas dataframe
-00023370: 202d 2070 6c65 6173 6520 656e 7375 7265   - please ensure
-00023380: 2069 7420 6973 2061 2064 6174 6166 7261   it is a datafra
-00023390: 6d65 2e20 4e6f 2061 7272 6179 7320 706c  me. No arrays pl
-000233a0: 6561 7365 2e0a 2020 2020 6269 6e5f 6469  ease..    bin_di
-000233b0: 6374 3a20 6469 6374 696f 6e61 7279 206f  ct: dictionary o
-000233c0: 6620 6e61 6d65 7320 6f66 2076 6172 6961  f names of varia
-000233d0: 626c 6573 2061 6e64 2074 6865 2062 696e  bles and the bin
-000233e0: 7320 7468 6174 2079 6f75 2077 616e 7420  s that you want 
-000233f0: 666f 7220 6561 6368 2076 6172 6961 626c  for each variabl
-00023400: 652e 0a20 2020 2073 7472 6174 6567 793a  e..    strategy:
-00023410: 2064 6566 6175 6c74 2069 7320 276b 6d65   default is 'kme
-00023420: 616e 7327 3a20 6275 7420 796f 7520 6361  ans': but you ca
-00023430: 6e20 6368 6f6f 7365 3a20 7b27 6761 7575  n choose: {'gauu
-00023440: 7369 616e 272c 2775 6e69 666f 726d 272c  sian','uniform',
-00023450: 2027 7175 616e 7469 6c65 272c 2027 6b6d   'quantile', 'km
-00023460: 6561 6e73 277d 0a0a 2020 2020 4f75 7470  eans'}..    Outp
-00023470: 7574 733a 0a20 2020 202d 2d2d 2d2d 2d2d  uts:.    -------
-00023480: 2d2d 2d0a 2020 2020 6466 3a20 7061 6e64  ---.    df: pand
-00023490: 6173 2064 6174 6166 7261 6d65 2077 6974  as dataframe wit
-000234a0: 6820 6e65 7720 7661 7269 6162 6c65 7320  h new variables 
-000234b0: 7769 7468 206e 616d 6573 2073 7563 6820  with names such 
-000234c0: 6173 3a20 2076 6172 6961 626c 652b 275f  as:  variable+'_
-000234d0: 6469 7363 7265 7465 270a 2020 2020 2222  discrete'.    ""
-000234e0: 220a 2020 2020 6466 203d 2063 6f70 792e  ".    df = copy.
-000234f0: 6465 6570 636f 7079 2874 7261 696e 290a  deepcopy(train).
-00023500: 2020 2020 7465 7374 203d 2063 6f70 792e      test = copy.
-00023510: 6465 6570 636f 7079 2874 6573 7429 0a20  deepcopy(test). 
-00023520: 2020 206e 756d 5f63 6f6c 7320 3d20 6c65     num_cols = le
-00023530: 6e28 6269 6e5f 6469 6374 290a 2020 2020  n(bin_dict).    
-00023540: 6e72 6f77 7320 3d20 696e 7428 286e 756d  nrows = int((num
-00023550: 5f63 6f6c 732f 3229 2b30 2e35 290a 2020  _cols/2)+0.5).  
-00023560: 2020 2370 7269 6e74 2827 6e72 6f77 7327    #print('nrows'
-00023570: 2c6e 726f 7773 290a 2020 2020 6966 2076  ,nrows).    if v
-00023580: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00023590: 6669 6720 3d20 706c 742e 6669 6775 7265  fig = plt.figure
-000235a0: 2866 6967 7369 7a65 3d28 3130 2c33 2a6e  (figsize=(10,3*n
-000235b0: 756d 5f63 6f6c 7329 290a 2020 2020 666f  um_cols)).    fo
-000235c0: 7220 692c 2028 636f 6c2c 2062 696e 7661  r i, (col, binva
-000235d0: 6c75 6529 2069 6e20 656e 756d 6572 6174  lue) in enumerat
-000235e0: 6528 6269 6e5f 6469 6374 2e69 7465 6d73  e(bin_dict.items
-000235f0: 2829 293a 0a20 2020 2020 2020 206e 6577  ()):.        new
-00023600: 5f63 6f6c 203d 2063 6f6c 2b27 5f64 6973  _col = col+'_dis
-00023610: 6372 6574 6527 0a20 2020 2020 2020 2069  crete'.        i
-00023620: 6620 7374 7261 7465 6779 203d 3d20 2767  f strategy == 'g
-00023630: 6175 7373 6961 6e27 3a0a 2020 2020 2020  aussian':.      
-00023640: 2020 2020 2020 6b62 6420 3d20 4761 7573        kbd = Gaus
-00023650: 7369 616e 4d69 7874 7572 6528 6e5f 636f  sianMixture(n_co
-00023660: 6d70 6f6e 656e 7473 3d62 696e 7661 6c75  mponents=binvalu
-00023670: 652c 2072 616e 646f 6d5f 7374 6174 653d  e, random_state=
-00023680: 3939 290a 2020 2020 2020 2020 2020 2020  99).            
-00023690: 6466 5b6e 6577 5f63 6f6c 5d20 3d20 6b62  df[new_col] = kb
-000236a0: 642e 6669 745f 7072 6564 6963 7428 6466  d.fit_predict(df
-000236b0: 5b5b 636f 6c5d 5d29 2e61 7374 7970 6528  [[col]]).astype(
-000236c0: 696e 7429 0a20 2020 2020 2020 2020 2020  int).           
-000236d0: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-000236e0: 6365 2874 6573 742c 2073 7472 293a 0a20  ce(test, str):. 
-000236f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00023700: 6573 745b 6e65 775f 636f 6c5d 203d 206b  est[new_col] = k
-00023710: 6264 2e70 7265 6469 6374 2874 6573 745b  bd.predict(test[
-00023720: 5b63 6f6c 5d5d 292e 6173 7479 7065 2869  [col]]).astype(i
-00023730: 6e74 290a 2020 2020 2020 2020 656c 7365  nt).        else
-00023740: 3a0a 2020 2020 2020 2020 2020 2020 6b62  :.            kb
-00023750: 6420 3d20 4b42 696e 7344 6973 6372 6574  d = KBinsDiscret
-00023760: 697a 6572 286e 5f62 696e 733d 6269 6e76  izer(n_bins=binv
-00023770: 616c 7565 2c20 656e 636f 6465 3d27 6f72  alue, encode='or
-00023780: 6469 6e61 6c27 2c20 7374 7261 7465 6779  dinal', strategy
-00023790: 3d73 7472 6174 6567 7929 0a20 2020 2020  =strategy).     
-000237a0: 2020 2020 2020 2064 665b 6e65 775f 636f         df[new_co
-000237b0: 6c5d 203d 206b 6264 2e66 6974 5f74 7261  l] = kbd.fit_tra
-000237c0: 6e73 666f 726d 2864 665b 5b63 6f6c 5d5d  nsform(df[[col]]
-000237d0: 292e 6173 7479 7065 2869 6e74 290a 2020  ).astype(int).  
-000237e0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000237f0: 2069 7369 6e73 7461 6e63 6528 7465 7374   isinstance(test
-00023800: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00023810: 2020 2020 2020 2020 7465 7374 5b6e 6577          test[new
-00023820: 5f63 6f6c 5d20 3d20 6b62 642e 7472 616e  _col] = kbd.tran
-00023830: 7366 6f72 6d28 7465 7374 5b5b 636f 6c5d  sform(test[[col]
-00023840: 5d29 2e61 7374 7970 6528 696e 7429 0a20  ]).astype(int). 
-00023850: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-00023860: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-00023870: 7831 203d 2070 6c74 2e73 7562 706c 6f74  x1 = plt.subplot
-00023880: 286e 726f 7773 2c32 2c69 2b31 290a 2020  (nrows,2,i+1).  
-00023890: 2020 2020 2020 2020 2020 6178 312e 7363            ax1.sc
-000238a0: 6174 7465 7228 6466 5b63 6f6c 5d2c 6466  atter(df[col],df
-000238b0: 5b6e 6577 5f63 6f6c 5d29 0a20 2020 2020  [new_col]).     
-000238c0: 2020 2020 2020 2061 7831 2e73 6574 5f74         ax1.set_t
-000238d0: 6974 6c65 286e 6577 5f63 6f6c 290a 2020  itle(new_col).  
-000238e0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-000238f0: 6e63 6528 7465 7374 2c20 7374 7229 3a0a  nce(test, str):.
-00023900: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00023910: 662c 2074 6573 740a 2020 2020 656c 7365  f, test.    else
-00023920: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00023930: 2064 660a 2323 2323 2323 2323 2323 2323   df.############
-00023940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023180: 230a 6672 6f6d 2073 6b6c 6561 726e 2e70  #.from sklearn.p
+00023190: 7265 7072 6f63 6573 7369 6e67 2069 6d70  reprocessing imp
+000231a0: 6f72 7420 4b42 696e 7344 6973 6372 6574  ort KBinsDiscret
+000231b0: 697a 6572 0a66 726f 6d20 736b 6c65 6172  izer.from sklear
+000231c0: 6e2e 6d69 7874 7572 6520 696d 706f 7274  n.mixture import
+000231d0: 2047 6175 7373 6961 6e4d 6978 7475 7265   GaussianMixture
+000231e0: 0a0a 6465 6620 4645 5f64 6973 6372 6574  ..def FE_discret
+000231f0: 697a 655f 6e75 6d65 7269 635f 7661 7269  ize_numeric_vari
+00023200: 6162 6c65 7328 7472 6169 6e2c 2062 696e  ables(train, bin
+00023210: 5f64 6963 742c 2074 6573 743d 2727 2c20  _dict, test='', 
+00023220: 7374 7261 7465 6779 3d27 6b6d 6561 6e73  strategy='kmeans
+00023230: 272c 7665 7262 6f73 653d 3029 3a0a 2020  ',verbose=0):.  
+00023240: 2020 2222 220a 2020 2020 5468 6973 2068    """.    This h
+00023250: 616e 6479 2066 756e 6374 696f 6e20 6469  andy function di
+00023260: 7363 7265 7469 7a65 7320 6e75 6d65 7269  scretizes numeri
+00023270: 6320 7661 7269 6162 6c65 7320 696e 746f  c variables into
+00023280: 2062 696e 6e65 6420 7661 7269 6162 6c65   binned variable
+00023290: 7320 7573 696e 6720 6b6d 6561 6e73 2061  s using kmeans a
+000232a0: 6c67 6f72 6974 686d 2e0a 2020 2020 596f  lgorithm..    Yo
+000232b0: 7520 6e65 6564 2074 6f20 7072 6f76 6964  u need to provid
+000232c0: 6520 7468 6520 6e61 6d65 7320 6f66 2074  e the names of t
+000232d0: 6865 2076 6172 6961 626c 6573 2061 6e64  he variables and
+000232e0: 2074 6865 206e 756d 6265 7273 206f 6620   the numbers of 
+000232f0: 6269 6e73 2066 6f72 2065 6163 6820 7661  bins for each va
+00023300: 7269 6162 6c65 2069 6e20 6120 6469 6374  riable in a dict
+00023310: 696f 6e61 7279 2e0a 2020 2020 4974 2077  ionary..    It w
+00023320: 696c 6c20 7265 7475 726e 2074 6865 2073  ill return the s
+00023330: 616d 6520 6461 7461 6672 616d 6520 7769  ame dataframe wi
+00023340: 7468 206e 6577 2062 696e 6e65 6420 7661  th new binned va
+00023350: 7269 6162 6c65 7320 7468 6174 2069 7420  riables that it 
+00023360: 6861 7320 6372 6561 7465 642e 0a0a 2020  has created...  
+00023370: 2020 496e 7075 7473 3a0a 2020 2020 2d2d    Inputs:.    --
+00023380: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6620  --------.    df 
+00023390: 3a20 7061 6e64 6173 2064 6174 6166 7261  : pandas datafra
+000233a0: 6d65 202d 2070 6c65 6173 6520 656e 7375  me - please ensu
+000233b0: 7265 2069 7420 6973 2061 2064 6174 6166  re it is a dataf
+000233c0: 7261 6d65 2e20 4e6f 2061 7272 6179 7320  rame. No arrays 
+000233d0: 706c 6561 7365 2e0a 2020 2020 6269 6e5f  please..    bin_
+000233e0: 6469 6374 3a20 6469 6374 696f 6e61 7279  dict: dictionary
+000233f0: 206f 6620 6e61 6d65 7320 6f66 2076 6172   of names of var
+00023400: 6961 626c 6573 2061 6e64 2074 6865 2062  iables and the b
+00023410: 696e 7320 7468 6174 2079 6f75 2077 616e  ins that you wan
+00023420: 7420 666f 7220 6561 6368 2076 6172 6961  t for each varia
+00023430: 626c 652e 0a20 2020 2073 7472 6174 6567  ble..    strateg
+00023440: 793a 2064 6566 6175 6c74 2069 7320 276b  y: default is 'k
+00023450: 6d65 616e 7327 3a20 6275 7420 796f 7520  means': but you 
+00023460: 6361 6e20 6368 6f6f 7365 3a20 7b27 6761  can choose: {'ga
+00023470: 7575 7369 616e 272c 2775 6e69 666f 726d  uusian','uniform
+00023480: 272c 2027 7175 616e 7469 6c65 272c 2027  ', 'quantile', '
+00023490: 6b6d 6561 6e73 277d 0a0a 2020 2020 4f75  kmeans'}..    Ou
+000234a0: 7470 7574 733a 0a20 2020 202d 2d2d 2d2d  tputs:.    -----
+000234b0: 2d2d 2d2d 2d0a 2020 2020 6466 3a20 7061  -----.    df: pa
+000234c0: 6e64 6173 2064 6174 6166 7261 6d65 2077  ndas dataframe w
+000234d0: 6974 6820 6e65 7720 7661 7269 6162 6c65  ith new variable
+000234e0: 7320 7769 7468 206e 616d 6573 2073 7563  s with names suc
+000234f0: 6820 6173 3a20 2076 6172 6961 626c 652b  h as:  variable+
+00023500: 275f 6469 7363 7265 7465 270a 2020 2020  '_discrete'.    
+00023510: 2222 220a 2020 2020 6466 203d 2063 6f70  """.    df = cop
+00023520: 792e 6465 6570 636f 7079 2874 7261 696e  y.deepcopy(train
+00023530: 290a 2020 2020 7465 7374 203d 2063 6f70  ).    test = cop
+00023540: 792e 6465 6570 636f 7079 2874 6573 7429  y.deepcopy(test)
+00023550: 0a20 2020 206e 756d 5f63 6f6c 7320 3d20  .    num_cols = 
+00023560: 6c65 6e28 6269 6e5f 6469 6374 290a 2020  len(bin_dict).  
+00023570: 2020 6e72 6f77 7320 3d20 696e 7428 286e    nrows = int((n
+00023580: 756d 5f63 6f6c 732f 3229 2b30 2e35 290a  um_cols/2)+0.5).
+00023590: 2020 2020 2370 7269 6e74 2827 6e72 6f77      #print('nrow
+000235a0: 7327 2c6e 726f 7773 290a 2020 2020 6966  s',nrows).    if
+000235b0: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+000235c0: 2020 6669 6720 3d20 706c 742e 6669 6775    fig = plt.figu
+000235d0: 7265 2866 6967 7369 7a65 3d28 3130 2c33  re(figsize=(10,3
+000235e0: 2a6e 756d 5f63 6f6c 7329 290a 2020 2020  *num_cols)).    
+000235f0: 666f 7220 692c 2028 636f 6c2c 2062 696e  for i, (col, bin
+00023600: 7661 6c75 6529 2069 6e20 656e 756d 6572  value) in enumer
+00023610: 6174 6528 6269 6e5f 6469 6374 2e69 7465  ate(bin_dict.ite
+00023620: 6d73 2829 293a 0a20 2020 2020 2020 206e  ms()):.        n
+00023630: 6577 5f63 6f6c 203d 2063 6f6c 2b27 5f64  ew_col = col+'_d
+00023640: 6973 6372 6574 6527 0a20 2020 2020 2020  iscrete'.       
+00023650: 2069 6620 7374 7261 7465 6779 203d 3d20   if strategy == 
+00023660: 2767 6175 7373 6961 6e27 3a0a 2020 2020  'gaussian':.    
+00023670: 2020 2020 2020 2020 6b62 6420 3d20 4761          kbd = Ga
+00023680: 7573 7369 616e 4d69 7874 7572 6528 6e5f  ussianMixture(n_
+00023690: 636f 6d70 6f6e 656e 7473 3d62 696e 7661  components=binva
+000236a0: 6c75 652c 2072 616e 646f 6d5f 7374 6174  lue, random_stat
+000236b0: 653d 3939 290a 2020 2020 2020 2020 2020  e=99).          
+000236c0: 2020 6466 5b6e 6577 5f63 6f6c 5d20 3d20    df[new_col] = 
+000236d0: 6b62 642e 6669 745f 7072 6564 6963 7428  kbd.fit_predict(
+000236e0: 6466 5b5b 636f 6c5d 5d29 2e61 7374 7970  df[[col]]).astyp
+000236f0: 6528 696e 7429 0a20 2020 2020 2020 2020  e(int).         
+00023700: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00023710: 616e 6365 2874 6573 742c 2073 7472 293a  ance(test, str):
+00023720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023730: 2074 6573 745b 6e65 775f 636f 6c5d 203d   test[new_col] =
+00023740: 206b 6264 2e70 7265 6469 6374 2874 6573   kbd.predict(tes
+00023750: 745b 5b63 6f6c 5d5d 292e 6173 7479 7065  t[[col]]).astype
+00023760: 2869 6e74 290a 2020 2020 2020 2020 656c  (int).        el
+00023770: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00023780: 6b62 6420 3d20 4b42 696e 7344 6973 6372  kbd = KBinsDiscr
+00023790: 6574 697a 6572 286e 5f62 696e 733d 6269  etizer(n_bins=bi
+000237a0: 6e76 616c 7565 2c20 656e 636f 6465 3d27  nvalue, encode='
+000237b0: 6f72 6469 6e61 6c27 2c20 7374 7261 7465  ordinal', strate
+000237c0: 6779 3d73 7472 6174 6567 7929 0a20 2020  gy=strategy).   
+000237d0: 2020 2020 2020 2020 2064 665b 6e65 775f           df[new_
+000237e0: 636f 6c5d 203d 206b 6264 2e66 6974 5f74  col] = kbd.fit_t
+000237f0: 7261 6e73 666f 726d 2864 665b 5b63 6f6c  ransform(df[[col
+00023800: 5d5d 292e 6173 7479 7065 2869 6e74 290a  ]]).astype(int).
+00023810: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00023820: 6f74 2069 7369 6e73 7461 6e63 6528 7465  ot isinstance(te
+00023830: 7374 2c20 7374 7229 3a0a 2020 2020 2020  st, str):.      
+00023840: 2020 2020 2020 2020 2020 7465 7374 5b6e            test[n
+00023850: 6577 5f63 6f6c 5d20 3d20 6b62 642e 7472  ew_col] = kbd.tr
+00023860: 616e 7366 6f72 6d28 7465 7374 5b5b 636f  ansform(test[[co
+00023870: 6c5d 5d29 2e61 7374 7970 6528 696e 7429  l]]).astype(int)
+00023880: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+00023890: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+000238a0: 2061 7831 203d 2070 6c74 2e73 7562 706c   ax1 = plt.subpl
+000238b0: 6f74 286e 726f 7773 2c32 2c69 2b31 290a  ot(nrows,2,i+1).
+000238c0: 2020 2020 2020 2020 2020 2020 6178 312e              ax1.
+000238d0: 7363 6174 7465 7228 6466 5b63 6f6c 5d2c  scatter(df[col],
+000238e0: 6466 5b6e 6577 5f63 6f6c 5d29 0a20 2020  df[new_col]).   
+000238f0: 2020 2020 2020 2020 2061 7831 2e73 6574           ax1.set
+00023900: 5f74 6974 6c65 286e 6577 5f63 6f6c 290a  _title(new_col).
+00023910: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00023920: 7461 6e63 6528 7465 7374 2c20 7374 7229  tance(test, str)
+00023930: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00023940: 2064 662c 2074 6573 740a 2020 2020 656c   df, test.    el
+00023950: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
+00023960: 726e 2064 660a 2323 2323 2323 2323 2323  rn df.##########
 00023970: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023980: 2323 2323 2323 0a64 6566 2046 455f 7472  ######.def FE_tr
-00023990: 616e 7366 6f72 6d5f 6e75 6d65 7269 635f  ansform_numeric_
-000239a0: 636f 6c75 6d6e 735f 746f 5f62 696e 7328  columns_to_bins(
-000239b0: 6466 2c20 6269 6e5f 6469 6374 2c20 7665  df, bin_dict, ve
-000239c0: 7262 6f73 653d 3029 3a0a 2020 2020 2222  rbose=0):.    ""
-000239d0: 220a 2020 2020 5468 6973 2068 616e 6479  ".    This handy
-000239e0: 2066 756e 6374 696f 6e20 6469 7363 7265   function discre
-000239f0: 7469 7a65 7320 6e75 6d65 7269 6320 7661  tizes numeric va
-00023a00: 7269 6162 6c65 7320 696e 746f 2062 696e  riables into bin
-00023a10: 6e65 6420 7661 7269 6162 6c65 7320 7573  ned variables us
-00023a20: 696e 6720 6b6d 6561 6e73 2061 6c67 6f72  ing kmeans algor
-00023a30: 6974 686d 2e0a 2020 2020 596f 7520 6e65  ithm..    You ne
-00023a40: 6564 2074 6f20 7072 6f76 6964 6520 7468  ed to provide th
-00023a50: 6520 6e61 6d65 7320 6f66 2074 6865 2076  e names of the v
-00023a60: 6172 6961 626c 6573 2061 6e64 2074 6865  ariables and the
-00023a70: 206e 756d 6265 7273 206f 6620 6269 6e73   numbers of bins
-00023a80: 2066 6f72 2065 6163 6820 7661 7269 6162   for each variab
-00023a90: 6c65 2069 6e20 6120 6469 6374 696f 6e61  le in a dictiona
-00023aa0: 7279 2e0a 2020 2020 4974 2077 696c 6c20  ry..    It will 
-00023ab0: 7265 7475 726e 2074 6865 2073 616d 6520  return the same 
-00023ac0: 6461 7461 6672 616d 6520 7769 7468 206e  dataframe with n
-00023ad0: 6577 2062 696e 6e65 6420 7661 7269 6162  ew binned variab
-00023ae0: 6c65 7320 7468 6174 2069 7420 6861 7320  les that it has 
-00023af0: 6372 6561 7465 642e 0a0a 2020 2020 496e  created...    In
-00023b00: 7075 7473 3a0a 2020 2020 2d2d 2d2d 2d2d  puts:.    ------
-00023b10: 2d2d 2d2d 0a20 2020 2064 6620 3a20 7061  ----.    df : pa
-00023b20: 6e64 6173 2064 6174 6166 7261 6d65 202d  ndas dataframe -
-00023b30: 2070 6c65 6173 6520 656e 7375 7265 2069   please ensure i
-00023b40: 7420 6973 2061 2064 6174 6166 7261 6d65  t is a dataframe
-00023b50: 2e20 4e6f 2061 7272 6179 7320 706c 6561  . No arrays plea
-00023b60: 7365 2e0a 2020 2020 6269 6e5f 6469 6374  se..    bin_dict
-00023b70: 3a20 6469 6374 696f 6e61 7279 206f 6620  : dictionary of 
-00023b80: 6e61 6d65 7320 6f66 2076 6172 6961 626c  names of variabl
-00023b90: 6573 2061 6e64 2074 6865 206b 696e 6420  es and the kind 
-00023ba0: 6f66 2074 7261 6e73 666f 726d 6174 696f  of transformatio
-00023bb0: 6e20 796f 7520 7761 6e74 0a20 2020 2020  n you want.     
-00023bc0: 2020 2064 6566 6175 6c74 2069 7320 276c     default is 'l
-00023bd0: 6f67 273a 2062 7574 2079 6f75 2063 616e  og': but you can
-00023be0: 2063 686f 6f73 653a 207b 276c 6f67 272c   choose: {'log',
-00023bf0: 276c 6f67 3130 272c 2027 7371 7274 272c  'log10', 'sqrt',
-00023c00: 2027 6d61 782d 6162 7327 7d0a 0a20 2020   'max-abs'}..   
-00023c10: 204f 7574 7075 7473 3a0a 2020 2020 2d2d   Outputs:.    --
-00023c20: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 663a  --------.    df:
-00023c30: 2070 616e 6461 7320 6461 7461 6672 616d   pandas datafram
-00023c40: 6520 7769 7468 206e 6577 2076 6172 6961  e with new varia
-00023c50: 626c 6573 2077 6974 6820 6e61 6d65 7320  bles with names 
-00023c60: 7375 6368 2061 733a 2020 7661 7269 6162  such as:  variab
-00023c70: 6c65 2b27 5f64 6973 6372 6574 6527 0a20  le+'_discrete'. 
-00023c80: 2020 2022 2222 0a20 2020 2064 6620 3d20     """.    df = 
-00023c90: 636f 7079 2e64 6565 7063 6f70 7928 6466  copy.deepcopy(df
-00023ca0: 290a 2020 2020 6e75 6d5f 636f 6c73 203d  ).    num_cols =
-00023cb0: 206c 656e 2862 696e 5f64 6963 7429 0a20   len(bin_dict). 
-00023cc0: 2020 206e 726f 7773 203d 2069 6e74 2828     nrows = int((
-00023cd0: 6e75 6d5f 636f 6c73 2f32 292b 302e 3529  num_cols/2)+0.5)
-00023ce0: 0a20 2020 2069 6620 7665 7262 6f73 653a  .    if verbose:
-00023cf0: 0a20 2020 2020 2020 2066 6967 203d 2070  .        fig = p
-00023d00: 6c74 2e66 6967 7572 6528 6669 6773 697a  lt.figure(figsiz
-00023d10: 653d 2831 302c 332a 6e75 6d5f 636f 6c73  e=(10,3*num_cols
-00023d20: 2929 0a20 2020 2066 6f72 2069 2c20 2863  )).    for i, (c
-00023d30: 6f6c 2c20 6269 6e76 616c 7565 2920 696e  ol, binvalue) in
-00023d40: 2065 6e75 6d65 7261 7465 2862 696e 5f64   enumerate(bin_d
-00023d50: 6963 742e 6974 656d 7328 2929 3a0a 2020  ict.items()):.  
-00023d60: 2020 2020 2020 6e65 775f 636f 6c20 3d20        new_col = 
-00023d70: 636f 6c2b 275f 272b 6269 6e76 616c 7565  col+'_'+binvalue
-00023d80: 0a20 2020 2020 2020 2069 6620 6269 6e76  .        if binv
-00023d90: 616c 7565 203d 3d20 276c 6f67 273a 0a20  alue == 'log':. 
-00023da0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00023db0: 2827 5761 726e 696e 673a 204e 6567 6174  ('Warning: Negat
-00023dc0: 6976 6520 7661 6c75 6573 2069 6e20 2573  ive values in %s
-00023dd0: 2068 6176 6520 6265 656e 206d 6164 6520   have been made 
-00023de0: 706f 7369 7469 7665 2062 6566 6f72 6520  positive before 
-00023df0: 6c6f 6720 7472 616e 7366 6f72 6d21 2720  log transform!' 
-00023e00: 2563 6f6c 290a 2020 2020 2020 2020 2020  %col).          
-00023e10: 2020 6466 2e6c 6f63 5b64 665b 636f 6c5d    df.loc[df[col]
-00023e20: 3d3d 302c 636f 6c5d 203d 2031 652d 3135  ==0,col] = 1e-15
-00023e30: 2020 2323 2320 6d61 6b65 2069 7420 6120    ### make it a 
-00023e40: 736d 616c 6c20 6e75 6d62 6572 0a20 2020  small number.   
-00023e50: 2020 2020 2020 2020 2064 665b 6e65 775f           df[new_
-00023e60: 636f 6c5d 203d 206e 702e 6162 7328 6466  col] = np.abs(df
-00023e70: 5b63 6f6c 5d2e 7661 6c75 6573 290a 2020  [col].values).  
-00023e80: 2020 2020 2020 2020 2020 6466 5b6e 6577            df[new
-00023e90: 5f63 6f6c 5d20 3d20 6e70 2e6c 6f67 2864  _col] = np.log(d
-00023ea0: 665b 6e65 775f 636f 6c5d 292e 7661 6c75  f[new_col]).valu
-00023eb0: 6573 0a20 2020 2020 2020 2065 6c69 6620  es.        elif 
-00023ec0: 6269 6e76 616c 7565 203d 3d20 276c 6f67  binvalue == 'log
-00023ed0: 3130 273a 0a20 2020 2020 2020 2020 2020  10':.           
-00023ee0: 2070 7269 6e74 2827 5761 726e 696e 673a   print('Warning:
-00023ef0: 204e 6567 6174 6976 6520 7661 6c75 6573   Negative values
-00023f00: 2069 6e20 2573 2068 6176 6520 6265 656e   in %s have been
-00023f10: 206d 6164 6520 706f 7369 7469 7665 2062   made positive b
-00023f20: 6566 6f72 6520 6c6f 6731 3020 7472 616e  efore log10 tran
-00023f30: 7366 6f72 6d21 2720 2563 6f6c 290a 2020  sform!' %col).  
-00023f40: 2020 2020 2020 2020 2020 6466 2e6c 6f63            df.loc
-00023f50: 5b64 665b 636f 6c5d 3d3d 302c 636f 6c5d  [df[col]==0,col]
-00023f60: 203d 2031 652d 3135 2020 2323 2320 6d61   = 1e-15  ### ma
-00023f70: 6b65 2069 7420 6120 736d 616c 6c20 6e75  ke it a small nu
-00023f80: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-00023f90: 2064 665b 6e65 775f 636f 6c5d 203d 206e   df[new_col] = n
-00023fa0: 702e 6162 7328 6466 5b63 6f6c 5d2e 7661  p.abs(df[col].va
-00023fb0: 6c75 6573 290a 2020 2020 2020 2020 2020  lues).          
-00023fc0: 2020 6466 5b6e 6577 5f63 6f6c 5d20 3d20    df[new_col] = 
-00023fd0: 6e70 2e6c 6f67 3130 2864 665b 6e65 775f  np.log10(df[new_
-00023fe0: 636f 6c5d 292e 7661 6c75 6573 0a20 2020  col]).values.   
-00023ff0: 2020 2020 2065 6c69 6620 6269 6e76 616c       elif binval
-00024000: 7565 203d 3d20 2773 7172 7427 3a0a 2020  ue == 'sqrt':.  
-00024010: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00024020: 2757 6172 6e69 6e67 3a20 4e65 6761 7469  'Warning: Negati
-00024030: 7665 2076 616c 7565 7320 696e 2025 7320  ve values in %s 
-00024040: 6861 7665 2062 6565 6e20 6d61 6465 2070  have been made p
-00024050: 6f73 6974 6976 6520 6265 666f 7265 2073  ositive before s
-00024060: 7172 7420 7472 616e 7366 6f72 6d21 2720  qrt transform!' 
-00024070: 2563 6f6c 290a 2020 2020 2020 2020 2020  %col).          
-00024080: 2020 6466 5b6e 6577 5f63 6f6c 5d20 3d20    df[new_col] = 
-00024090: 6e70 2e61 6273 2864 665b 636f 6c5d 2e76  np.abs(df[col].v
-000240a0: 616c 7565 7329 2020 2323 2320 6d61 6b65  alues)  ### make
-000240b0: 2069 7420 6120 736d 616c 6c20 6e75 6d62   it a small numb
-000240c0: 6572 0a20 2020 2020 2020 2020 2020 2064  er.            d
-000240d0: 665b 6e65 775f 636f 6c5d 203d 206e 702e  f[new_col] = np.
-000240e0: 7371 7274 2864 665b 6e65 775f 636f 6c5d  sqrt(df[new_col]
-000240f0: 292e 7661 6c75 6573 0a20 2020 2020 2020  ).values.       
-00024100: 2065 6c69 6620 6269 6e76 616c 7565 203d   elif binvalue =
-00024110: 3d20 276d 6178 2d61 6273 273a 0a20 2020  = 'max-abs':.   
-00024120: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00024130: 5761 726e 696e 673a 204e 6567 6174 6976  Warning: Negativ
-00024140: 6520 7661 6c75 6573 2069 6e20 2573 2068  e values in %s h
-00024150: 6176 6520 6265 656e 206d 6164 6520 706f  ave been made po
-00024160: 7369 7469 7665 2062 6566 6f72 6520 6d61  sitive before ma
-00024170: 782d 6162 7320 7472 616e 7366 6f72 6d21  x-abs transform!
-00024180: 2720 2563 6f6c 290a 2020 2020 2020 2020  ' %col).        
-00024190: 2020 2020 636f 6c5f 6d61 7820 3d20 6d61      col_max = ma
-000241a0: 7828 6e70 2e61 6273 2864 665b 636f 6c5d  x(np.abs(df[col]
-000241b0: 2e76 616c 7565 7329 290a 2020 2020 2020  .values)).      
-000241c0: 2020 2020 2020 6966 2063 6f6c 5f6d 6178        if col_max
-000241d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-000241e0: 2020 2020 2020 2063 6f6c 5f6d 6178 203d         col_max =
-000241f0: 2031 0a20 2020 2020 2020 2020 2020 2064   1.            d
-00024200: 665b 6e65 775f 636f 6c5d 203d 206e 702e  f[new_col] = np.
-00024210: 6162 7328 6466 5b63 6f6c 5d2e 7661 6c75  abs(df[col].valu
-00024220: 6573 292f 636f 6c5f 6d61 780a 2020 2020  es)/col_max.    
-00024230: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00024240: 2020 2020 2020 7072 696e 7428 2757 6172        print('War
-00024250: 6e69 6e67 3a20 4e65 6761 7469 7665 2076  ning: Negative v
-00024260: 616c 7565 7320 696e 2025 7320 6861 7665  alues in %s have
-00024270: 2062 6565 6e20 6d61 6465 2070 6f73 6974   been made posit
-00024280: 6976 6520 6265 666f 7265 206c 6f67 2074  ive before log t
-00024290: 7261 6e73 666f 726d 2127 2025 636f 6c29  ransform!' %col)
-000242a0: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
-000242b0: 6c6f 635b 6466 5b63 6f6c 5d3d 3d30 2c63  loc[df[col]==0,c
-000242c0: 6f6c 5d20 3d20 3165 2d31 3520 2023 2323  ol] = 1e-15  ###
-000242d0: 206d 616b 6520 6974 2061 2073 6d61 6c6c   make it a small
-000242e0: 206e 756d 6265 720a 2020 2020 2020 2020   number.        
-000242f0: 2020 2020 6466 5b6e 6577 5f63 6f6c 5d20      df[new_col] 
-00024300: 3d20 6e70 2e61 6273 2864 665b 636f 6c5d  = np.abs(df[col]
-00024310: 2e76 616c 7565 7329 0a20 2020 2020 2020  .values).       
-00024320: 2020 2020 2064 665b 6e65 775f 636f 6c5d       df[new_col]
-00024330: 203d 206e 702e 6c6f 6728 6466 5b6e 6577   = np.log(df[new
-00024340: 5f63 6f6c 5d29 2e76 616c 7565 730a 2020  _col]).values.  
-00024350: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-00024360: 3a0a 2020 2020 2020 2020 2020 2020 6178  :.            ax
-00024370: 3120 3d20 706c 742e 7375 6270 6c6f 7428  1 = plt.subplot(
-00024380: 6e72 6f77 732c 322c 692b 3129 0a20 2020  nrows,2,i+1).   
-00024390: 2020 2020 2020 2020 2064 665b 636f 6c5d           df[col]
-000243a0: 2e70 6c6f 742e 6b64 6528 6178 3d61 7831  .plot.kde(ax=ax1
-000243b0: 2c20 6c61 6265 6c3d 636f 6c2c 616c 7068  , label=col,alph
-000243c0: 613d 302e 352c 636f 6c6f 723d 2772 2729  a=0.5,color='r')
-000243d0: 0a20 2020 2020 2020 2020 2020 2061 7832  .            ax2
-000243e0: 203d 2061 7831 2e74 7769 6e79 2829 0a20   = ax1.twiny(). 
-000243f0: 2020 2020 2020 2020 2020 2064 665b 6e65             df[ne
-00024400: 775f 636f 6c5d 2e70 6c6f 742e 6b64 6528  w_col].plot.kde(
-00024410: 6178 3d61 7832 2c6c 6162 656c 3d6e 6577  ax=ax2,label=new
-00024420: 5f63 6f6c 2c61 6c70 6861 3d30 2e35 2c63  _col,alpha=0.5,c
-00024430: 6f6c 6f72 3d27 6227 290a 2020 2020 2020  olor='b').      
-00024440: 2020 2020 2020 706c 742e 6c65 6765 6e64        plt.legend
-00024450: 2829 3b0a 2020 2020 7265 7475 726e 2064  ();.    return d
-00024460: 660a 2323 2323 2323 2323 2323 2323 2323  f.##############
-00024470: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00024490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023980: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023990: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000239a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000239b0: 2323 2323 2323 2323 0a64 6566 2046 455f  ########.def FE_
+000239c0: 7472 616e 7366 6f72 6d5f 6e75 6d65 7269  transform_numeri
+000239d0: 635f 636f 6c75 6d6e 735f 746f 5f62 696e  c_columns_to_bin
+000239e0: 7328 6466 2c20 6269 6e5f 6469 6374 2c20  s(df, bin_dict, 
+000239f0: 7665 7262 6f73 653d 3029 3a0a 2020 2020  verbose=0):.    
+00023a00: 2222 220a 2020 2020 5468 6973 2068 616e  """.    This han
+00023a10: 6479 2066 756e 6374 696f 6e20 6469 7363  dy function disc
+00023a20: 7265 7469 7a65 7320 6e75 6d65 7269 6320  retizes numeric 
+00023a30: 7661 7269 6162 6c65 7320 696e 746f 2062  variables into b
+00023a40: 696e 6e65 6420 7661 7269 6162 6c65 7320  inned variables 
+00023a50: 7573 696e 6720 6b6d 6561 6e73 2061 6c67  using kmeans alg
+00023a60: 6f72 6974 686d 2e0a 2020 2020 596f 7520  orithm..    You 
+00023a70: 6e65 6564 2074 6f20 7072 6f76 6964 6520  need to provide 
+00023a80: 7468 6520 6e61 6d65 7320 6f66 2074 6865  the names of the
+00023a90: 2076 6172 6961 626c 6573 2061 6e64 2074   variables and t
+00023aa0: 6865 206e 756d 6265 7273 206f 6620 6269  he numbers of bi
+00023ab0: 6e73 2066 6f72 2065 6163 6820 7661 7269  ns for each vari
+00023ac0: 6162 6c65 2069 6e20 6120 6469 6374 696f  able in a dictio
+00023ad0: 6e61 7279 2e0a 2020 2020 4974 2077 696c  nary..    It wil
+00023ae0: 6c20 7265 7475 726e 2074 6865 2073 616d  l return the sam
+00023af0: 6520 6461 7461 6672 616d 6520 7769 7468  e dataframe with
+00023b00: 206e 6577 2062 696e 6e65 6420 7661 7269   new binned vari
+00023b10: 6162 6c65 7320 7468 6174 2069 7420 6861  ables that it ha
+00023b20: 7320 6372 6561 7465 642e 0a0a 2020 2020  s created...    
+00023b30: 496e 7075 7473 3a0a 2020 2020 2d2d 2d2d  Inputs:.    ----
+00023b40: 2d2d 2d2d 2d2d 0a20 2020 2064 6620 3a20  ------.    df : 
+00023b50: 7061 6e64 6173 2064 6174 6166 7261 6d65  pandas dataframe
+00023b60: 202d 2070 6c65 6173 6520 656e 7375 7265   - please ensure
+00023b70: 2069 7420 6973 2061 2064 6174 6166 7261   it is a datafra
+00023b80: 6d65 2e20 4e6f 2061 7272 6179 7320 706c  me. No arrays pl
+00023b90: 6561 7365 2e0a 2020 2020 6269 6e5f 6469  ease..    bin_di
+00023ba0: 6374 3a20 6469 6374 696f 6e61 7279 206f  ct: dictionary o
+00023bb0: 6620 6e61 6d65 7320 6f66 2076 6172 6961  f names of varia
+00023bc0: 626c 6573 2061 6e64 2074 6865 206b 696e  bles and the kin
+00023bd0: 6420 6f66 2074 7261 6e73 666f 726d 6174  d of transformat
+00023be0: 696f 6e20 796f 7520 7761 6e74 0a20 2020  ion you want.   
+00023bf0: 2020 2020 2064 6566 6175 6c74 2069 7320       default is 
+00023c00: 276c 6f67 273a 2062 7574 2079 6f75 2063  'log': but you c
+00023c10: 616e 2063 686f 6f73 653a 207b 276c 6f67  an choose: {'log
+00023c20: 272c 276c 6f67 3130 272c 2027 7371 7274  ','log10', 'sqrt
+00023c30: 272c 2027 6d61 782d 6162 7327 7d0a 0a20  ', 'max-abs'}.. 
+00023c40: 2020 204f 7574 7075 7473 3a0a 2020 2020     Outputs:.    
+00023c50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+00023c60: 663a 2070 616e 6461 7320 6461 7461 6672  f: pandas datafr
+00023c70: 616d 6520 7769 7468 206e 6577 2076 6172  ame with new var
+00023c80: 6961 626c 6573 2077 6974 6820 6e61 6d65  iables with name
+00023c90: 7320 7375 6368 2061 733a 2020 7661 7269  s such as:  vari
+00023ca0: 6162 6c65 2b27 5f64 6973 6372 6574 6527  able+'_discrete'
+00023cb0: 0a20 2020 2022 2222 0a20 2020 2064 6620  .    """.    df 
+00023cc0: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
+00023cd0: 6466 290a 2020 2020 6e75 6d5f 636f 6c73  df).    num_cols
+00023ce0: 203d 206c 656e 2862 696e 5f64 6963 7429   = len(bin_dict)
+00023cf0: 0a20 2020 206e 726f 7773 203d 2069 6e74  .    nrows = int
+00023d00: 2828 6e75 6d5f 636f 6c73 2f32 292b 302e  ((num_cols/2)+0.
+00023d10: 3529 0a20 2020 2069 6620 7665 7262 6f73  5).    if verbos
+00023d20: 653a 0a20 2020 2020 2020 2066 6967 203d  e:.        fig =
+00023d30: 2070 6c74 2e66 6967 7572 6528 6669 6773   plt.figure(figs
+00023d40: 697a 653d 2831 302c 332a 6e75 6d5f 636f  ize=(10,3*num_co
+00023d50: 6c73 2929 0a20 2020 2066 6f72 2069 2c20  ls)).    for i, 
+00023d60: 2863 6f6c 2c20 6269 6e76 616c 7565 2920  (col, binvalue) 
+00023d70: 696e 2065 6e75 6d65 7261 7465 2862 696e  in enumerate(bin
+00023d80: 5f64 6963 742e 6974 656d 7328 2929 3a0a  _dict.items()):.
+00023d90: 2020 2020 2020 2020 6e65 775f 636f 6c20          new_col 
+00023da0: 3d20 636f 6c2b 275f 272b 6269 6e76 616c  = col+'_'+binval
+00023db0: 7565 0a20 2020 2020 2020 2069 6620 6269  ue.        if bi
+00023dc0: 6e76 616c 7565 203d 3d20 276c 6f67 273a  nvalue == 'log':
+00023dd0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00023de0: 6e74 2827 5761 726e 696e 673a 204e 6567  nt('Warning: Neg
+00023df0: 6174 6976 6520 7661 6c75 6573 2069 6e20  ative values in 
+00023e00: 2573 2068 6176 6520 6265 656e 206d 6164  %s have been mad
+00023e10: 6520 706f 7369 7469 7665 2062 6566 6f72  e positive befor
+00023e20: 6520 6c6f 6720 7472 616e 7366 6f72 6d21  e log transform!
+00023e30: 2720 2563 6f6c 290a 2020 2020 2020 2020  ' %col).        
+00023e40: 2020 2020 6466 2e6c 6f63 5b64 665b 636f      df.loc[df[co
+00023e50: 6c5d 3d3d 302c 636f 6c5d 203d 2031 652d  l]==0,col] = 1e-
+00023e60: 3135 2020 2323 2320 6d61 6b65 2069 7420  15  ### make it 
+00023e70: 6120 736d 616c 6c20 6e75 6d62 6572 0a20  a small number. 
+00023e80: 2020 2020 2020 2020 2020 2064 665b 6e65             df[ne
+00023e90: 775f 636f 6c5d 203d 206e 702e 6162 7328  w_col] = np.abs(
+00023ea0: 6466 5b63 6f6c 5d2e 7661 6c75 6573 290a  df[col].values).
+00023eb0: 2020 2020 2020 2020 2020 2020 6466 5b6e              df[n
+00023ec0: 6577 5f63 6f6c 5d20 3d20 6e70 2e6c 6f67  ew_col] = np.log
+00023ed0: 2864 665b 6e65 775f 636f 6c5d 292e 7661  (df[new_col]).va
+00023ee0: 6c75 6573 0a20 2020 2020 2020 2065 6c69  lues.        eli
+00023ef0: 6620 6269 6e76 616c 7565 203d 3d20 276c  f binvalue == 'l
+00023f00: 6f67 3130 273a 0a20 2020 2020 2020 2020  og10':.         
+00023f10: 2020 2070 7269 6e74 2827 5761 726e 696e     print('Warnin
+00023f20: 673a 204e 6567 6174 6976 6520 7661 6c75  g: Negative valu
+00023f30: 6573 2069 6e20 2573 2068 6176 6520 6265  es in %s have be
+00023f40: 656e 206d 6164 6520 706f 7369 7469 7665  en made positive
+00023f50: 2062 6566 6f72 6520 6c6f 6731 3020 7472   before log10 tr
+00023f60: 616e 7366 6f72 6d21 2720 2563 6f6c 290a  ansform!' %col).
+00023f70: 2020 2020 2020 2020 2020 2020 6466 2e6c              df.l
+00023f80: 6f63 5b64 665b 636f 6c5d 3d3d 302c 636f  oc[df[col]==0,co
+00023f90: 6c5d 203d 2031 652d 3135 2020 2323 2320  l] = 1e-15  ### 
+00023fa0: 6d61 6b65 2069 7420 6120 736d 616c 6c20  make it a small 
+00023fb0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
+00023fc0: 2020 2064 665b 6e65 775f 636f 6c5d 203d     df[new_col] =
+00023fd0: 206e 702e 6162 7328 6466 5b63 6f6c 5d2e   np.abs(df[col].
+00023fe0: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
+00023ff0: 2020 2020 6466 5b6e 6577 5f63 6f6c 5d20      df[new_col] 
+00024000: 3d20 6e70 2e6c 6f67 3130 2864 665b 6e65  = np.log10(df[ne
+00024010: 775f 636f 6c5d 292e 7661 6c75 6573 0a20  w_col]).values. 
+00024020: 2020 2020 2020 2065 6c69 6620 6269 6e76         elif binv
+00024030: 616c 7565 203d 3d20 2773 7172 7427 3a0a  alue == 'sqrt':.
+00024040: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00024050: 7428 2757 6172 6e69 6e67 3a20 4e65 6761  t('Warning: Nega
+00024060: 7469 7665 2076 616c 7565 7320 696e 2025  tive values in %
+00024070: 7320 6861 7665 2062 6565 6e20 6d61 6465  s have been made
+00024080: 2070 6f73 6974 6976 6520 6265 666f 7265   positive before
+00024090: 2073 7172 7420 7472 616e 7366 6f72 6d21   sqrt transform!
+000240a0: 2720 2563 6f6c 290a 2020 2020 2020 2020  ' %col).        
+000240b0: 2020 2020 6466 5b6e 6577 5f63 6f6c 5d20      df[new_col] 
+000240c0: 3d20 6e70 2e61 6273 2864 665b 636f 6c5d  = np.abs(df[col]
+000240d0: 2e76 616c 7565 7329 2020 2323 2320 6d61  .values)  ### ma
+000240e0: 6b65 2069 7420 6120 736d 616c 6c20 6e75  ke it a small nu
+000240f0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+00024100: 2064 665b 6e65 775f 636f 6c5d 203d 206e   df[new_col] = n
+00024110: 702e 7371 7274 2864 665b 6e65 775f 636f  p.sqrt(df[new_co
+00024120: 6c5d 292e 7661 6c75 6573 0a20 2020 2020  l]).values.     
+00024130: 2020 2065 6c69 6620 6269 6e76 616c 7565     elif binvalue
+00024140: 203d 3d20 276d 6178 2d61 6273 273a 0a20   == 'max-abs':. 
+00024150: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00024160: 2827 5761 726e 696e 673a 204e 6567 6174  ('Warning: Negat
+00024170: 6976 6520 7661 6c75 6573 2069 6e20 2573  ive values in %s
+00024180: 2068 6176 6520 6265 656e 206d 6164 6520   have been made 
+00024190: 706f 7369 7469 7665 2062 6566 6f72 6520  positive before 
+000241a0: 6d61 782d 6162 7320 7472 616e 7366 6f72  max-abs transfor
+000241b0: 6d21 2720 2563 6f6c 290a 2020 2020 2020  m!' %col).      
+000241c0: 2020 2020 2020 636f 6c5f 6d61 7820 3d20        col_max = 
+000241d0: 6d61 7828 6e70 2e61 6273 2864 665b 636f  max(np.abs(df[co
+000241e0: 6c5d 2e76 616c 7565 7329 290a 2020 2020  l].values)).    
+000241f0: 2020 2020 2020 2020 6966 2063 6f6c 5f6d          if col_m
+00024200: 6178 203d 3d20 303a 0a20 2020 2020 2020  ax == 0:.       
+00024210: 2020 2020 2020 2020 2063 6f6c 5f6d 6178           col_max
+00024220: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00024230: 2064 665b 6e65 775f 636f 6c5d 203d 206e   df[new_col] = n
+00024240: 702e 6162 7328 6466 5b63 6f6c 5d2e 7661  p.abs(df[col].va
+00024250: 6c75 6573 292f 636f 6c5f 6d61 780a 2020  lues)/col_max.  
+00024260: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00024270: 2020 2020 2020 2020 7072 696e 7428 2757          print('W
+00024280: 6172 6e69 6e67 3a20 4e65 6761 7469 7665  arning: Negative
+00024290: 2076 616c 7565 7320 696e 2025 7320 6861   values in %s ha
+000242a0: 7665 2062 6565 6e20 6d61 6465 2070 6f73  ve been made pos
+000242b0: 6974 6976 6520 6265 666f 7265 206c 6f67  itive before log
+000242c0: 2074 7261 6e73 666f 726d 2127 2025 636f   transform!' %co
+000242d0: 6c29 0a20 2020 2020 2020 2020 2020 2064  l).            d
+000242e0: 662e 6c6f 635b 6466 5b63 6f6c 5d3d 3d30  f.loc[df[col]==0
+000242f0: 2c63 6f6c 5d20 3d20 3165 2d31 3520 2023  ,col] = 1e-15  #
+00024300: 2323 206d 616b 6520 6974 2061 2073 6d61  ## make it a sma
+00024310: 6c6c 206e 756d 6265 720a 2020 2020 2020  ll number.      
+00024320: 2020 2020 2020 6466 5b6e 6577 5f63 6f6c        df[new_col
+00024330: 5d20 3d20 6e70 2e61 6273 2864 665b 636f  ] = np.abs(df[co
+00024340: 6c5d 2e76 616c 7565 7329 0a20 2020 2020  l].values).     
+00024350: 2020 2020 2020 2064 665b 6e65 775f 636f         df[new_co
+00024360: 6c5d 203d 206e 702e 6c6f 6728 6466 5b6e  l] = np.log(df[n
+00024370: 6577 5f63 6f6c 5d29 2e76 616c 7565 730a  ew_col]).values.
+00024380: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+00024390: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000243a0: 6178 3120 3d20 706c 742e 7375 6270 6c6f  ax1 = plt.subplo
+000243b0: 7428 6e72 6f77 732c 322c 692b 3129 0a20  t(nrows,2,i+1). 
+000243c0: 2020 2020 2020 2020 2020 2064 665b 636f             df[co
+000243d0: 6c5d 2e70 6c6f 742e 6b64 6528 6178 3d61  l].plot.kde(ax=a
+000243e0: 7831 2c20 6c61 6265 6c3d 636f 6c2c 616c  x1, label=col,al
+000243f0: 7068 613d 302e 352c 636f 6c6f 723d 2772  pha=0.5,color='r
+00024400: 2729 0a20 2020 2020 2020 2020 2020 2061  ').            a
+00024410: 7832 203d 2061 7831 2e74 7769 6e79 2829  x2 = ax1.twiny()
+00024420: 0a20 2020 2020 2020 2020 2020 2064 665b  .            df[
+00024430: 6e65 775f 636f 6c5d 2e70 6c6f 742e 6b64  new_col].plot.kd
+00024440: 6528 6178 3d61 7832 2c6c 6162 656c 3d6e  e(ax=ax2,label=n
+00024450: 6577 5f63 6f6c 2c61 6c70 6861 3d30 2e35  ew_col,alpha=0.5
+00024460: 2c63 6f6c 6f72 3d27 6227 290a 2020 2020  ,color='b').    
+00024470: 2020 2020 2020 2020 706c 742e 6c65 6765          plt.lege
+00024480: 6e64 2829 3b0a 2020 2020 7265 7475 726e  nd();.    return
+00024490: 2064 660a 2323 2323 2323 2323 2323 2323   df.############
 000244a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000244b0: 2323 230a 6672 6f6d 2069 7465 7274 6f6f  ###.from itertoo
-000244c0: 6c73 2069 6d70 6f72 7420 6379 636c 652c  ls import cycle,
-000244d0: 2063 6f6d 6269 6e61 7469 6f6e 730a 6465   combinations.de
-000244e0: 6620 4645 5f63 7265 6174 655f 696e 7465  f FE_create_inte
-000244f0: 7261 6374 696f 6e5f 7661 7273 2864 662c  raction_vars(df,
-00024500: 2069 6e74 786e 5f76 6172 7329 3a0a 2020   intxn_vars):.  
-00024510: 2020 2222 220a 2020 2020 5468 6973 2068    """.    This h
-00024520: 616e 6479 2066 756e 6374 696f 6e20 6372  andy function cr
-00024530: 6561 7465 7320 696e 7465 7261 6374 696f  eates interactio
-00024540: 6e20 7661 7269 6162 6c65 7320 616d 6f6e  n variables amon
-00024550: 6720 7061 6972 7320 6f66 206e 756d 6572  g pairs of numer
-00024560: 6963 2076 6172 7320 796f 7520 7365 6e64  ic vars you send
-00024570: 2069 6e2e 0a20 2020 2059 6f75 7220 696e   in..    Your in
-00024580: 7075 7420 6d75 7374 2062 6520 6120 6461  put must be a da
-00024590: 7461 6672 616d 6520 616e 6420 6120 6c69  taframe and a li
-000245a0: 7374 206f 6620 7475 706c 6573 2e20 4561  st of tuples. Ea
-000245b0: 6368 2074 7570 6c65 206d 7573 7420 636f  ch tuple must co
-000245c0: 6e74 6169 6e20 6120 7061 6972 206f 6620  ntain a pair of 
-000245d0: 7661 7269 6162 6c65 732e 0a20 2020 2041  variables..    A
-000245e0: 6c6c 2076 6172 6961 626c 6573 206d 7573  ll variables mus
-000245f0: 7420 6265 206e 756d 6572 6963 2e20 446f  t be numeric. Do
-00024600: 7562 6c65 2063 6865 636b 2079 6f75 7220  uble check your 
-00024610: 696e 7075 7420 6265 666f 7265 2073 656e  input before sen
-00024620: 6469 6e67 2074 6865 6d20 696e 2e0a 2020  ding them in..  
-00024630: 2020 2222 220a 2020 2020 6966 2074 7970    """.    if typ
-00024640: 6528 6466 2920 3d3d 2064 6173 6b2e 6461  e(df) == dask.da
-00024650: 7461 6672 616d 652e 636f 7265 2e44 6174  taframe.core.Dat
-00024660: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
-00024670: 2323 2073 6b69 7020 6966 2069 7420 6973  ## skip if it is
-00024680: 2061 2064 6173 6b20 6461 7461 6672 616d   a dask datafram
-00024690: 6520 2323 2323 0a20 2020 2020 2020 2070  e ####.        p
-000246a0: 6173 730a 2020 2020 656c 7365 3a0a 2020  ass.    else:.  
-000246b0: 2020 2020 2020 6466 203d 2064 662e 636f        df = df.co
-000246c0: 7079 2864 6565 703d 5472 7565 290a 2020  py(deep=True).  
-000246d0: 2020 636f 6d62 6f73 203d 2063 6f6d 6269    combos = combi
-000246e0: 6e61 7469 6f6e 7328 696e 7478 6e5f 7661  nations(intxn_va
-000246f0: 7273 2c20 3229 0a20 2020 2023 2323 2049  rs, 2).    ### I
-00024700: 2068 6176 6520 7465 7374 6564 2074 6869   have tested thi
-00024710: 7320 666f 7220 626f 7468 2063 6174 6567  s for both categ
-00024720: 6f72 7920 616e 6420 6f62 6a65 6374 2064  ory and object d
-00024730: 7479 7065 7320 736f 2064 6f6e 2774 2077  types so don't w
-00024740: 6f72 7279 2023 2323 0a20 2020 2066 6f72  orry ###.    for
-00024750: 2028 6561 6368 5f69 6e74 786e 312c 6561   (each_intxn1,ea
-00024760: 6368 5f69 6e74 786e 3229 2020 696e 2063  ch_intxn2)  in c
-00024770: 6f6d 626f 733a 0a20 2020 2020 2020 206e  ombos:.        n
-00024780: 6577 5f63 6f6c 203d 2065 6163 685f 696e  ew_col = each_in
-00024790: 7478 6e31 202b 2027 5f78 5f27 202b 2065  txn1 + '_x_' + e
-000247a0: 6163 685f 696e 7478 6e32 0a20 2020 2020  ach_intxn2.     
-000247b0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000247c0: 2020 2020 6466 5b6e 6577 5f63 6f6c 5d20      df[new_col] 
-000247d0: 3d20 6466 5b65 6163 685f 696e 7478 6e31  = df[each_intxn1
-000247e0: 5d2e 6173 7479 7065 2873 7472 2920 2b20  ].astype(str) + 
-000247f0: 2720 2720 2b20 6466 5b65 6163 685f 696e  ' ' + df[each_in
-00024800: 7478 6e32 5d2e 6173 7479 7065 2873 7472  txn2].astype(str
-00024810: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00024820: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00024830: 6e74 696e 7565 0a20 2020 2023 2323 2074  ntinue.    ### t
-00024840: 6869 7320 7769 6c6c 2072 6574 7572 6e20  his will return 
-00024850: 6578 7472 6120 6665 6174 7572 6573 2067  extra features g
-00024860: 656e 6572 6174 6564 2062 7920 696e 7465  enerated by inte
-00024870: 7261 6374 696f 6e73 2023 2323 2320 2020  ractions ####   
-00024880: 200a 2020 2020 7265 7475 726e 2064 660a   .    return df.
-00024890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000248a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000248b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000248c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000244b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000244c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000244d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000244e0: 2323 2323 230a 6672 6f6d 2069 7465 7274  #####.from itert
+000244f0: 6f6f 6c73 2069 6d70 6f72 7420 6379 636c  ools import cycl
+00024500: 652c 2063 6f6d 6269 6e61 7469 6f6e 730a  e, combinations.
+00024510: 6465 6620 4645 5f63 7265 6174 655f 696e  def FE_create_in
+00024520: 7465 7261 6374 696f 6e5f 7661 7273 2864  teraction_vars(d
+00024530: 662c 2069 6e74 786e 5f76 6172 7329 3a0a  f, intxn_vars):.
+00024540: 2020 2020 2222 220a 2020 2020 5468 6973      """.    This
+00024550: 2068 616e 6479 2066 756e 6374 696f 6e20   handy function 
+00024560: 6372 6561 7465 7320 696e 7465 7261 6374  creates interact
+00024570: 696f 6e20 7661 7269 6162 6c65 7320 616d  ion variables am
+00024580: 6f6e 6720 7061 6972 7320 6f66 206e 756d  ong pairs of num
+00024590: 6572 6963 2076 6172 7320 796f 7520 7365  eric vars you se
+000245a0: 6e64 2069 6e2e 0a20 2020 2059 6f75 7220  nd in..    Your 
+000245b0: 696e 7075 7420 6d75 7374 2062 6520 6120  input must be a 
+000245c0: 6461 7461 6672 616d 6520 616e 6420 6120  dataframe and a 
+000245d0: 6c69 7374 206f 6620 7475 706c 6573 2e20  list of tuples. 
+000245e0: 4561 6368 2074 7570 6c65 206d 7573 7420  Each tuple must 
+000245f0: 636f 6e74 6169 6e20 6120 7061 6972 206f  contain a pair o
+00024600: 6620 7661 7269 6162 6c65 732e 0a20 2020  f variables..   
+00024610: 2041 6c6c 2076 6172 6961 626c 6573 206d   All variables m
+00024620: 7573 7420 6265 206e 756d 6572 6963 2e20  ust be numeric. 
+00024630: 446f 7562 6c65 2063 6865 636b 2079 6f75  Double check you
+00024640: 7220 696e 7075 7420 6265 666f 7265 2073  r input before s
+00024650: 656e 6469 6e67 2074 6865 6d20 696e 2e0a  ending them in..
+00024660: 2020 2020 2222 220a 2020 2020 6966 2074      """.    if t
+00024670: 7970 6528 6466 2920 3d3d 2064 6173 6b2e  ype(df) == dask.
+00024680: 6461 7461 6672 616d 652e 636f 7265 2e44  dataframe.core.D
+00024690: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
+000246a0: 2020 2323 2073 6b69 7020 6966 2069 7420    ## skip if it 
+000246b0: 6973 2061 2064 6173 6b20 6461 7461 6672  is a dask datafr
+000246c0: 616d 6520 2323 2323 0a20 2020 2020 2020  ame ####.       
+000246d0: 2070 6173 730a 2020 2020 656c 7365 3a0a   pass.    else:.
+000246e0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+000246f0: 636f 7079 2864 6565 703d 5472 7565 290a  copy(deep=True).
+00024700: 2020 2020 636f 6d62 6f73 203d 2063 6f6d      combos = com
+00024710: 6269 6e61 7469 6f6e 7328 696e 7478 6e5f  binations(intxn_
+00024720: 7661 7273 2c20 3229 0a20 2020 2023 2323  vars, 2).    ###
+00024730: 2049 2068 6176 6520 7465 7374 6564 2074   I have tested t
+00024740: 6869 7320 666f 7220 626f 7468 2063 6174  his for both cat
+00024750: 6567 6f72 7920 616e 6420 6f62 6a65 6374  egory and object
+00024760: 2064 7479 7065 7320 736f 2064 6f6e 2774   dtypes so don't
+00024770: 2077 6f72 7279 2023 2323 0a20 2020 2066   worry ###.    f
+00024780: 6f72 2028 6561 6368 5f69 6e74 786e 312c  or (each_intxn1,
+00024790: 6561 6368 5f69 6e74 786e 3229 2020 696e  each_intxn2)  in
+000247a0: 2063 6f6d 626f 733a 0a20 2020 2020 2020   combos:.       
+000247b0: 206e 6577 5f63 6f6c 203d 2065 6163 685f   new_col = each_
+000247c0: 696e 7478 6e31 202b 2027 5f78 5f27 202b  intxn1 + '_x_' +
+000247d0: 2065 6163 685f 696e 7478 6e32 0a20 2020   each_intxn2.   
+000247e0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000247f0: 2020 2020 2020 6466 5b6e 6577 5f63 6f6c        df[new_col
+00024800: 5d20 3d20 6466 5b65 6163 685f 696e 7478  ] = df[each_intx
+00024810: 6e31 5d2e 6173 7479 7065 2873 7472 2920  n1].astype(str) 
+00024820: 2b20 2720 2720 2b20 6466 5b65 6163 685f  + ' ' + df[each_
+00024830: 696e 7478 6e32 5d2e 6173 7479 7065 2873  intxn2].astype(s
+00024840: 7472 290a 2020 2020 2020 2020 6578 6365  tr).        exce
+00024850: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00024860: 636f 6e74 696e 7565 0a20 2020 2023 2323  continue.    ###
+00024870: 2074 6869 7320 7769 6c6c 2072 6574 7572   this will retur
+00024880: 6e20 6578 7472 6120 6665 6174 7572 6573  n extra features
+00024890: 2067 656e 6572 6174 6564 2062 7920 696e   generated by in
+000248a0: 7465 7261 6374 696f 6e73 2023 2323 2320  teractions #### 
+000248b0: 2020 200a 2020 2020 7265 7475 726e 2064     .    return d
+000248c0: 660a 2323 2323 2323 2323 2323 2323 2323  f.##############
 000248d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000248e0: 2323 0a69 6d70 6f72 7420 6d61 7470 6c6f  ##.import matplo
-000248f0: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
-00024900: 6c74 0a64 6566 2045 4441 5f62 696e 6e69  lt.def EDA_binni
-00024910: 6e67 5f6e 756d 6572 6963 5f63 6f6c 756d  ng_numeric_colum
-00024920: 6e5f 6469 7370 6c61 7969 6e67 5f62 696e  n_displaying_bin
-00024930: 7328 6466 742c 2074 6172 6765 742c 2062  s(dft, target, b
-00024940: 696e 733d 342c 2074 6573 743d 2222 293a  ins=4, test=""):
-00024950: 0a20 2020 2022 2222 0a20 2020 2054 6869  .    """.    Thi
-00024960: 7320 7370 6c69 7473 2074 6865 2064 6174  s splits the dat
-00024970: 6120 636f 6c75 6d6e 2069 6e74 6f20 7468  a column into th
-00024980: 6520 6e75 6d62 6572 206f 6620 6269 6e73  e number of bins
-00024990: 2073 7065 6369 6669 6564 2061 6e64 2072   specified and r
-000249a0: 6574 7572 6e73 206c 6162 656c 732c 2062  eturns labels, b
-000249b0: 696e 732c 2061 6e64 2064 6174 6166 7261  ins, and datafra
-000249c0: 6d65 2e0a 2020 2020 4f75 7470 7574 733a  me..    Outputs:
-000249d0: 0a20 2020 2020 2020 6c61 6265 6c73 203d  .       labels =
-000249e0: 2074 6865 206e 616d 6573 206f 6620 7468   the names of th
-000249f0: 6520 6269 6e73 0a20 2020 2020 2020 6564  e bins.       ed
-00024a00: 6765 7320 3d20 7468 6520 6564 6765 7320  ges = the edges 
-00024a10: 6f66 2074 6865 2062 696e 730a 2020 2020  of the bins.    
-00024a20: 2020 2064 6674 203d 2074 6865 2064 6174     dft = the dat
-00024a30: 6166 7261 6d65 2077 6974 6820 616e 2061  aframe with an a
-00024a40: 6464 6564 2063 6f6c 756d 6e20 6361 6c6c  dded column call
-00024a50: 6564 2022 6269 6e6e 6564 5f22 2b6e 616d  ed "binned_"+nam
-00024a60: 6520 6f66 2074 6865 2063 6f6c 756d 6e20  e of the column 
-00024a70: 796f 7520 7365 6e74 2069 6e0a 2020 2020  you sent in.    
-00024a80: 2222 220a 2020 2020 6466 7420 3d20 636f  """.    dft = co
-00024a90: 7079 2e64 6565 7063 6f70 7928 6466 7429  py.deepcopy(dft)
-00024aa0: 0a20 2020 205f 2c20 6564 6765 7320 3d20  .    _, edges = 
-00024ab0: 7064 2e71 6375 7428 6466 745b 7461 7267  pd.qcut(dft[targ
-00024ac0: 6574 5d2e 6472 6f70 6e61 2861 7869 733d  et].dropna(axis=
-00024ad0: 3029 2c71 3d62 696e 732c 2072 6574 6269  0),q=bins, retbi
-00024ae0: 6e73 3d54 7275 652c 2064 7570 6c69 6361  ns=True, duplica
-00024af0: 7465 733d 2764 726f 7027 290a 2020 2020  tes='drop').    
-00024b00: 2323 2320 6e6f 7720 7765 2063 7265 6174  ### now we creat
-00024b10: 6520 6172 7469 6669 6369 616c 206c 6162  e artificial lab
-00024b20: 656c 7320 746f 206d 6174 6368 2074 6865  els to match the
-00024b30: 2062 696e 7320 6564 6765 7320 2323 2323   bins edges ####
-00024b40: 0a20 2020 206c 7320 3d20 5b5d 0a20 2020  .    ls = [].   
-00024b50: 2066 6f72 2069 2c20 7820 696e 2065 6e75   for i, x in enu
-00024b60: 6d65 7261 7465 2865 6467 6573 293a 0a20  merate(edges):. 
-00024b70: 2020 2020 2020 2023 7072 696e 7428 2769         #print('i
-00024b80: 203d 2025 732c 206e 6578 7420 6920 3d20   = %s, next i = 
-00024b90: 2573 2720 2528 692c 692b 3129 290a 2020  %s' %(i,i+1)).  
-00024ba0: 2020 2020 2020 6966 2069 203c 206c 656e        if i < len
-00024bb0: 2865 6467 6573 292d 313a 0a20 2020 2020  (edges)-1:.     
-00024bc0: 2020 2020 2020 206c 732e 6170 7065 6e64         ls.append
-00024bd0: 2827 6672 6f6d 5f27 2b73 7472 2872 6f75  ('from_'+str(rou
-00024be0: 6e64 2865 6467 6573 5b69 5d2c 3329 292b  nd(edges[i],3))+
-00024bf0: 275f 746f 5f27 2b73 7472 2872 6f75 6e64  '_to_'+str(round
-00024c00: 2865 6467 6573 5b69 2b31 5d2c 3329 2929  (edges[i+1],3)))
-00024c10: 0a20 2020 2023 2323 2323 204e 6578 7420  .    ##### Next 
-00024c20: 7765 2061 6464 2061 2063 6f6c 756d 6e20  we add a column 
-00024c30: 746f 2068 6f6c 6420 7468 6520 6269 6e73  to hold the bins
-00024c40: 2063 7265 6174 6564 2062 7920 6162 6f76   created by abov
-00024c50: 6520 2323 2323 2323 2323 2323 2323 2323  e ##############
-00024c60: 230a 2020 2020 6466 745b 2762 696e 6e65  #.    dft['binne
-00024c70: 645f 272b 7461 7267 6574 5d20 3d20 7064  d_'+target] = pd
-00024c80: 2e63 7574 2864 6674 5b74 6172 6765 745d  .cut(dft[target]
-00024c90: 2c20 6269 6e73 3d65 6467 6573 2c20 7265  , bins=edges, re
-00024ca0: 7462 696e 733d 4661 6c73 652c 206c 6162  tbins=False, lab
-00024cb0: 656c 733d 6c73 2c20 696e 636c 7564 655f  els=ls, include_
-00024cc0: 6c6f 7765 7374 3d54 7275 6529 2e76 616c  lowest=True).val
-00024cd0: 7565 732e 746f 6c69 7374 2829 0a20 2020  ues.tolist().   
-00024ce0: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00024cf0: 6365 2874 6573 742c 2073 7472 293a 0a20  ce(test, str):. 
-00024d00: 2020 2020 2020 2074 6573 745b 2762 696e         test['bin
-00024d10: 6e65 645f 272b 7461 7267 6574 5d20 3d20  ned_'+target] = 
-00024d20: 7064 2e63 7574 2874 6573 745b 7461 7267  pd.cut(test[targ
-00024d30: 6574 5d2c 2062 696e 733d 6564 6765 732c  et], bins=edges,
-00024d40: 2072 6574 6269 6e73 3d46 616c 7365 2c20   retbins=False, 
-00024d50: 6c61 6265 6c73 3d6c 732c 2069 6e63 6c75  labels=ls, inclu
-00024d60: 6465 5f6c 6f77 6573 743d 5472 7565 292e  de_lowest=True).
-00024d70: 7661 6c75 6573 2e74 6f6c 6973 7428 290a  values.tolist().
-00024d80: 2020 2020 6e72 6f77 7320 3d20 696e 7428      nrows = int(
-00024d90: 6c65 6e28 6564 6765 7329 2f32 202b 2031  len(edges)/2 + 1
-00024da0: 290a 2020 2020 706c 742e 6669 6775 7265  ).    plt.figure
-00024db0: 2866 6967 7369 7a65 3d28 3135 2c6e 726f  (figsize=(15,nro
-00024dc0: 7773 2a33 2929 0a20 2020 2070 6c74 2e73  ws*3)).    plt.s
-00024dd0: 7562 706c 6f74 735f 6164 6a75 7374 2868  ubplots_adjust(h
-00024de0: 7370 6163 653d 2e35 290a 2020 2020 636f  space=.5).    co
-00024df0: 6c6c 6563 745f 6269 6e73 203d 205b 5d0a  llect_bins = [].
-00024e00: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00024e10: 6765 286c 656e 2865 6467 6573 2929 3a0a  ge(len(edges)):.
-00024e20: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
-00024e30: 303a 0a20 2020 2020 2020 2020 2020 2063  0:.            c
-00024e40: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00024e50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00024e60: 2020 6466 7463 203d 2064 6674 5b28 6466    dftc = dft[(df
-00024e70: 745b 7461 7267 6574 5d3e 6564 6765 735b  t[target]>edges[
-00024e80: 692d 315d 2920 2620 2864 6674 5b74 6172  i-1]) & (dft[tar
-00024e90: 6765 745d 3c3d 6564 6765 735b 695d 295d  get]<=edges[i])]
-00024ea0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00024eb0: 6c65 6374 5f62 696e 732e 6170 7065 6e64  lect_bins.append
-00024ec0: 2864 6674 6329 0a20 2020 2020 2020 2020  (dftc).         
-00024ed0: 2020 2061 7831 203d 2070 6c74 2e73 7562     ax1 = plt.sub
-00024ee0: 706c 6f74 286e 726f 7773 2c20 322c 2069  plot(nrows, 2, i
-00024ef0: 290a 2020 2020 2020 2020 2020 2020 6466  ).            df
-00024f00: 7463 5b74 6172 6765 745d 2e68 6973 7428  tc[target].hist(
-00024f10: 6269 6e73 3d33 302c 2061 783d 6178 3129  bins=30, ax=ax1)
-00024f20: 0a20 2020 2020 2020 2020 2020 2061 7831  .            ax1
-00024f30: 2e73 6574 5f74 6974 6c65 2827 6269 6e20  .set_title('bin 
-00024f40: 2564 3a20 7369 7a65 3a20 2564 2c20 2573  %d: size: %d, %s
-00024f50: 2025 302e 3266 2074 6f20 2530 2e32 6627   %0.2f to %0.2f'
-00024f60: 2025 2869 2c20 6466 7463 2e73 6861 7065   %(i, dftc.shape
-00024f70: 5b30 5d2c 2074 6172 6765 742c 0a20 2020  [0], target,.   
-00024f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00024fc0: 6467 6573 5b69 2d31 5d2c 2065 6467 6573  dges[i-1], edges
-00024fd0: 5b69 5d29 290a 2020 2020 7265 7475 726e  [i])).    return
-00024fe0: 206c 732c 2065 6467 6573 2c20 6466 742c   ls, edges, dft,
-00024ff0: 2074 6573 740a 2323 2323 2323 2323 2323   test.##########
-00025000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000248e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000248f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024900: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024910: 2323 2323 0a69 6d70 6f72 7420 6d61 7470  ####.import matp
+00024920: 6c6f 746c 6962 2e70 7970 6c6f 7420 6173  lotlib.pyplot as
+00024930: 2070 6c74 0a64 6566 2045 4441 5f62 696e   plt.def EDA_bin
+00024940: 6e69 6e67 5f6e 756d 6572 6963 5f63 6f6c  ning_numeric_col
+00024950: 756d 6e5f 6469 7370 6c61 7969 6e67 5f62  umn_displaying_b
+00024960: 696e 7328 6466 742c 2074 6172 6765 742c  ins(dft, target,
+00024970: 2062 696e 733d 342c 2074 6573 743d 2222   bins=4, test=""
+00024980: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+00024990: 6869 7320 7370 6c69 7473 2074 6865 2064  his splits the d
+000249a0: 6174 6120 636f 6c75 6d6e 2069 6e74 6f20  ata column into 
+000249b0: 7468 6520 6e75 6d62 6572 206f 6620 6269  the number of bi
+000249c0: 6e73 2073 7065 6369 6669 6564 2061 6e64  ns specified and
+000249d0: 2072 6574 7572 6e73 206c 6162 656c 732c   returns labels,
+000249e0: 2062 696e 732c 2061 6e64 2064 6174 6166   bins, and dataf
+000249f0: 7261 6d65 2e0a 2020 2020 4f75 7470 7574  rame..    Output
+00024a00: 733a 0a20 2020 2020 2020 6c61 6265 6c73  s:.       labels
+00024a10: 203d 2074 6865 206e 616d 6573 206f 6620   = the names of 
+00024a20: 7468 6520 6269 6e73 0a20 2020 2020 2020  the bins.       
+00024a30: 6564 6765 7320 3d20 7468 6520 6564 6765  edges = the edge
+00024a40: 7320 6f66 2074 6865 2062 696e 730a 2020  s of the bins.  
+00024a50: 2020 2020 2064 6674 203d 2074 6865 2064       dft = the d
+00024a60: 6174 6166 7261 6d65 2077 6974 6820 616e  ataframe with an
+00024a70: 2061 6464 6564 2063 6f6c 756d 6e20 6361   added column ca
+00024a80: 6c6c 6564 2022 6269 6e6e 6564 5f22 2b6e  lled "binned_"+n
+00024a90: 616d 6520 6f66 2074 6865 2063 6f6c 756d  ame of the colum
+00024aa0: 6e20 796f 7520 7365 6e74 2069 6e0a 2020  n you sent in.  
+00024ab0: 2020 2222 220a 2020 2020 6466 7420 3d20    """.    dft = 
+00024ac0: 636f 7079 2e64 6565 7063 6f70 7928 6466  copy.deepcopy(df
+00024ad0: 7429 0a20 2020 205f 2c20 6564 6765 7320  t).    _, edges 
+00024ae0: 3d20 7064 2e71 6375 7428 6466 745b 7461  = pd.qcut(dft[ta
+00024af0: 7267 6574 5d2e 6472 6f70 6e61 2861 7869  rget].dropna(axi
+00024b00: 733d 3029 2c71 3d62 696e 732c 2072 6574  s=0),q=bins, ret
+00024b10: 6269 6e73 3d54 7275 652c 2064 7570 6c69  bins=True, dupli
+00024b20: 6361 7465 733d 2764 726f 7027 290a 2020  cates='drop').  
+00024b30: 2020 2323 2320 6e6f 7720 7765 2063 7265    ### now we cre
+00024b40: 6174 6520 6172 7469 6669 6369 616c 206c  ate artificial l
+00024b50: 6162 656c 7320 746f 206d 6174 6368 2074  abels to match t
+00024b60: 6865 2062 696e 7320 6564 6765 7320 2323  he bins edges ##
+00024b70: 2323 0a20 2020 206c 7320 3d20 5b5d 0a20  ##.    ls = []. 
+00024b80: 2020 2066 6f72 2069 2c20 7820 696e 2065     for i, x in e
+00024b90: 6e75 6d65 7261 7465 2865 6467 6573 293a  numerate(edges):
+00024ba0: 0a20 2020 2020 2020 2023 7072 696e 7428  .        #print(
+00024bb0: 2769 203d 2025 732c 206e 6578 7420 6920  'i = %s, next i 
+00024bc0: 3d20 2573 2720 2528 692c 692b 3129 290a  = %s' %(i,i+1)).
+00024bd0: 2020 2020 2020 2020 6966 2069 203c 206c          if i < l
+00024be0: 656e 2865 6467 6573 292d 313a 0a20 2020  en(edges)-1:.   
+00024bf0: 2020 2020 2020 2020 206c 732e 6170 7065           ls.appe
+00024c00: 6e64 2827 6672 6f6d 5f27 2b73 7472 2872  nd('from_'+str(r
+00024c10: 6f75 6e64 2865 6467 6573 5b69 5d2c 3329  ound(edges[i],3)
+00024c20: 292b 275f 746f 5f27 2b73 7472 2872 6f75  )+'_to_'+str(rou
+00024c30: 6e64 2865 6467 6573 5b69 2b31 5d2c 3329  nd(edges[i+1],3)
+00024c40: 2929 0a20 2020 2023 2323 2323 204e 6578  )).    ##### Nex
+00024c50: 7420 7765 2061 6464 2061 2063 6f6c 756d  t we add a colum
+00024c60: 6e20 746f 2068 6f6c 6420 7468 6520 6269  n to hold the bi
+00024c70: 6e73 2063 7265 6174 6564 2062 7920 6162  ns created by ab
+00024c80: 6f76 6520 2323 2323 2323 2323 2323 2323  ove ############
+00024c90: 2323 230a 2020 2020 6466 745b 2762 696e  ###.    dft['bin
+00024ca0: 6e65 645f 272b 7461 7267 6574 5d20 3d20  ned_'+target] = 
+00024cb0: 7064 2e63 7574 2864 6674 5b74 6172 6765  pd.cut(dft[targe
+00024cc0: 745d 2c20 6269 6e73 3d65 6467 6573 2c20  t], bins=edges, 
+00024cd0: 7265 7462 696e 733d 4661 6c73 652c 206c  retbins=False, l
+00024ce0: 6162 656c 733d 6c73 2c20 696e 636c 7564  abels=ls, includ
+00024cf0: 655f 6c6f 7765 7374 3d54 7275 6529 2e76  e_lowest=True).v
+00024d00: 616c 7565 732e 746f 6c69 7374 2829 0a20  alues.tolist(). 
+00024d10: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00024d20: 616e 6365 2874 6573 742c 2073 7472 293a  ance(test, str):
+00024d30: 0a20 2020 2020 2020 2074 6573 745b 2762  .        test['b
+00024d40: 696e 6e65 645f 272b 7461 7267 6574 5d20  inned_'+target] 
+00024d50: 3d20 7064 2e63 7574 2874 6573 745b 7461  = pd.cut(test[ta
+00024d60: 7267 6574 5d2c 2062 696e 733d 6564 6765  rget], bins=edge
+00024d70: 732c 2072 6574 6269 6e73 3d46 616c 7365  s, retbins=False
+00024d80: 2c20 6c61 6265 6c73 3d6c 732c 2069 6e63  , labels=ls, inc
+00024d90: 6c75 6465 5f6c 6f77 6573 743d 5472 7565  lude_lowest=True
+00024da0: 292e 7661 6c75 6573 2e74 6f6c 6973 7428  ).values.tolist(
+00024db0: 290a 2020 2020 6e72 6f77 7320 3d20 696e  ).    nrows = in
+00024dc0: 7428 6c65 6e28 6564 6765 7329 2f32 202b  t(len(edges)/2 +
+00024dd0: 2031 290a 2020 2020 706c 742e 6669 6775   1).    plt.figu
+00024de0: 7265 2866 6967 7369 7a65 3d28 3135 2c6e  re(figsize=(15,n
+00024df0: 726f 7773 2a33 2929 0a20 2020 2070 6c74  rows*3)).    plt
+00024e00: 2e73 7562 706c 6f74 735f 6164 6a75 7374  .subplots_adjust
+00024e10: 2868 7370 6163 653d 2e35 290a 2020 2020  (hspace=.5).    
+00024e20: 636f 6c6c 6563 745f 6269 6e73 203d 205b  collect_bins = [
+00024e30: 5d0a 2020 2020 666f 7220 6920 696e 2072  ].    for i in r
+00024e40: 616e 6765 286c 656e 2865 6467 6573 2929  ange(len(edges))
+00024e50: 3a0a 2020 2020 2020 2020 6966 2069 203d  :.        if i =
+00024e60: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00024e70: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00024e80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00024e90: 2020 2020 6466 7463 203d 2064 6674 5b28      dftc = dft[(
+00024ea0: 6466 745b 7461 7267 6574 5d3e 6564 6765  dft[target]>edge
+00024eb0: 735b 692d 315d 2920 2620 2864 6674 5b74  s[i-1]) & (dft[t
+00024ec0: 6172 6765 745d 3c3d 6564 6765 735b 695d  arget]<=edges[i]
+00024ed0: 295d 0a20 2020 2020 2020 2020 2020 2063  )].            c
+00024ee0: 6f6c 6c65 6374 5f62 696e 732e 6170 7065  ollect_bins.appe
+00024ef0: 6e64 2864 6674 6329 0a20 2020 2020 2020  nd(dftc).       
+00024f00: 2020 2020 2061 7831 203d 2070 6c74 2e73       ax1 = plt.s
+00024f10: 7562 706c 6f74 286e 726f 7773 2c20 322c  ubplot(nrows, 2,
+00024f20: 2069 290a 2020 2020 2020 2020 2020 2020   i).            
+00024f30: 6466 7463 5b74 6172 6765 745d 2e68 6973  dftc[target].his
+00024f40: 7428 6269 6e73 3d33 302c 2061 783d 6178  t(bins=30, ax=ax
+00024f50: 3129 0a20 2020 2020 2020 2020 2020 2061  1).            a
+00024f60: 7831 2e73 6574 5f74 6974 6c65 2827 6269  x1.set_title('bi
+00024f70: 6e20 2564 3a20 7369 7a65 3a20 2564 2c20  n %d: size: %d, 
+00024f80: 2573 2025 302e 3266 2074 6f20 2530 2e32  %s %0.2f to %0.2
+00024f90: 6627 2025 2869 2c20 6466 7463 2e73 6861  f' %(i, dftc.sha
+00024fa0: 7065 5b30 5d2c 2074 6172 6765 742c 0a20  pe[0], target,. 
+00024fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024ff0: 2065 6467 6573 5b69 2d31 5d2c 2065 6467   edges[i-1], edg
+00025000: 6573 5b69 5d29 290a 2020 2020 7265 7475  es[i])).    retu
+00025010: 726e 206c 732c 2065 6467 6573 2c20 6466  rn ls, edges, df
+00025020: 742c 2074 6573 740a 2323 2323 2323 2323  t, test.########
 00025030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025040: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00025050: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
-00025060: 6f72 7420 5061 7468 0a69 6d70 6f72 7420  ort Path.import 
-00025070: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
-00025080: 7420 6173 2070 6c74 0a69 6d70 6f72 7420  t as plt.import 
-00025090: 7365 6162 6f72 6e20 6173 2073 6e73 0a66  seaborn as sns.f
-000250a0: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
-000250b0: 6f72 7420 6461 7465 7469 6d65 2c20 6461  ort datetime, da
-000250c0: 7465 0a66 726f 6d20 736b 6c65 6172 6e2e  te.from sklearn.
-000250d0: 6d65 7472 6963 7320 696d 706f 7274 206d  metrics import m
-000250e0: 6561 6e5f 7371 7561 7265 645f 6572 726f  ean_squared_erro
-000250f0: 722c 2072 6f63 5f61 7563 5f73 636f 7265  r, roc_auc_score
-00025100: 0a66 726f 6d20 736b 6c65 6172 6e2e 7072  .from sklearn.pr
-00025110: 6570 726f 6365 7373 696e 6720 696d 706f  eprocessing impo
-00025120: 7274 206d 696e 6d61 785f 7363 616c 650a  rt minmax_scale.
-00025130: 2323 2323 2054 6869 7320 6973 2077 6865  #### This is whe
-00025140: 7265 2077 6520 6164 6420 6f74 6865 7220  re we add other 
-00025150: 6c69 6272 6172 6965 7320 746f 2066 6f72  libraries to for
-00025160: 6d20 6120 7069 7065 6c69 6e65 2023 2323  m a pipeline ###
-00025170: 0a69 6d70 6f72 7420 636f 7079 0a69 6d70  .import copy.imp
-00025180: 6f72 7420 7469 6d65 0a69 6d70 6f72 7420  ort time.import 
-00025190: 7265 0a66 726f 6d20 7363 6970 792e 6e64  re.from scipy.nd
-000251a0: 696d 6167 6520 696d 706f 7274 2063 6f6e  image import con
-000251b0: 766f 6c76 650a 6672 6f6d 2073 6b6c 6561  volve.from sklea
-000251c0: 726e 2069 6d70 6f72 7420 2064 6174 6173  rn import  datas
-000251d0: 6574 732c 206d 6574 7269 6373 0a66 726f  ets, metrics.fro
-000251e0: 6d20 736b 6c65 6172 6e2e 6d6f 6465 6c5f  m sklearn.model_
-000251f0: 7365 6c65 6374 696f 6e20 696d 706f 7274  selection import
-00025200: 2074 7261 696e 5f74 6573 745f 7370 6c69   train_test_spli
-00025210: 740a 6672 6f6d 2073 6b6c 6561 726e 2e70  t.from sklearn.p
-00025220: 6970 656c 696e 6520 696d 706f 7274 2050  ipeline import P
-00025230: 6970 656c 696e 650a 6672 6f6d 2073 6b6c  ipeline.from skl
-00025240: 6561 726e 2e6d 6f64 656c 5f73 656c 6563  earn.model_selec
-00025250: 7469 6f6e 2069 6d70 6f72 7420 4b46 6f6c  tion import KFol
-00025260: 642c 2053 7472 6174 6966 6965 6453 6875  d, StratifiedShu
-00025270: 6666 6c65 5370 6c69 740a 0a64 6566 2061  ffleSplit..def a
-00025280: 6464 5f74 6578 745f 7061 6464 696e 6773  dd_text_paddings
-00025290: 2874 7261 696e 5f64 6174 612c 6e6c 705f  (train_data,nlp_
-000252a0: 636f 6c75 6d6e 2c67 6c6f 7665 5f66 696c  column,glove_fil
-000252b0: 656e 616d 655f 7769 7468 5f70 6174 682c  ename_with_path,
-000252c0: 746f 6b65 6e69 7a65 642c 0a20 2020 2020  tokenized,.     
-000252d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252e0: 2020 2020 2020 2066 6974 5f66 6c61 673d         fit_flag=
-000252f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00025040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025080: 230a 6672 6f6d 2070 6174 686c 6962 2069  #.from pathlib i
+00025090: 6d70 6f72 7420 5061 7468 0a69 6d70 6f72  mport Path.impor
+000250a0: 7420 6d61 7470 6c6f 746c 6962 2e70 7970  t matplotlib.pyp
+000250b0: 6c6f 7420 6173 2070 6c74 0a69 6d70 6f72  lot as plt.impor
+000250c0: 7420 7365 6162 6f72 6e20 6173 2073 6e73  t seaborn as sns
+000250d0: 0a66 726f 6d20 6461 7465 7469 6d65 2069  .from datetime i
+000250e0: 6d70 6f72 7420 6461 7465 7469 6d65 2c20  mport datetime, 
+000250f0: 6461 7465 0a66 726f 6d20 736b 6c65 6172  date.from sklear
+00025100: 6e2e 6d65 7472 6963 7320 696d 706f 7274  n.metrics import
+00025110: 206d 6561 6e5f 7371 7561 7265 645f 6572   mean_squared_er
+00025120: 726f 722c 2072 6f63 5f61 7563 5f73 636f  ror, roc_auc_sco
+00025130: 7265 0a66 726f 6d20 736b 6c65 6172 6e2e  re.from sklearn.
+00025140: 7072 6570 726f 6365 7373 696e 6720 696d  preprocessing im
+00025150: 706f 7274 206d 696e 6d61 785f 7363 616c  port minmax_scal
+00025160: 650a 2323 2323 2054 6869 7320 6973 2077  e.#### This is w
+00025170: 6865 7265 2077 6520 6164 6420 6f74 6865  here we add othe
+00025180: 7220 6c69 6272 6172 6965 7320 746f 2066  r libraries to f
+00025190: 6f72 6d20 6120 7069 7065 6c69 6e65 2023  orm a pipeline #
+000251a0: 2323 0a69 6d70 6f72 7420 636f 7079 0a69  ##.import copy.i
+000251b0: 6d70 6f72 7420 7469 6d65 0a69 6d70 6f72  mport time.impor
+000251c0: 7420 7265 0a66 726f 6d20 7363 6970 792e  t re.from scipy.
+000251d0: 6e64 696d 6167 6520 696d 706f 7274 2063  ndimage import c
+000251e0: 6f6e 766f 6c76 650a 6672 6f6d 2073 6b6c  onvolve.from skl
+000251f0: 6561 726e 2069 6d70 6f72 7420 2064 6174  earn import  dat
+00025200: 6173 6574 732c 206d 6574 7269 6373 0a66  asets, metrics.f
+00025210: 726f 6d20 736b 6c65 6172 6e2e 6d6f 6465  rom sklearn.mode
+00025220: 6c5f 7365 6c65 6374 696f 6e20 696d 706f  l_selection impo
+00025230: 7274 2074 7261 696e 5f74 6573 745f 7370  rt train_test_sp
+00025240: 6c69 740a 6672 6f6d 2073 6b6c 6561 726e  lit.from sklearn
+00025250: 2e70 6970 656c 696e 6520 696d 706f 7274  .pipeline import
+00025260: 2050 6970 656c 696e 650a 6672 6f6d 2073   Pipeline.from s
+00025270: 6b6c 6561 726e 2e6d 6f64 656c 5f73 656c  klearn.model_sel
+00025280: 6563 7469 6f6e 2069 6d70 6f72 7420 4b46  ection import KF
+00025290: 6f6c 642c 2053 7472 6174 6966 6965 6453  old, StratifiedS
+000252a0: 6875 6666 6c65 5370 6c69 740a 0a64 6566  huffleSplit..def
+000252b0: 2061 6464 5f74 6578 745f 7061 6464 696e   add_text_paddin
+000252c0: 6773 2874 7261 696e 5f64 6174 612c 6e6c  gs(train_data,nl
+000252d0: 705f 636f 6c75 6d6e 2c67 6c6f 7665 5f66  p_column,glove_f
+000252e0: 696c 656e 616d 655f 7769 7468 5f70 6174  ilename_with_pat
+000252f0: 682c 746f 6b65 6e69 7a65 642c 0a20 2020  h,tokenized,.   
 00025300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025310: 2020 6d61 785f 6c65 6e67 7468 3d31 3030    max_length=100
-00025320: 293a 0a20 2020 2022 2222 0a20 2020 2023  ):.    """.    #
-00025330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025310: 2020 2020 2020 2020 2066 6974 5f66 6c61           fit_fla
+00025320: 673d 5472 7565 2c0a 2020 2020 2020 2020  g=True,.        
+00025330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025340: 2020 2020 6d61 785f 6c65 6e67 7468 3d31      max_length=1
+00025350: 3030 293a 0a20 2020 2022 2222 0a20 2020  00):.    """.   
+00025360: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
 00025370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00025380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025390: 230a 2020 2020 5468 6973 2066 756e 6374  #.    This funct
-000253a0: 696f 6e20 7573 6573 2061 2047 6c6f 5665  ion uses a GloVe
-000253b0: 2070 7265 2d74 7261 696e 6564 206d 6f64   pre-trained mod
-000253c0: 656c 2074 6f20 6164 6420 656d 6265 6464  el to add embedd
-000253d0: 696e 6773 2074 6f20 796f 7572 2064 6174  ings to your dat
-000253e0: 6120 7365 742e 0a20 2020 2023 2323 2323  a set..    #####
-000253f0: 2323 2320 2049 204e 2050 2055 2054 2023  ###  I N P U T #
-00025400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025410: 2323 2323 2323 2323 2323 2323 233a 0a20  #############:. 
-00025420: 2020 2064 6174 613a 2044 6174 6146 7261     data: DataFra
-00025430: 6d65 0a20 2020 206e 6c70 5f63 6f6c 756d  me.    nlp_colum
-00025440: 6e3a 206e 616d 6520 6f66 2074 6865 204e  n: name of the N
-00025450: 4c50 2063 6f6c 756d 6e20 696e 2074 6865  LP column in the
-00025460: 2044 6174 6146 7261 6d65 0a20 2020 2074   DataFrame.    t
-00025470: 6172 6765 743a 206e 616d 6520 6f66 2074  arget: name of t
-00025480: 6865 2074 6172 6765 7420 7661 7269 6162  he target variab
-00025490: 6c65 2069 6e20 7468 6520 4461 7461 4672  le in the DataFr
-000254a0: 616d 650a 2020 2020 676c 6f76 6566 696c  ame.    glovefil
-000254b0: 653a 206c 6f63 6174 696f 6e20 6f66 2077  e: location of w
-000254c0: 6865 7265 2074 6865 2067 6c6f 7665 2e74  here the glove.t
-000254d0: 7874 2066 696c 6520 6973 2e20 596f 7520  xt file is. You 
-000254e0: 6d75 7374 2067 6976 6520 7468 6520 6675  must give the fu
-000254f0: 6c6c 2070 6174 6820 746f 2074 6861 7420  ll path to that 
-00025500: 6669 6c65 2e0a 2020 2020 6d61 785f 6c65  file..    max_le
-00025510: 6e67 7468 3a20 7370 6563 6966 7920 7468  ngth: specify th
-00025520: 6520 6469 6d65 6e73 696f 6e20 6f66 2074  e dimension of t
-00025530: 6865 2067 6c6f 7665 2076 6563 746f 7220  he glove vector 
-00025540: 2079 6f75 2063 616e 2068 6176 6520 7570   you can have up
-00025550: 746f 2074 6865 2064 696d 656e 7369 6f6e  to the dimension
-00025560: 206f 6620 7468 6520 676c 6f76 6520 7478   of the glove tx
-00025570: 7420 6669 6c65 2e0a 2020 2020 2020 2020  t file..        
-00025580: 2020 204d 616b 6520 7375 7265 2079 6f75     Make sure you
-00025590: 2064 6f6e 2774 2065 7863 6565 6420 7468   don't exceed th
-000255a0: 6520 6469 6d65 6e73 696f 6e20 7370 6563  e dimension spec
-000255b0: 6966 6965 6420 696e 2074 6865 2067 6c6f  ified in the glo
-000255c0: 7665 2e74 7874 2066 696c 652e 204f 7468  ve.txt file. Oth
-000255d0: 6572 7769 7365 2c20 6572 726f 7220 7265  erwise, error re
-000255e0: 7375 6c74 2e0a 2020 2020 2323 2323 2323  sult..    ######
-000255f0: 2320 4f20 5520 5420 5020 5520 5420 2323  # O U T P U T ##
-00025600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025610: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
-00025620: 5468 6520 6461 7461 6672 616d 6520 6973  The dataframe is
-00025630: 2073 706c 6974 2069 6e74 6f20 7472 6169   split into trai
-00025640: 6e20 616e 6420 7465 7374 2061 6e64 2061  n and test and a
-00025650: 7265 206d 6f64 6966 6965 6420 696e 746f  re modified into
-00025660: 2074 6865 2073 7065 6369 6669 6564 2076   the specified v
-00025670: 6563 746f 7220 6469 6d65 6e73 696f 6e20  ector dimension 
-00025680: 6f66 206d 6178 5f6c 656e 6774 680a 2020  of max_length.  
-00025690: 2020 585f 7472 6169 6e5f 7061 6464 6564    X_train_padded
-000256a0: 3a20 7468 6520 7472 6169 6e20 6461 7461  : the train data
-000256b0: 6672 616d 6520 7769 7468 2064 696d 656e  frame with dimen
-000256c0: 7369 6f6e 2073 7065 6369 6669 6564 2069  sion specified i
-000256d0: 6e20 6d61 785f 6c65 6e67 7468 0a20 2020  n max_length.   
-000256e0: 2079 5f74 7261 696e 3a20 7468 6520 7461   y_train: the ta
-000256f0: 7267 6574 2076 6563 746f 7220 7573 696e  rget vector usin
-00025700: 6720 6461 7461 2061 6e64 2074 6172 6765  g data and targe
-00025710: 7420 636f 6c75 6d6e 0a20 2020 2058 5f74  t column.    X_t
-00025720: 6573 745f 7061 6464 6564 3a20 2074 6865  est_padded:  the
-00025730: 2074 6573 7420 6461 7461 6672 616d 6520   test dataframe 
-00025740: 7769 7468 2064 696d 656e 7369 6f6e 2073  with dimension s
-00025750: 7065 6369 6669 6564 2069 6e20 6d61 785f  pecified in max_
-00025760: 6c65 6e67 7468 0a20 2020 2074 6f6b 656e  length.    token
-00025770: 697a 6564 3a20 5468 6973 2069 7320 7468  ized: This is th
-00025780: 6520 746f 6b65 6e69 7a65 7220 7468 6174  e tokenizer that
-00025790: 2077 6173 2075 7365 6420 746f 2073 706c   was used to spl
-000257a0: 6974 2074 6865 2077 6f72 6473 2069 6e20  it the words in 
-000257b0: 6461 7461 2073 6574 2e20 5468 6973 206d  data set. This m
-000257c0: 7573 7420 6265 2075 7365 6420 6c61 7465  ust be used late
-000257d0: 722e 0a20 2020 2023 2323 2323 2323 2323  r..    #########
-000257e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000257f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000253a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000253b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000253c0: 2323 230a 2020 2020 5468 6973 2066 756e  ###.    This fun
+000253d0: 6374 696f 6e20 7573 6573 2061 2047 6c6f  ction uses a Glo
+000253e0: 5665 2070 7265 2d74 7261 696e 6564 206d  Ve pre-trained m
+000253f0: 6f64 656c 2074 6f20 6164 6420 656d 6265  odel to add embe
+00025400: 6464 696e 6773 2074 6f20 796f 7572 2064  ddings to your d
+00025410: 6174 6120 7365 742e 0a20 2020 2023 2323  ata set..    ###
+00025420: 2323 2323 2320 2049 204e 2050 2055 2054  #####  I N P U T
+00025430: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00025440: 2323 2323 2323 2323 2323 2323 2323 233a  ###############:
+00025450: 0a20 2020 2064 6174 613a 2044 6174 6146  .    data: DataF
+00025460: 7261 6d65 0a20 2020 206e 6c70 5f63 6f6c  rame.    nlp_col
+00025470: 756d 6e3a 206e 616d 6520 6f66 2074 6865  umn: name of the
+00025480: 204e 4c50 2063 6f6c 756d 6e20 696e 2074   NLP column in t
+00025490: 6865 2044 6174 6146 7261 6d65 0a20 2020  he DataFrame.   
+000254a0: 2074 6172 6765 743a 206e 616d 6520 6f66   target: name of
+000254b0: 2074 6865 2074 6172 6765 7420 7661 7269   the target vari
+000254c0: 6162 6c65 2069 6e20 7468 6520 4461 7461  able in the Data
+000254d0: 4672 616d 650a 2020 2020 676c 6f76 6566  Frame.    glovef
+000254e0: 696c 653a 206c 6f63 6174 696f 6e20 6f66  ile: location of
+000254f0: 2077 6865 7265 2074 6865 2067 6c6f 7665   where the glove
+00025500: 2e74 7874 2066 696c 6520 6973 2e20 596f  .txt file is. Yo
+00025510: 7520 6d75 7374 2067 6976 6520 7468 6520  u must give the 
+00025520: 6675 6c6c 2070 6174 6820 746f 2074 6861  full path to tha
+00025530: 7420 6669 6c65 2e0a 2020 2020 6d61 785f  t file..    max_
+00025540: 6c65 6e67 7468 3a20 7370 6563 6966 7920  length: specify 
+00025550: 7468 6520 6469 6d65 6e73 696f 6e20 6f66  the dimension of
+00025560: 2074 6865 2067 6c6f 7665 2076 6563 746f   the glove vecto
+00025570: 7220 2079 6f75 2063 616e 2068 6176 6520  r  you can have 
+00025580: 7570 746f 2074 6865 2064 696d 656e 7369  upto the dimensi
+00025590: 6f6e 206f 6620 7468 6520 676c 6f76 6520  on of the glove 
+000255a0: 7478 7420 6669 6c65 2e0a 2020 2020 2020  txt file..      
+000255b0: 2020 2020 204d 616b 6520 7375 7265 2079       Make sure y
+000255c0: 6f75 2064 6f6e 2774 2065 7863 6565 6420  ou don't exceed 
+000255d0: 7468 6520 6469 6d65 6e73 696f 6e20 7370  the dimension sp
+000255e0: 6563 6966 6965 6420 696e 2074 6865 2067  ecified in the g
+000255f0: 6c6f 7665 2e74 7874 2066 696c 652e 204f  love.txt file. O
+00025600: 7468 6572 7769 7365 2c20 6572 726f 7220  therwise, error 
+00025610: 7265 7375 6c74 2e0a 2020 2020 2323 2323  result..    ####
+00025620: 2323 2320 4f20 5520 5420 5020 5520 5420  ### O U T P U T 
+00025630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025640: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
+00025650: 2020 5468 6520 6461 7461 6672 616d 6520    The dataframe 
+00025660: 6973 2073 706c 6974 2069 6e74 6f20 7472  is split into tr
+00025670: 6169 6e20 616e 6420 7465 7374 2061 6e64  ain and test and
+00025680: 2061 7265 206d 6f64 6966 6965 6420 696e   are modified in
+00025690: 746f 2074 6865 2073 7065 6369 6669 6564  to the specified
+000256a0: 2076 6563 746f 7220 6469 6d65 6e73 696f   vector dimensio
+000256b0: 6e20 6f66 206d 6178 5f6c 656e 6774 680a  n of max_length.
+000256c0: 2020 2020 585f 7472 6169 6e5f 7061 6464      X_train_padd
+000256d0: 6564 3a20 7468 6520 7472 6169 6e20 6461  ed: the train da
+000256e0: 7461 6672 616d 6520 7769 7468 2064 696d  taframe with dim
+000256f0: 656e 7369 6f6e 2073 7065 6369 6669 6564  ension specified
+00025700: 2069 6e20 6d61 785f 6c65 6e67 7468 0a20   in max_length. 
+00025710: 2020 2079 5f74 7261 696e 3a20 7468 6520     y_train: the 
+00025720: 7461 7267 6574 2076 6563 746f 7220 7573  target vector us
+00025730: 696e 6720 6461 7461 2061 6e64 2074 6172  ing data and tar
+00025740: 6765 7420 636f 6c75 6d6e 0a20 2020 2058  get column.    X
+00025750: 5f74 6573 745f 7061 6464 6564 3a20 2074  _test_padded:  t
+00025760: 6865 2074 6573 7420 6461 7461 6672 616d  he test datafram
+00025770: 6520 7769 7468 2064 696d 656e 7369 6f6e  e with dimension
+00025780: 2073 7065 6369 6669 6564 2069 6e20 6d61   specified in ma
+00025790: 785f 6c65 6e67 7468 0a20 2020 2074 6f6b  x_length.    tok
+000257a0: 656e 697a 6564 3a20 5468 6973 2069 7320  enized: This is 
+000257b0: 7468 6520 746f 6b65 6e69 7a65 7220 7468  the tokenizer th
+000257c0: 6174 2077 6173 2075 7365 6420 746f 2073  at was used to s
+000257d0: 706c 6974 2074 6865 2077 6f72 6473 2069  plit the words i
+000257e0: 6e20 6461 7461 2073 6574 2e20 5468 6973  n data set. This
+000257f0: 206d 7573 7420 6265 2075 7365 6420 6c61   must be used la
+00025800: 7465 722e 0a20 2020 2023 2323 2323 2323  ter..    #######
 00025810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00025820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025830: 2323 2323 2323 2323 230a 2020 2020 2222  #########.    ""
-00025840: 220a 2020 2020 7472 6169 6e5f 696e 6465  ".    train_inde
-00025850: 7820 3d20 7472 6169 6e5f 6461 7461 2e69  x = train_data.i
-00025860: 6e64 6578 0a20 2020 2023 2323 2045 6e63  ndex.    ### Enc
-00025870: 6f64 6520 5472 6169 6e20 6461 7461 2074  ode Train data t
-00025880: 6578 7420 696e 746f 2073 6571 7565 6e63  ext into sequenc
-00025890: 6573 0a20 2020 2074 7261 696e 5f64 6174  es.    train_dat
-000258a0: 615f 656e 636f 6465 6420 3d20 746f 6b65  a_encoded = toke
-000258b0: 6e69 7a65 642e 7465 7874 735f 746f 5f73  nized.texts_to_s
-000258c0: 6571 7565 6e63 6573 2874 7261 696e 5f64  equences(train_d
-000258d0: 6174 615b 6e6c 705f 636f 6c75 6d6e 5d29  ata[nlp_column])
-000258e0: 0a20 2020 2023 2323 2050 6164 5f53 6571  .    ### Pad_Seq
-000258f0: 7565 6e63 6573 2066 756e 6374 696f 6e20  uences function 
-00025900: 6973 2075 7365 6420 746f 206d 616b 6520  is used to make 
-00025910: 6c69 7374 7320 6f66 2075 6e65 7175 616c  lists of unequal
-00025920: 206c 656e 6774 6820 746f 2073 7461 636b   length to stack
-00025930: 6564 2073 6574 7320 6f66 2070 6164 6465  ed sets of padde
-00025940: 6420 616e 6420 7472 756e 6361 7465 6420  d and truncated 
-00025950: 6172 7261 7973 0a20 2020 2023 2323 2050  arrays.    ### P
-00025960: 6164 2053 6571 7565 6e63 6573 2066 6f72  ad Sequences for
-00025970: 2054 7261 696e 0a20 2020 2058 5f74 7261   Train.    X_tra
-00025980: 696e 5f70 6164 6465 6420 3d20 7061 645f  in_padded = pad_
-00025990: 7365 7175 656e 6365 7328 7472 6169 6e5f  sequences(train_
-000259a0: 6461 7461 5f65 6e63 6f64 6564 2c0a 2020  data_encoded,.  
-000259b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259c0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000259d0: 786c 656e 3d6d 6178 5f6c 656e 6774 682c  xlen=max_length,
-000259e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025860: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+00025870: 2222 220a 2020 2020 7472 6169 6e5f 696e  """.    train_in
+00025880: 6465 7820 3d20 7472 6169 6e5f 6461 7461  dex = train_data
+00025890: 2e69 6e64 6578 0a20 2020 2023 2323 2045  .index.    ### E
+000258a0: 6e63 6f64 6520 5472 6169 6e20 6461 7461  ncode Train data
+000258b0: 2074 6578 7420 696e 746f 2073 6571 7565   text into seque
+000258c0: 6e63 6573 0a20 2020 2074 7261 696e 5f64  nces.    train_d
+000258d0: 6174 615f 656e 636f 6465 6420 3d20 746f  ata_encoded = to
+000258e0: 6b65 6e69 7a65 642e 7465 7874 735f 746f  kenized.texts_to
+000258f0: 5f73 6571 7565 6e63 6573 2874 7261 696e  _sequences(train
+00025900: 5f64 6174 615b 6e6c 705f 636f 6c75 6d6e  _data[nlp_column
+00025910: 5d29 0a20 2020 2023 2323 2050 6164 5f53  ]).    ### Pad_S
+00025920: 6571 7565 6e63 6573 2066 756e 6374 696f  equences functio
+00025930: 6e20 6973 2075 7365 6420 746f 206d 616b  n is used to mak
+00025940: 6520 6c69 7374 7320 6f66 2075 6e65 7175  e lists of unequ
+00025950: 616c 206c 656e 6774 6820 746f 2073 7461  al length to sta
+00025960: 636b 6564 2073 6574 7320 6f66 2070 6164  cked sets of pad
+00025970: 6465 6420 616e 6420 7472 756e 6361 7465  ded and truncate
+00025980: 6420 6172 7261 7973 0a20 2020 2023 2323  d arrays.    ###
+00025990: 2050 6164 2053 6571 7565 6e63 6573 2066   Pad Sequences f
+000259a0: 6f72 2054 7261 696e 0a20 2020 2058 5f74  or Train.    X_t
+000259b0: 7261 696e 5f70 6164 6465 6420 3d20 7061  rain_padded = pa
+000259c0: 645f 7365 7175 656e 6365 7328 7472 6169  d_sequences(trai
+000259d0: 6e5f 6461 7461 5f65 6e63 6f64 6564 2c0a  n_data_encoded,.
+000259e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000259f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a00: 2070 6164 6469 6e67 3d27 706f 7374 272c   padding='post',
-00025a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025a00: 6d61 786c 656e 3d6d 6178 5f6c 656e 6774  maxlen=max_lengt
+00025a10: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
 00025a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a30: 7472 756e 6361 7469 6e67 3d27 706f 7374  truncating='post
-00025a40: 2729 0a20 2020 2070 7269 6e74 2827 2020  ').    print('  
-00025a50: 2020 4461 7461 2073 6861 7065 2061 6674    Data shape aft
-00025a60: 6572 2070 6164 6469 6e67 203d 2025 7327  er padding = %s'
-00025a70: 2025 2858 5f74 7261 696e 5f70 6164 6465   %(X_train_padde
-00025a80: 642e 7368 6170 652c 2929 0a20 2020 206e  d.shape,)).    n
-00025a90: 6577 5f63 6f6c 7320 3d20 5b27 676c 6f76  ew_cols = ['glov
-00025aa0: 655f 6469 6d5f 2720 2b20 7374 7228 782b  e_dim_' + str(x+
-00025ab0: 3129 2066 6f72 2078 2069 6e20 7261 6e67  1) for x in rang
-00025ac0: 6528 585f 7472 6169 6e5f 7061 6464 6564  e(X_train_padded
-00025ad0: 2e73 6861 7065 5b31 5d29 5d0a 2020 2020  .shape[1])].    
-00025ae0: 585f 7472 6169 6e5f 7061 6464 6564 203d  X_train_padded =
-00025af0: 2070 642e 4461 7461 4672 616d 6528 585f   pd.DataFrame(X_
-00025b00: 7472 6169 6e5f 7061 6464 6564 2c20 636f  train_padded, co
-00025b10: 6c75 6d6e 733d 6e65 775f 636f 6c73 2c20  lumns=new_cols, 
-00025b20: 696e 6465 783d 7472 6169 6e5f 696e 6465  index=train_inde
-00025b30: 7829 0a20 2020 2069 6620 6669 745f 666c  x).    if fit_fl
-00025b40: 6167 3a0a 2020 2020 2020 2020 7265 7475  ag:.        retu
-00025b50: 726e 2058 5f74 7261 696e 5f70 6164 6465  rn X_train_padde
-00025b60: 642c 2074 6f6b 656e 697a 6564 2c20 766f  d, tokenized, vo
-00025b70: 6361 625f 7369 7a65 0a20 2020 2065 6c73  cab_size.    els
-00025b80: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00025b90: 6e20 585f 7472 6169 6e5f 7061 6464 6564  n X_train_padded
-00025ba0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00025bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025a30: 2020 2070 6164 6469 6e67 3d27 706f 7374     padding='post
+00025a40: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00025a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a60: 2020 7472 756e 6361 7469 6e67 3d27 706f    truncating='po
+00025a70: 7374 2729 0a20 2020 2070 7269 6e74 2827  st').    print('
+00025a80: 2020 2020 4461 7461 2073 6861 7065 2061      Data shape a
+00025a90: 6674 6572 2070 6164 6469 6e67 203d 2025  fter padding = %
+00025aa0: 7327 2025 2858 5f74 7261 696e 5f70 6164  s' %(X_train_pad
+00025ab0: 6465 642e 7368 6170 652c 2929 0a20 2020  ded.shape,)).   
+00025ac0: 206e 6577 5f63 6f6c 7320 3d20 5b27 676c   new_cols = ['gl
+00025ad0: 6f76 655f 6469 6d5f 2720 2b20 7374 7228  ove_dim_' + str(
+00025ae0: 782b 3129 2066 6f72 2078 2069 6e20 7261  x+1) for x in ra
+00025af0: 6e67 6528 585f 7472 6169 6e5f 7061 6464  nge(X_train_padd
+00025b00: 6564 2e73 6861 7065 5b31 5d29 5d0a 2020  ed.shape[1])].  
+00025b10: 2020 585f 7472 6169 6e5f 7061 6464 6564    X_train_padded
+00025b20: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00025b30: 585f 7472 6169 6e5f 7061 6464 6564 2c20  X_train_padded, 
+00025b40: 636f 6c75 6d6e 733d 6e65 775f 636f 6c73  columns=new_cols
+00025b50: 2c20 696e 6465 783d 7472 6169 6e5f 696e  , index=train_in
+00025b60: 6465 7829 0a20 2020 2069 6620 6669 745f  dex).    if fit_
+00025b70: 666c 6167 3a0a 2020 2020 2020 2020 7265  flag:.        re
+00025b80: 7475 726e 2058 5f74 7261 696e 5f70 6164  turn X_train_pad
+00025b90: 6465 642c 2074 6f6b 656e 697a 6564 2c20  ded, tokenized, 
+00025ba0: 766f 6361 625f 7369 7a65 0a20 2020 2065  vocab_size.    e
+00025bb0: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+00025bc0: 7572 6e20 585f 7472 6169 6e5f 7061 6464  urn X_train_padd
+00025bd0: 6564 0a23 2323 2323 2323 2323 2323 2323  ed.#############
 00025be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00025bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025c00: 2323 2323 2323 0a64 6566 206c 6f61 645f  ######.def load_
-00025c10: 656d 6265 6464 696e 6773 2874 6f6b 656e  embeddings(token
-00025c20: 697a 6564 2c67 6c6f 7665 5f66 696c 656e  ized,glove_filen
-00025c30: 616d 655f 7769 7468 5f70 6174 682c 766f  ame_with_path,vo
-00025c40: 6361 625f 7369 7a65 2c67 6c6f 7665 5f64  cab_size,glove_d
-00025c50: 696d 656e 7369 6f6e 293a 0a20 2020 2022  imension):.    "
-00025c60: 2222 0a20 2020 2023 2323 2323 2323 2323  "".    #########
-00025c70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025c90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025c10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025c20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025c30: 2323 2323 2323 2323 0a64 6566 206c 6f61  ########.def loa
+00025c40: 645f 656d 6265 6464 696e 6773 2874 6f6b  d_embeddings(tok
+00025c50: 656e 697a 6564 2c67 6c6f 7665 5f66 696c  enized,glove_fil
+00025c60: 656e 616d 655f 7769 7468 5f70 6174 682c  ename_with_path,
+00025c70: 766f 6361 625f 7369 7a65 2c67 6c6f 7665  vocab_size,glove
+00025c80: 5f64 696d 656e 7369 6f6e 293a 0a20 2020  _dimension):.   
+00025c90: 2022 2222 0a20 2020 2023 2323 2323 2323   """.    #######
 00025ca0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00025cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025cc0: 2323 2323 2323 2323 230a 2020 2020 2320  #########.    # 
-00025cd0: 676c 6f76 655f 6669 6c65 6e61 6d65 5f77  glove_filename_w
-00025ce0: 6974 685f 7061 7468 3a20 4d61 6b65 2073  ith_path: Make s
-00025cf0: 7572 6520 7520 6861 7665 2064 6f77 6e6c  ure u have downl
-00025d00: 6f61 6465 6420 616e 6420 756e 7a69 7070  oaded and unzipp
-00025d10: 6564 2074 6865 2047 6c6f 5665 2022 2e74  ed the GloVe ".t
-00025d20: 7874 2220 6669 6c65 2074 6f20 7468 6520  xt" file to the 
-00025d30: 6c6f 6361 7469 6f6e 2068 6572 652e 0a20  location here.. 
-00025d40: 2020 2023 2077 6520 6e6f 7720 6372 6561     # we now crea
-00025d50: 7465 2061 2064 6963 7469 6f6e 6172 7920  te a dictionary 
-00025d60: 7468 6174 206d 6170 7320 476c 6f56 6520  that maps GloVe 
-00025d70: 746f 6b65 6e73 2074 6f20 3130 302c 206f  tokens to 100, o
-00025d80: 7220 3230 302d 206f 7220 3330 302d 6469  r 200- or 300-di
-00025d90: 6d65 6e73 696f 6e61 6c20 7265 616c 2d76  mensional real-v
-00025da0: 616c 7565 6420 7665 6374 6f72 730a 2020  alued vectors.  
-00025db0: 2020 2320 5468 656e 2077 6520 6c6f 6164    # Then we load
-00025dc0: 2074 6865 2077 686f 6c65 2065 6d62 6564   the whole embed
-00025dd0: 6469 6e67 2069 6e74 6f20 6d65 6d6f 7279  ding into memory
-00025de0: 2e20 4d61 6b65 2073 7572 6520 796f 7520  . Make sure you 
-00025df0: 6861 7665 2070 6c65 6e74 7920 6f66 206d  have plenty of m
-00025e00: 656d 6f72 7920 696e 2079 6f75 7220 6d61  emory in your ma
-00025e10: 6368 696e 6521 0a20 2020 2023 2323 2323  chine!.    #####
-00025e20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025e30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025e40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025cf0: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+00025d00: 2320 676c 6f76 655f 6669 6c65 6e61 6d65  # glove_filename
+00025d10: 5f77 6974 685f 7061 7468 3a20 4d61 6b65  _with_path: Make
+00025d20: 2073 7572 6520 7520 6861 7665 2064 6f77   sure u have dow
+00025d30: 6e6c 6f61 6465 6420 616e 6420 756e 7a69  nloaded and unzi
+00025d40: 7070 6564 2074 6865 2047 6c6f 5665 2022  pped the GloVe "
+00025d50: 2e74 7874 2220 6669 6c65 2074 6f20 7468  .txt" file to th
+00025d60: 6520 6c6f 6361 7469 6f6e 2068 6572 652e  e location here.
+00025d70: 0a20 2020 2023 2077 6520 6e6f 7720 6372  .    # we now cr
+00025d80: 6561 7465 2061 2064 6963 7469 6f6e 6172  eate a dictionar
+00025d90: 7920 7468 6174 206d 6170 7320 476c 6f56  y that maps GloV
+00025da0: 6520 746f 6b65 6e73 2074 6f20 3130 302c  e tokens to 100,
+00025db0: 206f 7220 3230 302d 206f 7220 3330 302d   or 200- or 300-
+00025dc0: 6469 6d65 6e73 696f 6e61 6c20 7265 616c  dimensional real
+00025dd0: 2d76 616c 7565 6420 7665 6374 6f72 730a  -valued vectors.
+00025de0: 2020 2020 2320 5468 656e 2077 6520 6c6f      # Then we lo
+00025df0: 6164 2074 6865 2077 686f 6c65 2065 6d62  ad the whole emb
+00025e00: 6564 6469 6e67 2069 6e74 6f20 6d65 6d6f  edding into memo
+00025e10: 7279 2e20 4d61 6b65 2073 7572 6520 796f  ry. Make sure yo
+00025e20: 7520 6861 7665 2070 6c65 6e74 7920 6f66  u have plenty of
+00025e30: 206d 656d 6f72 7920 696e 2079 6f75 7220   memory in your 
+00025e40: 6d61 6368 696e 6521 0a20 2020 2023 2323  machine!.    ###
 00025e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00025e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00025e70: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
-00025e80: 2020 2222 220a 2020 2020 4d41 585f 4e55    """.    MAX_NU
-00025e90: 4d5f 574f 5244 5320 3d20 3130 3030 3030  M_WORDS = 100000
-00025ea0: 0a20 2020 2067 6c6f 7665 5f70 6174 6820  .    glove_path 
-00025eb0: 3d20 5061 7468 2867 6c6f 7665 5f66 696c  = Path(glove_fil
-00025ec0: 656e 616d 655f 7769 7468 5f70 6174 6829  ename_with_path)
-00025ed0: 0a20 2020 2070 7269 6e74 2827 2020 2020  .    print('    
-00025ee0: 4372 6561 7469 6e67 2065 6d62 6564 6469  Creating embeddi
-00025ef0: 6e67 732e 2054 6869 7320 7769 6c6c 2074  ngs. This will t
-00025f00: 616b 6520 7469 6d65 2e2e 2e27 290a 2020  ake time...').  
-00025f10: 2020 656d 6265 6464 696e 6773 5f69 6e64    embeddings_ind
-00025f20: 6578 203d 2064 6963 7428 290a 2020 2020  ex = dict().    
-00025f30: 666f 7220 6c69 6e65 2069 6e20 676c 6f76  for line in glov
-00025f40: 655f 7061 7468 2e6f 7065 6e28 656e 636f  e_path.open(enco
-00025f50: 6469 6e67 3d27 6c61 7469 6e31 2729 3a0a  ding='latin1'):.
-00025f60: 2020 2020 2020 2020 7661 6c75 6573 203d          values =
-00025f70: 206c 696e 652e 7370 6c69 7428 290a 2020   line.split().  
-00025f80: 2020 2020 2020 776f 7264 203d 2076 616c        word = val
-00025f90: 7565 735b 305d 0a20 2020 2020 2020 2074  ues[0].        t
-00025fa0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00025fb0: 636f 6566 7320 3d20 6e70 2e61 7361 7272  coefs = np.asarr
-00025fc0: 6179 2876 616c 7565 735b 313a 5d2c 2064  ay(values[1:], d
-00025fd0: 7479 7065 3d27 666c 6f61 7433 3227 290a  type='float32').
-00025fe0: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00025ff0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00026000: 696e 7565 0a20 2020 2020 2020 2065 6d62  inue.        emb
-00026010: 6564 6469 6e67 735f 696e 6465 785b 776f  eddings_index[wo
-00026020: 7264 5d20 3d20 636f 6566 730a 2020 2020  rd] = coefs.    
-00026030: 7072 696e 7428 274c 6f61 6465 6420 7b3a  print('Loaded {:
-00026040: 2c64 7d20 476c 6f76 6520 7665 6374 6f72  ,d} Glove vector
-00026050: 732e 272e 666f 726d 6174 286c 656e 2865  s.'.format(len(e
-00026060: 6d62 6564 6469 6e67 735f 696e 6465 7829  mbeddings_index)
-00026070: 2929 0a20 2020 2023 5468 6572 6520 6172  )).    #There ar
-00026080: 6520 6172 6f75 6e64 2033 3430 2c30 3030  e around 340,000
-00026090: 2077 6f72 6420 7665 6374 6f72 7320 7468   word vectors th
-000260a0: 6174 2077 6520 7573 6520 746f 2063 7265  at we use to cre
-000260b0: 6174 6520 616e 2065 6d62 6564 6469 6e67  ate an embedding
-000260c0: 206d 6174 7269 780a 2020 2020 2320 7468   matrix.    # th
-000260d0: 6174 206d 6174 6368 6573 2074 6865 2076  at matches the v
-000260e0: 6f63 6162 756c 6172 7920 736f 2074 6861  ocabulary so tha
-000260f0: 7420 7468 6520 524e 4e20 6d6f 6465 6c20  t the RNN model 
-00026100: 6361 6e20 6163 6365 7373 2065 6d62 6564  can access embed
-00026110: 6469 6e67 7320 6279 2074 6865 2074 6f6b  dings by the tok
-00026120: 656e 2069 6e64 6578 0a20 2020 2023 2070  en index.    # p
-00026130: 7265 7061 7265 2065 6d62 6564 6469 6e67  repare embedding
-00026140: 206d 6174 7269 780a 2020 2020 776f 7264   matrix.    word
-00026150: 5f69 6e64 6578 203d 2074 6f6b 656e 697a  _index = tokeniz
-00026160: 6564 2e77 6f72 645f 696e 6465 780a 2020  ed.word_index.  
-00026170: 2020 656d 6265 6464 696e 675f 6d61 7472    embedding_matr
-00026180: 6978 203d 206e 702e 7a65 726f 7328 2876  ix = np.zeros((v
-00026190: 6f63 6162 5f73 697a 652c 2067 6c6f 7665  ocab_size, glove
-000261a0: 5f64 696d 656e 7369 6f6e 2929 0a20 2020  _dimension)).   
-000261b0: 2070 7269 6e74 2827 5072 6570 6172 696e   print('Preparin
-000261c0: 6720 656d 6265 6464 696e 6720 6d61 7472  g embedding matr
-000261d0: 6978 2e27 290a 2020 2020 666f 7220 776f  ix.').    for wo
-000261e0: 7264 2c20 6920 696e 2077 6f72 645f 696e  rd, i in word_in
-000261f0: 6465 782e 6974 656d 7328 293a 0a20 2020  dex.items():.   
-00026200: 2020 2020 2069 6620 6920 3e3d 204d 4158       if i >= MAX
-00026210: 5f4e 554d 5f57 4f52 4453 3a0a 2020 2020  _NUM_WORDS:.    
-00026220: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00026230: 0a20 2020 2020 2020 2065 6d62 6564 6469  .        embeddi
-00026240: 6e67 5f76 6563 746f 7220 3d20 656d 6265  ng_vector = embe
-00026250: 6464 696e 6773 5f69 6e64 6578 2e67 6574  ddings_index.get
-00026260: 2877 6f72 6429 0a20 2020 2020 2020 2069  (word).        i
-00026270: 6620 656d 6265 6464 696e 675f 7665 6374  f embedding_vect
-00026280: 6f72 2069 7320 6e6f 7420 4e6f 6e65 3a0a  or is not None:.
-00026290: 2020 2020 2020 2020 2020 2020 2320 776f              # wo
-000262a0: 7264 7320 6e6f 7420 666f 756e 6420 696e  rds not found in
-000262b0: 2065 6d62 6564 6469 6e67 2069 6e64 6578   embedding index
-000262c0: 2077 696c 6c20 6265 2061 6c6c 2d7a 6572   will be all-zer
-000262d0: 6f73 2e0a 2020 2020 2020 2020 2020 2020  os..            
-000262e0: 656d 6265 6464 696e 675f 6d61 7472 6978  embedding_matrix
-000262f0: 5b69 5d20 3d20 656d 6265 6464 696e 675f  [i] = embedding_
-00026300: 7665 6374 6f72 0a20 2020 2070 7269 6e74  vector.    print
-00026310: 2827 2020 2020 436f 6d70 6c65 7465 642e  ('    Completed.
-00026320: 2729 0a20 2020 2072 6574 7572 6e20 656d  ').    return em
-00026330: 6265 6464 696e 675f 6d61 7472 6978 2c20  bedding_matrix, 
-00026340: 676c 6f76 655f 6469 6d65 6e73 696f 6e0a  glove_dimension.
-00026350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025e90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00025ea0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00025eb0: 2020 2020 2222 220a 2020 2020 4d41 585f      """.    MAX_
+00025ec0: 4e55 4d5f 574f 5244 5320 3d20 3130 3030  NUM_WORDS = 1000
+00025ed0: 3030 0a20 2020 2067 6c6f 7665 5f70 6174  00.    glove_pat
+00025ee0: 6820 3d20 5061 7468 2867 6c6f 7665 5f66  h = Path(glove_f
+00025ef0: 696c 656e 616d 655f 7769 7468 5f70 6174  ilename_with_pat
+00025f00: 6829 0a20 2020 2070 7269 6e74 2827 2020  h).    print('  
+00025f10: 2020 4372 6561 7469 6e67 2065 6d62 6564    Creating embed
+00025f20: 6469 6e67 732e 2054 6869 7320 7769 6c6c  dings. This will
+00025f30: 2074 616b 6520 7469 6d65 2e2e 2e27 290a   take time...').
+00025f40: 2020 2020 656d 6265 6464 696e 6773 5f69      embeddings_i
+00025f50: 6e64 6578 203d 2064 6963 7428 290a 2020  ndex = dict().  
+00025f60: 2020 666f 7220 6c69 6e65 2069 6e20 676c    for line in gl
+00025f70: 6f76 655f 7061 7468 2e6f 7065 6e28 656e  ove_path.open(en
+00025f80: 636f 6469 6e67 3d27 6c61 7469 6e31 2729  coding='latin1')
+00025f90: 3a0a 2020 2020 2020 2020 7661 6c75 6573  :.        values
+00025fa0: 203d 206c 696e 652e 7370 6c69 7428 290a   = line.split().
+00025fb0: 2020 2020 2020 2020 776f 7264 203d 2076          word = v
+00025fc0: 616c 7565 735b 305d 0a20 2020 2020 2020  alues[0].       
+00025fd0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00025fe0: 2020 636f 6566 7320 3d20 6e70 2e61 7361    coefs = np.asa
+00025ff0: 7272 6179 2876 616c 7565 735b 313a 5d2c  rray(values[1:],
+00026000: 2064 7479 7065 3d27 666c 6f61 7433 3227   dtype='float32'
+00026010: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00026020: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+00026030: 6e74 696e 7565 0a20 2020 2020 2020 2065  ntinue.        e
+00026040: 6d62 6564 6469 6e67 735f 696e 6465 785b  mbeddings_index[
+00026050: 776f 7264 5d20 3d20 636f 6566 730a 2020  word] = coefs.  
+00026060: 2020 7072 696e 7428 274c 6f61 6465 6420    print('Loaded 
+00026070: 7b3a 2c64 7d20 476c 6f76 6520 7665 6374  {:,d} Glove vect
+00026080: 6f72 732e 272e 666f 726d 6174 286c 656e  ors.'.format(len
+00026090: 2865 6d62 6564 6469 6e67 735f 696e 6465  (embeddings_inde
+000260a0: 7829 2929 0a20 2020 2023 5468 6572 6520  x))).    #There 
+000260b0: 6172 6520 6172 6f75 6e64 2033 3430 2c30  are around 340,0
+000260c0: 3030 2077 6f72 6420 7665 6374 6f72 7320  00 word vectors 
+000260d0: 7468 6174 2077 6520 7573 6520 746f 2063  that we use to c
+000260e0: 7265 6174 6520 616e 2065 6d62 6564 6469  reate an embeddi
+000260f0: 6e67 206d 6174 7269 780a 2020 2020 2320  ng matrix.    # 
+00026100: 7468 6174 206d 6174 6368 6573 2074 6865  that matches the
+00026110: 2076 6f63 6162 756c 6172 7920 736f 2074   vocabulary so t
+00026120: 6861 7420 7468 6520 524e 4e20 6d6f 6465  hat the RNN mode
+00026130: 6c20 6361 6e20 6163 6365 7373 2065 6d62  l can access emb
+00026140: 6564 6469 6e67 7320 6279 2074 6865 2074  eddings by the t
+00026150: 6f6b 656e 2069 6e64 6578 0a20 2020 2023  oken index.    #
+00026160: 2070 7265 7061 7265 2065 6d62 6564 6469   prepare embeddi
+00026170: 6e67 206d 6174 7269 780a 2020 2020 776f  ng matrix.    wo
+00026180: 7264 5f69 6e64 6578 203d 2074 6f6b 656e  rd_index = token
+00026190: 697a 6564 2e77 6f72 645f 696e 6465 780a  ized.word_index.
+000261a0: 2020 2020 656d 6265 6464 696e 675f 6d61      embedding_ma
+000261b0: 7472 6978 203d 206e 702e 7a65 726f 7328  trix = np.zeros(
+000261c0: 2876 6f63 6162 5f73 697a 652c 2067 6c6f  (vocab_size, glo
+000261d0: 7665 5f64 696d 656e 7369 6f6e 2929 0a20  ve_dimension)). 
+000261e0: 2020 2070 7269 6e74 2827 5072 6570 6172     print('Prepar
+000261f0: 696e 6720 656d 6265 6464 696e 6720 6d61  ing embedding ma
+00026200: 7472 6978 2e27 290a 2020 2020 666f 7220  trix.').    for 
+00026210: 776f 7264 2c20 6920 696e 2077 6f72 645f  word, i in word_
+00026220: 696e 6465 782e 6974 656d 7328 293a 0a20  index.items():. 
+00026230: 2020 2020 2020 2069 6620 6920 3e3d 204d         if i >= M
+00026240: 4158 5f4e 554d 5f57 4f52 4453 3a0a 2020  AX_NUM_WORDS:.  
+00026250: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00026260: 7565 0a20 2020 2020 2020 2065 6d62 6564  ue.        embed
+00026270: 6469 6e67 5f76 6563 746f 7220 3d20 656d  ding_vector = em
+00026280: 6265 6464 696e 6773 5f69 6e64 6578 2e67  beddings_index.g
+00026290: 6574 2877 6f72 6429 0a20 2020 2020 2020  et(word).       
+000262a0: 2069 6620 656d 6265 6464 696e 675f 7665   if embedding_ve
+000262b0: 6374 6f72 2069 7320 6e6f 7420 4e6f 6e65  ctor is not None
+000262c0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+000262d0: 776f 7264 7320 6e6f 7420 666f 756e 6420  words not found 
+000262e0: 696e 2065 6d62 6564 6469 6e67 2069 6e64  in embedding ind
+000262f0: 6578 2077 696c 6c20 6265 2061 6c6c 2d7a  ex will be all-z
+00026300: 6572 6f73 2e0a 2020 2020 2020 2020 2020  eros..          
+00026310: 2020 656d 6265 6464 696e 675f 6d61 7472    embedding_matr
+00026320: 6978 5b69 5d20 3d20 656d 6265 6464 696e  ix[i] = embeddin
+00026330: 675f 7665 6374 6f72 0a20 2020 2070 7269  g_vector.    pri
+00026340: 6e74 2827 2020 2020 436f 6d70 6c65 7465  nt('    Complete
+00026350: 642e 2729 0a20 2020 2072 6574 7572 6e20  d.').    return 
+00026360: 656d 6265 6464 696e 675f 6d61 7472 6978  embedding_matrix
+00026370: 2c20 676c 6f76 655f 6469 6d65 6e73 696f  , glove_dimensio
+00026380: 6e0a 2323 2323 2323 2323 2323 2323 2323  n.##############
 00026390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000263a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000263b0: 2323 2323 230a 696d 706f 7274 2063 6f70  #####.import cop
-000263c0: 790a 6465 6620 4645 5f63 6f6e 7665 7274  y.def FE_convert
-000263d0: 5f6d 6978 6564 5f64 6174 6174 7970 6573  _mixed_datatypes
-000263e0: 5f74 6f5f 7374 7269 6e67 2864 6629 3a0a  _to_string(df):.
-000263f0: 2020 2020 6466 203d 2063 6f70 792e 6465      df = copy.de
-00026400: 6570 636f 7079 2864 6629 0a20 2020 2066  epcopy(df).    f
-00026410: 6f72 2063 6f6c 2069 6e20 6466 2e63 6f6c  or col in df.col
-00026420: 756d 6e73 3a0a 2020 2020 2020 2020 6966  umns:.        if
-00026430: 206c 656e 2864 665b 636f 6c5d 2e61 7070   len(df[col].app
-00026440: 6c79 2874 7970 6529 2e76 616c 7565 5f63  ly(type).value_c
-00026450: 6f75 6e74 7328 2929 203e 2031 3a0a 2020  ounts()) > 1:.  
-00026460: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00026470: 274d 6978 6564 2064 6174 6120 7479 7065  'Mixed data type
-00026480: 2064 6574 6563 7465 6420 696e 2025 7320   detected in %s 
-00026490: 636f 6c75 6d6e 2e20 436f 6e76 6572 7469  column. Converti
-000264a0: 6e67 2061 6c6c 2072 6f77 7320 746f 2073  ng all rows to s
-000264b0: 7472 696e 6720 7479 7065 206e 6f77 2e2e  tring type now..
-000264c0: 2e27 2025 636f 6c29 0a20 2020 2020 2020  .' %col).       
-000264d0: 2020 2020 2064 665b 636f 6c5d 203d 2064       df[col] = d
-000264e0: 665b 636f 6c5d 2e6d 6170 286c 616d 6264  f[col].map(lambd
-000264f0: 6120 783a 2078 2069 6620 6973 696e 7374  a x: x if isinst
-00026500: 616e 6365 2878 2c20 7374 7229 2065 6c73  ance(x, str) els
-00026510: 6520 7374 7228 7829 292e 7661 6c75 6573  e str(x)).values
-00026520: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00026530: 6c65 6e28 6466 5b63 6f6c 5d2e 6170 706c  len(df[col].appl
-00026540: 7928 7479 7065 292e 7661 6c75 655f 636f  y(type).value_co
-00026550: 756e 7473 2829 2920 3d3d 2031 3a0a 2020  unts()) == 1:.  
-00026560: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00026570: 696e 7428 2720 2020 2063 6f6d 706c 6574  int('    complet
-00026580: 6564 2e27 290a 2020 2020 2020 2020 2020  ed.').          
-00026590: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000265a0: 2020 2020 2020 2020 7072 696e 7428 2720          print(' 
-000265b0: 2020 2063 6f75 6c64 206e 6f74 2063 6861     could not cha
-000265c0: 6e67 6520 636f 6c75 6d6e 2074 7970 652e  nge column type.
-000265d0: 2046 6978 2069 7420 6d61 6e75 616c 6c79   Fix it manually
-000265e0: 2061 6e64 2074 6865 6e20 7265 2d72 756e   and then re-run
-000265f0: 2045 4441 2e27 290a 2020 2020 7265 7475   EDA.').    retu
-00026600: 726e 2064 660a 2323 2323 2323 2323 2323  rn df.##########
-00026610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000263b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000263c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000263d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000263e0: 2323 2323 2323 230a 696d 706f 7274 2063  #######.import c
+000263f0: 6f70 790a 6465 6620 4645 5f63 6f6e 7665  opy.def FE_conve
+00026400: 7274 5f6d 6978 6564 5f64 6174 6174 7970  rt_mixed_datatyp
+00026410: 6573 5f74 6f5f 7374 7269 6e67 2864 6629  es_to_string(df)
+00026420: 3a0a 2020 2020 6466 203d 2063 6f70 792e  :.    df = copy.
+00026430: 6465 6570 636f 7079 2864 6629 0a20 2020  deepcopy(df).   
+00026440: 2066 6f72 2063 6f6c 2069 6e20 6466 2e63   for col in df.c
+00026450: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
+00026460: 6966 206c 656e 2864 665b 636f 6c5d 2e61  if len(df[col].a
+00026470: 7070 6c79 2874 7970 6529 2e76 616c 7565  pply(type).value
+00026480: 5f63 6f75 6e74 7328 2929 203e 2031 3a0a  _counts()) > 1:.
+00026490: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000264a0: 7428 274d 6978 6564 2064 6174 6120 7479  t('Mixed data ty
+000264b0: 7065 2064 6574 6563 7465 6420 696e 2025  pe detected in %
+000264c0: 7320 636f 6c75 6d6e 2e20 436f 6e76 6572  s column. Conver
+000264d0: 7469 6e67 2061 6c6c 2072 6f77 7320 746f  ting all rows to
+000264e0: 2073 7472 696e 6720 7479 7065 206e 6f77   string type now
+000264f0: 2e2e 2e27 2025 636f 6c29 0a20 2020 2020  ...' %col).     
+00026500: 2020 2020 2020 2064 665b 636f 6c5d 203d         df[col] =
+00026510: 2064 665b 636f 6c5d 2e6d 6170 286c 616d   df[col].map(lam
+00026520: 6264 6120 783a 2078 2069 6620 6973 696e  bda x: x if isin
+00026530: 7374 616e 6365 2878 2c20 7374 7229 2065  stance(x, str) e
+00026540: 6c73 6520 7374 7228 7829 292e 7661 6c75  lse str(x)).valu
+00026550: 6573 0a20 2020 2020 2020 2020 2020 2069  es.            i
+00026560: 6620 6c65 6e28 6466 5b63 6f6c 5d2e 6170  f len(df[col].ap
+00026570: 706c 7928 7479 7065 292e 7661 6c75 655f  ply(type).value_
+00026580: 636f 756e 7473 2829 2920 3d3d 2031 3a0a  counts()) == 1:.
+00026590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265a0: 7072 696e 7428 2720 2020 2063 6f6d 706c  print('    compl
+000265b0: 6574 6564 2e27 290a 2020 2020 2020 2020  eted.').        
+000265c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000265d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000265e0: 2720 2020 2063 6f75 6c64 206e 6f74 2063  '    could not c
+000265f0: 6861 6e67 6520 636f 6c75 6d6e 2074 7970  hange column typ
+00026600: 652e 2046 6978 2069 7420 6d61 6e75 616c  e. Fix it manual
+00026610: 6c79 2061 6e64 2074 6865 6e20 7265 2d72  ly and then re-r
+00026620: 756e 2045 4441 2e27 290a 2020 2020 7265  un EDA.').    re
+00026630: 7475 726e 2064 660a 2323 2323 2323 2323  turn df.########
 00026640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026650: 2323 2323 2323 2323 0a64 6566 2072 656d  ########.def rem
-00026660: 6f76 655f 6475 706c 6963 6174 655f 636f  ove_duplicate_co
-00026670: 6c73 5f69 6e5f 6461 7461 7365 7428 6466  ls_in_dataset(df
-00026680: 293a 0a20 2020 2064 6620 3d20 636f 7079  ):.    df = copy
-00026690: 2e64 6565 7063 6f70 7928 6466 290a 2020  .deepcopy(df).  
-000266a0: 2020 6e75 6d62 6572 5f64 7570 6c69 6361    number_duplica
-000266b0: 7465 7320 3d20 6466 2e63 6f6c 756d 6e73  tes = df.columns
-000266c0: 2e64 7570 6c69 6361 7465 6428 292e 6173  .duplicated().as
-000266d0: 7479 7065 2869 6e74 292e 7375 6d28 290a  type(int).sum().
-000266e0: 2020 2020 6475 706c 6963 6174 6573 203d      duplicates =
-000266f0: 2064 662e 636f 6c75 6d6e 735b 6466 2e63   df.columns[df.c
-00026700: 6f6c 756d 6e73 2e64 7570 6c69 6361 7465  olumns.duplicate
-00026710: 6428 295d 0a20 2020 2069 6620 206e 756d  d()].    if  num
-00026720: 6265 725f 6475 706c 6963 6174 6573 203e  ber_duplicates >
-00026730: 2030 3a0a 2020 2020 2020 2020 7072 696e   0:.        prin
-00026740: 7428 2752 656d 6f76 696e 6720 2564 2064  t('Removing %d d
-00026750: 7570 6c69 6361 7465 2063 6f6c 756d 6e28  uplicate column(
-00026760: 7329 206f 6620 2573 2720 2528 6e75 6d62  s) of %s' %(numb
-00026770: 6572 5f64 7570 6c69 6361 7465 732c 2064  er_duplicates, d
-00026780: 7570 6c69 6361 7465 7329 290a 2020 2020  uplicates)).    
-00026790: 2020 2020 6466 203d 2064 662e 6c6f 635b      df = df.loc[
-000267a0: 3a2c 7e64 662e 636f 6c75 6d6e 732e 6475  :,~df.columns.du
-000267b0: 706c 6963 6174 6564 2829 5d0a 2020 2020  plicated()].    
-000267c0: 7265 7475 726e 2064 660a 2323 2323 2323  return df.######
-000267d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000267e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000267f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026680: 2323 2323 2323 2323 2323 0a64 6566 2072  ##########.def r
+00026690: 656d 6f76 655f 6475 706c 6963 6174 655f  emove_duplicate_
+000266a0: 636f 6c73 5f69 6e5f 6461 7461 7365 7428  cols_in_dataset(
+000266b0: 6466 293a 0a20 2020 2064 6620 3d20 636f  df):.    df = co
+000266c0: 7079 2e64 6565 7063 6f70 7928 6466 290a  py.deepcopy(df).
+000266d0: 2020 2020 6e75 6d62 6572 5f64 7570 6c69      number_dupli
+000266e0: 6361 7465 7320 3d20 6466 2e63 6f6c 756d  cates = df.colum
+000266f0: 6e73 2e64 7570 6c69 6361 7465 6428 292e  ns.duplicated().
+00026700: 6173 7479 7065 2869 6e74 292e 7375 6d28  astype(int).sum(
+00026710: 290a 2020 2020 6475 706c 6963 6174 6573  ).    duplicates
+00026720: 203d 2064 662e 636f 6c75 6d6e 735b 6466   = df.columns[df
+00026730: 2e63 6f6c 756d 6e73 2e64 7570 6c69 6361  .columns.duplica
+00026740: 7465 6428 295d 0a20 2020 2069 6620 206e  ted()].    if  n
+00026750: 756d 6265 725f 6475 706c 6963 6174 6573  umber_duplicates
+00026760: 203e 2030 3a0a 2020 2020 2020 2020 7072   > 0:.        pr
+00026770: 696e 7428 2752 656d 6f76 696e 6720 2564  int('Removing %d
+00026780: 2064 7570 6c69 6361 7465 2063 6f6c 756d   duplicate colum
+00026790: 6e28 7329 206f 6620 2573 2720 2528 6e75  n(s) of %s' %(nu
+000267a0: 6d62 6572 5f64 7570 6c69 6361 7465 732c  mber_duplicates,
+000267b0: 2064 7570 6c69 6361 7465 7329 290a 2020   duplicates)).  
+000267c0: 2020 2020 2020 6466 203d 2064 662e 6c6f        df = df.lo
+000267d0: 635b 3a2c 7e64 662e 636f 6c75 6d6e 732e  c[:,~df.columns.
+000267e0: 6475 706c 6963 6174 6564 2829 5d0a 2020  duplicated()].  
+000267f0: 2020 7265 7475 726e 2064 660a 2323 2323    return df.####
 00026800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026810: 2323 2323 230a 6465 6620 4645 5f73 706c  #####.def FE_spl
-00026820: 6974 5f6c 6973 745f 696e 746f 5f63 6f6c  it_list_into_col
-00026830: 756d 6e73 2864 662c 2063 6f6c 2c20 636f  umns(df, col, co
-00026840: 6c73 5f69 6e3d 5b5d 293a 0a20 2020 2022  ls_in=[]):.    "
-00026850: 2222 0a20 2020 2054 6869 7320 6973 2061  "".    This is a
-00026860: 2046 6561 7475 7265 2045 6e67 696e 6565   Feature Enginee
-00026870: 7269 6e67 2066 756e 6374 696f 6e2e 2049  ring function. I
-00026880: 7420 7769 6c6c 2061 7574 6f6d 6174 6963  t will automatic
-00026890: 616c 6c79 2064 6574 6563 7420 6f62 6a65  ally detect obje
-000268a0: 6374 2076 6172 6961 626c 6573 2074 6861  ct variables tha
-000268b0: 7420 636f 6e74 6169 6e20 6c69 7374 730a  t contain lists.
-000268c0: 2020 2020 616e 6420 636f 6e76 6572 7420      and convert 
-000268d0: 7468 656d 2069 6e74 6f20 6e65 7720 636f  them into new co
-000268e0: 6c75 6d6e 732e 2059 6f75 206e 6565 6420  lumns. You need 
-000268f0: 746f 2070 726f 7669 6465 2074 6865 2064  to provide the d
-00026900: 6174 6166 7261 6d65 2c20 7468 6520 6e61  ataframe, the na
-00026910: 6d65 206f 6620 7468 6520 6f62 6a65 6374  me of the object
-00026920: 2063 6f6c 756d 6e2e 0a20 2020 204f 7074   column..    Opt
-00026930: 696f 6e61 6c6c 792c 2079 6f75 2063 616e  ionally, you can
-00026940: 2064 6563 6964 6520 746f 2073 656e 6420   decide to send 
-00026950: 7468 6520 6e61 6d65 7320 6f66 2074 6865  the names of the
-00026960: 206e 6577 2063 6f6c 756d 6e73 2079 6f75   new columns you
-00026970: 2077 616e 7420 746f 2063 7265 6174 6520   want to create 
-00026980: 6173 2063 6f6c 735f 696e 2e0a 2020 2020  as cols_in..    
-00026990: 4974 2077 696c 6c20 7265 7475 726e 2074  It will return t
-000269a0: 6865 2064 6174 6166 7261 6d65 2077 6974  he dataframe wit
-000269b0: 6820 6164 6469 7469 6f6e 616c 2063 6f6c  h additional col
-000269c0: 756d 6e73 2e20 4974 2077 696c 6c20 6472  umns. It will dr
-000269d0: 6f70 2074 6865 2063 6f6c 756d 6e20 7768  op the column wh
-000269e0: 6963 6820 796f 7520 7365 6e74 2069 6e20  ich you sent in 
-000269f0: 6173 2069 6e70 7574 2e0a 0a20 2020 2049  as input...    I
-00026a00: 6e70 7574 733a 0a20 2020 202d 2d2d 2d2d  nputs:.    -----
-00026a10: 2d2d 2d0a 2020 2020 6466 3a20 7061 6e64  ---.    df: pand
-00026a20: 6173 2064 6174 6166 7261 6d65 0a20 2020  as dataframe.   
-00026a30: 2063 6f6c 3a20 6e61 6d65 206f 6620 7468   col: name of th
-00026a40: 6520 6f62 6a65 6374 2063 6f6c 756d 6e20  e object column 
-00026a50: 7468 6174 2063 6f6e 7461 696e 7320 6120  that contains a 
-00026a60: 6c69 7374 2e20 5265 6d65 6d62 6572 2069  list. Remember i
-00026a70: 7420 6d75 7374 2062 6520 6120 6c69 7374  t must be a list
-00026a80: 2061 6e64 206e 6f74 2061 2073 7472 696e   and not a strin
-00026a90: 672e 0a20 2020 2063 6f6c 735f 696e 3a20  g..    cols_in: 
-00026aa0: 6e61 6d65 7320 6f66 2074 6865 2063 6f6c  names of the col
-00026ab0: 756d 6e73 2079 6f75 2077 616e 7420 746f  umns you want to
-00026ac0: 2063 7265 6174 652e 2049 6620 7468 6520   create. If the 
-00026ad0: 6e75 6d62 6572 206f 6620 636f 6c75 6d6e  number of column
-00026ae0: 7320 6973 206c 6573 7320 7468 616e 206c  s is less than l
-00026af0: 6973 7420 6c65 6e67 7468 2c0a 2020 2020  ist length,.    
-00026b00: 2020 2020 2020 2020 2069 7420 7769 6c6c           it will
-00026b10: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
-00026b20: 686f 6f73 6520 6f6e 6c79 2074 6865 2066  hoose only the f
-00026b30: 6973 7420 6665 7720 6974 656d 7320 6f66  ist few items of
-00026b40: 2074 6865 206c 6973 7420 746f 206d 6174   the list to mat
-00026b50: 6368 2074 6865 206c 656e 6774 6820 6f66  ch the length of
-00026b60: 2063 6f6c 735f 696e 2e0a 2020 2020 0a20   cols_in..    . 
-00026b70: 2020 204f 7574 7075 7473 3a0a 2020 2020     Outputs:.    
-00026b80: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6466  ---------.    df
-00026b90: 3a20 7061 6e64 6173 2064 6174 6166 7261  : pandas datafra
-00026ba0: 6d65 2077 6974 6820 6e65 7720 636f 6c75  me with new colu
-00026bb0: 6d6e 7320 616e 6420 7769 7468 6f75 7420  mns and without 
-00026bc0: 7468 6520 636f 6c75 6d6e 2079 6f75 2073  the column you s
-00026bd0: 656e 7420 696e 2061 7320 696e 7075 742e  ent in as input.
-00026be0: 0a20 2020 2022 2222 0a20 2020 2064 6620  .    """.    df 
-00026bf0: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
-00026c00: 6466 290a 2020 2020 6966 2063 6f6c 735f  df).    if cols_
-00026c10: 696e 3a0a 2020 2020 2020 2020 6d61 785f  in:.        max_
-00026c20: 636f 6c5f 6c65 6e67 7468 203d 206c 656e  col_length = len
-00026c30: 2863 6f6c 735f 696e 290a 2020 2020 2020  (cols_in).      
-00026c40: 2020 6466 5b63 6f6c 735f 696e 5d20 3d20    df[cols_in] = 
-00026c50: 6466 5b63 6f6c 5d2e 6170 706c 7928 7064  df[col].apply(pd
-00026c60: 2e53 6572 6965 7329 2e76 616c 7565 735b  .Series).values[
-00026c70: 3a2c 3a6d 6178 5f63 6f6c 5f6c 656e 6774  :,:max_col_lengt
-00026c80: 685d 0a20 2020 2020 2020 2064 6620 3d20  h].        df = 
-00026c90: 6466 2e64 726f 7028 636f 6c2c 6178 6973  df.drop(col,axis
-00026ca0: 3d31 290a 2020 2020 656c 7365 3a0a 2020  =1).    else:.  
-00026cb0: 2020 2020 2020 6966 206c 656e 2864 665b        if len(df[
-00026cc0: 636f 6c5d 2e6d 6170 2874 7970 6529 2e76  col].map(type).v
-00026cd0: 616c 7565 5f63 6f75 6e74 7328 2929 3d3d  alue_counts())==
-00026ce0: 3120 616e 6420 6466 5b63 6f6c 5d2e 6d61  1 and df[col].ma
-00026cf0: 7028 7479 7065 292e 7661 6c75 655f 636f  p(type).value_co
-00026d00: 756e 7473 2829 2e69 6e64 6578 5b30 5d3d  unts().index[0]=
-00026d10: 3d6c 6973 743a 0a20 2020 2020 2020 2020  =list:.         
-00026d20: 2020 2023 2323 2052 656d 656d 6265 7220     ### Remember 
-00026d30: 7468 6174 2066 696c 6c6e 6120 6f6e 6c79  that fillna only
-00026d40: 2077 6f72 6b73 2061 7420 6461 7461 6672   works at datafr
-00026d50: 616d 6520 6c65 7665 6c21 2023 2323 0a20  ame level! ###. 
-00026d60: 2020 2020 2020 2020 2020 206d 6178 5f63             max_c
-00026d70: 6f6c 5f6c 656e 6774 6820 3d20 6466 5b5b  ol_length = df[[
-00026d80: 636f 6c5d 5d2e 6669 6c6c 6e61 2827 6d69  col]].fillna('mi
-00026d90: 7373 696e 6727 292e 6d61 7028 6c65 6e29  ssing').map(len)
-00026da0: 2e6d 6178 2829 0a20 2020 2020 2020 2020  .max().         
-00026db0: 2020 2063 6f6c 7320 3d20 5b63 6f6c 2b27     cols = [col+'
-00026dc0: 5f27 2b73 7472 2869 2920 666f 7220 6920  _'+str(i) for i 
-00026dd0: 696e 2072 616e 6765 286d 6178 5f63 6f6c  in range(max_col
-00026de0: 5f6c 656e 6774 6829 5d0a 2020 2020 2020  _length)].      
-00026df0: 2020 2020 2020 6466 5b63 6f6c 735d 203d        df[cols] =
-00026e00: 2064 665b 636f 6c5d 2e61 7070 6c79 2870   df[col].apply(p
-00026e10: 642e 5365 7269 6573 290a 2020 2020 2020  d.Series).      
-00026e20: 2020 2020 2020 6466 203d 2064 662e 6472        df = df.dr
-00026e30: 6f70 2863 6f6c 2c61 7869 733d 3129 0a20  op(col,axis=1). 
-00026e40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00026e50: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00026e60: 436f 6c75 6d6e 2025 7320 646f 6573 206e  Column %s does n
-00026e70: 6f74 2063 6f6e 7461 696e 206c 6973 7473  ot contain lists
-00026e80: 206f 7220 6861 7320 6d69 7865 6420 7479   or has mixed ty
-00026e90: 7065 7320 6f74 6865 7220 7468 616e 206c  pes other than l
-00026ea0: 6973 7473 2e20 4669 7820 6974 2061 6e64  ists. Fix it and
-00026eb0: 2072 6572 756e 2e27 2025 636f 6c29 0a20   rerun.' %col). 
-00026ec0: 2020 2072 6574 7572 6e20 6466 0a23 2323     return df.###
-00026ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026840: 2323 2323 2323 230a 6465 6620 4645 5f73  #######.def FE_s
+00026850: 706c 6974 5f6c 6973 745f 696e 746f 5f63  plit_list_into_c
+00026860: 6f6c 756d 6e73 2864 662c 2063 6f6c 2c20  olumns(df, col, 
+00026870: 636f 6c73 5f69 6e3d 5b5d 293a 0a20 2020  cols_in=[]):.   
+00026880: 2022 2222 0a20 2020 2054 6869 7320 6973   """.    This is
+00026890: 2061 2046 6561 7475 7265 2045 6e67 696e   a Feature Engin
+000268a0: 6565 7269 6e67 2066 756e 6374 696f 6e2e  eering function.
+000268b0: 2049 7420 7769 6c6c 2061 7574 6f6d 6174   It will automat
+000268c0: 6963 616c 6c79 2064 6574 6563 7420 6f62  ically detect ob
+000268d0: 6a65 6374 2076 6172 6961 626c 6573 2074  ject variables t
+000268e0: 6861 7420 636f 6e74 6169 6e20 6c69 7374  hat contain list
+000268f0: 730a 2020 2020 616e 6420 636f 6e76 6572  s.    and conver
+00026900: 7420 7468 656d 2069 6e74 6f20 6e65 7720  t them into new 
+00026910: 636f 6c75 6d6e 732e 2059 6f75 206e 6565  columns. You nee
+00026920: 6420 746f 2070 726f 7669 6465 2074 6865  d to provide the
+00026930: 2064 6174 6166 7261 6d65 2c20 7468 6520   dataframe, the 
+00026940: 6e61 6d65 206f 6620 7468 6520 6f62 6a65  name of the obje
+00026950: 6374 2063 6f6c 756d 6e2e 0a20 2020 204f  ct column..    O
+00026960: 7074 696f 6e61 6c6c 792c 2079 6f75 2063  ptionally, you c
+00026970: 616e 2064 6563 6964 6520 746f 2073 656e  an decide to sen
+00026980: 6420 7468 6520 6e61 6d65 7320 6f66 2074  d the names of t
+00026990: 6865 206e 6577 2063 6f6c 756d 6e73 2079  he new columns y
+000269a0: 6f75 2077 616e 7420 746f 2063 7265 6174  ou want to creat
+000269b0: 6520 6173 2063 6f6c 735f 696e 2e0a 2020  e as cols_in..  
+000269c0: 2020 4974 2077 696c 6c20 7265 7475 726e    It will return
+000269d0: 2074 6865 2064 6174 6166 7261 6d65 2077   the dataframe w
+000269e0: 6974 6820 6164 6469 7469 6f6e 616c 2063  ith additional c
+000269f0: 6f6c 756d 6e73 2e20 4974 2077 696c 6c20  olumns. It will 
+00026a00: 6472 6f70 2074 6865 2063 6f6c 756d 6e20  drop the column 
+00026a10: 7768 6963 6820 796f 7520 7365 6e74 2069  which you sent i
+00026a20: 6e20 6173 2069 6e70 7574 2e0a 0a20 2020  n as input...   
+00026a30: 2049 6e70 7574 733a 0a20 2020 202d 2d2d   Inputs:.    ---
+00026a40: 2d2d 2d2d 2d0a 2020 2020 6466 3a20 7061  -----.    df: pa
+00026a50: 6e64 6173 2064 6174 6166 7261 6d65 0a20  ndas dataframe. 
+00026a60: 2020 2063 6f6c 3a20 6e61 6d65 206f 6620     col: name of 
+00026a70: 7468 6520 6f62 6a65 6374 2063 6f6c 756d  the object colum
+00026a80: 6e20 7468 6174 2063 6f6e 7461 696e 7320  n that contains 
+00026a90: 6120 6c69 7374 2e20 5265 6d65 6d62 6572  a list. Remember
+00026aa0: 2069 7420 6d75 7374 2062 6520 6120 6c69   it must be a li
+00026ab0: 7374 2061 6e64 206e 6f74 2061 2073 7472  st and not a str
+00026ac0: 696e 672e 0a20 2020 2063 6f6c 735f 696e  ing..    cols_in
+00026ad0: 3a20 6e61 6d65 7320 6f66 2074 6865 2063  : names of the c
+00026ae0: 6f6c 756d 6e73 2079 6f75 2077 616e 7420  olumns you want 
+00026af0: 746f 2063 7265 6174 652e 2049 6620 7468  to create. If th
+00026b00: 6520 6e75 6d62 6572 206f 6620 636f 6c75  e number of colu
+00026b10: 6d6e 7320 6973 206c 6573 7320 7468 616e  mns is less than
+00026b20: 206c 6973 7420 6c65 6e67 7468 2c0a 2020   list length,.  
+00026b30: 2020 2020 2020 2020 2020 2069 7420 7769             it wi
+00026b40: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00026b50: 2063 686f 6f73 6520 6f6e 6c79 2074 6865   choose only the
+00026b60: 2066 6973 7420 6665 7720 6974 656d 7320   fist few items 
+00026b70: 6f66 2074 6865 206c 6973 7420 746f 206d  of the list to m
+00026b80: 6174 6368 2074 6865 206c 656e 6774 6820  atch the length 
+00026b90: 6f66 2063 6f6c 735f 696e 2e0a 2020 2020  of cols_in..    
+00026ba0: 0a20 2020 204f 7574 7075 7473 3a0a 2020  .    Outputs:.  
+00026bb0: 2020 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020    ---------.    
+00026bc0: 6466 3a20 7061 6e64 6173 2064 6174 6166  df: pandas dataf
+00026bd0: 7261 6d65 2077 6974 6820 6e65 7720 636f  rame with new co
+00026be0: 6c75 6d6e 7320 616e 6420 7769 7468 6f75  lumns and withou
+00026bf0: 7420 7468 6520 636f 6c75 6d6e 2079 6f75  t the column you
+00026c00: 2073 656e 7420 696e 2061 7320 696e 7075   sent in as inpu
+00026c10: 742e 0a20 2020 2022 2222 0a20 2020 2064  t..    """.    d
+00026c20: 6620 3d20 636f 7079 2e64 6565 7063 6f70  f = copy.deepcop
+00026c30: 7928 6466 290a 2020 2020 6966 2063 6f6c  y(df).    if col
+00026c40: 735f 696e 3a0a 2020 2020 2020 2020 6d61  s_in:.        ma
+00026c50: 785f 636f 6c5f 6c65 6e67 7468 203d 206c  x_col_length = l
+00026c60: 656e 2863 6f6c 735f 696e 290a 2020 2020  en(cols_in).    
+00026c70: 2020 2020 6466 5b63 6f6c 735f 696e 5d20      df[cols_in] 
+00026c80: 3d20 6466 5b63 6f6c 5d2e 6170 706c 7928  = df[col].apply(
+00026c90: 7064 2e53 6572 6965 7329 2e76 616c 7565  pd.Series).value
+00026ca0: 735b 3a2c 3a6d 6178 5f63 6f6c 5f6c 656e  s[:,:max_col_len
+00026cb0: 6774 685d 0a20 2020 2020 2020 2064 6620  gth].        df 
+00026cc0: 3d20 6466 2e64 726f 7028 636f 6c2c 6178  = df.drop(col,ax
+00026cd0: 6973 3d31 290a 2020 2020 656c 7365 3a0a  is=1).    else:.
+00026ce0: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
+00026cf0: 665b 636f 6c5d 2e6d 6170 2874 7970 6529  f[col].map(type)
+00026d00: 2e76 616c 7565 5f63 6f75 6e74 7328 2929  .value_counts())
+00026d10: 3d3d 3120 616e 6420 6466 5b63 6f6c 5d2e  ==1 and df[col].
+00026d20: 6d61 7028 7479 7065 292e 7661 6c75 655f  map(type).value_
+00026d30: 636f 756e 7473 2829 2e69 6e64 6578 5b30  counts().index[0
+00026d40: 5d3d 3d6c 6973 743a 0a20 2020 2020 2020  ]==list:.       
+00026d50: 2020 2020 2023 2323 2052 656d 656d 6265       ### Remembe
+00026d60: 7220 7468 6174 2066 696c 6c6e 6120 6f6e  r that fillna on
+00026d70: 6c79 2077 6f72 6b73 2061 7420 6461 7461  ly works at data
+00026d80: 6672 616d 6520 6c65 7665 6c21 2023 2323  frame level! ###
+00026d90: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00026da0: 5f63 6f6c 5f6c 656e 6774 6820 3d20 6466  _col_length = df
+00026db0: 5b5b 636f 6c5d 5d2e 6669 6c6c 6e61 2827  [[col]].fillna('
+00026dc0: 6d69 7373 696e 6727 292e 6d61 7028 6c65  missing').map(le
+00026dd0: 6e29 2e6d 6178 2829 0a20 2020 2020 2020  n).max().       
+00026de0: 2020 2020 2063 6f6c 7320 3d20 5b63 6f6c       cols = [col
+00026df0: 2b27 5f27 2b73 7472 2869 2920 666f 7220  +'_'+str(i) for 
+00026e00: 6920 696e 2072 616e 6765 286d 6178 5f63  i in range(max_c
+00026e10: 6f6c 5f6c 656e 6774 6829 5d0a 2020 2020  ol_length)].    
+00026e20: 2020 2020 2020 2020 6466 5b63 6f6c 735d          df[cols]
+00026e30: 203d 2064 665b 636f 6c5d 2e61 7070 6c79   = df[col].apply
+00026e40: 2870 642e 5365 7269 6573 290a 2020 2020  (pd.Series).    
+00026e50: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+00026e60: 6472 6f70 2863 6f6c 2c61 7869 733d 3129  drop(col,axis=1)
+00026e70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00026e80: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00026e90: 2827 436f 6c75 6d6e 2025 7320 646f 6573  ('Column %s does
+00026ea0: 206e 6f74 2063 6f6e 7461 696e 206c 6973   not contain lis
+00026eb0: 7473 206f 7220 6861 7320 6d69 7865 6420  ts or has mixed 
+00026ec0: 7479 7065 7320 6f74 6865 7220 7468 616e  types other than
+00026ed0: 206c 6973 7473 2e20 4669 7820 6974 2061   lists. Fix it a
+00026ee0: 6e64 2072 6572 756e 2e27 2025 636f 6c29  nd rerun.' %col)
+00026ef0: 0a20 2020 2072 6574 7572 6e20 6466 0a23  .    return df.#
 00026f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00026f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00026f20: 2323 2323 2323 2323 2323 0a64 6566 2045  ##########.def E
-00026f30: 4441 5f72 616e 646f 6d6c 795f 7365 6c65  DA_randomly_sele
-00026f40: 6374 5f72 6f77 735f 6672 6f6d 5f64 6174  ct_rows_from_dat
-00026f50: 6166 7261 6d65 2874 7261 696e 5f64 6174  aframe(train_dat
-00026f60: 6166 7261 6d65 2c20 7461 7267 6574 732c  aframe, targets,
-00026f70: 206e 726f 7773 5f6c 696d 6974 2c20 4453   nrows_limit, DS
-00026f80: 5f4c 454e 3d27 2729 3a0a 2020 2020 6d61  _LEN=''):.    ma
-00026f90: 7872 6f77 7320 3d20 3130 3030 300a 2020  xrows = 10000.  
-00026fa0: 2020 7472 6169 6e5f 6461 7461 6672 616d    train_datafram
-00026fb0: 6520 3d20 636f 7079 2e64 6565 7063 6f70  e = copy.deepcop
-00026fc0: 7928 7472 6169 6e5f 6461 7461 6672 616d  y(train_datafram
-00026fd0: 6529 0a20 2020 2063 6f70 795f 7461 7267  e).    copy_targ
-00026fe0: 6574 7320 3d20 636f 7079 2e64 6565 7063  ets = copy.deepc
-00026ff0: 6f70 7928 7461 7267 6574 7329 0a20 2020  opy(targets).   
-00027000: 2069 6620 6e6f 7420 4453 5f4c 454e 3a0a   if not DS_LEN:.
-00027010: 2020 2020 2020 2020 4453 5f4c 454e 203d          DS_LEN =
-00027020: 2074 7261 696e 5f64 6174 6166 7261 6d65   train_dataframe
-00027030: 2e73 6861 7065 5b30 5d0a 2020 2020 2323  .shape[0].    ##
-00027040: 2323 2323 2320 7765 2072 616e 646f 6d6c  ##### we randoml
-00027050: 7920 7361 6d70 6c65 2061 2073 6d61 6c6c  y sample a small
-00027060: 2064 6174 6173 6574 2074 6f20 636c 6173   dataset to clas
-00027070: 7369 6679 2066 6561 7475 7265 7320 2323  sify features ##
-00027080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027090: 2323 230a 2020 2020 7465 7374 5f73 697a  ###.    test_siz
-000270a0: 6520 3d20 6d69 6e28 302e 392c 2028 3120  e = min(0.9, (1 
-000270b0: 2d20 286d 6178 726f 7773 2f44 535f 4c45  - (maxrows/DS_LE
-000270c0: 4e29 2929 2023 2323 206d 616b 6520 7375  N))) ### make su
-000270d0: 7265 2074 6865 7265 2069 7320 6120 736d  re there is a sm
-000270e0: 616c 6c20 7472 6169 6e20 7369 7a65 0a20  all train size. 
-000270f0: 2020 2069 6620 7465 7374 5f73 697a 6520     if test_size 
-00027100: 3c3d 2030 3a0a 2020 2020 2020 2020 7465  <= 0:.        te
-00027110: 7374 5f73 697a 6520 3d20 302e 390a 2020  st_size = 0.9.  
-00027120: 2020 2323 2320 2020 466c 6f61 7420 7661    ###   Float va
-00027130: 7269 6162 6c65 7320 6172 6520 636f 6e73  riables are cons
-00027140: 6964 6572 6564 2052 6567 7265 7373 696f  idered Regressio
-00027150: 6e20 2323 2323 2323 2323 2323 2323 2323  n ##############
-00027160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027170: 2323 2323 2323 230a 2020 2020 6d6f 6465  #######.    mode
-00027180: 6c74 7970 652c 205f 203d 2061 6e61 6c79  ltype, _ = analy
-00027190: 7a65 5f70 726f 626c 656d 5f74 7970 6528  ze_problem_type(
-000271a0: 7472 6169 6e5f 6461 7461 6672 616d 655b  train_dataframe[
-000271b0: 636f 7079 5f74 6172 6765 7473 5d2c 2063  copy_targets], c
-000271c0: 6f70 795f 7461 7267 6574 732c 2076 6572  opy_targets, ver
-000271d0: 626f 7365 3d30 290a 2020 2020 2323 2323  bose=0).    ####
-000271e0: 2323 2320 4966 2069 7420 6973 2061 2063  ### If it is a c
-000271f0: 6c61 7373 6966 6963 6174 696f 6e20 7072  lassification pr
-00027200: 6f62 6c65 6d2c 2079 6f75 206e 6565 6420  oblem, you need 
-00027210: 746f 2073 7472 6174 6966 7920 616e 6420  to stratify and 
-00027220: 7365 6c65 6374 2073 616d 706c 6520 2323  select sample ##
-00027230: 230a 2020 2020 6966 206d 6f64 656c 7479  #.    if modelty
-00027240: 7065 2021 3d20 2752 6567 7265 7373 696f  pe != 'Regressio
-00027250: 6e27 3a0a 2020 2020 2020 2020 7072 696e  n':.        prin
-00027260: 7428 2720 2020 206c 6f61 6469 6e67 2061  t('    loading a
-00027270: 2072 616e 646f 6d20 7361 6d70 6c65 206f   random sample o
-00027280: 6620 2564 2072 6f77 7320 696e 746f 2070  f %d rows into p
-00027290: 616e 6461 7320 666f 7220 4544 4127 2025  andas for EDA' %
-000272a0: 6e72 6f77 735f 6c69 6d69 7429 0a20 2020  nrows_limit).   
-000272b0: 2020 2020 2066 6f72 2065 6163 685f 7461       for each_ta
-000272c0: 7267 6574 2069 6e20 636f 7079 5f74 6172  rget in copy_tar
-000272d0: 6765 7473 3a0a 2020 2020 2020 2020 2020  gets:.          
-000272e0: 2020 2323 2320 596f 7520 6e65 6564 2074    ### You need t
-000272f0: 6f20 7265 6d6f 7665 2072 6f77 7320 7468  o remove rows th
-00027300: 6174 2068 6176 6520 7665 7279 2063 6c61  at have very cla
-00027310: 7373 2073 616d 706c 6573 202d 2074 6861  ss samples - tha
-00027320: 7420 6973 2061 2070 726f 626c 656d 2077  t is a problem w
-00027330: 6869 6c65 2073 706c 6974 7469 6e67 2074  hile splitting t
-00027340: 7261 696e 5f73 6d61 6c6c 0a20 2020 2020  rain_small.     
-00027350: 2020 2020 2020 206c 6973 745f 6f66 5f66         list_of_f
-00027360: 6577 5f63 6c61 7373 6573 203d 2074 7261  ew_classes = tra
-00027370: 696e 5f64 6174 6166 7261 6d65 5b65 6163  in_dataframe[eac
-00027380: 685f 7461 7267 6574 5d2e 7661 6c75 655f  h_target].value_
-00027390: 636f 756e 7473 2829 5b74 7261 696e 5f64  counts()[train_d
-000273a0: 6174 6166 7261 6d65 5b65 6163 685f 7461  ataframe[each_ta
-000273b0: 7267 6574 5d2e 7661 6c75 655f 636f 756e  rget].value_coun
-000273c0: 7473 2829 3c3d 335d 2e69 6e64 6578 2e74  ts()<=3].index.t
-000273d0: 6f6c 6973 7428 290a 2020 2020 2020 2020  olist().        
-000273e0: 2020 2020 7472 6169 6e5f 6461 7461 6672      train_datafr
-000273f0: 616d 6520 3d20 7472 6169 6e5f 6461 7461  ame = train_data
-00027400: 6672 616d 652e 6c6f 635b 7e28 7472 6169  frame.loc[~(trai
-00027410: 6e5f 6461 7461 6672 616d 655b 6561 6368  n_dataframe[each
-00027420: 5f74 6172 6765 745d 2e69 7369 6e28 6c69  _target].isin(li
-00027430: 7374 5f6f 665f 6665 775f 636c 6173 7365  st_of_few_classe
-00027440: 7329 295d 0a20 2020 2020 2020 2074 7279  s))].        try
-00027450: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00027460: 6169 6e5f 736d 616c 6c2c 205f 203d 2074  ain_small, _ = t
-00027470: 7261 696e 5f74 6573 745f 7370 6c69 7428  rain_test_split(
-00027480: 7472 6169 6e5f 6461 7461 6672 616d 652c  train_dataframe,
-00027490: 2074 6573 745f 7369 7a65 3d74 6573 745f   test_size=test_
-000274a0: 7369 7a65 2c20 7374 7261 7469 6679 3d74  size, stratify=t
-000274b0: 7261 696e 5f64 6174 6166 7261 6d65 5b74  rain_dataframe[t
-000274c0: 6172 6765 7473 5d29 0a20 2020 2020 2020  argets]).       
-000274d0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-000274e0: 2020 2020 2023 2320 5468 6973 2073 706c       ## This spl
-000274f0: 6974 2073 6f6d 6574 696d 6573 2065 7272  it sometimes err
-00027500: 6f72 732e 2049 7420 6973 2074 6865 6e20  ors. It is then 
-00027510: 6265 7474 6572 2074 6f20 7370 6c69 7420  better to split 
-00027520: 7573 696e 6720 6120 7261 6e64 6f6d 2073  using a random s
-00027530: 616d 706c 6520 2323 0a20 2020 2020 2020  ample ##.       
-00027540: 2020 2020 2074 7261 696e 5f73 6d61 6c6c       train_small
-00027550: 203d 2074 7261 696e 5f64 6174 6166 7261   = train_datafra
-00027560: 6d65 2e73 616d 706c 6528 6e3d 6e72 6f77  me.sample(n=nrow
-00027570: 735f 6c69 6d69 742c 2072 6570 6c61 6365  s_limit, replace
-00027580: 3d54 7275 652c 2072 616e 646f 6d5f 7374  =True, random_st
-00027590: 6174 653d 3939 290a 2020 2020 656c 7365  ate=99).    else
-000275a0: 3a0a 2020 2020 2020 2020 2323 2320 466f  :.        ### Fo
-000275b0: 7220 5265 6772 6573 7369 6f6e 2070 726f  r Regression pro
-000275c0: 626c 656d 733a 206c 6f61 6420 6120 736d  blems: load a sm
-000275d0: 616c 6c20 7361 6d70 6c65 206f 6620 6461  all sample of da
-000275e0: 7461 2069 6e74 6f20 6120 7061 6e64 6173  ta into a pandas
-000275f0: 2064 6174 6166 7261 6d65 2023 230a 2020   dataframe ##.  
-00027600: 2020 2020 2020 7072 696e 7428 2720 2020        print('   
-00027610: 206c 6f61 6469 6e67 2061 2073 6571 7565   loading a seque
-00027620: 6e74 6961 6c20 7361 6d70 6c65 206f 6620  ntial sample of 
-00027630: 2564 2072 6f77 7320 696e 746f 2070 616e  %d rows into pan
-00027640: 6461 7320 666f 7220 4544 4127 2025 6e72  das for EDA' %nr
-00027650: 6f77 735f 6c69 6d69 7429 0a20 2020 2020  ows_limit).     
-00027660: 2020 2074 7261 696e 5f73 6d61 6c6c 203d     train_small =
-00027670: 2074 7261 696e 5f64 6174 6166 7261 6d65   train_dataframe
-00027680: 5b3a 6e72 6f77 735f 6c69 6d69 745d 0a20  [:nrows_limit]. 
-00027690: 2020 2072 6574 7572 6e20 7472 6169 6e5f     return train_
-000276a0: 736d 616c 6c0a 2323 2323 2323 2323 2323  small.##########
-000276b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000276d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00026f50: 2323 2323 2323 2323 2323 2323 0a64 6566  ############.def
+00026f60: 2045 4441 5f72 616e 646f 6d6c 795f 7365   EDA_randomly_se
+00026f70: 6c65 6374 5f72 6f77 735f 6672 6f6d 5f64  lect_rows_from_d
+00026f80: 6174 6166 7261 6d65 2874 7261 696e 5f64  ataframe(train_d
+00026f90: 6174 6166 7261 6d65 2c20 7461 7267 6574  ataframe, target
+00026fa0: 732c 206e 726f 7773 5f6c 696d 6974 2c20  s, nrows_limit, 
+00026fb0: 4453 5f4c 454e 3d27 2729 3a0a 2020 2020  DS_LEN=''):.    
+00026fc0: 6d61 7872 6f77 7320 3d20 3130 3030 300a  maxrows = 10000.
+00026fd0: 2020 2020 7472 6169 6e5f 6461 7461 6672      train_datafr
+00026fe0: 616d 6520 3d20 636f 7079 2e64 6565 7063  ame = copy.deepc
+00026ff0: 6f70 7928 7472 6169 6e5f 6461 7461 6672  opy(train_datafr
+00027000: 616d 6529 0a20 2020 2063 6f70 795f 7461  ame).    copy_ta
+00027010: 7267 6574 7320 3d20 636f 7079 2e64 6565  rgets = copy.dee
+00027020: 7063 6f70 7928 7461 7267 6574 7329 0a20  pcopy(targets). 
+00027030: 2020 2069 6620 6e6f 7420 4453 5f4c 454e     if not DS_LEN
+00027040: 3a0a 2020 2020 2020 2020 4453 5f4c 454e  :.        DS_LEN
+00027050: 203d 2074 7261 696e 5f64 6174 6166 7261   = train_datafra
+00027060: 6d65 2e73 6861 7065 5b30 5d0a 2020 2020  me.shape[0].    
+00027070: 2323 2323 2323 2320 7765 2072 616e 646f  ####### we rando
+00027080: 6d6c 7920 7361 6d70 6c65 2061 2073 6d61  mly sample a sma
+00027090: 6c6c 2064 6174 6173 6574 2074 6f20 636c  ll dataset to cl
+000270a0: 6173 7369 6679 2066 6561 7475 7265 7320  assify features 
+000270b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000270c0: 2323 2323 230a 2020 2020 7465 7374 5f73  #####.    test_s
+000270d0: 697a 6520 3d20 6d69 6e28 302e 392c 2028  ize = min(0.9, (
+000270e0: 3120 2d20 286d 6178 726f 7773 2f44 535f  1 - (maxrows/DS_
+000270f0: 4c45 4e29 2929 2023 2323 206d 616b 6520  LEN))) ### make 
+00027100: 7375 7265 2074 6865 7265 2069 7320 6120  sure there is a 
+00027110: 736d 616c 6c20 7472 6169 6e20 7369 7a65  small train size
+00027120: 0a20 2020 2069 6620 7465 7374 5f73 697a  .    if test_siz
+00027130: 6520 3c3d 2030 3a0a 2020 2020 2020 2020  e <= 0:.        
+00027140: 7465 7374 5f73 697a 6520 3d20 302e 390a  test_size = 0.9.
+00027150: 2020 2020 2323 2320 2020 466c 6f61 7420      ###   Float 
+00027160: 7661 7269 6162 6c65 7320 6172 6520 636f  variables are co
+00027170: 6e73 6964 6572 6564 2052 6567 7265 7373  nsidered Regress
+00027180: 696f 6e20 2323 2323 2323 2323 2323 2323  ion ############
+00027190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000271a0: 2323 2323 2323 2323 230a 2020 2020 6d6f  #########.    mo
+000271b0: 6465 6c74 7970 652c 205f 203d 2061 6e61  deltype, _ = ana
+000271c0: 6c79 7a65 5f70 726f 626c 656d 5f74 7970  lyze_problem_typ
+000271d0: 6528 7472 6169 6e5f 6461 7461 6672 616d  e(train_datafram
+000271e0: 655b 636f 7079 5f74 6172 6765 7473 5d2c  e[copy_targets],
+000271f0: 2063 6f70 795f 7461 7267 6574 732c 2076   copy_targets, v
+00027200: 6572 626f 7365 3d30 290a 2020 2020 2323  erbose=0).    ##
+00027210: 2323 2323 2320 4966 2069 7420 6973 2061  ##### If it is a
+00027220: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+00027230: 7072 6f62 6c65 6d2c 2079 6f75 206e 6565  problem, you nee
+00027240: 6420 746f 2073 7472 6174 6966 7920 616e  d to stratify an
+00027250: 6420 7365 6c65 6374 2073 616d 706c 6520  d select sample 
+00027260: 2323 230a 2020 2020 6966 206d 6f64 656c  ###.    if model
+00027270: 7479 7065 2021 3d20 2752 6567 7265 7373  type != 'Regress
+00027280: 696f 6e27 3a0a 2020 2020 2020 2020 7072  ion':.        pr
+00027290: 696e 7428 2720 2020 206c 6f61 6469 6e67  int('    loading
+000272a0: 2061 2072 616e 646f 6d20 7361 6d70 6c65   a random sample
+000272b0: 206f 6620 2564 2072 6f77 7320 696e 746f   of %d rows into
+000272c0: 2070 616e 6461 7320 666f 7220 4544 4127   pandas for EDA'
+000272d0: 2025 6e72 6f77 735f 6c69 6d69 7429 0a20   %nrows_limit). 
+000272e0: 2020 2020 2020 2066 6f72 2065 6163 685f         for each_
+000272f0: 7461 7267 6574 2069 6e20 636f 7079 5f74  target in copy_t
+00027300: 6172 6765 7473 3a0a 2020 2020 2020 2020  argets:.        
+00027310: 2020 2020 2323 2320 596f 7520 6e65 6564      ### You need
+00027320: 2074 6f20 7265 6d6f 7665 2072 6f77 7320   to remove rows 
+00027330: 7468 6174 2068 6176 6520 7665 7279 2063  that have very c
+00027340: 6c61 7373 2073 616d 706c 6573 202d 2074  lass samples - t
+00027350: 6861 7420 6973 2061 2070 726f 626c 656d  hat is a problem
+00027360: 2077 6869 6c65 2073 706c 6974 7469 6e67   while splitting
+00027370: 2074 7261 696e 5f73 6d61 6c6c 0a20 2020   train_small.   
+00027380: 2020 2020 2020 2020 206c 6973 745f 6f66           list_of
+00027390: 5f66 6577 5f63 6c61 7373 6573 203d 2074  _few_classes = t
+000273a0: 7261 696e 5f64 6174 6166 7261 6d65 5b65  rain_dataframe[e
+000273b0: 6163 685f 7461 7267 6574 5d2e 7661 6c75  ach_target].valu
+000273c0: 655f 636f 756e 7473 2829 5b74 7261 696e  e_counts()[train
+000273d0: 5f64 6174 6166 7261 6d65 5b65 6163 685f  _dataframe[each_
+000273e0: 7461 7267 6574 5d2e 7661 6c75 655f 636f  target].value_co
+000273f0: 756e 7473 2829 3c3d 335d 2e69 6e64 6578  unts()<=3].index
+00027400: 2e74 6f6c 6973 7428 290a 2020 2020 2020  .tolist().      
+00027410: 2020 2020 2020 7472 6169 6e5f 6461 7461        train_data
+00027420: 6672 616d 6520 3d20 7472 6169 6e5f 6461  frame = train_da
+00027430: 7461 6672 616d 652e 6c6f 635b 7e28 7472  taframe.loc[~(tr
+00027440: 6169 6e5f 6461 7461 6672 616d 655b 6561  ain_dataframe[ea
+00027450: 6368 5f74 6172 6765 745d 2e69 7369 6e28  ch_target].isin(
+00027460: 6c69 7374 5f6f 665f 6665 775f 636c 6173  list_of_few_clas
+00027470: 7365 7329 295d 0a20 2020 2020 2020 2074  ses))].        t
+00027480: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00027490: 7472 6169 6e5f 736d 616c 6c2c 205f 203d  train_small, _ =
+000274a0: 2074 7261 696e 5f74 6573 745f 7370 6c69   train_test_spli
+000274b0: 7428 7472 6169 6e5f 6461 7461 6672 616d  t(train_datafram
+000274c0: 652c 2074 6573 745f 7369 7a65 3d74 6573  e, test_size=tes
+000274d0: 745f 7369 7a65 2c20 7374 7261 7469 6679  t_size, stratify
+000274e0: 3d74 7261 696e 5f64 6174 6166 7261 6d65  =train_dataframe
+000274f0: 5b74 6172 6765 7473 5d29 0a20 2020 2020  [targets]).     
+00027500: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00027510: 2020 2020 2020 2023 2320 5468 6973 2073         ## This s
+00027520: 706c 6974 2073 6f6d 6574 696d 6573 2065  plit sometimes e
+00027530: 7272 6f72 732e 2049 7420 6973 2074 6865  rrors. It is the
+00027540: 6e20 6265 7474 6572 2074 6f20 7370 6c69  n better to spli
+00027550: 7420 7573 696e 6720 6120 7261 6e64 6f6d  t using a random
+00027560: 2073 616d 706c 6520 2323 0a20 2020 2020   sample ##.     
+00027570: 2020 2020 2020 2074 7261 696e 5f73 6d61         train_sma
+00027580: 6c6c 203d 2074 7261 696e 5f64 6174 6166  ll = train_dataf
+00027590: 7261 6d65 2e73 616d 706c 6528 6e3d 6e72  rame.sample(n=nr
+000275a0: 6f77 735f 6c69 6d69 742c 2072 6570 6c61  ows_limit, repla
+000275b0: 6365 3d54 7275 652c 2072 616e 646f 6d5f  ce=True, random_
+000275c0: 7374 6174 653d 3939 290a 2020 2020 656c  state=99).    el
+000275d0: 7365 3a0a 2020 2020 2020 2020 2323 2320  se:.        ### 
+000275e0: 466f 7220 5265 6772 6573 7369 6f6e 2070  For Regression p
+000275f0: 726f 626c 656d 733a 206c 6f61 6420 6120  roblems: load a 
+00027600: 736d 616c 6c20 7361 6d70 6c65 206f 6620  small sample of 
+00027610: 6461 7461 2069 6e74 6f20 6120 7061 6e64  data into a pand
+00027620: 6173 2064 6174 6166 7261 6d65 2023 230a  as dataframe ##.
+00027630: 2020 2020 2020 2020 7072 696e 7428 2720          print(' 
+00027640: 2020 206c 6f61 6469 6e67 2061 2073 6571     loading a seq
+00027650: 7565 6e74 6961 6c20 7361 6d70 6c65 206f  uential sample o
+00027660: 6620 2564 2072 6f77 7320 696e 746f 2070  f %d rows into p
+00027670: 616e 6461 7320 666f 7220 4544 4127 2025  andas for EDA' %
+00027680: 6e72 6f77 735f 6c69 6d69 7429 0a20 2020  nrows_limit).   
+00027690: 2020 2020 2074 7261 696e 5f73 6d61 6c6c       train_small
+000276a0: 203d 2074 7261 696e 5f64 6174 6166 7261   = train_datafra
+000276b0: 6d65 5b3a 6e72 6f77 735f 6c69 6d69 745d  me[:nrows_limit]
+000276c0: 0a20 2020 2072 6574 7572 6e20 7472 6169  .    return trai
+000276d0: 6e5f 736d 616c 6c0a 2323 2323 2323 2323  n_small.########
 000276e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000276f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00027700: 2323 2323 2323 0a63 6c61 7373 2046 6561  ######.class Fea
-00027710: 7475 7265 5769 7a28 4261 7365 4573 7469  tureWiz(BaseEsti
-00027720: 6d61 746f 722c 2054 7261 6e73 666f 726d  mator, Transform
-00027730: 6572 4d69 7869 6e29 3a0a 2020 2020 6465  erMixin):.    de
-00027740: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00027750: 2063 6f72 725f 6c69 6d69 743d 302e 3930   corr_limit=0.90
-00027760: 2c20 7665 7262 6f73 653d 322c 2073 6570  , verbose=2, sep
-00027770: 3d27 2c27 2c20 0a20 2020 2020 2020 2068  =',', .        h
-00027780: 6561 6465 723d 302c 2066 6561 7475 7265  eader=0, feature
-00027790: 5f65 6e67 673d 2727 2c20 6361 7465 676f  _engg='', catego
-000277a0: 7279 5f65 6e63 6f64 6572 733d 2727 2c0a  ry_encoders='',.
-000277b0: 2020 2020 2020 2020 6461 736b 5f78 6762          dask_xgb
-000277c0: 6f6f 7374 5f66 6c61 673d 4661 6c73 652c  oost_flag=False,
-000277d0: 206e 726f 7773 3d4e 6f6e 652c 2073 6b69   nrows=None, ski
-000277e0: 705f 7375 6c6f 763d 4661 6c73 6529 3a0a  p_sulov=False):.
-000277f0: 2020 2020 2020 2020 7072 696e 7428 2222          print(""
-00027800: 2277 697a 203d 2046 6561 7475 7265 5769  "wiz = FeatureWi
-00027810: 7a28 7665 7262 6f73 653d 3129 0a20 2020  z(verbose=1).   
-00027820: 2020 2020 2058 5f74 7261 696e 5f73 656c       X_train_sel
-00027830: 6563 7465 6420 3d20 7769 7a2e 6669 745f  ected = wiz.fit_
-00027840: 7472 616e 7366 6f72 6d28 585f 7472 6169  transform(X_trai
-00027850: 6e2c 2079 5f74 7261 696e 290a 2020 2020  n, y_train).    
-00027860: 2020 2020 585f 7465 7374 5f73 656c 6563      X_test_selec
-00027870: 7465 6420 3d20 7769 7a2e 7472 616e 7366  ted = wiz.transf
-00027880: 6f72 6d28 585f 7465 7374 290a 2020 2020  orm(X_test).    
-00027890: 2020 2020 7769 7a2e 6665 6174 7572 6573      wiz.features
-000278a0: 2020 2323 2320 7072 6f76 6964 6573 2061    ### provides a
-000278b0: 206c 6973 7420 6f66 2073 656c 6563 7465   list of selecte
-000278c0: 6420 6665 6174 7572 6573 2023 2323 2020  d features ###  
-000278d0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000278e0: 2020 2022 2222 290a 2020 2020 2020 2020     """).        
-000278f0: 7365 6c66 2e66 6561 7475 7265 7320 3d20  self.features = 
-00027900: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-00027910: 662e 636f 7272 5f6c 696d 6974 3d20 636f  f.corr_limit= co
-00027920: 7272 5f6c 696d 6974 0a20 2020 2020 2020  rr_limit.       
-00027930: 2073 656c 662e 7665 7262 6f73 653d 7665   self.verbose=ve
-00027940: 7262 6f73 650a 2020 2020 2020 2020 7365  rbose.        se
-00027950: 6c66 2e73 6570 3d73 6570 0a20 2020 2020  lf.sep=sep.     
-00027960: 2020 2073 656c 662e 6865 6164 6572 3d68     self.header=h
-00027970: 6561 6465 720a 2020 2020 2020 2020 7365  eader.        se
-00027980: 6c66 2e74 6573 745f 6461 7461 203d 2022  lf.test_data = "
-00027990: 2220 2323 206c 6561 7665 2074 6573 7464  " ## leave testd
-000279a0: 6174 6120 7065 726d 616e 656e 746c 7920  ata permanently 
-000279b0: 6173 2065 6d70 7479 2066 6f72 206e 6f77  as empty for now
-000279c0: 2023 230a 2020 2020 2020 2020 7365 6c66   ##.        self
-000279d0: 2e66 6561 7475 7265 5f65 6e67 673d 6665  .feature_engg=fe
-000279e0: 6174 7572 655f 656e 6767 0a20 2020 2020  ature_engg.     
-000279f0: 2020 2073 656c 662e 6361 7465 676f 7279     self.category
-00027a00: 5f65 6e63 6f64 6572 733d 6361 7465 676f  _encoders=catego
-00027a10: 7279 5f65 6e63 6f64 6572 730a 2020 2020  ry_encoders.    
-00027a20: 2020 2020 7365 6c66 2e64 6173 6b5f 7867      self.dask_xg
-00027a30: 626f 6f73 745f 666c 6167 3d64 6173 6b5f  boost_flag=dask_
-00027a40: 7867 626f 6f73 745f 666c 6167 0a20 2020  xgboost_flag.   
-00027a50: 2020 2020 2073 656c 662e 6e72 6f77 733d       self.nrows=
-00027a60: 6e72 6f77 730a 2020 2020 2020 2020 7365  nrows.        se
-00027a70: 6c66 2e73 6b69 705f 7375 6c6f 763d 736b  lf.skip_sulov=sk
-00027a80: 6970 5f73 756c 6f76 0a20 2020 2020 2020  ip_sulov.       
-00027a90: 2073 656c 662e 585f 7365 6c20 3d20 4e6f   self.X_sel = No
-00027aa0: 6e65 0a0a 2020 2020 6465 6620 6669 7428  ne..    def fit(
-00027ab0: 7365 6c66 2c20 582c 2079 293a 0a20 2020  self, X, y):.   
-00027ac0: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
-00027ad0: 3d20 7469 6d65 2e74 696d 6528 290a 2020  = time.time().  
-00027ae0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00027af0: 6e63 6528 582c 206e 702e 6e64 6172 7261  nce(X, np.ndarra
-00027b00: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
-00027b10: 7072 696e 7428 2758 2069 6e70 7574 206d  print('X input m
-00027b20: 7573 7420 6265 2061 2064 6174 6166 7261  ust be a datafra
-00027b30: 6d65 2073 696e 6365 2077 6520 7573 6520  me since we use 
-00027b40: 636f 6c75 6d6e 206e 616d 6573 2074 6f20  column names to 
-00027b50: 6275 696c 6420 6461 7461 2070 6970 656c  build data pipel
-00027b60: 696e 6573 2e20 5265 7475 726e 696e 6727  ines. Returning'
-00027b70: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00027b80: 7475 726e 2058 2c20 790a 2020 2020 2020  turn X, y.      
-00027b90: 2020 585f 696e 6465 7820 3d20 582e 696e    X_index = X.in
-00027ba0: 6465 780a 2020 2020 2020 2020 6966 2069  dex.        if i
-00027bb0: 7369 6e73 7461 6e63 6528 792c 206e 702e  sinstance(y, np.
-00027bc0: 6e64 6172 7261 7929 3a0a 2020 2020 2020  ndarray):.      
-00027bd0: 2020 2020 2020 7072 696e 7428 2720 2020        print('   
-00027be0: 7920 696e 7075 7420 6973 2061 6e20 6e75  y input is an nu
-00027bf0: 6d70 7920 6172 7261 7920 616e 6420 6865  mpy array and he
-00027c00: 6e63 6520 636f 6e76 6572 7420 696e 746f  nce convert into
-00027c10: 2061 2073 6572 6965 7320 6f72 2064 6174   a series or dat
-00027c20: 6166 7261 6d65 2061 6e64 2072 652d 7472  aframe and re-tr
-00027c30: 792e 2729 0a20 2020 2020 2020 2020 2020  y.').           
-00027c40: 2072 6574 7572 6e20 582c 2079 0a20 2020   return X, y.   
-00027c50: 2020 2020 2079 5f69 6e64 6578 203d 2079       y_index = y
-00027c60: 2e69 6e64 6578 0a20 2020 2020 2020 2069  .index.        i
-00027c70: 6620 2858 5f69 6e64 6578 203d 3d20 795f  f (X_index == y_
-00027c80: 696e 6465 7829 2e61 6c6c 2829 3a0a 2020  index).all():.  
-00027c90: 2020 2020 2020 2020 2020 6466 203d 2070            df = p
-00027ca0: 642e 636f 6e63 6174 285b 582c 2079 5d2c  d.concat([X, y],
-00027cb0: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
-00027cc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00027cd0: 2020 2064 6620 3d20 7064 2e63 6f6e 6361     df = pd.conca
-00027ce0: 7428 5b58 2e72 6573 6574 5f69 6e64 6578  t([X.reset_index
-00027cf0: 2864 726f 703d 5472 7565 292c 2079 5d2c  (drop=True), y],
-00027d00: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
-00027d10: 2020 2020 2064 662e 696e 6465 7820 3d20       df.index = 
-00027d20: 585f 696e 6465 780a 2020 2020 2020 2020  X_index.        
-00027d30: 2323 2320 4e6f 7720 796f 7520 6361 6e20  ### Now you can 
-00027d40: 7072 6f63 6573 7320 7468 6520 5820 616e  process the X an
-00027d50: 6420 7920 6461 7461 7365 7473 2023 2323  d y datasets ###
-00027d60: 230a 2020 2020 2020 2020 6966 2069 7369  #.        if isi
-00027d70: 6e73 7461 6e63 6528 792c 2070 642e 5365  nstance(y, pd.Se
-00027d80: 7269 6573 293a 0a20 2020 2020 2020 2020  ries):.         
-00027d90: 2020 2074 6172 6765 7420 3d20 792e 6e61     target = y.na
-00027da0: 6d65 0a20 2020 2020 2020 2020 2020 2069  me.            i
-00027db0: 6620 7461 7267 6574 2069 7320 4e6f 6e65  f target is None
-00027dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00027dd0: 2020 7072 696e 7428 2720 2020 7920 696e    print('   y in
-00027de0: 7075 7420 6973 2061 2070 616e 6461 7320  put is a pandas 
-00027df0: 7365 7269 6573 2077 6974 6820 6e6f 206e  series with no n
-00027e00: 616d 652e 2043 6f6e 7665 7274 2069 7420  ame. Convert it 
-00027e10: 616e 6420 7265 2d74 7279 2e27 290a 2020  and re-try.').  
-00027e20: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00027e30: 7475 726e 2058 2c20 7920 2020 2020 2020  turn X, y       
-00027e40: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00027e50: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00027e60: 6528 792c 2070 642e 4461 7461 4672 616d  e(y, pd.DataFram
-00027e70: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00027e80: 7461 7267 6574 203d 2079 2e63 6f6c 756d  target = y.colum
-00027e90: 6e73 2e74 6f6c 6973 7428 290a 2020 2020  ns.tolist().    
-00027ea0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00027eb0: 6e63 6528 582c 206e 702e 6e64 6172 7261  nce(X, np.ndarra
-00027ec0: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
-00027ed0: 7072 696e 7428 2779 206d 7573 7420 6265  print('y must be
-00027ee0: 2061 2070 642e 5365 7269 6573 206f 7220   a pd.Series or 
-00027ef0: 7064 2e44 6174 6146 7261 6d65 2073 696e  pd.DataFrame sin
-00027f00: 6365 2077 6520 7573 6520 636f 6c75 6d6e  ce we use column
-00027f10: 206e 616d 6573 2074 6f20 6275 696c 6420   names to build 
-00027f20: 6461 7461 2070 6970 656c 696e 652e 2052  data pipeline. R
-00027f30: 6574 7572 6e69 6e67 2729 0a20 2020 2020  eturning').     
-00027f40: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
-00027f50: 2c20 7b7d 0a20 2020 2020 2020 2023 2323  , {}.        ###
-00027f60: 2320 5365 6e64 2074 6172 6765 7420 7661  # Send target va
-00027f70: 7269 6162 6c65 2061 7320 6974 2069 7320  riable as it is 
-00027f80: 736f 2074 6861 7420 795f 7472 6169 6e20  so that y_train 
-00027f90: 6973 2061 6e61 6c79 7a65 6420 7072 6f70  is analyzed prop
-00027fa0: 6572 6c79 2023 2323 0a20 2020 2020 2020  erly ###.       
-00027fb0: 2023 2053 656c 6563 7420 6665 6174 7572   # Select featur
-00027fc0: 6573 2075 7369 6e67 2066 6561 7475 7265  es using feature
-00027fd0: 7769 7a0a 2020 2020 2020 2020 6665 6174  wiz.        feat
-00027fe0: 7572 6573 2c20 585f 7365 6c20 3d20 6665  ures, X_sel = fe
-00027ff0: 6174 7572 6577 697a 2864 662c 2074 6172  aturewiz(df, tar
-00028000: 6765 742c 2073 656c 662e 636f 7272 5f6c  get, self.corr_l
-00028010: 696d 6974 2c20 7365 6c66 2e76 6572 626f  imit, self.verbo
-00028020: 7365 2c20 7365 6c66 2e73 6570 2c20 0a20  se, self.sep, . 
-00028030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00028040: 656c 662e 6865 6164 6572 2c20 7365 6c66  elf.header, self
-00028050: 2e74 6573 745f 6461 7461 2c20 7365 6c66  .test_data, self
-00028060: 2e66 6561 7475 7265 5f65 6e67 672c 2073  .feature_engg, s
-00028070: 656c 662e 6361 7465 676f 7279 5f65 6e63  elf.category_enc
-00028080: 6f64 6572 732c 0a20 2020 2020 2020 2020  oders,.         
-00028090: 2020 2020 2020 2073 656c 662e 6461 736b         self.dask
-000280a0: 5f78 6762 6f6f 7374 5f66 6c61 672c 2073  _xgboost_flag, s
-000280b0: 656c 662e 6e72 6f77 732c 2073 656c 662e  elf.nrows, self.
-000280c0: 736b 6970 5f73 756c 6f76 290a 2020 2020  skip_sulov).    
-000280d0: 2020 2020 2320 436f 6e76 6572 7420 7468      # Convert th
-000280e0: 6520 7265 6d61 696e 696e 6720 636f 6c75  e remaining colu
-000280f0: 6d6e 206e 616d 6573 2062 6163 6b20 746f  mn names back to
-00028100: 2069 6e74 6567 6572 7320 616e 6420 6472   integers and dr
-00028110: 6f70 2074 6865 0a20 2020 2020 2020 2064  op the.        d
-00028120: 6966 6674 696d 6520 3d20 6d61 7828 312c  ifftime = max(1,
-00028130: 2069 6e74 2874 696d 652e 7469 6d65 2829   int(time.time()
-00028140: 2d73 7461 7274 5f74 696d 6529 290a 2020  -start_time)).  
-00028150: 2020 2020 2020 7072 696e 7428 2720 2020        print('   
-00028160: 2054 696d 6520 7461 6b65 6e20 746f 2063   Time taken to c
-00028170: 7265 6174 6520 656e 7469 7265 2070 6970  reate entire pip
-00028180: 656c 696e 6520 3d20 2573 2073 6563 6f6e  eline = %s secon
-00028190: 6428 7329 2720 2564 6966 6674 696d 6529  d(s)' %difftime)
-000281a0: 0a20 2020 2020 2020 2023 2063 6f6c 756d  .        # colum
-000281b0: 6e20 6f66 206c 6162 656c 730a 2020 2020  n of labels.    
-000281c0: 2020 2020 7365 6c66 2e66 6561 7475 7265      self.feature
-000281d0: 7320 3d20 6665 6174 7572 6573 0a20 2020  s = features.   
-000281e0: 2020 2020 2073 656c 662e 585f 7365 6c20       self.X_sel 
-000281f0: 3d20 585f 7365 6c0a 2020 2020 2020 2020  = X_sel.        
-00028200: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
-00028210: 2064 6566 2074 7261 6e73 666f 726d 2873   def transform(s
-00028220: 656c 662c 2058 293a 0a20 2020 2020 2020  elf, X):.       
-00028230: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00028240: 2020 7265 7475 726e 2058 5b73 656c 662e    return X[self.
-00028250: 6665 6174 7572 6573 5d0a 2020 2020 2020  features].      
-00028260: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00028270: 2020 2020 2020 7072 696e 7428 2752 6574        print('Ret
-00028280: 7572 6e69 6e67 2074 7261 6e73 666f 726d  urning transform
-00028290: 6564 2064 6174 6166 7261 6d65 2077 6974  ed dataframe wit
-000282a0: 6820 2564 2066 6561 7475 7265 7327 2025  h %d features' %
-000282b0: 6c65 6e28 7365 6c66 2e66 6561 7475 7265  len(self.feature
-000282c0: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
-000282d0: 7265 7475 726e 2073 656c 662e 585f 7365  return self.X_se
-000282e0: 6c0a 2323 2323 2323 2323 2323 2323 2323  l.##############
-000282f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00027730: 2323 2323 2323 2323 0a63 6c61 7373 2046  ########.class F
+00027740: 6561 7475 7265 5769 7a28 4261 7365 4573  eatureWiz(BaseEs
+00027750: 7469 6d61 746f 722c 2054 7261 6e73 666f  timator, Transfo
+00027760: 726d 6572 4d69 7869 6e29 3a0a 2020 2020  rmerMixin):.    
+00027770: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00027780: 662c 2063 6f72 725f 6c69 6d69 743d 302e  f, corr_limit=0.
+00027790: 3930 2c20 7665 7262 6f73 653d 322c 2073  90, verbose=2, s
+000277a0: 6570 3d27 2c27 2c20 0a20 2020 2020 2020  ep=',', .       
+000277b0: 2068 6561 6465 723d 302c 2066 6561 7475   header=0, featu
+000277c0: 7265 5f65 6e67 673d 2727 2c20 6361 7465  re_engg='', cate
+000277d0: 676f 7279 5f65 6e63 6f64 6572 733d 2727  gory_encoders=''
+000277e0: 2c0a 2020 2020 2020 2020 6461 736b 5f78  ,.        dask_x
+000277f0: 6762 6f6f 7374 5f66 6c61 673d 4661 6c73  gboost_flag=Fals
+00027800: 652c 206e 726f 7773 3d4e 6f6e 652c 2073  e, nrows=None, s
+00027810: 6b69 705f 7375 6c6f 763d 4661 6c73 6529  kip_sulov=False)
+00027820: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00027830: 2222 2277 697a 203d 2046 6561 7475 7265  """wiz = Feature
+00027840: 5769 7a28 7665 7262 6f73 653d 3129 0a20  Wiz(verbose=1). 
+00027850: 2020 2020 2020 2058 5f74 7261 696e 5f73         X_train_s
+00027860: 656c 6563 7465 6420 3d20 7769 7a2e 6669  elected = wiz.fi
+00027870: 745f 7472 616e 7366 6f72 6d28 585f 7472  t_transform(X_tr
+00027880: 6169 6e2c 2079 5f74 7261 696e 290a 2020  ain, y_train).  
+00027890: 2020 2020 2020 585f 7465 7374 5f73 656c        X_test_sel
+000278a0: 6563 7465 6420 3d20 7769 7a2e 7472 616e  ected = wiz.tran
+000278b0: 7366 6f72 6d28 585f 7465 7374 290a 2020  sform(X_test).  
+000278c0: 2020 2020 2020 7769 7a2e 6665 6174 7572        wiz.featur
+000278d0: 6573 2020 2323 2320 7072 6f76 6964 6573  es  ### provides
+000278e0: 2061 206c 6973 7420 6f66 2073 656c 6563   a list of selec
+000278f0: 7465 6420 6665 6174 7572 6573 2023 2323  ted features ###
+00027900: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00027910: 2020 2020 2022 2222 290a 2020 2020 2020       """).      
+00027920: 2020 7365 6c66 2e66 6561 7475 7265 7320    self.features 
+00027930: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00027940: 656c 662e 636f 7272 5f6c 696d 6974 3d20  elf.corr_limit= 
+00027950: 636f 7272 5f6c 696d 6974 0a20 2020 2020  corr_limit.     
+00027960: 2020 2073 656c 662e 7665 7262 6f73 653d     self.verbose=
+00027970: 7665 7262 6f73 650a 2020 2020 2020 2020  verbose.        
+00027980: 7365 6c66 2e73 6570 3d73 6570 0a20 2020  self.sep=sep.   
+00027990: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000279a0: 3d68 6561 6465 720a 2020 2020 2020 2020  =header.        
+000279b0: 7365 6c66 2e74 6573 745f 6461 7461 203d  self.test_data =
+000279c0: 2022 2220 2323 206c 6561 7665 2074 6573   "" ## leave tes
+000279d0: 7464 6174 6120 7065 726d 616e 656e 746c  tdata permanentl
+000279e0: 7920 6173 2065 6d70 7479 2066 6f72 206e  y as empty for n
+000279f0: 6f77 2023 230a 2020 2020 2020 2020 7365  ow ##.        se
+00027a00: 6c66 2e66 6561 7475 7265 5f65 6e67 673d  lf.feature_engg=
+00027a10: 6665 6174 7572 655f 656e 6767 0a20 2020  feature_engg.   
+00027a20: 2020 2020 2073 656c 662e 6361 7465 676f       self.catego
+00027a30: 7279 5f65 6e63 6f64 6572 733d 6361 7465  ry_encoders=cate
+00027a40: 676f 7279 5f65 6e63 6f64 6572 730a 2020  gory_encoders.  
+00027a50: 2020 2020 2020 7365 6c66 2e64 6173 6b5f        self.dask_
+00027a60: 7867 626f 6f73 745f 666c 6167 3d64 6173  xgboost_flag=das
+00027a70: 6b5f 7867 626f 6f73 745f 666c 6167 0a20  k_xgboost_flag. 
+00027a80: 2020 2020 2020 2073 656c 662e 6e72 6f77         self.nrow
+00027a90: 733d 6e72 6f77 730a 2020 2020 2020 2020  s=nrows.        
+00027aa0: 7365 6c66 2e73 6b69 705f 7375 6c6f 763d  self.skip_sulov=
+00027ab0: 736b 6970 5f73 756c 6f76 0a20 2020 2020  skip_sulov.     
+00027ac0: 2020 2073 656c 662e 585f 7365 6c20 3d20     self.X_sel = 
+00027ad0: 4e6f 6e65 0a0a 2020 2020 6465 6620 6669  None..    def fi
+00027ae0: 7428 7365 6c66 2c20 582c 2079 293a 0a20  t(self, X, y):. 
+00027af0: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
+00027b00: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
+00027b10: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00027b20: 7461 6e63 6528 582c 206e 702e 6e64 6172  tance(X, np.ndar
+00027b30: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
+00027b40: 2020 7072 696e 7428 2758 2069 6e70 7574    print('X input
+00027b50: 206d 7573 7420 6265 2061 2064 6174 6166   must be a dataf
+00027b60: 7261 6d65 2073 696e 6365 2077 6520 7573  rame since we us
+00027b70: 6520 636f 6c75 6d6e 206e 616d 6573 2074  e column names t
+00027b80: 6f20 6275 696c 6420 6461 7461 2070 6970  o build data pip
+00027b90: 656c 696e 6573 2e20 5265 7475 726e 696e  elines. Returnin
+00027ba0: 6727 290a 2020 2020 2020 2020 2020 2020  g').            
+00027bb0: 7265 7475 726e 2058 2c20 790a 2020 2020  return X, y.    
+00027bc0: 2020 2020 585f 696e 6465 7820 3d20 582e      X_index = X.
+00027bd0: 696e 6465 780a 2020 2020 2020 2020 6966  index.        if
+00027be0: 2069 7369 6e73 7461 6e63 6528 792c 206e   isinstance(y, n
+00027bf0: 702e 6e64 6172 7261 7929 3a0a 2020 2020  p.ndarray):.    
+00027c00: 2020 2020 2020 2020 7072 696e 7428 2720          print(' 
+00027c10: 2020 7920 696e 7075 7420 6973 2061 6e20    y input is an 
+00027c20: 6e75 6d70 7920 6172 7261 7920 616e 6420  numpy array and 
+00027c30: 6865 6e63 6520 636f 6e76 6572 7420 696e  hence convert in
+00027c40: 746f 2061 2073 6572 6965 7320 6f72 2064  to a series or d
+00027c50: 6174 6166 7261 6d65 2061 6e64 2072 652d  ataframe and re-
+00027c60: 7472 792e 2729 0a20 2020 2020 2020 2020  try.').         
+00027c70: 2020 2072 6574 7572 6e20 582c 2079 0a20     return X, y. 
+00027c80: 2020 2020 2020 2079 5f69 6e64 6578 203d         y_index =
+00027c90: 2079 2e69 6e64 6578 0a20 2020 2020 2020   y.index.       
+00027ca0: 2069 6620 2858 5f69 6e64 6578 203d 3d20   if (X_index == 
+00027cb0: 795f 696e 6465 7829 2e61 6c6c 2829 3a0a  y_index).all():.
+00027cc0: 2020 2020 2020 2020 2020 2020 6466 203d              df =
+00027cd0: 2070 642e 636f 6e63 6174 285b 582c 2079   pd.concat([X, y
+00027ce0: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
+00027cf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00027d00: 2020 2020 2064 6620 3d20 7064 2e63 6f6e       df = pd.con
+00027d10: 6361 7428 5b58 2e72 6573 6574 5f69 6e64  cat([X.reset_ind
+00027d20: 6578 2864 726f 703d 5472 7565 292c 2079  ex(drop=True), y
+00027d30: 5d2c 2061 7869 733d 3129 0a20 2020 2020  ], axis=1).     
+00027d40: 2020 2020 2020 2064 662e 696e 6465 7820         df.index 
+00027d50: 3d20 585f 696e 6465 780a 2020 2020 2020  = X_index.      
+00027d60: 2020 2323 2320 4e6f 7720 796f 7520 6361    ### Now you ca
+00027d70: 6e20 7072 6f63 6573 7320 7468 6520 5820  n process the X 
+00027d80: 616e 6420 7920 6461 7461 7365 7473 2023  and y datasets #
+00027d90: 2323 230a 2020 2020 2020 2020 6966 2069  ###.        if i
+00027da0: 7369 6e73 7461 6e63 6528 792c 2070 642e  sinstance(y, pd.
+00027db0: 5365 7269 6573 293a 0a20 2020 2020 2020  Series):.       
+00027dc0: 2020 2020 2074 6172 6765 7420 3d20 792e       target = y.
+00027dd0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00027de0: 2069 6620 7461 7267 6574 2069 7320 4e6f   if target is No
+00027df0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027e00: 2020 2020 7072 696e 7428 2720 2020 7920      print('   y 
+00027e10: 696e 7075 7420 6973 2061 2070 616e 6461  input is a panda
+00027e20: 7320 7365 7269 6573 2077 6974 6820 6e6f  s series with no
+00027e30: 206e 616d 652e 2043 6f6e 7665 7274 2069   name. Convert i
+00027e40: 7420 616e 6420 7265 2d74 7279 2e27 290a  t and re-try.').
+00027e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027e60: 7265 7475 726e 2058 2c20 7920 2020 2020  return X, y     
+00027e70: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00027e80: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00027e90: 6e63 6528 792c 2070 642e 4461 7461 4672  nce(y, pd.DataFr
+00027ea0: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
+00027eb0: 2020 7461 7267 6574 203d 2079 2e63 6f6c    target = y.col
+00027ec0: 756d 6e73 2e74 6f6c 6973 7428 290a 2020  umns.tolist().  
+00027ed0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00027ee0: 7461 6e63 6528 582c 206e 702e 6e64 6172  tance(X, np.ndar
+00027ef0: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
+00027f00: 2020 7072 696e 7428 2779 206d 7573 7420    print('y must 
+00027f10: 6265 2061 2070 642e 5365 7269 6573 206f  be a pd.Series o
+00027f20: 7220 7064 2e44 6174 6146 7261 6d65 2073  r pd.DataFrame s
+00027f30: 696e 6365 2077 6520 7573 6520 636f 6c75  ince we use colu
+00027f40: 6d6e 206e 616d 6573 2074 6f20 6275 696c  mn names to buil
+00027f50: 6420 6461 7461 2070 6970 656c 696e 652e  d data pipeline.
+00027f60: 2052 6574 7572 6e69 6e67 2729 0a20 2020   Returning').   
+00027f70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00027f80: 7b7d 2c20 7b7d 0a20 2020 2020 2020 2023  {}, {}.        #
+00027f90: 2323 2320 5365 6e64 2074 6172 6765 7420  ### Send target 
+00027fa0: 7661 7269 6162 6c65 2061 7320 6974 2069  variable as it i
+00027fb0: 7320 736f 2074 6861 7420 795f 7472 6169  s so that y_trai
+00027fc0: 6e20 6973 2061 6e61 6c79 7a65 6420 7072  n is analyzed pr
+00027fd0: 6f70 6572 6c79 2023 2323 0a20 2020 2020  operly ###.     
+00027fe0: 2020 2023 2053 656c 6563 7420 6665 6174     # Select feat
+00027ff0: 7572 6573 2075 7369 6e67 2066 6561 7475  ures using featu
+00028000: 7265 7769 7a0a 2020 2020 2020 2020 6665  rewiz.        fe
+00028010: 6174 7572 6573 2c20 585f 7365 6c20 3d20  atures, X_sel = 
+00028020: 6665 6174 7572 6577 697a 2864 662c 2074  featurewiz(df, t
+00028030: 6172 6765 742c 2073 656c 662e 636f 7272  arget, self.corr
+00028040: 5f6c 696d 6974 2c20 7365 6c66 2e76 6572  _limit, self.ver
+00028050: 626f 7365 2c20 7365 6c66 2e73 6570 2c20  bose, self.sep, 
+00028060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028070: 2073 656c 662e 6865 6164 6572 2c20 7365   self.header, se
+00028080: 6c66 2e74 6573 745f 6461 7461 2c20 7365  lf.test_data, se
+00028090: 6c66 2e66 6561 7475 7265 5f65 6e67 672c  lf.feature_engg,
+000280a0: 2073 656c 662e 6361 7465 676f 7279 5f65   self.category_e
+000280b0: 6e63 6f64 6572 732c 0a20 2020 2020 2020  ncoders,.       
+000280c0: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
+000280d0: 736b 5f78 6762 6f6f 7374 5f66 6c61 672c  sk_xgboost_flag,
+000280e0: 2073 656c 662e 6e72 6f77 732c 2073 656c   self.nrows, sel
+000280f0: 662e 736b 6970 5f73 756c 6f76 290a 2020  f.skip_sulov).  
+00028100: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
+00028110: 7468 6520 7265 6d61 696e 696e 6720 636f  the remaining co
+00028120: 6c75 6d6e 206e 616d 6573 2062 6163 6b20  lumn names back 
+00028130: 746f 2069 6e74 6567 6572 7320 616e 6420  to integers and 
+00028140: 6472 6f70 2074 6865 0a20 2020 2020 2020  drop the.       
+00028150: 2064 6966 6674 696d 6520 3d20 6d61 7828   difftime = max(
+00028160: 312c 2069 6e74 2874 696d 652e 7469 6d65  1, int(time.time
+00028170: 2829 2d73 7461 7274 5f74 696d 6529 290a  ()-start_time)).
+00028180: 2020 2020 2020 2020 7072 696e 7428 2720          print(' 
+00028190: 2020 2054 696d 6520 7461 6b65 6e20 746f     Time taken to
+000281a0: 2063 7265 6174 6520 656e 7469 7265 2070   create entire p
+000281b0: 6970 656c 696e 6520 3d20 2573 2073 6563  ipeline = %s sec
+000281c0: 6f6e 6428 7329 2720 2564 6966 6674 696d  ond(s)' %difftim
+000281d0: 6529 0a20 2020 2020 2020 2023 2063 6f6c  e).        # col
+000281e0: 756d 6e20 6f66 206c 6162 656c 730a 2020  umn of labels.  
+000281f0: 2020 2020 2020 7365 6c66 2e66 6561 7475        self.featu
+00028200: 7265 7320 3d20 6665 6174 7572 6573 0a20  res = features. 
+00028210: 2020 2020 2020 2073 656c 662e 585f 7365         self.X_se
+00028220: 6c20 3d20 585f 7365 6c0a 2020 2020 2020  l = X_sel.      
+00028230: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+00028240: 2020 2064 6566 2074 7261 6e73 666f 726d     def transform
+00028250: 2873 656c 662c 2058 293a 0a20 2020 2020  (self, X):.     
+00028260: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00028270: 2020 2020 7265 7475 726e 2058 5b73 656c      return X[sel
+00028280: 662e 6665 6174 7572 6573 5d0a 2020 2020  f.features].    
+00028290: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+000282a0: 2020 2020 2020 2020 7072 696e 7428 2752          print('R
+000282b0: 6574 7572 6e69 6e67 2074 7261 6e73 666f  eturning transfo
+000282c0: 726d 6564 2064 6174 6166 7261 6d65 2077  rmed dataframe w
+000282d0: 6974 6820 2564 2066 6561 7475 7265 7327  ith %d features'
+000282e0: 2025 6c65 6e28 7365 6c66 2e66 6561 7475   %len(self.featu
+000282f0: 7265 7329 290a 2020 2020 2020 2020 2020  res)).          
+00028300: 2020 7265 7475 726e 2073 656c 662e 585f    return self.X_
+00028310: 7365 6c0a 2323 2323 2323 2323 2323 2323  sel.############
 00028320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00028330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028340: 2323 2323 230a 6465 6620 4544 415f 7265  #####.def EDA_re
-00028350: 6d6f 7665 5f73 7065 6369 616c 5f63 6861  move_special_cha
-00028360: 7273 2864 6629 3a0a 2020 2020 2222 220a  rs(df):.    """.
-00028370: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-00028380: 6e20 7265 6d6f 7665 7320 7370 6563 6961  n removes specia
-00028390: 6c20 6368 6172 7320 6672 6f6d 2063 6f6c  l chars from col
-000283a0: 756d 6e20 6e61 6d65 7320 616e 6420 7265  umn names and re
-000283b0: 7475 726e 7320 6120 6466 2077 6974 6820  turns a df with 
-000283c0: 6e65 7720 636f 6c75 6d6e 206e 616d 6573  new column names
-000283d0: 2e0a 2020 2020 496e 7075 7473 2061 6e64  ..    Inputs and
-000283e0: 206f 7574 7075 7473 2061 7265 2062 6f74   outputs are bot
-000283f0: 6820 7468 6520 7361 6d65 2064 6174 6166  h the same dataf
-00028400: 7261 6d65 2065 7863 6570 7420 636f 6c75  rame except colu
-00028410: 6d6e 206e 616d 6573 2061 7265 2063 6861  mn names are cha
-00028420: 6e67 6564 2e0a 2020 2020 2222 220a 2020  nged..    """.  
-00028430: 2020 696d 706f 7274 2063 6f70 790a 2020    import copy.  
-00028440: 2020 696d 706f 7274 2072 650a 2020 2020    import re.    
-00028450: 636f 6c73 203d 2064 662e 636f 6c75 6d6e  cols = df.column
-00028460: 732e 746f 6c69 7374 2829 0a20 2020 2063  s.tolist().    c
-00028470: 6f70 795f 636f 6c73 203d 2063 6f70 792e  opy_cols = copy.
-00028480: 6465 6570 636f 7079 2863 6f6c 7329 0a20  deepcopy(cols). 
-00028490: 2020 2073 6572 203d 2070 642e 5365 7269     ser = pd.Seri
-000284a0: 6573 2863 6f6c 7329 0a20 2020 2023 2323  es(cols).    ###
-000284b0: 2054 6869 7320 6675 6e63 7469 6f6e 2072   This function r
-000284c0: 656d 6f76 6573 2061 6c6c 2073 7065 6369  emoves all speci
-000284d0: 616c 2063 6861 7273 2066 726f 6d20 6120  al chars from a 
-000284e0: 6c69 7374 2023 2323 0a20 2020 2072 656d  list ###.    rem
-000284f0: 6f76 655f 7370 6563 6961 6c5f 6368 6172  ove_special_char
-00028500: 7320 3d20 206c 616d 6264 6120 783a 7265  s =  lambda x:re
-00028510: 2e73 7562 2827 5b5e 412d 5a61 2d7a 302d  .sub('[^A-Za-z0-
-00028520: 395f 5d2b 272c 2027 272c 2078 290a 2020  9_]+', '', x).  
-00028530: 2020 6e65 776c 7320 3d20 7365 722e 6d61    newls = ser.ma
-00028540: 7028 7265 6d6f 7665 5f73 7065 6369 616c  p(remove_special
-00028550: 5f63 6861 7273 292e 7661 6c75 6573 2e74  _chars).values.t
-00028560: 6f6c 6973 7428 290a 2020 2020 6466 2e63  olist().    df.c
-00028570: 6f6c 756d 6e73 203d 206e 6577 6c73 0a20  olumns = newls. 
-00028580: 2020 2072 6574 7572 6e20 6466 0a23 2323     return df.###
-00028590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000285a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000285b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028370: 2323 2323 2323 230a 6465 6620 4544 415f  #######.def EDA_
+00028380: 7265 6d6f 7665 5f73 7065 6369 616c 5f63  remove_special_c
+00028390: 6861 7273 2864 6629 3a0a 2020 2020 2222  hars(df):.    ""
+000283a0: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
+000283b0: 696f 6e20 7265 6d6f 7665 7320 7370 6563  ion removes spec
+000283c0: 6961 6c20 6368 6172 7320 6672 6f6d 2063  ial chars from c
+000283d0: 6f6c 756d 6e20 6e61 6d65 7320 616e 6420  olumn names and 
+000283e0: 7265 7475 726e 7320 6120 6466 2077 6974  returns a df wit
+000283f0: 6820 6e65 7720 636f 6c75 6d6e 206e 616d  h new column nam
+00028400: 6573 2e0a 2020 2020 496e 7075 7473 2061  es..    Inputs a
+00028410: 6e64 206f 7574 7075 7473 2061 7265 2062  nd outputs are b
+00028420: 6f74 6820 7468 6520 7361 6d65 2064 6174  oth the same dat
+00028430: 6166 7261 6d65 2065 7863 6570 7420 636f  aframe except co
+00028440: 6c75 6d6e 206e 616d 6573 2061 7265 2063  lumn names are c
+00028450: 6861 6e67 6564 2e0a 2020 2020 2222 220a  hanged..    """.
+00028460: 2020 2020 696d 706f 7274 2063 6f70 790a      import copy.
+00028470: 2020 2020 696d 706f 7274 2072 650a 2020      import re.  
+00028480: 2020 636f 6c73 203d 2064 662e 636f 6c75    cols = df.colu
+00028490: 6d6e 732e 746f 6c69 7374 2829 0a20 2020  mns.tolist().   
+000284a0: 2063 6f70 795f 636f 6c73 203d 2063 6f70   copy_cols = cop
+000284b0: 792e 6465 6570 636f 7079 2863 6f6c 7329  y.deepcopy(cols)
+000284c0: 0a20 2020 2073 6572 203d 2070 642e 5365  .    ser = pd.Se
+000284d0: 7269 6573 2863 6f6c 7329 0a20 2020 2023  ries(cols).    #
+000284e0: 2323 2054 6869 7320 6675 6e63 7469 6f6e  ## This function
+000284f0: 2072 656d 6f76 6573 2061 6c6c 2073 7065   removes all spe
+00028500: 6369 616c 2063 6861 7273 2066 726f 6d20  cial chars from 
+00028510: 6120 6c69 7374 2023 2323 0a20 2020 2072  a list ###.    r
+00028520: 656d 6f76 655f 7370 6563 6961 6c5f 6368  emove_special_ch
+00028530: 6172 7320 3d20 206c 616d 6264 6120 783a  ars =  lambda x:
+00028540: 7265 2e73 7562 2827 5b5e 412d 5a61 2d7a  re.sub('[^A-Za-z
+00028550: 302d 395f 5d2b 272c 2027 272c 2078 290a  0-9_]+', '', x).
+00028560: 2020 2020 6e65 776c 7320 3d20 7365 722e      newls = ser.
+00028570: 6d61 7028 7265 6d6f 7665 5f73 7065 6369  map(remove_speci
+00028580: 616c 5f63 6861 7273 292e 7661 6c75 6573  al_chars).values
+00028590: 2e74 6f6c 6973 7428 290a 2020 2020 6466  .tolist().    df
+000285a0: 2e63 6f6c 756d 6e73 203d 206e 6577 6c73  .columns = newls
+000285b0: 0a20 2020 2072 6574 7572 6e20 6466 0a23  .    return df.#
 000285c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000285d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000285e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000285f0: 0a64 6566 2064 6173 6b5f 7867 626f 6f73  .def dask_xgboos
-00028600: 745f 7472 6169 6e69 6e67 2858 5f74 7261  t_training(X_tra
-00028610: 696e 782c 2079 5f74 7261 696e 782c 2070  inx, y_trainx, p
-00028620: 6172 616d 7329 3a0a 2020 2020 0a20 2020  arams):.    .   
-00028630: 2063 6c75 7374 6572 203d 2064 6173 6b2e   cluster = dask.
-00028640: 6469 7374 7269 6275 7465 642e 4c6f 6361  distributed.Loca
-00028650: 6c43 6c75 7374 6572 2829 0a20 2020 2064  lCluster().    d
-00028660: 6173 6b5f 636c 6965 6e74 203d 2064 6173  ask_client = das
-00028670: 6b2e 6469 7374 7269 6275 7465 642e 436c  k.distributed.Cl
-00028680: 6965 6e74 2863 6c75 7374 6572 290a 2020  ient(cluster).  
-00028690: 2020 585f 7472 6169 6e78 203d 2064 642e    X_trainx = dd.
-000286a0: 6672 6f6d 5f70 616e 6461 7328 585f 7472  from_pandas(X_tr
-000286b0: 6169 6e2c 206e 7061 7274 6974 696f 6e73  ain, npartitions
-000286c0: 3d31 290a 2020 2020 795f 7472 6169 6e78  =1).    y_trainx
-000286d0: 203d 2064 642e 6672 6f6d 5f70 616e 6461   = dd.from_panda
-000286e0: 7328 795f 7472 6169 6e2c 206e 7061 7274  s(y_train, npart
-000286f0: 6974 696f 6e73 3d31 290a 2020 2020 7072  itions=1).    pr
-00028700: 696e 7428 2244 4153 4b20 5847 426f 6f73  int("DASK XGBoos
-00028710: 7420 7472 6169 6e69 6e67 2e2e 2e22 290a  t training...").
-00028720: 2020 2020 6474 7261 696e 203d 2078 6762      dtrain = xgb
-00028730: 2e64 6173 6b2e 4461 736b 444d 6174 7269  .dask.DaskDMatri
-00028740: 7828 6461 736b 5f63 6c69 656e 742c 2058  x(dask_client, X
-00028750: 5f74 7261 696e 782c 2079 5f74 7261 696e  _trainx, y_train
-00028760: 7829 0a20 2020 2062 7374 203d 2078 6762  x).    bst = xgb
-00028770: 2e64 6173 6b2e 7472 6169 6e28 6461 736b  .dask.train(dask
-00028780: 5f63 6c69 656e 742c 2070 6172 616d 732c  _client, params,
-00028790: 2064 7472 6169 6e2c 206e 756d 5f62 6f6f   dtrain, num_boo
-000287a0: 7374 5f72 6f75 6e64 3d31 3029 0a20 2020  st_round=10).   
-000287b0: 2064 6173 6b5f 636c 6965 6e74 2e63 6c6f   dask_client.clo
-000287c0: 7365 2829 0a20 2020 2070 7269 6e74 2822  se().    print("
-000287d0: 2020 2020 7472 6169 6e69 6e67 2063 6f6d      training com
-000287e0: 706c 6574 6564 2e2e 2e22 290a 2020 2020  pleted...").    
-000287f0: 7265 7475 726e 2062 7374 0a23 2323 2323  return bst.#####
-00028800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000285f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028620: 2323 0a64 6566 2064 6173 6b5f 7867 626f  ##.def dask_xgbo
+00028630: 6f73 745f 7472 6169 6e69 6e67 2858 5f74  ost_training(X_t
+00028640: 7261 696e 782c 2079 5f74 7261 696e 782c  rainx, y_trainx,
+00028650: 2070 6172 616d 7329 3a0a 2020 2020 0a20   params):.    . 
+00028660: 2020 2063 6c75 7374 6572 203d 2064 6173     cluster = das
+00028670: 6b2e 6469 7374 7269 6275 7465 642e 4c6f  k.distributed.Lo
+00028680: 6361 6c43 6c75 7374 6572 2829 0a20 2020  calCluster().   
+00028690: 2064 6173 6b5f 636c 6965 6e74 203d 2064   dask_client = d
+000286a0: 6173 6b2e 6469 7374 7269 6275 7465 642e  ask.distributed.
+000286b0: 436c 6965 6e74 2863 6c75 7374 6572 290a  Client(cluster).
+000286c0: 2020 2020 585f 7472 6169 6e78 203d 2064      X_trainx = d
+000286d0: 642e 6672 6f6d 5f70 616e 6461 7328 585f  d.from_pandas(X_
+000286e0: 7472 6169 6e2c 206e 7061 7274 6974 696f  train, npartitio
+000286f0: 6e73 3d31 290a 2020 2020 795f 7472 6169  ns=1).    y_trai
+00028700: 6e78 203d 2064 642e 6672 6f6d 5f70 616e  nx = dd.from_pan
+00028710: 6461 7328 795f 7472 6169 6e2c 206e 7061  das(y_train, npa
+00028720: 7274 6974 696f 6e73 3d31 290a 2020 2020  rtitions=1).    
+00028730: 7072 696e 7428 2244 4153 4b20 5847 426f  print("DASK XGBo
+00028740: 6f73 7420 7472 6169 6e69 6e67 2e2e 2e22  ost training..."
+00028750: 290a 2020 2020 6474 7261 696e 203d 2078  ).    dtrain = x
+00028760: 6762 2e64 6173 6b2e 4461 736b 444d 6174  gb.dask.DaskDMat
+00028770: 7269 7828 6461 736b 5f63 6c69 656e 742c  rix(dask_client,
+00028780: 2058 5f74 7261 696e 782c 2079 5f74 7261   X_trainx, y_tra
+00028790: 696e 7829 0a20 2020 2062 7374 203d 2078  inx).    bst = x
+000287a0: 6762 2e64 6173 6b2e 7472 6169 6e28 6461  gb.dask.train(da
+000287b0: 736b 5f63 6c69 656e 742c 2070 6172 616d  sk_client, param
+000287c0: 732c 2064 7472 6169 6e2c 206e 756d 5f62  s, dtrain, num_b
+000287d0: 6f6f 7374 5f72 6f75 6e64 3d31 3029 0a20  oost_round=10). 
+000287e0: 2020 2064 6173 6b5f 636c 6965 6e74 2e63     dask_client.c
+000287f0: 6c6f 7365 2829 0a20 2020 2070 7269 6e74  lose().    print
+00028800: 2822 2020 2020 7472 6169 6e69 6e67 2063  ("    training c
+00028810: 6f6d 706c 6574 6564 2e2e 2e22 290a 2020  ompleted...").  
+00028820: 2020 7265 7475 726e 2062 7374 0a23 2323    return bst.###
 00028830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028840: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00028850: 6465 6620 4645 5f72 656d 6f76 655f 636f  def FE_remove_co
-00028860: 6d6d 6173 5f69 6e5f 6e75 6d65 7269 6373  mmas_in_numerics
-00028870: 2874 7261 696e 2c20 6e75 6d73 3d5b 5d29  (train, nums=[])
-00028880: 3a0a 2020 2020 2222 2220 0a20 2020 2054  :.    """ .    T
-00028890: 6869 7320 6675 6e63 7469 6f6e 2072 656d  his function rem
-000288a0: 6f76 6573 2063 6f6d 6d61 7320 696e 206e  oves commas in n
-000288b0: 756d 6572 6963 2063 6f6c 756d 6e73 2061  umeric columns a
-000288c0: 6e64 2072 6574 7572 6e73 2074 6865 2063  nd returns the c
-000288d0: 6f6c 756d 6e73 2074 7261 6e73 666f 726d  olumns transform
-000288e0: 6564 2e0a 2020 2020 596f 7520 6361 6e20  ed..    You can 
-000288f0: 7365 6e64 2069 6e20 6120 6461 7461 6672  send in a datafr
-00028900: 616d 6520 7769 7468 206f 6e65 2063 6f6c  ame with one col
-00028910: 756d 6e20 6e61 6d65 2061 7320 6120 7374  umn name as a st
-00028920: 7269 6e67 206f 7220 6120 6c69 7374 206f  ring or a list o
-00028930: 6620 636f 6c75 6d6e 732e 0a20 2020 2052  f columns..    R
-00028940: 6574 7572 6e73 2061 2073 696e 676c 6520  eturns a single 
-00028950: 6172 7261 7920 6966 206f 6e6c 7920 6f6e  array if only on
-00028960: 6520 636f 6c75 6d6e 2069 7320 7365 6e74  e column is sent
-00028970: 2e0a 2020 2020 5265 7475 726e 7320 7468  ..    Returns th
-00028980: 6520 656e 7469 7265 2064 6174 6166 7261  e entire datafra
-00028990: 6d65 2069 6620 6120 6c69 7374 206f 6620  me if a list of 
-000289a0: 636f 6c75 6d6e 7320 6973 2073 656e 742e  columns is sent.
-000289b0: 2054 6869 7320 696e 636c 7564 6573 2061   This includes a
-000289c0: 6c6c 2063 6f6c 756d 6e73 2e0a 2020 2020  ll columns..    
-000289d0: 2222 220a 2020 2020 7472 6169 6e20 3d20  """.    train = 
-000289e0: 636f 7079 2e64 6565 7063 6f70 7928 7472  copy.deepcopy(tr
-000289f0: 6169 6e29 0a20 2020 2069 6620 6973 696e  ain).    if isin
-00028a00: 7374 616e 6365 286e 756d 732c 2073 7472  stance(nums, str
-00028a10: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00028a20: 6e20 7472 6169 6e5b 6561 6368 5f6e 756d  n train[each_num
-00028a30: 5d2e 6d61 7028 6c61 6d62 6461 2078 3a20  ].map(lambda x: 
-00028a40: 666c 6f61 7428 2222 2e6a 6f69 6e28 2078  float("".join( x
-00028a50: 2e73 706c 6974 2822 2c22 2929 2929 2e76  .split(",")))).v
-00028a60: 616c 7565 730a 2020 2020 656c 7365 3a0a  alues.    else:.
-00028a70: 2020 2020 2020 2020 666f 7220 6561 6368          for each
-00028a80: 5f6e 756d 2069 6e20 6e75 6d73 3a0a 2020  _num in nums:.  
-00028a90: 2020 2020 2020 2020 2020 7472 6169 6e5b            train[
-00028aa0: 6561 6368 5f6e 756d 5d20 3d20 7472 6169  each_num] = trai
-00028ab0: 6e5b 6561 6368 5f6e 756d 5d2e 6d61 7028  n[each_num].map(
-00028ac0: 6c61 6d62 6461 2078 3a20 666c 6f61 7428  lambda x: float(
-00028ad0: 2222 2e6a 6f69 6e28 2078 2e73 706c 6974  "".join( x.split
-00028ae0: 2822 2c22 2929 2929 2e76 616c 7565 730a  (",")))).values.
-00028af0: 2020 2020 7265 7475 726e 2074 7261 696e      return train
-00028b00: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00028b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028880: 230a 6465 6620 4645 5f72 656d 6f76 655f  #.def FE_remove_
+00028890: 636f 6d6d 6173 5f69 6e5f 6e75 6d65 7269  commas_in_numeri
+000288a0: 6373 2874 7261 696e 2c20 6e75 6d73 3d5b  cs(train, nums=[
+000288b0: 5d29 3a0a 2020 2020 2222 2220 0a20 2020  ]):.    """ .   
+000288c0: 2054 6869 7320 6675 6e63 7469 6f6e 2072   This function r
+000288d0: 656d 6f76 6573 2063 6f6d 6d61 7320 696e  emoves commas in
+000288e0: 206e 756d 6572 6963 2063 6f6c 756d 6e73   numeric columns
+000288f0: 2061 6e64 2072 6574 7572 6e73 2074 6865   and returns the
+00028900: 2063 6f6c 756d 6e73 2074 7261 6e73 666f   columns transfo
+00028910: 726d 6564 2e0a 2020 2020 596f 7520 6361  rmed..    You ca
+00028920: 6e20 7365 6e64 2069 6e20 6120 6461 7461  n send in a data
+00028930: 6672 616d 6520 7769 7468 206f 6e65 2063  frame with one c
+00028940: 6f6c 756d 6e20 6e61 6d65 2061 7320 6120  olumn name as a 
+00028950: 7374 7269 6e67 206f 7220 6120 6c69 7374  string or a list
+00028960: 206f 6620 636f 6c75 6d6e 732e 0a20 2020   of columns..   
+00028970: 2052 6574 7572 6e73 2061 2073 696e 676c   Returns a singl
+00028980: 6520 6172 7261 7920 6966 206f 6e6c 7920  e array if only 
+00028990: 6f6e 6520 636f 6c75 6d6e 2069 7320 7365  one column is se
+000289a0: 6e74 2e0a 2020 2020 5265 7475 726e 7320  nt..    Returns 
+000289b0: 7468 6520 656e 7469 7265 2064 6174 6166  the entire dataf
+000289c0: 7261 6d65 2069 6620 6120 6c69 7374 206f  rame if a list o
+000289d0: 6620 636f 6c75 6d6e 7320 6973 2073 656e  f columns is sen
+000289e0: 742e 2054 6869 7320 696e 636c 7564 6573  t. This includes
+000289f0: 2061 6c6c 2063 6f6c 756d 6e73 2e0a 2020   all columns..  
+00028a00: 2020 2222 220a 2020 2020 7472 6169 6e20    """.    train 
+00028a10: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
+00028a20: 7472 6169 6e29 0a20 2020 2069 6620 6973  train).    if is
+00028a30: 696e 7374 616e 6365 286e 756d 732c 2073  instance(nums, s
+00028a40: 7472 293a 0a20 2020 2020 2020 2072 6574  tr):.        ret
+00028a50: 7572 6e20 7472 6169 6e5b 6561 6368 5f6e  urn train[each_n
+00028a60: 756d 5d2e 6d61 7028 6c61 6d62 6461 2078  um].map(lambda x
+00028a70: 3a20 666c 6f61 7428 2222 2e6a 6f69 6e28  : float("".join(
+00028a80: 2078 2e73 706c 6974 2822 2c22 2929 2929   x.split(","))))
+00028a90: 2e76 616c 7565 730a 2020 2020 656c 7365  .values.    else
+00028aa0: 3a0a 2020 2020 2020 2020 666f 7220 6561  :.        for ea
+00028ab0: 6368 5f6e 756d 2069 6e20 6e75 6d73 3a0a  ch_num in nums:.
+00028ac0: 2020 2020 2020 2020 2020 2020 7472 6169              trai
+00028ad0: 6e5b 6561 6368 5f6e 756d 5d20 3d20 7472  n[each_num] = tr
+00028ae0: 6169 6e5b 6561 6368 5f6e 756d 5d2e 6d61  ain[each_num].ma
+00028af0: 7028 6c61 6d62 6461 2078 3a20 666c 6f61  p(lambda x: floa
+00028b00: 7428 2222 2e6a 6f69 6e28 2078 2e73 706c  t("".join( x.spl
+00028b10: 6974 2822 2c22 2929 2929 2e76 616c 7565  it(",")))).value
+00028b20: 730a 2020 2020 7265 7475 726e 2074 7261  s.    return tra
+00028b30: 696e 0a23 2323 2323 2323 2323 2323 2323  in.#############
 00028b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00028b50: 2323 2323 230a 0a0a                      #####...
+00028b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028b60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028b70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00028b80: 2323 2323 2323 230a 0a0a                 #######...
```

### Comparing `featurewiz-0.2.7/featurewiz/ml_models.py` & `featurewiz-0.2.8/featurewiz/ml_models.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/my_encoders.py` & `featurewiz-0.2.8/featurewiz/my_encoders.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/settings.py` & `featurewiz-0.2.8/featurewiz/settings.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/stacking_models.py` & `featurewiz-0.2.8/featurewiz/stacking_models.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz/sulov_method.py` & `featurewiz-0.2.8/featurewiz/sulov_method.py`

 * *Files identical despite different names*

### Comparing `featurewiz-0.2.7/featurewiz.egg-info/PKG-INFO` & `featurewiz-0.2.8/featurewiz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,190 +1,165 @@
 Metadata-Version: 2.1
 Name: featurewiz
-Version: 0.2.7
+Version: 0.2.8
 Summary: Select Best Features from your data set - any size - now with XGBoost!
 Home-page: https://github.com/AutoViML/featurewiz
 Author: Ram Seshadri
 Author-email: rsesha2001@yahoo.com
 License: Apache License 2.0
 Description: # featurewiz
+        `featurewiz` is a powerful feature selection library that has a number of features that make it stand out from the competition, including:
+        <ol>
+        <li>It provides one of the best automatic feature selection algorithms (Minimum Redundancy Maximum Relevance (MRMR)) described by wikipedia as: <a href="https://en.wikipedia.org/wiki/Minimum_redundancy_feature_selection">"The MRMR selection has been found to be more powerful than the maximum relevance feature selection"</a> such as Boruta.</li>
+        <li>It selects the best number of un-correlated features that have maximum mutual information about the target without having to specify the number of features</li>
+        <li>It is fast and easy to use, and comes with a number of helpful features, such as a built-in categorical-to-numeric encoder and a powerful feature engineering module</li>
+        <li>It is well-documented, and it comes with a number of <a href="https://github.com/AutoViML/featurewiz/tree/main/examples">examples</a>.</li>
+        <li>It is actively maintained, and it is regularly updated with new features and bug fixes.</li>
+        </ol>
+        If you are looking for a single feature selection library, we would definitely recommend checking out featurewiz. It is a powerful tool that can help you to improve the performance of your machine learning models.
         
-        ![banner](featurewiz_logos.png)
-        
-        ##  Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
-        <a href="updates.md">Check out more latest updates from this page</a><br>
-        As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo), featurewiz is now available on conda-forge. You can try:<br>
-        
-        ```
-         conda install -c conda-forge featurewiz
-        ```
-        
-        ### If the above conda install fails, you can try installing featurewiz this way:
-        ##Step 1: Install featurewiz first<br>
-        
-        ```
-         !pip install featurewiz --ignore-installed --no-deps
-         !pip install xlrd --ignore-installed --no-deps 
-        ```
-        
-        ##Step 2: Next, install Pillow since Kaggle has an incompatible version. <br>
+        # Table of Contents
+        <ul>
+        <li><a href="#introduction">What is featurewiz</a></li>
+        <li><a href="#working">How it works</a></li>
+        <li><a href="#tips">Tips for using featurewiz</a></li>
+        <li><a href="#install">How to install featurewiz</a></li>
+        <li><a href="#usage">Usage</a></li>
+        <li><a href="#api">API</a></li>
+        <li><a href="#additional">Additional Tips</a></li>
+        <li><a href="#maintainers">Maintainers</a></li>
+        <li><a href="#contributing">Contributing</a></li>
+        <li><a href="#license">License</a></li>
+        <li><a href="#disclaimer">Disclaimer</a></li>
+        </ul>
+        <p>
         
-        ```
-         !pip install Pillow==9.0.0
-        ```
+        ![banner](featurewiz_logos.png)
         
-        ## What is featurewiz?
+        ## Introduction
         `featurewiz` a new python library for creating and selecting the best features in your data set fast!
         `featurewiz` can be used in one or two ways. Both are explained below.
         
-        ## 1.  Feature Engineering
+        ### 1.  Feature Engineering
         <p>The first step is not absolutely necessary but it can be used to create new features that may or may not be helpful (be careful with automated feature engineering tools!).<p>
         1. <b>Performing Feature Engineering</b>: One of the gaps in open source AutoML tools and especially Auto_ViML has been the lack of feature engineering capabilities that high powered competitions such as Kaggle required. The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables was difficult and sifting through those hundreds of new features to find best features was difficult and left only to "experts" or "professionals". featurewiz was created to help you in this endeavor.<br>
         <p>featurewiz now enables you to add hundreds of such features with a single line of code. Set the "feature_engg" flag to "interactions", "groupby" or "target" and featurewiz will select the best encoders for each of those options and create hundreds (perhaps thousands) of features in one go. Not only that, using the next step, featurewiz will sift through numerous such variables and find only the least correlated and most relevant features to your model. All in one step!.<br>
         
-        You must use this syntax for feature engg. Otherwise, featurewiz will give an error:
-        
-        ```
-        import featurewiz as FW
-        outputs = FW.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
-        		header=0, test_data='',feature_engg='', category_encoders='',
-        		dask_xgboost_flag=False, nrows=None)
-        ```
-        
         ![feature_engg](feature_engg.jpg)
         
-        ## 2.  Feature Selection
+        ### 2.  Feature Selection
         <p>The second step is Feature Selection. `featurewiz` uses the MRMR (Minimum Redundancy Maximum Relevance) algorithm as the basis for its feature selection. <br>
         <b> Why do Feature Selection</b>? Once you have created 100's of new features, you still have three questions left to answer:
         1. How do we interpret those newly created features?
         2. Which of these features is important and which are useless? How many of them are highly correlated to each other causing redundancy?
         3. Does the model overfit now on these new features and perform better or worse than before?
         <br>
         All are very important questions and featurewiz answers them by using the SULOV method and Recursive XGBoost to reduce features in your dataset to the best "minimum optimal" features for the model.<br>
         <p><b>SULOV</b>: SULOV stands for `Searching for Uncorrelated List of Variables`. The SULOV algorithm is based on the Minimum-Redundancy-Maximum-Relevance (MRMR) <a href="https://towardsdatascience.com/mrmr-explained-exactly-how-you-wished-someone-explained-to-you-9cf4ed27458b">algorithm explained in this article</a> as one of the best feature selection methods. To understand how MRMR works and how it is different from `Boruta` and other feature selection methods, see the chart below. Here "Minimal Optimal" refers to the MRMR and featurewiz kind of algorithms while "all-relevant" refers to Boruta kind of algorithms.<br>
         
         ![MRMR_chart](MRMR.png)
-        <br>
-        The working of the SULOV algorithm is as follows:
+        
+        ## Working
+        `featurewiz` performs feature selection in 2 steps. Each step is explained below.
+        <b>The working of the `SULOV` algorithm</b> is as follows:
         <ol>
-        <li>Find all the pairs of highly correlated variables exceeding a correlation threshold (say absolute(0.7)).
-        <li>Then find their MIS score (Mutual Information Score) to the target variable. MIS is a non-parametric scoring method. So its suitable for all kinds of variables and target.
-        <li>Now take each pair of correlated variables, then knock off the one with the lower MIS score.
-        <li>What’s left is the ones with the highest Information scores and least correlation with each other.
+        <li>Find all the pairs of highly correlated variables exceeding a correlation threshold (say absolute(0.7)).</li>
+        <li>Then find their MIS score (Mutual Information Score) to the target variable. MIS is a non-parametric scoring method. So its suitable for all kinds of variables and target.</li>
+        <li>Now take each pair of correlated variables, then knock off the one with the lower MIS score.</li>
+        <li>What’s left is the ones with the highest Information scores and least correlation with each other.</li>
         </ol>
         
         ![sulov](SULOV.jpg)
         
-        <b>Recursive XGBoost</b>: Once SULOV has selected variables that have high mutual information scores with least less correlation amongst them, we use XGBoost to repeatedly find best features among the remaining variables after SULOV. The Recursive XGBoost method is explained in this chart below.
-        Here is how it works:
+        <b>The working of the Recursive XGBoost</b> is as follows: 
+        Once SULOV has selected variables that have high mutual information scores with least less correlation amongst them, featurewiz uses XGBoost to repeatedly find the best features among the remaining variables after SULOV. 
         <ol>
-        <li>Select all variables in data set and the full data split into train and valid sets.
-        <li>Find top X features (could be 10) on train using valid for early stopping (to prevent over-fitting)
-        <li>Then take next set of vars and find top X
-        <li>Do this 5 times. Combine all selected features and de-duplicate them.
+        <li>Select all variables in data set and the full data split into train and valid sets.</li>
+        <li>Find top X features (could be 10) on train using valid for early stopping (to prevent over-fitting)</li>
+        <li>Then take next set of vars and find top X</li>
+        <li>Do this 5 times. Combine all selected features and de-duplicate them.</li>
         </ol>
         
         ![xgboost](xgboost.jpg)
         
-        <b>Building the simplest and most "interpretable" model</b>: featurewiz represents the "next best" step you must perform after doing feature engineering  since you might have added some highly correlated or even useless features when you use automated feature engineering. featurewiz ensures you have the least number of features needed to build a high performing or equivalent model.
-        
-        <b>A WORD OF CAUTION:</b> Just because you can engineer new features, doesn't mean you should always create tons of new features. You must make sure you understand what the new features stand for before you attempt to build a model with these (sometimes useless) features. featurewiz displays the SULOV chart which can show you how the 100's of newly created variables added to your dataset are highly correlated to each other and were removed. This will help you understand how feature selection works in featurewiz.
-        
-        ## Table of Contents
-        <ul>
-        <li><a href="#background">Background</a></li>
-        <li><a href="#install">Install</a></li>
-        <li><a href="#usage">Usage</a></li>
-        <li><a href="#api">API</a></li>
-        <li><a href="#maintainers">Maintainers</a></li>
-        <li><a href="#contributing">Contributing</a></li>
-        <li><a href="#license">License</a></li>
-        </ul>
-        
-        ## Background
-        
-        ![background](featurewiz_background.jpg)
-        
-        To learn more about how featurewiz works under the hood, watch this [video](https://www.youtube.com/embed/ZiNutwPcAU0)<br>
-        
-        <p>featurewiz was designed for selecting High Performance variables with the fewest steps.
-        
-        In most cases, featurewiz builds models with 20%-99% fewer features than your original data set with nearly the same or slightly lower performance (this is based on my trials. Your experience may vary).<br>
-        <p>
-        featurewiz is every Data Scientist's feature wizard that will:<ol>
-        <li><b>Automatically pre-process data</b>: you can send in your entire dataframe "as is" and featurewiz will classify and change/label encode categorical variables changes to help XGBoost processing. It classifies variables as numeric or categorical or NLP or date-time variables automatically so it can use them correctly to model.<br>
-        <li><b>Perform feature engineering automatically</b>: The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables is difficult and sifting through those hundreds of new features is painstaking and left only to "experts". Now, with featurewiz you can create hundreds or even thousands of new features with the click of a mouse. This is very helpful when you have a small number of features to start with. However, be careful with this option. You can very easily create a monster with this option.
-        <li><b>Perform feature reduction automatically</b>. When you have small data sets and you know your domain well, it is easy to perhaps do EDA and identify which variables are important. But when you have a very large data set with hundreds if not thousands of variables, selecting the best features from your model can mean the difference between a bloated and highly complex model or a simple model with the fewest and most information-rich features. featurewiz uses XGBoost repeatedly to perform feature selection. You must try it on your large data sets and compare!<br>
-        <li><b>Explain SULOV method graphically </b> using networkx library so you can see which variables are highly correlated to which ones and which of those have high or low mutual information scores automatically. Just set verbose = 2 to see the graph. <br>
-        <li><b>Build a fast LightGBM model </b> using the features selected by featurewiz. There is a function called "simple_lightgbm_model" which you can use to build a fast model. It is a new module, so check it out.<br>
-        </ol>
-        
-        <b>***  Notes of Gratitude ***</b>:<br>
+        ## Tips
+        Here are some additional tips for ML engineers and data scientists when using featurewiz:
         <ol>
-        <li><b>Alex Lekov</b> (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/automl_alex) for his DataBunch and encoders modules which are used by the tool (although with some modifications).</li>
-        <li><b>Category Encoders</b> library in Python : This is an amazing library. Make sure you read all about the encoders that featurewiz uses here: https://contrib.scikit-learn.org/category_encoders/index.html </li>
+        <li><b>Always cross-validate your results</b>: When you use a feature selection tool, it is important to cross-validate your results. This means that you should split your data into a training set and a test set. Use the training set to select features, and then evaluate your model on the test set. This will help you to ensure that your model is not overfitting to the training data.</li>
+        <li><b>Use multiple feature selection tools</b>: It is a good idea to use multiple feature selection tools and compare the results. This will help you to get a better understanding of which features are most important for your data.</li>
+        <li><b>Don't forget to engineer new features</b>: Feature selection is only one part of the process of building a good machine learning model. You should also spend time engineering your features to make them as informative as possible. This can involve things like creating new features, transforming existing features, and removing irrelevant features.</li>
+        <li><b>Don't overfit your model</b>: It is important to avoid overfitting your model to the training data. Overfitting occurs when your model learns the noise in the training data, rather than the underlying signal. To avoid overfitting, you can use regularization techniques, such as lasso or elasticnet.</li>
+        <li><b>Start with a small number of features</b>: When you are first starting out, it is a good idea to start with a small number of features. This will help you to avoid overfitting your model. As you become more experienced, you can experiment with adding more features.</li>
         </ol>
         
         ## Install
         
         **Prerequsites:**
         <ol>
         <li><b>featurewiz is built using xgboost, dask, numpy, pandas and matplotlib</b>. It should run on most Python 3 Anaconda installations. You won't have to import any special libraries other than "dask", "XGBoost" and "networkx" library. Optionally, it uses LightGBM for fast modeling, which it installs automatically. </li>
         <li><b>We use "networkx" library for charts and interpretability</b>. <br>But if you don't have these libraries, featurewiz will install those for you automatically.</li>
         </ol>
-        - [Anaconda](https://docs.anaconda.com/anaconda/install/)
-        
-        To clone featurewiz, it is better to create a new environment, and install the required dependencies:
-        
-        To install from PyPi:
-        
-        ```
-        conda create -n <your_env_name> python=3.7 anaconda
-        conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
-        pip install featurewiz --ignore-installed --no-deps
-        pip install lazytransform
-        or
-        pip install git+https://github.com/AutoViML/featurewiz.git
-        ```
-        
         To install from source:
         
         ```
         cd <featurewiz_Destination>
         git clone git@github.com:AutoViML/featurewiz.git
         # or download and unzip https://github.com/AutoViML/featurewiz/archive/master.zip
         conda create -n <your_env_name> python=3.7 anaconda
         conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
         cd featurewiz
         pip install -r requirements.txt
         ```
         
+        ##  Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
+        <a href="updates.md">Check out more latest updates from this page</a><br>
+        As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo), featurewiz is now available on conda-forge. You can try:<br>
+        
+        ```
+         conda install -c conda-forge featurewiz
+        ```
+        
+        ### If the above conda install fails, you can try installing featurewiz this way:
+        ##Step 1: Install featurewiz first<br>
+        
+        ```
+         !pip install featurewiz --ignore-installed --no-deps
+         !pip install xlrd --ignore-installed --no-deps 
+        ```
+        
+        ##Step 2: Next, install Pillow since Kaggle has an incompatible version. <br>
+        
+        ```
+         !pip install Pillow==9.0.0
+        ```
+        
         ## Usage
         
-        As of Jan 2022, you now invoke featurewiz in two ways for two different goals. For feature selection, you must use the scikit-learn compatible fit and predict transformer syntax such as below.
+        For feature selection, you must use the newer syntax which is similar to the scikit-learn fit and predict transformer syntax below.
         
         ```
         from featurewiz import FeatureWiz
-        features = FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='', dask_xgboost_flag=False, nrows=None, verbose=2)
-        X_train_selected = features.fit_transform(X_train, y_train)
-        X_test_selected = features.transform(X_test)
-        features.features  ### provides the list of selected features ###
+        fwiz = FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='', dask_xgboost_flag=False, nrows=None, verbose=2)
+        X_train_selected = fwiz.fit_transform(X_train, y_train)
+        X_test_selected = fwiz.transform(X_test)
+        ### get list of selected features ###
+        fwiz.features  
         ```
         
         Alternatively, you can use featurewiz for feature engineering using this older syntax. Otherwise, it will give an error. If you want to combine feature engg and then feature selection, you must use this older syntax:
         
         ```
-        import featurewiz as FW
-        outputs = FW.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
+        import featurewiz as fwiz
+        outputs = fwiz.featurewiz(dataname=train, target=target, corr_limit=0.70, verbose=2, sep=',', 
         		header=0, test_data='',feature_engg='', category_encoders='',
         		dask_xgboost_flag=False, nrows=None)
         ```
         
         `outputs`: There will always be multiple objects in output. The objects in that tuple can vary:
-        1. "features" and "train": It be a list (of selected features) and one dataframe (if you sent in train only)
+        1. "features" and "trainm": It be a list (of selected features) and one dataframe (if you sent in train only)
         2. "trainm" and "testm": It can be two dataframes when you send in both test and train but with selected features.
         <ol>
         <li>Both the selected features and dataframes are ready for you to now to do further modeling.
         <li>Featurewiz works on any multi-class, multi-label data Set. So you can have as many target labels as you want.
         <li>You don't have to tell Featurewiz whether it is a Regression or Classification problem. It will decide that automatically.
         </ol>
         
@@ -224,23 +199,46 @@
             - `WOEEncoder`: WOEEncoder uses the Weight of Evidence technique for categorical features. It supports only one kind of target: binary. For polynomial target support, it uses a PolynomialWrapper. It cannot be used for Regression.
             - `JamesSteinEncoder`: JamesSteinEncoder uses the James-Stein estimator. It supports 2 kinds of targets: binary and continuous. For polynomial target support, it uses PolynomialWrapper.
             For feature value i, James-Stein estimator returns a weighted average of:
             The mean target value for the observed feature value i.
             The mean target value (regardless of the feature value).
             - `dask_xgboost_flag`: Default is False. Set to True to use dask_xgboost estimator. You can turn it off if it gives an error. Then it will use pandas and regular xgboost to do the job.
             - `nrows`: default `None`. You can set the number of rows to read from your datafile if it is too large to fit into either dask or pandas. But you won't have to if you use dask. 
-        **Return values**
+        
+        **Output values**
         -   `outputs`: Output is always a tuple. We can call our outputs in that tuple: out1 and out2.
             -   `out1` and `out2`: If you sent in just one dataframe or filename as input, you will get:
                 - 1. `features`: It will be a list (of selected features) and
                 - 2. `trainm`: It will be a dataframe (if you sent in a file or dataname as input)
             -   `out1` and `out2`: If you sent in two files or dataframes (train and test), you will get:
                 - 1. `trainm`: a modified train dataframe with engineered and selected features from dataname and
                 - 2. `testm`: a modified test dataframe with engineered and selected features from test_data.
         
+        ## Additional
+        
+        ![background](featurewiz_background.jpg)
+        
+        To learn more about how featurewiz works under the hood, watch this [video](https://www.youtube.com/embed/ZiNutwPcAU0)<br>
+        <p>featurewiz was designed for selecting High Performance variables with the fewest steps.
+        In most cases, featurewiz builds models with 20%-99% fewer features than your original data set with nearly the same or slightly lower performance (this is based on my trials. Your experience may vary).<br>
+        <p>
+        featurewiz is every Data Scientist's feature wizard that will:<ol>
+        <li><b>Automatically pre-process data</b>: you can send in your entire dataframe "as is" and featurewiz will classify and change/label encode categorical variables changes to help XGBoost processing. It classifies variables as numeric or categorical or NLP or date-time variables automatically so it can use them correctly to model.<br>
+        <li><b>Perform feature engineering automatically</b>: The ability to create "interaction" variables or adding "group-by" features or "target-encoding" categorical variables is difficult and sifting through those hundreds of new features is painstaking and left only to "experts". Now, with featurewiz you can create hundreds or even thousands of new features with the click of a mouse. This is very helpful when you have a small number of features to start with. However, be careful with this option. You can very easily create a monster with this option.
+        <li><b>Perform feature reduction automatically</b>. When you have small data sets and you know your domain well, it is easy to perhaps do EDA and identify which variables are important. But when you have a very large data set with hundreds if not thousands of variables, selecting the best features from your model can mean the difference between a bloated and highly complex model or a simple model with the fewest and most information-rich features. featurewiz uses XGBoost repeatedly to perform feature selection. You must try it on your large data sets and compare!<br>
+        <li><b>Explain SULOV method graphically </b> using networkx library so you can see which variables are highly correlated to which ones and which of those have high or low mutual information scores automatically. Just set verbose = 2 to see the graph. <br>
+        <li><b>Build a fast XGBoost or LightGBM model using the features selected by featurewiz</b>. There is a function called "simple_lightgbm_model" which you can use to build a fast model. It is a new module, so check it out.<br>
+        </ol>
+        
+        <b>*** A Note of Gratitude ***</b>:<br>
+        <ol>
+        <li><b>Alex Lekov</b> (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/automl_alex) for his DataBunch and encoders modules which are used by the tool (although with some modifications).</li>
+        <li><b>Category Encoders</b> library in Python : This is an amazing library. Make sure you read all about the encoders that featurewiz uses here: https://contrib.scikit-learn.org/category_encoders/index.html </li>
+        </ol>
+        
         ## Maintainers
         
         * [@AutoViML](https://github.com/AutoViML)
         
         ## Contributing
         
         See [the contributing file](CONTRIBUTING.md)!
```

#### html2text {}

```diff
@@ -1,26 +1,44 @@
-Metadata-Version: 2.1 Name: featurewiz Version: 0.2.7 Summary: Select Best
+Metadata-Version: 2.1 Name: featurewiz Version: 0.2.8 Summary: Select Best
 Features from your data set - any size - now with XGBoost! Home-page: https://
 github.com/AutoViML/featurewiz Author: Ram Seshadri Author-email:
-rsesha2001@yahoo.com License: Apache License 2.0 Description: # featurewiz !
-[banner](featurewiz_logos.png) ## Good News: You can install featurewiz on
-Colab and Kaggle easily in 2 steps! Check_out_more_latest_updates_from_this
-page
-As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo),
-featurewiz is now available on conda-forge. You can try:
-``` conda install -c conda-forge featurewiz ``` ### If the above conda install
-fails, you can try installing featurewiz this way: ##Step 1: Install featurewiz
-first
-``` !pip install featurewiz --ignore-installed --no-deps !pip install xlrd --
-ignore-installed --no-deps ``` ##Step 2: Next, install Pillow since Kaggle has
-an incompatible version.
-``` !pip install Pillow==9.0.0 ``` ## What is featurewiz? `featurewiz` a new
-python library for creating and selecting the best features in your data set
-fast! `featurewiz` can be used in one or two ways. Both are explained below. ##
-1. Feature Engineering
+rsesha2001@yahoo.com License: Apache License 2.0 Description: # featurewiz
+`featurewiz` is a powerful feature selection library that has a number of
+features that make it stand out from the competition, including:
+   1. It provides one of the best automatic feature selection algorithms
+      (Minimum Redundancy Maximum Relevance (MRMR)) described by wikipedia as:
+      "The_MRMR_selection_has_been_found_to_be_more_powerful_than_the_maximum
+      relevance_feature_selection" such as Boruta.
+   2. It selects the best number of un-correlated features that have maximum
+      mutual information about the target without having to specify the number
+      of features
+   3. It is fast and easy to use, and comes with a number of helpful features,
+      such as a built-in categorical-to-numeric encoder and a powerful feature
+      engineering module
+   4. It is well-documented, and it comes with a number of examples.
+   5. It is actively maintained, and it is regularly updated with new features
+      and bug fixes.
+If you are looking for a single feature selection library, we would definitely
+recommend checking out featurewiz. It is a powerful tool that can help you to
+improve the performance of your machine learning models. # Table of Contents
+    * What_is_featurewiz
+    * How_it_works
+    * Tips_for_using_featurewiz
+    * How_to_install_featurewiz
+    * Usage
+    * API
+    * Additional_Tips
+    * Maintainers
+    * Contributing
+    * License
+    * Disclaimer
+![banner](featurewiz_logos.png) ## Introduction `featurewiz` a new python
+library for creating and selecting the best features in your data set fast!
+`featurewiz` can be used in one or two ways. Both are explained below. ### 1.
+Feature Engineering
 The first step is not absolutely necessary but it can be used to create new
 features that may or may not be helpful (be careful with automated feature
 engineering tools!).
 1. Performing Feature Engineering: One of the gaps in open source AutoML tools
 and especially Auto_ViML has been the lack of feature engineering capabilities
 that high powered competitions such as Kaggle required. The ability to create
 "interaction" variables or adding "group-by" features or "target-encoding"
@@ -30,19 +48,15 @@
 featurewiz now enables you to add hundreds of such features with a single line
 of code. Set the "feature_engg" flag to "interactions", "groupby" or "target"
 and featurewiz will select the best encoders for each of those options and
 create hundreds (perhaps thousands) of features in one go. Not only that, using
 the next step, featurewiz will sift through numerous such variables and find
 only the least correlated and most relevant features to your model. All in one
 step!.
-You must use this syntax for feature engg. Otherwise, featurewiz will give an
-error: ``` import featurewiz as FW outputs = FW.featurewiz(dataname=train,
-target=target, corr_limit=0.70, verbose=2, sep=',', header=0,
-test_data='',feature_engg='', category_encoders='', dask_xgboost_flag=False,
-nrows=None) ``` ![feature_engg](feature_engg.jpg) ## 2. Feature Selection
+![feature_engg](feature_engg.jpg) ### 2. Feature Selection
 The second step is Feature Selection. `featurewiz` uses the MRMR (Minimum
 Redundancy Maximum Relevance) algorithm as the basis for its feature selection.
 
 Why do Feature Selection? Once you have created 100's of new features, you
 still have three questions left to answer: 1. How do we interpret those newly
 created features? 2. Which of these features is important and which are
 useless? How many of them are highly correlated to each other causing
@@ -54,133 +68,100 @@
 SULOV: SULOV stands for `Searching for Uncorrelated List of Variables`. The
 SULOV algorithm is based on the Minimum-Redundancy-Maximum-Relevance (MRMR)
 algorithm_explained_in_this_article as one of the best feature selection
 methods. To understand how MRMR works and how it is different from `Boruta` and
 other feature selection methods, see the chart below. Here "Minimal Optimal"
 refers to the MRMR and featurewiz kind of algorithms while "all-relevant"
 refers to Boruta kind of algorithms.
-![MRMR_chart](MRMR.png)
-The working of the SULOV algorithm is as follows:
+![MRMR_chart](MRMR.png) ## Working `featurewiz` performs feature selection in 2
+steps. Each step is explained below. The working of the `SULOV` algorithm is as
+follows:
    1. Find all the pairs of highly correlated variables exceeding a correlation
       threshold (say absolute(0.7)).
    2. Then find their MIS score (Mutual Information Score) to the target
       variable. MIS is a non-parametric scoring method. So its suitable for all
       kinds of variables and target.
    3. Now take each pair of correlated variables, then knock off the one with
       the lower MIS score.
    4. Whatâs left is the ones with the highest Information scores and least
       correlation with each other.
-![sulov](SULOV.jpg) Recursive XGBoost: Once SULOV has selected variables that
-have high mutual information scores with least less correlation amongst them,
-we use XGBoost to repeatedly find best features among the remaining variables
-after SULOV. The Recursive XGBoost method is explained in this chart below.
-Here is how it works:
+![sulov](SULOV.jpg) The working of the Recursive XGBoost is as follows: Once
+SULOV has selected variables that have high mutual information scores with
+least less correlation amongst them, featurewiz uses XGBoost to repeatedly find
+the best features among the remaining variables after SULOV.
    1. Select all variables in data set and the full data split into train and
       valid sets.
    2. Find top X features (could be 10) on train using valid for early stopping
       (to prevent over-fitting)
    3. Then take next set of vars and find top X
    4. Do this 5 times. Combine all selected features and de-duplicate them.
-![xgboost](xgboost.jpg) Building the simplest and most "interpretable" model:
-featurewiz represents the "next best" step you must perform after doing feature
-engineering since you might have added some highly correlated or even useless
-features when you use automated feature engineering. featurewiz ensures you
-have the least number of features needed to build a high performing or
-equivalent model. A WORD OF CAUTION: Just because you can engineer new
-features, doesn't mean you should always create tons of new features. You must
-make sure you understand what the new features stand for before you attempt to
-build a model with these (sometimes useless) features. featurewiz displays the
-SULOV chart which can show you how the 100's of newly created variables added
-to your dataset are highly correlated to each other and were removed. This will
-help you understand how feature selection works in featurewiz. ## Table of
-Contents
-    * Background
-    * Install
-    * Usage
-    * API
-    * Maintainers
-    * Contributing
-    * License
-## Background ![background](featurewiz_background.jpg) To learn more about how
-featurewiz works under the hood, watch this [video](https://www.youtube.com/
-embed/ZiNutwPcAU0)
-featurewiz was designed for selecting High Performance variables with the
-fewest steps. In most cases, featurewiz builds models with 20%-99% fewer
-features than your original data set with nearly the same or slightly lower
-performance (this is based on my trials. Your experience may vary).
-featurewiz is every Data Scientist's feature wizard that will:
-   1. Automatically pre-process data: you can send in your entire dataframe "as
-      is" and featurewiz will classify and change/label encode categorical
-      variables changes to help XGBoost processing. It classifies variables as
-      numeric or categorical or NLP or date-time variables automatically so it
-      can use them correctly to model.
-   2. Perform feature engineering automatically: The ability to create
-      "interaction" variables or adding "group-by" features or "target-
-      encoding" categorical variables is difficult and sifting through those
-      hundreds of new features is painstaking and left only to "experts". Now,
-      with featurewiz you can create hundreds or even thousands of new features
-      with the click of a mouse. This is very helpful when you have a small
-      number of features to start with. However, be careful with this option.
-      You can very easily create a monster with this option.
-   3. Perform feature reduction automatically. When you have small data sets
-      and you know your domain well, it is easy to perhaps do EDA and identify
-      which variables are important. But when you have a very large data set
-      with hundreds if not thousands of variables, selecting the best features
-      from your model can mean the difference between a bloated and highly
-      complex model or a simple model with the fewest and most information-rich
-      features. featurewiz uses XGBoost repeatedly to perform feature
-      selection. You must try it on your large data sets and compare!
-   4. Explain SULOV method graphically using networkx library so you can see
-      which variables are highly correlated to which ones and which of those
-      have high or low mutual information scores automatically. Just set
-      verbose = 2 to see the graph.
-   5. Build a fast LightGBM model using the features selected by featurewiz.
-      There is a function called "simple_lightgbm_model" which you can use to
-      build a fast model. It is a new module, so check it out.
-*** Notes of Gratitude ***:
-   1. Alex Lekov (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/
-      automl_alex) for his DataBunch and encoders modules which are used by the
-      tool (although with some modifications).
-   2. Category Encoders library in Python : This is an amazing library. Make
-      sure you read all about the encoders that featurewiz uses here: https://
-      contrib.scikit-learn.org/category_encoders/index.html
+![xgboost](xgboost.jpg) ## Tips Here are some additional tips for ML engineers
+and data scientists when using featurewiz:
+   1. Always cross-validate your results: When you use a feature selection
+      tool, it is important to cross-validate your results. This means that you
+      should split your data into a training set and a test set. Use the
+      training set to select features, and then evaluate your model on the test
+      set. This will help you to ensure that your model is not overfitting to
+      the training data.
+   2. Use multiple feature selection tools: It is a good idea to use multiple
+      feature selection tools and compare the results. This will help you to
+      get a better understanding of which features are most important for your
+      data.
+   3. Don't forget to engineer new features: Feature selection is only one part
+      of the process of building a good machine learning model. You should also
+      spend time engineering your features to make them as informative as
+      possible. This can involve things like creating new features,
+      transforming existing features, and removing irrelevant features.
+   4. Don't overfit your model: It is important to avoid overfitting your model
+      to the training data. Overfitting occurs when your model learns the noise
+      in the training data, rather than the underlying signal. To avoid
+      overfitting, you can use regularization techniques, such as lasso or
+      elasticnet.
+   5. Start with a small number of features: When you are first starting out,
+      it is a good idea to start with a small number of features. This will
+      help you to avoid overfitting your model. As you become more experienced,
+      you can experiment with adding more features.
 ## Install **Prerequsites:**
    1. featurewiz is built using xgboost, dask, numpy, pandas and matplotlib. It
       should run on most Python 3 Anaconda installations. You won't have to
       import any special libraries other than "dask", "XGBoost" and "networkx"
       library. Optionally, it uses LightGBM for fast modeling, which it
       installs automatically.
    2. We use "networkx" library for charts and interpretability.
       But if you don't have these libraries, featurewiz will install those for
       you automatically.
-- [Anaconda](https://docs.anaconda.com/anaconda/install/) To clone featurewiz,
-it is better to create a new environment, and install the required
-dependencies: To install from PyPi: ``` conda create -n  python=3.7 anaconda
-conda activate  # ON WINDOWS: `source activate ` pip install featurewiz --
-ignore-installed --no-deps pip install lazytransform or pip install git+https:/
-/github.com/AutoViML/featurewiz.git ``` To install from source: ``` cd  git
-clone git@github.com:AutoViML/featurewiz.git # or download and unzip https://
-github.com/AutoViML/featurewiz/archive/master.zip conda create -n  python=3.7
-anaconda conda activate  # ON WINDOWS: `source activate ` cd featurewiz pip
-install -r requirements.txt ``` ## Usage As of Jan 2022, you now invoke
-featurewiz in two ways for two different goals. For feature selection, you must
-use the scikit-learn compatible fit and predict transformer syntax such as
-below. ``` from featurewiz import FeatureWiz features = FeatureWiz
-(corr_limit=0.70, feature_engg='', category_encoders='',
+To install from source: ``` cd  git clone git@github.com:AutoViML/
+featurewiz.git # or download and unzip https://github.com/AutoViML/featurewiz/
+archive/master.zip conda create -n  python=3.7 anaconda conda activate  # ON
+WINDOWS: `source activate ` cd featurewiz pip install -r requirements.txt ```
+## Good News: You can install featurewiz on Colab and Kaggle easily in 2 steps!
+Check_out_more_latest_updates_from_this_page
+As of June 2022, thanks to [arturdaraujo](https://github.com/arturdaraujo),
+featurewiz is now available on conda-forge. You can try:
+``` conda install -c conda-forge featurewiz ``` ### If the above conda install
+fails, you can try installing featurewiz this way: ##Step 1: Install featurewiz
+first
+``` !pip install featurewiz --ignore-installed --no-deps !pip install xlrd --
+ignore-installed --no-deps ``` ##Step 2: Next, install Pillow since Kaggle has
+an incompatible version.
+``` !pip install Pillow==9.0.0 ``` ## Usage For feature selection, you must use
+the newer syntax which is similar to the scikit-learn fit and predict
+transformer syntax below. ``` from featurewiz import FeatureWiz fwiz =
+FeatureWiz(corr_limit=0.70, feature_engg='', category_encoders='',
 dask_xgboost_flag=False, nrows=None, verbose=2) X_train_selected =
-features.fit_transform(X_train, y_train) X_test_selected = features.transform
-(X_test) features.features ### provides the list of selected features ### ```
-Alternatively, you can use featurewiz for feature engineering using this older
-syntax. Otherwise, it will give an error. If you want to combine feature engg
-and then feature selection, you must use this older syntax: ``` import
-featurewiz as FW outputs = FW.featurewiz(dataname=train, target=target,
-corr_limit=0.70, verbose=2, sep=',', header=0, test_data='',feature_engg='',
+fwiz.fit_transform(X_train, y_train) X_test_selected = fwiz.transform(X_test)
+### get list of selected features ### fwiz.features ``` Alternatively, you can
+use featurewiz for feature engineering using this older syntax. Otherwise, it
+will give an error. If you want to combine feature engg and then feature
+selection, you must use this older syntax: ``` import featurewiz as fwiz
+outputs = fwiz.featurewiz(dataname=train, target=target, corr_limit=0.70,
+verbose=2, sep=',', header=0, test_data='',feature_engg='',
 category_encoders='', dask_xgboost_flag=False, nrows=None) ``` `outputs`: There
 will always be multiple objects in output. The objects in that tuple can vary:
-1. "features" and "train": It be a list (of selected features) and one
+1. "features" and "trainm": It be a list (of selected features) and one
 dataframe (if you sent in train only) 2. "trainm" and "testm": It can be two
 dataframes when you send in both test and train but with selected features.
    1. Both the selected features and dataframes are ready for you to now to do
       further modeling.
    2. Featurewiz works on any multi-class, multi-label data Set. So you can
       have as many target labels as you want.
    3. You don't have to tell Featurewiz whether it is a Regression or
@@ -252,23 +233,66 @@
 support, it uses PolynomialWrapper. For feature value i, James-Stein estimator
 returns a weighted average of: The mean target value for the observed feature
 value i. The mean target value (regardless of the feature value). -
 `dask_xgboost_flag`: Default is False. Set to True to use dask_xgboost
 estimator. You can turn it off if it gives an error. Then it will use pandas
 and regular xgboost to do the job. - `nrows`: default `None`. You can set the
 number of rows to read from your datafile if it is too large to fit into either
-dask or pandas. But you won't have to if you use dask. **Return values** -
+dask or pandas. But you won't have to if you use dask. **Output values** -
 `outputs`: Output is always a tuple. We can call our outputs in that tuple:
 out1 and out2. - `out1` and `out2`: If you sent in just one dataframe or
 filename as input, you will get: - 1. `features`: It will be a list (of
 selected features) and - 2. `trainm`: It will be a dataframe (if you sent in a
 file or dataname as input) - `out1` and `out2`: If you sent in two files or
 dataframes (train and test), you will get: - 1. `trainm`: a modified train
 dataframe with engineered and selected features from dataname and - 2. `testm`:
 a modified test dataframe with engineered and selected features from test_data.
+## Additional ![background](featurewiz_background.jpg) To learn more about how
+featurewiz works under the hood, watch this [video](https://www.youtube.com/
+embed/ZiNutwPcAU0)
+featurewiz was designed for selecting High Performance variables with the
+fewest steps. In most cases, featurewiz builds models with 20%-99% fewer
+features than your original data set with nearly the same or slightly lower
+performance (this is based on my trials. Your experience may vary).
+featurewiz is every Data Scientist's feature wizard that will:
+   1. Automatically pre-process data: you can send in your entire dataframe "as
+      is" and featurewiz will classify and change/label encode categorical
+      variables changes to help XGBoost processing. It classifies variables as
+      numeric or categorical or NLP or date-time variables automatically so it
+      can use them correctly to model.
+   2. Perform feature engineering automatically: The ability to create
+      "interaction" variables or adding "group-by" features or "target-
+      encoding" categorical variables is difficult and sifting through those
+      hundreds of new features is painstaking and left only to "experts". Now,
+      with featurewiz you can create hundreds or even thousands of new features
+      with the click of a mouse. This is very helpful when you have a small
+      number of features to start with. However, be careful with this option.
+      You can very easily create a monster with this option.
+   3. Perform feature reduction automatically. When you have small data sets
+      and you know your domain well, it is easy to perhaps do EDA and identify
+      which variables are important. But when you have a very large data set
+      with hundreds if not thousands of variables, selecting the best features
+      from your model can mean the difference between a bloated and highly
+      complex model or a simple model with the fewest and most information-rich
+      features. featurewiz uses XGBoost repeatedly to perform feature
+      selection. You must try it on your large data sets and compare!
+   4. Explain SULOV method graphically using networkx library so you can see
+      which variables are highly correlated to which ones and which of those
+      have high or low mutual information scores automatically. Just set
+      verbose = 2 to see the graph.
+   5. Build a fast XGBoost or LightGBM model using the features selected by
+      featurewiz. There is a function called "simple_lightgbm_model" which you
+      can use to build a fast model. It is a new module, so check it out.
+*** A Note of Gratitude ***:
+   1. Alex Lekov (https://github.com/Alex-Lekov/AutoML_Alex/tree/master/
+      automl_alex) for his DataBunch and encoders modules which are used by the
+      tool (although with some modifications).
+   2. Category Encoders library in Python : This is an amazing library. Make
+      sure you read all about the encoders that featurewiz uses here: https://
+      contrib.scikit-learn.org/category_encoders/index.html
 ## Maintainers * [@AutoViML](https://github.com/AutoViML) ## Contributing See
 [the contributing file](CONTRIBUTING.md)! PRs accepted. ## License Apache
 License 2.0 Â© 2020 Ram Seshadri ## DISCLAIMER This project is not an official
 Google project. It is not supported by Google and Google specifically disclaims
 all warranties as to its quality, merchantability, or fitness for a particular
 purpose. Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
```

### Comparing `featurewiz-0.2.7/setup.py` & `featurewiz-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="featurewiz",
-    version="0.2.7",
+    version="0.2.8",
     author="Ram Seshadri",
     author_email="rsesha2001@yahoo.com",
     description="Select Best Features from your data set - any size - now with XGBoost!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/featurewiz",
```

