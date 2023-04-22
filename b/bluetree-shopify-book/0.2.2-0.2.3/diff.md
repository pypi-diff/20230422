# Comparing `tmp/bluetree_shopify_book-0.2.2.tar.gz` & `tmp/bluetree_shopify_book-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetree_shopify_book-0.2.2.tar", last modified: Tue Mar 28 08:24:05 2023, max compression
+gzip compressed data, was "bluetree_shopify_book-0.2.3.tar", last modified: Sat Apr 22 13:06:44 2023, max compression
```

## Comparing `bluetree_shopify_book-0.2.2.tar` & `bluetree_shopify_book-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-03-28 08:24:05.909765 bluetree_shopify_book-0.2.2/
--rw-r--r--   0 sikegame   (501) staff       (20)     1080 2023-03-07 06:09:50.000000 bluetree_shopify_book-0.2.2/LICENSE.txt
--rw-r--r--   0 sikegame   (501) staff       (20)     4889 2023-03-28 08:24:05.910008 bluetree_shopify_book-0.2.2/PKG-INFO
--rw-r--r--   0 sikegame   (501) staff       (20)     3170 2023-03-06 09:05:16.000000 bluetree_shopify_book-0.2.2/README.md
--rw-r--r--   0 sikegame   (501) staff       (20)       90 2023-03-07 06:05:35.000000 bluetree_shopify_book-0.2.2/pyproject.toml
--rw-r--r--   0 sikegame   (501) staff       (20)     1174 2023-03-28 08:24:05.911405 bluetree_shopify_book-0.2.2/setup.cfg
-drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-03-28 08:24:05.891122 bluetree_shopify_book-0.2.2/src/
-drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-03-28 08:24:05.903931 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/
--rw-r--r--   0 sikegame   (501) staff       (20)       41 2023-03-07 03:20:34.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/__init__.py
--rw-r--r--   0 sikegame   (501) staff       (20)     2966 2023-03-10 07:53:18.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/adapters.py
--rw-r--r--   0 sikegame   (501) staff       (20)    10272 2023-03-28 08:23:31.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/app.py
--rw-r--r--   0 sikegame   (501) staff       (20)     1575 2023-03-07 06:14:44.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/csv.py
--rw-r--r--   0 sikegame   (501) staff       (20)     1668 2023-03-26 08:04:34.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/document.graphql
--rw-r--r--   0 sikegame   (501) staff       (20)      454 2023-03-04 02:47:32.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/exceptions.py
--rw-r--r--   0 sikegame   (501) staff       (20)     6433 2023-03-27 07:16:58.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/schema.py
--rw-r--r--   0 sikegame   (501) staff       (20)     1482 2023-03-27 04:53:19.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/utils.py
--rw-r--r--   0 sikegame   (501) staff       (20)     2538 2023-03-03 06:05:51.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/validators.py
-drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-03-28 08:24:05.909219 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/
--rw-r--r--   0 sikegame   (501) staff       (20)     4889 2023-03-28 08:24:05.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/PKG-INFO
--rw-r--r--   0 sikegame   (501) staff       (20)      626 2023-03-28 08:24:05.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/SOURCES.txt
--rw-r--r--   0 sikegame   (501) staff       (20)        1 2023-03-28 08:24:05.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/dependency_links.txt
--rw-r--r--   0 sikegame   (501) staff       (20)      309 2023-03-28 08:24:05.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/requires.txt
--rw-r--r--   0 sikegame   (501) staff       (20)       22 2023-03-28 08:24:05.000000 bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/top_level.txt
+drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-04-22 13:06:44.075957 bluetree_shopify_book-0.2.3/
+-rw-r--r--   0 sikegame   (501) staff       (20)     1080 2023-03-07 06:09:50.000000 bluetree_shopify_book-0.2.3/LICENSE.txt
+-rw-r--r--   0 sikegame   (501) staff       (20)     4889 2023-04-22 13:06:44.076158 bluetree_shopify_book-0.2.3/PKG-INFO
+-rw-r--r--   0 sikegame   (501) staff       (20)     3170 2023-03-06 09:05:16.000000 bluetree_shopify_book-0.2.3/README.md
+-rw-r--r--   0 sikegame   (501) staff       (20)       90 2023-03-07 06:05:35.000000 bluetree_shopify_book-0.2.3/pyproject.toml
+-rw-r--r--   0 sikegame   (501) staff       (20)     1174 2023-04-22 13:06:44.077486 bluetree_shopify_book-0.2.3/setup.cfg
+drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-04-22 13:06:44.065808 bluetree_shopify_book-0.2.3/src/
+drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-04-22 13:06:44.072421 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/
+-rw-r--r--   0 sikegame   (501) staff       (20)       41 2023-03-07 03:20:34.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/__init__.py
+-rw-r--r--   0 sikegame   (501) staff       (20)     2966 2023-03-10 07:53:18.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/adapters.py
+-rw-r--r--   0 sikegame   (501) staff       (20)    11889 2023-04-22 07:57:48.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/app.py
+-rw-r--r--   0 sikegame   (501) staff       (20)     1575 2023-03-07 06:14:44.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/csv.py
+-rw-r--r--   0 sikegame   (501) staff       (20)     2033 2023-04-22 07:57:21.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/document.graphql
+-rw-r--r--   0 sikegame   (501) staff       (20)      454 2023-03-04 02:47:32.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/exceptions.py
+-rw-r--r--   0 sikegame   (501) staff       (20)     6433 2023-03-27 07:16:58.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/schema.py
+-rw-r--r--   0 sikegame   (501) staff       (20)     1482 2023-03-27 04:53:19.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/utils.py
+-rw-r--r--   0 sikegame   (501) staff       (20)     2538 2023-03-03 06:05:51.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/validators.py
+drwxr-xr-x   0 sikegame   (501) staff       (20)        0 2023-04-22 13:06:44.075469 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/
+-rw-r--r--   0 sikegame   (501) staff       (20)     4889 2023-04-22 13:06:44.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/PKG-INFO
+-rw-r--r--   0 sikegame   (501) staff       (20)      626 2023-04-22 13:06:44.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/SOURCES.txt
+-rw-r--r--   0 sikegame   (501) staff       (20)        1 2023-04-22 13:06:44.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/dependency_links.txt
+-rw-r--r--   0 sikegame   (501) staff       (20)      309 2023-04-22 13:06:44.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/requires.txt
+-rw-r--r--   0 sikegame   (501) staff       (20)       22 2023-04-22 13:06:44.000000 bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/top_level.txt
```

### Comparing `bluetree_shopify_book-0.2.2/LICENSE.txt` & `bluetree_shopify_book-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/PKG-INFO` & `bluetree_shopify_book-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetree_shopify_book
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for managing books in Shopify
 Home-page: https://github.com/sikegame/bluetree-shopify-book
 Author: Shinsuke JJ Ikegame
 Author-email: jj@digitalnomad.jp
 Project-URL: Bug Tracker, https://github.com/sikegame/bluetree-shopify-book/issues
 Project-URL: repository, https://github.com/sikegame/bluetree-shopify-book
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetree_shopify_book-0.2.2/README.md` & `bluetree_shopify_book-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/setup.cfg` & `bluetree_shopify_book-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bluetree_shopify_book
-version = 0.2.2
+version = 0.2.3
 author = Shinsuke JJ Ikegame
 author_email = jj@digitalnomad.jp
 description = A Python package for managing books in Shopify
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/sikegame/bluetree-shopify-book
 project_urls =
```

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/adapters.py` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/adapters.py`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/app.py` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,36 @@
             query=document,
             variables=dict(id=f"gid://shopify/Product/{product_id}"),
             operation_name="product",
         )
         data = json.loads(result)
         return to_shopify_book(data["data"]["product"])
 
+    def get_book_by_isbn(self, isbn: str) -> t.Optional[ShopifyBook]:
+        """
+        Gets a book by its ISBN.
+
+        Args:
+            isbn (str): The ISBN of the book.
+
+        Returns:
+            Optional[ShopifyBook]: A ShopifyBook object representing the book, or None if no book was found with the
+            specified ISBN.
+        """
+        result = shopify.GraphQL().execute(
+            query=document,
+            variables=dict(filter=f"sku:{isbn}"),
+            operation_name="productByISBN",
+        )
+        data = json.loads(result)
+        edges = data["data"]["productVariants"]["edges"]
+        if len(edges) == 0:
+            return None
+        return to_shopify_book(edges[0]["node"]["product"])
+    
     def check_has_book(self, isbn: str) -> bool:
         """
         Checks if a book with the given ISBN exists in the Shopify store.
 
         Args:
             isbn (str): The ISBN of the book to check.
 
@@ -171,14 +193,38 @@
         """
         shopify.GraphQL().execute(
             query=document,
             variables=dict(input={"id": f"gid://shopify/Product/{product_id}"}),
             operation_name="productDelete",
         )
 
+    def add_products_to_collection(self, collection_id: int, product_ids: list[int]):
+        """
+        Add one or more products to a Shopify collection.
+
+        Args:
+            collection_id (int): The ID of the collection to add products to.
+            product_ids (list[int]): A list of product IDs to add to the collection.
+
+        Returns:
+            dict: A dictionary representing the response data from the Shopify API.
+        """
+        result = shopify.GraphQL().execute(
+            query=document,
+            variables=dict(
+                id=f"gid://shopify/Collection/{collection_id}",
+                productIds=[
+                    f"gid://shopify/Product/{product_id}" for product_id in product_ids
+                ],
+            ),
+            operation_name="collectionAddProductsV2",
+        )
+        data = json.loads(result)
+        return data
+
     def get_publications(self) -> list[Publication]:
         """
         Gets a list of publications in the Shopify store.
 
         Returns:
             list[any]: A list of publication objects.
         """
```

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/csv.py` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/csv.py`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/document.graphql` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/document.graphql`

 * *Files 15% similar despite different names*

```diff
@@ -36,14 +36,26 @@
         id
         sku
       }
     }
   }
 }
 
+query productByISBN($filter: String!) {
+  productVariants(first: 1, query: $filter) {
+    edges {
+      node {
+        product {
+          ...Product
+        }
+      }
+    }
+  }
+}
+
 mutation productCreate($input: ProductInput!) {
   productCreate(input: $input) {
     product {
       ...Product
     }
   }
 }
@@ -103,7 +115,16 @@
   publishablePublish(id: $id, input: $input) {
     userErrors {
       field
       message
     }
   }
 }
+
+mutation collectionAddProductsV2($id: ID!, $productIds: [ID!]!) {
+  collectionAddProductsV2(id: $id, productIds: $productIds) {
+    userErrors {
+      field
+      message
+    }
+  }
+}
```

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/schema.py` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/schema.py`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/utils.py` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/utils.py`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book/validators.py` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book/validators.py`

 * *Files identical despite different names*

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/PKG-INFO` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetree-shopify-book
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for managing books in Shopify
 Home-page: https://github.com/sikegame/bluetree-shopify-book
 Author: Shinsuke JJ Ikegame
 Author-email: jj@digitalnomad.jp
 Project-URL: Bug Tracker, https://github.com/sikegame/bluetree-shopify-book/issues
 Project-URL: repository, https://github.com/sikegame/bluetree-shopify-book
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluetree_shopify_book-0.2.2/src/bluetree_shopify_book.egg-info/SOURCES.txt` & `bluetree_shopify_book-0.2.3/src/bluetree_shopify_book.egg-info/SOURCES.txt`

 * *Files identical despite different names*

