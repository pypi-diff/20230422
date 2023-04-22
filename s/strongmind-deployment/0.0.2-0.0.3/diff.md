# Comparing `tmp/strongmind_deployment-0.0.2-py3-none-any.whl.zip` & `tmp/strongmind_deployment-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3865 bytes, number of entries: 7
+Zip file size: 3972 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     2541 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     2797 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
 -rw-r--r--  2.0 unx     1786 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
-?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.2.dist-info/RECORD
-7 files, 6736 bytes uncompressed, 2743 bytes compressed:  59.3%
+?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/RECORD
+7 files, 6992 bytes uncompressed, 2850 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
-Filename: strongmind_deployment-0.0.2.dist-info/METADATA
+Filename: strongmind_deployment-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-0.0.2.dist-info/WHEEL
+Filename: strongmind_deployment-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-0.0.2.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-0.0.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-0.0.2.dist-info/RECORD
+Filename: strongmind_deployment-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -3,41 +3,51 @@
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 from pulumi import Config, export, Output
 
 
+def get_aws_account_and_region():
+    current_identity = aws.get_caller_identity()
+    current_region = aws.get_region()
+    return current_identity.account_id, current_region
+
+
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
+        if kwargs.get("get_aws_account_and_region"):
+            get_aws_account_and_region_func = kwargs.get("get_aws_account_and_region")
+        else:
+            get_aws_account_and_region_func = get_aws_account_and_region
+
         self.app_path = kwargs.get('app_path') or './'
         self.container_port = kwargs.get('container_port') or 3000
         self.cpu = kwargs.get('cpu') or 256
         self.memory = kwargs.get("memory") or 512
 
         self.ecs_cluster = aws.ecs.Cluster("cluster",
                                            name=name,
                                            opts=pulumi.ResourceOptions(parent=self),
                                            )
         self.load_balancer = awsx.lb.ApplicationLoadBalancer("loadbalancer",
                                                              name=name,
                                                              opts=pulumi.ResourceOptions(parent=self),
                                                              )
-        self.repo = awsx.ecr.Repository("repo",
-                                        name=name,
-                                        force_delete=True,
-                                        opts=pulumi.ResourceOptions(parent=self),
-                                        )
+        account_id, region = get_aws_account_and_region_func()
 
+        repo_url = f"{account_id}.dkr.ecr.{region}.amazonaws.com/{name}"
         image_name = os.getenv('IMAGE_TAG', f'{name}:latest')
+        image = f"{repo_url}/{image_name}"
+
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
                 container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
-                    image=pulumi.Output.concat(self.repo.url, f"/{image_name}"),
+                    image=image,
                     cpu=self.cpu,
                     memory=self.memory,
                     essential=True,
                     port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
                         container_port=self.container_port,
                         host_port=self.container_port,
                         target_group=self.load_balancer.default_target_group,
```

## Comparing `strongmind_deployment-0.0.2.dist-info/METADATA` & `strongmind_deployment-0.0.3.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-0.0.2.dist-info/licenses/LICENSE` & `strongmind_deployment-0.0.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-0.0.2.dist-info/RECORD` & `strongmind_deployment-0.0.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-strongmind_deployment/container.py,sha256=UnP-k7H0dbj4rRUKWhJDYaFtnDCUhObvn-RwufCFkfM,2541
+strongmind_deployment/container.py,sha256=s34cuhUuoZ-Y1Bto-3Rt8kmMm1S6vnA3FXjXeOQVLsI,2797
 strongmind_deployment/rails.py,sha256=n1vt_e_VBidG1FBV3p7QqncMGxth3_cNzXUAeCdq6ho,1786
-strongmind_deployment-0.0.2.dist-info/METADATA,sha256=QlxZXELCqLQ_6tl7N8bcRGmD-J7sBIX5rOGBgl_xUH4,646
-strongmind_deployment-0.0.2.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-strongmind_deployment-0.0.2.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-0.0.2.dist-info/RECORD,,
+strongmind_deployment-0.0.3.dist-info/METADATA,sha256=UWExAQ6PzQPENVWjevp0dwO3aGZzUtiMqVgs9_2ZY2c,646
+strongmind_deployment-0.0.3.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+strongmind_deployment-0.0.3.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-0.0.3.dist-info/RECORD,,
```

