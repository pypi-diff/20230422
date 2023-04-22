# Comparing `tmp/iam_actions-1.2.20230421.tar.gz` & `tmp/iam_actions-1.2.20230422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230421.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230422.tar", max compression
```

## Comparing `iam_actions-1.2.20230421.tar` & `iam_actions-1.2.20230422.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/README.md
--rw-r--r--   0        0        0      228 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/__init__.py
--rw-r--r--   0        0        0  4223594 2023-04-21 02:28:10.166390 iam_actions-1.2.20230421/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-21 02:26:05.821502 iam_actions-1.2.20230421/iam_actions/generate/services.py
--rw-r--r--   0        0        0   543318 2023-04-21 02:28:10.166390 iam_actions-1.2.20230421/iam_actions/policies.json
--rw-r--r--   0        0        0   190691 2023-04-21 02:28:10.166390 iam_actions-1.2.20230421/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   526910 2023-04-21 02:28:10.166390 iam_actions-1.2.20230421/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-21 02:28:11.202397 iam_actions-1.2.20230421/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230421/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230421/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/README.md
+-rw-r--r--   0        0        0      228 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4220933 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-22 02:26:17.093102 iam_actions-1.2.20230422/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   543343 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/policies.json
+-rw-r--r--   0        0        0   190303 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   526934 2023-04-22 02:28:09.830322 iam_actions-1.2.20230422/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-22 02:28:10.598330 iam_actions-1.2.20230422/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230422/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230422/PKG-INFO
```

### Comparing `iam_actions-1.2.20230421/LICENSE` & `iam_actions-1.2.20230422/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/README.md` & `iam_actions-1.2.20230422/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/actions.json` & `iam_actions-1.2.20230422/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998614296112633%*

 * *Differences: {"'connect'": "{'CreateParticipant': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'CreateParticipant'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *              "AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'ram'": "{'AcceptResourceShareInvitation': {'access_level': 'Undocumented', 'condition_keys': "*

 * *          "[], 'description': 'Not Documented by AWS', 'resources': []}, 'AssociateResourceShare': "*

 * *          "{'access_level': 'Undocumented', 'condition […]*

```diff
@@ -29538,14 +29538,22 @@
             "description": "Grants permission to create an integration association with an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance",
                 "integration-association"
             ]
         },
+        "CreateParticipant": {
+            "access_level": "Undocumented",
+            "action": "CreateParticipant",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateQueue": {
             "access_level": "Write",
             "action": "CreateQueue",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "connect:InstanceId"
@@ -109021,52 +109029,36 @@
             "resources": [
                 "user"
             ]
         }
     },
     "ram": {
         "AcceptResourceShareInvitation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AcceptResourceShareInvitation",
-            "condition_keys": [
-                "ram:ShareOwnerAccountId"
-            ],
-            "description": "Grants permission to accept the specified resource share invitation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share-invitation"
-            ]
+            "resources": []
         },
         "AssociateResourceShare": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateResourceShare",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ram:AllowsExternalPrincipals",
-                "ram:Principal",
-                "ram:RequestedResourceType",
-                "ram:ResourceArn",
-                "ram:ResourceShareName"
-            ],
-            "description": "Grants permission to associate resource(s) and/or principal(s) to a resource share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "AssociateResourceSharePermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AssociateResourceSharePermission",
             "condition_keys": [],
-            "description": "Grants permission to associate a Permission with a Resource Share",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "permission",
-                "resource-share"
-            ]
+            "resources": []
         },
         "CreatePermission": {
             "access_level": "Undocumented",
             "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
@@ -109077,25 +109069,18 @@
             "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateResourceShare": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateResourceShare",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys",
-                "ram:Principal",
-                "ram:RequestedAllowsExternalPrincipals",
-                "ram:RequestedResourceType",
-                "ram:ResourceArn"
-            ],
-            "description": "Grants permission to create a resource share with provided resource(s) and/or principal(s)",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeletePermission": {
             "access_level": "Undocumented",
             "action": "DeletePermission",
             "condition_keys": [],
@@ -109108,219 +109093,180 @@
             "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteResourceShare": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteResourceShare",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ram:AllowsExternalPrincipals",
-                "ram:ResourceShareName"
-            ],
-            "description": "Grants permission to delete resource share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "DisassociateResourceShare": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateResourceShare",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ram:AllowsExternalPrincipals",
-                "ram:Principal",
-                "ram:RequestedResourceType",
-                "ram:ResourceArn",
-                "ram:ResourceShareName"
-            ],
-            "description": "Grants permission to disassociate resource(s) and/or principal(s) from a resource share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "DisassociateResourceSharePermission": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
-            "description": "Grants permission to disassociate a Permission from a Resource Share",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "permission",
-                "resource-share"
-            ]
+            "resources": []
         },
         "EnableSharingWithAwsOrganization": {
-            "access_level": "Permissions management",
+            "access_level": "Undocumented",
             "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
-            "description": "Grants permission to access customer's organization and create a SLR in the customer's account",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPermission": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetPermission",
-            "condition_keys": [
-                "ram:PermissionArn"
-            ],
-            "description": "Grants permission to get the contents of an AWS RAM permission",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "permission"
-            ]
+            "resources": []
         },
         "GetResourcePolicies": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetResourcePolicies",
             "condition_keys": [],
-            "description": "Grants permission to get the policies for the specified resources that you own and have shared",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourceShareAssociations": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetResourceShareAssociations",
             "condition_keys": [],
-            "description": "Grants permission to get a set of resource share associations from a provided list or with a specified status of the specified type",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourceShareInvitations": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetResourceShareInvitations",
             "condition_keys": [],
-            "description": "Grants permission to get resource share invitations by the specified invitation arn or those for the resource share",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetResourceShares": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "GetResourceShares",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to get a set of resource shares from a provided list or with a specified status",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPendingInvitationResources": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "ListPendingInvitationResources",
             "condition_keys": [],
-            "description": "Grants permission to list the resources in a resource share that is shared with you but that the invitation is still pending for",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share-invitation"
-            ]
+            "resources": []
         },
         "ListPermissionAssociations": {
             "access_level": "Undocumented",
             "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPermissionVersions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListPermissionVersions",
             "condition_keys": [],
-            "description": "Grants permission to list the versions of an AWS RAM permission",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPermissions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListPermissions",
             "condition_keys": [],
-            "description": "Grants permission to list the AWS RAM permissions",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPrincipals": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListPrincipals",
             "condition_keys": [],
-            "description": "Grants permission to list the principals that you have shared resources with or that have shared resources with you",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
             "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListResourceSharePermissions": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListResourceSharePermissions",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ram:AllowsExternalPrincipals",
-                "ram:ResourceShareName"
-            ],
-            "description": "Grants permission to list the Permissions associated with a Resource Share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "ListResourceTypes": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListResourceTypes",
             "condition_keys": [],
-            "description": "Grants permission to list the shareable resource types supported by AWS RAM",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListResources": {
-            "access_level": "List",
+            "access_level": "Undocumented",
             "action": "ListResources",
             "condition_keys": [],
-            "description": "Grants permission to list the resources that you added to resource shares or the resources that are shared with you",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
             "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PromoteResourceShareCreatedFromPolicy": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
-            "description": "Grants permission to promote the specified resource share",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "RejectResourceShareInvitation": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RejectResourceShareInvitation",
-            "condition_keys": [
-                "ram:ShareOwnerAccountId"
-            ],
-            "description": "Grants permission to reject the specified resource share invitation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share-invitation"
-            ]
+            "resources": []
         },
         "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
             "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
@@ -109331,53 +109277,36 @@
             "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "TagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to tag the specified resource share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "UntagResource": {
-            "access_level": "Tagging",
+            "access_level": "Undocumented",
             "action": "UntagResource",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to untag the specified resource share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         },
         "UpdateResourceShare": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "UpdateResourceShare",
-            "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ram:AllowsExternalPrincipals",
-                "ram:RequestedAllowsExternalPrincipals",
-                "ram:ResourceShareName"
-            ],
-            "description": "Grants permission to update attributes of the resource share",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "resource-share"
-            ]
+            "resources": []
         }
     },
     "rbin": {
         "CreateRule": {
             "access_level": "Write",
             "action": "CreateRule",
             "condition_keys": [
```

### Comparing `iam_actions-1.2.20230421/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230422/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230422/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/generate/generate.py` & `iam_actions-1.2.20230422/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230422/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230422/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/generate/services.py` & `iam_actions-1.2.20230422/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230421/iam_actions/policies.json` & `iam_actions-1.2.20230422/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999382834911%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect': {'Actions': {insert: [(20, 'CreateParticipant')]}}}"}*

```diff
@@ -11198,14 +11198,15 @@
                 "ClaimPhoneNumber",
                 "CreateAgentStatus",
                 "CreateContactFlow",
                 "CreateContactFlowModule",
                 "CreateHoursOfOperation",
                 "CreateInstance",
                 "CreateIntegrationAssociation",
+                "CreateParticipant",
                 "CreateQueue",
                 "CreateQuickConnect",
                 "CreateRoutingProfile",
                 "CreateRule",
                 "CreateSecurityProfile",
                 "CreateTaskTemplate",
                 "CreateTrafficDistributionGroup",
```

### Comparing `iam_actions-1.2.20230421/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230422/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985955056179775%*

 * *Differences: {"'ram'": '{replace: OrderedDict()}'}*

```diff
@@ -4819,28 +4819,15 @@
             "condition_keys": null
         },
         "user": {
             "arn_pattern": "arn:*:quicksight:*:*:user/*",
             "condition_keys": null
         }
     },
-    "ram": {
-        "permission": {
-            "arn_pattern": "arn:*:ram::*:permission/*",
-            "condition_keys": "ram:PermissionArn"
-        },
-        "resource-share": {
-            "arn_pattern": "arn:*:ram:*:*:resource-share/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "resource-share-invitation": {
-            "arn_pattern": "arn:*:ram:*:*:resource-share-invitation/*",
-            "condition_keys": "ram:ShareOwnerAccountId"
-        }
-    },
+    "ram": {},
     "rbin": {
         "rule": {
             "arn_pattern": "arn:*:rbin:*:*:rule/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "rds": {
```

### Comparing `iam_actions-1.2.20230421/iam_actions/services.json` & `iam_actions-1.2.20230422/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993533635442%*

 * *Differences: {"'connect'": "{'Actions': {insert: [(20, 'CreateParticipant')]}}"}*

```diff
@@ -4514,14 +4514,15 @@
             "ClaimPhoneNumber",
             "CreateAgentStatus",
             "CreateContactFlow",
             "CreateContactFlowModule",
             "CreateHoursOfOperation",
             "CreateInstance",
             "CreateIntegrationAssociation",
+            "CreateParticipant",
             "CreateQueue",
             "CreateQuickConnect",
             "CreateRoutingProfile",
             "CreateRule",
             "CreateSecurityProfile",
             "CreateTaskTemplate",
             "CreateTrafficDistributionGroup",
```

### Comparing `iam_actions-1.2.20230421/pyproject.toml` & `iam_actions-1.2.20230422/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230421"
+version = "1.2.20230422"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230421/setup.py` & `iam_actions-1.2.20230422/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230421',
+    'version': '1.2.20230422',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230421/PKG-INFO` & `iam_actions-1.2.20230422/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230421
+Version: 1.2.20230422
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

