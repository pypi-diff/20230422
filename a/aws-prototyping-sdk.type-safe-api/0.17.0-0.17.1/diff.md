# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.17.0.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.17.0.tar", last modified: Fri Apr 21 06:11:41 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.17.1.tar", last modified: Sat Apr 22 04:18:33 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.17.0.tar` & `aws_prototyping_sdk.type_safe_api-0.17.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:11:41.893804 aws_prototyping_sdk.type_safe_api-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    54094 2023-04-21 06:11:41.893804 aws_prototyping_sdk.type_safe_api-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53153 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:11:41.893804 aws_prototyping_sdk.type_safe_api-0.17.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:11:41.889804 aws_prototyping_sdk.type_safe_api-0.17.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:11:41.889804 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:11:41.893804 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   285917 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:11:41.893804 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   851219 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.17.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:11:19.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:11:41.893804 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54094 2023-04-21 06:11:41.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-21 06:11:41.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:11:41.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 06:11:41.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 06:11:41.000000 aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:18:33.219305 aws_prototyping_sdk.type_safe_api-0.17.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-04-22 04:18:33.219305 aws_prototyping_sdk.type_safe_api-0.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55396 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 04:18:33.219305 aws_prototyping_sdk.type_safe_api-0.17.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:18:33.207305 aws_prototyping_sdk.type_safe_api-0.17.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:18:33.207305 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:18:33.211305 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   288160 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:18:33.219305 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   855350 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.17.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:18:17.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:18:33.207305 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-04-22 04:18:33.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-22 04:18:33.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:18:33.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-22 04:18:33.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 04:18:33.000000 aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.17.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.17.0
+Version: 0.17.1
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -75,27 +75,27 @@
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
   }
 });
 
-// Create a CDK infrastructure project
+// Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
 infra.addDeps(api.runtime.typescript!.package.packageName);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
-In your CDK application, consume the `Api` construct, vended from the generated typescript infrastructure package.
+In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
@@ -124,15 +124,19 @@
     });
   }
 }
 ```
 
 #### Implement a Lambda Handler
 
-The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like. In typescript, the implementation of `say-hello.ts` would look like:
+The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like.
+
+In the above CDK application, we used `NodejsFunction` with the entry point as `say-hello.ts`, so we can define the lambda function in the same `infra` project.
+
+In typescript, the implementation of `say-hello.ts` would look like:
 
 ```python
 import { sayHelloHandler } from "myapi-typescript-runtime"; // <- generated typescript runtime package
 
 // Use the handler wrapper for type-safety to ensure you correctly implement your modelled API operation
 export const handler = sayHelloHandler(async ({ input }) => {
   return {
@@ -1488,7 +1492,36 @@
 
 // Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
 monorepo.addImplicitDependency(api.model, shapes);
 
 // Add a local file dependency on the built shapes jar
 api.model.smithy!.addSmithyDeps(shapes.smithy!);
 ```
+
+#### Local API Development Server
+
+You can use the [AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html) to run a local development server for your API. You can achieve this using the following steps:
+
+1. Synthesize your CDK stack containing your `Api` construct (this might be your `AwsCdkTypeScriptApp` project for example), with the context property `type-safe-api-local` set to `true`, for example:
+
+```bash
+cd packages/infra
+npx cdk synth --context type-safe-api-local=true
+```
+
+1. Use the AWS SAM CLI to start the local development server, pointing it at the cloudformation template synthesized from the above command (note that the command will fail if docker is not running)
+
+```bash
+sam local start-api -t cdk.out/<your-stack>.template.json
+```
+
+You will need to repeat the above steps every time you make a code change for them to be reflected in your local development server.
+
+See the [AWS SAM CLI Reference](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/sam-cli-command-reference-sam-local-start-api.html) for more information on the commands to run.
+
+Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
+
+##### Limitations
+
+Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
+
+Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/README.md` & `aws_prototyping_sdk.type_safe_api-0.17.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,27 @@
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
   }
 });
 
-// Create a CDK infrastructure project
+// Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
 infra.addDeps(api.runtime.typescript!.package.packageName);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
-In your CDK application, consume the `Api` construct, vended from the generated typescript infrastructure package.
+In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
@@ -100,15 +100,19 @@
     });
   }
 }
 ```
 
 #### Implement a Lambda Handler
 
-The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like. In typescript, the implementation of `say-hello.ts` would look like:
+The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like.
+
+In the above CDK application, we used `NodejsFunction` with the entry point as `say-hello.ts`, so we can define the lambda function in the same `infra` project.
+
+In typescript, the implementation of `say-hello.ts` would look like:
 
 ```python
 import { sayHelloHandler } from "myapi-typescript-runtime"; // <- generated typescript runtime package
 
 // Use the handler wrapper for type-safety to ensure you correctly implement your modelled API operation
 export const handler = sayHelloHandler(async ({ input }) => {
   return {
@@ -1464,7 +1468,36 @@
 
 // Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
 monorepo.addImplicitDependency(api.model, shapes);
 
 // Add a local file dependency on the built shapes jar
 api.model.smithy!.addSmithyDeps(shapes.smithy!);
 ```
+
+#### Local API Development Server
+
+You can use the [AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html) to run a local development server for your API. You can achieve this using the following steps:
+
+1. Synthesize your CDK stack containing your `Api` construct (this might be your `AwsCdkTypeScriptApp` project for example), with the context property `type-safe-api-local` set to `true`, for example:
+
+```bash
+cd packages/infra
+npx cdk synth --context type-safe-api-local=true
+```
+
+1. Use the AWS SAM CLI to start the local development server, pointing it at the cloudformation template synthesized from the above command (note that the command will fail if docker is not running)
+
+```bash
+sam local start-api -t cdk.out/<your-stack>.template.json
+```
+
+You will need to repeat the above steps every time you make a code change for them to be reflected in your local development server.
+
+See the [AWS SAM CLI Reference](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/sam-cli-command-reference-sam-local-start-api.html) for more information on the commands to run.
+
+Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
+
+##### Limitations
+
+Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
+
+Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/setup.py` & `aws_prototyping_sdk.type_safe_api-0.17.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.17.0",
+    "version": "0.17.1",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.17.0.jsii.tgz"
+            "type-safe-api@0.17.1.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,27 +52,27 @@
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
   }
 });
 
-// Create a CDK infrastructure project
+// Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
 infra.addDeps(api.runtime.typescript!.package.packageName);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
-In your CDK application, consume the `Api` construct, vended from the generated typescript infrastructure package.
+In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
@@ -101,15 +101,19 @@
     });
   }
 }
 ```
 
 #### Implement a Lambda Handler
 
-The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like. In typescript, the implementation of `say-hello.ts` would look like:
+The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like.
+
+In the above CDK application, we used `NodejsFunction` with the entry point as `say-hello.ts`, so we can define the lambda function in the same `infra` project.
+
+In typescript, the implementation of `say-hello.ts` would look like:
 
 ```python
 import { sayHelloHandler } from "myapi-typescript-runtime"; // <- generated typescript runtime package
 
 // Use the handler wrapper for type-safety to ensure you correctly implement your modelled API operation
 export const handler = sayHelloHandler(async ({ input }) => {
   return {
@@ -1465,14 +1469,43 @@
 
 // Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
 monorepo.addImplicitDependency(api.model, shapes);
 
 // Add a local file dependency on the built shapes jar
 api.model.smithy!.addSmithyDeps(shapes.smithy!);
 ```
+
+#### Local API Development Server
+
+You can use the [AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html) to run a local development server for your API. You can achieve this using the following steps:
+
+1. Synthesize your CDK stack containing your `Api` construct (this might be your `AwsCdkTypeScriptApp` project for example), with the context property `type-safe-api-local` set to `true`, for example:
+
+```bash
+cd packages/infra
+npx cdk synth --context type-safe-api-local=true
+```
+
+1. Use the AWS SAM CLI to start the local development server, pointing it at the cloudformation template synthesized from the above command (note that the command will fail if docker is not running)
+
+```bash
+sam local start-api -t cdk.out/<your-stack>.template.json
+```
+
+You will need to repeat the above steps every time you make a code change for them to be reflected in your local development server.
+
+See the [AWS SAM CLI Reference](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/sam-cli-command-reference-sam-local-start-api.html) for more information on the commands to run.
+
+Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
+
+##### Limitations
+
+Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
+
+Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.17.0
+Version: 0.17.1
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -75,27 +75,27 @@
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
   }
 });
 
-// Create a CDK infrastructure project
+// Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
 infra.addDeps(api.runtime.typescript!.package.packageName);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
-In your CDK application, consume the `Api` construct, vended from the generated typescript infrastructure package.
+In your CDK application (ie within the `infra` project we created), consume the `Api` construct, vended from the generated typescript infrastructure package.
 
 ```python
 import { Stack, StackProps } from 'aws-cdk-lib';
 import { Construct } from 'constructs';
 import { Api } from "myapi-typescript-infra"; // <- generated typescript infrastructure package
 import { Authorizers, Integrations } from "@aws-prototyping-sdk/type-safe-api";
 import { NodejsFunction } from "aws-cdk-lib/aws-lambda-nodejs";
@@ -124,15 +124,19 @@
     });
   }
 }
 ```
 
 #### Implement a Lambda Handler
 
-The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like. In typescript, the implementation of `say-hello.ts` would look like:
+The generated runtime projects include lambda handler wrappers which provide type-safety for implementing your API operations. You can implement your lambda handlers in any of the supported languages, and even mix and match languages for different operations if you like.
+
+In the above CDK application, we used `NodejsFunction` with the entry point as `say-hello.ts`, so we can define the lambda function in the same `infra` project.
+
+In typescript, the implementation of `say-hello.ts` would look like:
 
 ```python
 import { sayHelloHandler } from "myapi-typescript-runtime"; // <- generated typescript runtime package
 
 // Use the handler wrapper for type-safety to ensure you correctly implement your modelled API operation
 export const handler = sayHelloHandler(async ({ input }) => {
   return {
@@ -1488,7 +1492,36 @@
 
 // Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
 monorepo.addImplicitDependency(api.model, shapes);
 
 // Add a local file dependency on the built shapes jar
 api.model.smithy!.addSmithyDeps(shapes.smithy!);
 ```
+
+#### Local API Development Server
+
+You can use the [AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html) to run a local development server for your API. You can achieve this using the following steps:
+
+1. Synthesize your CDK stack containing your `Api` construct (this might be your `AwsCdkTypeScriptApp` project for example), with the context property `type-safe-api-local` set to `true`, for example:
+
+```bash
+cd packages/infra
+npx cdk synth --context type-safe-api-local=true
+```
+
+1. Use the AWS SAM CLI to start the local development server, pointing it at the cloudformation template synthesized from the above command (note that the command will fail if docker is not running)
+
+```bash
+sam local start-api -t cdk.out/<your-stack>.template.json
+```
+
+You will need to repeat the above steps every time you make a code change for them to be reflected in your local development server.
+
+See the [AWS SAM CLI Reference](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/sam-cli-command-reference-sam-local-start-api.html) for more information on the commands to run.
+
+Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
+
+##### Limitations
+
+Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
+
+Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.0/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.17.1/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.17.0.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.17.1.jsii.tgz
```

