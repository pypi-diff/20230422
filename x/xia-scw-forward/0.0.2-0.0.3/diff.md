# Comparing `tmp/xia_scw_forward-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_forward-0.0.3-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 111593 bytes, number of entries: 12
--rw-r--r--  2.0 unx      103 b- defN 23-Apr-21 21:41 xia_scw_forward/__init__.py
--rw-r--r--  2.0 unx   259072 b- defN 23-Apr-21 21:48 xia_scw_forward/forward.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/backend.tf
--rw-rw-rw-  2.0 unx     2631 b- defN 23-Apr-21 21:41 xia_scw_forward/templates/ScwForward/main.tf
--rw-rw-rw-  2.0 unx      708 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 19:27 xia_scw_forward/templates/ScwForward/provider.tf
--rw-rw-rw-  2.0 unx     2451 b- defN 23-Apr-21 20:34 xia_scw_forward/templates/ScwForward/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 21:48 xia_scw_forward-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      727 b- defN 23-Apr-21 21:48 xia_scw_forward-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 21:48 xia_scw_forward-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-21 21:48 xia_scw_forward-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1127 b- defN 23-Apr-21 21:48 xia_scw_forward-0.0.2.dist-info/RECORD
-12 files, 267498 bytes uncompressed, 109647 bytes compressed:  59.0%
+Zip file size: 89406 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-21 22:02 xia_scw_forward/__init__.py
+-rw-r--r--  2.0 unx   235496 b- defN 23-Apr-21 22:03 xia_scw_forward/forward.cpython-310-darwin.so
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-21 19:28 xia_scw_forward/templates/ScwForward/backend.tf
+-rw-r--r--  2.0 unx     2632 b- defN 23-Apr-21 22:02 xia_scw_forward/templates/ScwForward/main.tf
+-rw-r--r--  2.0 unx      750 b- defN 23-Apr-21 22:02 xia_scw_forward/templates/ScwForward/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 19:28 xia_scw_forward/templates/ScwForward/provider.tf
+-rw-r--r--  2.0 unx     2622 b- defN 23-Apr-21 22:02 xia_scw_forward/templates/ScwForward/variables.tf
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-21 22:03 xia_scw_forward-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      690 b- defN 23-Apr-21 22:03 xia_scw_forward-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-21 22:03 xia_scw_forward-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-21 22:03 xia_scw_forward-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1131 b- defN 23-Apr-21 22:03 xia_scw_forward-0.0.3.dist-info/RECORD
+12 files, 244112 bytes uncompressed, 87454 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: xia_scw_forward/__init__.py
 Comment: 
 
-Filename: xia_scw_forward/forward.cp39-win_amd64.pyd
+Filename: xia_scw_forward/forward.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_forward/templates/ScwForward/backend.tf
 Comment: 
 
 Filename: xia_scw_forward/templates/ScwForward/main.tf
 Comment: 
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_forward/templates/ScwForward/provider.tf
 Comment: 
 
 Filename: xia_scw_forward/templates/ScwForward/variables.tf
 Comment: 
 
-Filename: xia_scw_forward-0.0.2.dist-info/LICENSE.txt
+Filename: xia_scw_forward-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_forward-0.0.2.dist-info/METADATA
+Filename: xia_scw_forward-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_forward-0.0.2.dist-info/WHEEL
+Filename: xia_scw_forward-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_forward-0.0.2.dist-info/top_level.txt
+Filename: xia_scw_forward-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_forward-0.0.2.dist-info/RECORD
+Filename: xia_scw_forward-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_forward/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_forward.forward import ScwForward
 
 
 __all__ = [
     "ScwForward"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## xia_scw_forward/templates/ScwForward/main.tf

```diff
@@ -33,15 +33,15 @@
 }
 
 resource scaleway_vpc_public_gateway_pat_rule service_pat {
     gateway_id = data.scaleway_vpc_public_gateway.main.id
     private_ip = var.lan_ip
     private_port = var.lan_port
     public_port = var.wan_port
-    protocol = "tcp"
+    protocol = var.protocol
     depends_on = [scaleway_vpc_public_gateway_dhcp_reservation.main]
 }
 
 locals {
   default_ssh = [
     "ufw allow ssh",
     "ufw --force enable"
@@ -78,15 +78,15 @@
 
     connection {
       type        = "ssh"
       user        = "root"
       private_key = file(var.ssh_private_key)
       host        = var.lan_ip
 
-      bastion_host        = "212.47.239.148"
+      bastion_host        = var.wan_ip
       bastion_port        = 59999
       bastion_user        = "bastion"
       bastion_private_key = file(var.ssh_private_key)
 
       timeout              = "5m"   # Maximum time to wait for the connection to become available
     }
   }
```

## xia_scw_forward/templates/ScwForward/output.tf

```diff
@@ -10,14 +10,18 @@
   value = var.instance_name
 }
 
 output "service_name" {
   value = var.service_name
 }
 
+output "wan_ip" {
+  value = var.wan_ip
+}
+
 output "lan_name" {
   value = data.scaleway_vpc_private_network.service.name
 }
 
 output "lan_ip" {
   value = scaleway_vpc_public_gateway_pat_rule.service_pat.private_ip
 }
```

## xia_scw_forward/templates/ScwForward/variables.tf

```diff
@@ -22,14 +22,21 @@
 variable "service_name" {
   type = string
   default = null  #xia#
   #xia# default = {% if service_name is defined and service_name is not none %}"{{ service_name }}"{% else %}null{% endif %}
 
 }
 
+variable "wan_ip" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if wan_ip is defined and wan_ip is not none %}"{{ wan_ip }}"{% else %}null{% endif %}
+
+}
+
 variable "lan_name" {
   type = string
   default = null  #xia#
   #xia# default = {% if lan_name is defined and lan_name is not none %}"{{ lan_name }}"{% else %}null{% endif %}
 
 }
```

## Comparing `xia_scw_forward-0.0.2.dist-info/RECORD` & `xia_scw_forward-0.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_scw_forward/__init__.py,sha256=C7vLuSciY7sCajiTNG-3pOPPJYBcnigfy6BElk68p7I,103
-xia_scw_forward/forward.cp39-win_amd64.pyd,sha256=r2pafLJ3ooKzsWWQKaf2d1mWEHlL5k8wYbjYhSV5VC4,259072
+xia_scw_forward/__init__.py,sha256=8SY3Z7-4EN46Yx_xjLGUWouay690Amb8QRG7LurdA6s,103
+xia_scw_forward/forward.cpython-310-darwin.so,sha256=6R7uTGgp2yaQd4fNK6C9VTzwgz3iaH-8-KoGfdPN34Y,235496
 xia_scw_forward/templates/ScwForward/backend.tf,sha256=E6fgAX-nMcTt9oErRKvK67uJPdB-O77YJpzAvf06zgs,69
-xia_scw_forward/templates/ScwForward/main.tf,sha256=R8SaL521GrPhdJGcCpODjfwrPfWT6YbL0DcHsJ8Bh20,2631
-xia_scw_forward/templates/ScwForward/output.tf,sha256=nREGFAc1hXpAdRGd04io4QsRo28FX-EwgjFNg1PI4aU,708
+xia_scw_forward/templates/ScwForward/main.tf,sha256=iNZkC4CvemRAfG1So8ofAVRER29KQtUJr_CsZ8YJsaU,2632
+xia_scw_forward/templates/ScwForward/output.tf,sha256=GcIL3yrYiuAYNeu0fLTDt8x-r1aAI6n683ImMFqbQbs,750
 xia_scw_forward/templates/ScwForward/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
-xia_scw_forward/templates/ScwForward/variables.tf,sha256=gXB-8PH9d91xwJNg6dRt_KEPPQizfoZOLxO6E1exba4,2451
-xia_scw_forward-0.0.2.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
-xia_scw_forward-0.0.2.dist-info/METADATA,sha256=Yzpm_eRgGKAk7w14ABSUdq1izF68Ar1fxhkCbU4e1rk,727
-xia_scw_forward-0.0.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_forward-0.0.2.dist-info/top_level.txt,sha256=zSdl1uiLifiOddj8F4TdDzODhdXe_Ny7s_A4Dfprpw0,16
-xia_scw_forward-0.0.2.dist-info/RECORD,,
+xia_scw_forward/templates/ScwForward/variables.tf,sha256=YlKoBHn9q-L9pO08wVvwRdnrxsnh1Vec-bAUsiwF65A,2622
+xia_scw_forward-0.0.3.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
+xia_scw_forward-0.0.3.dist-info/METADATA,sha256=SstHpvZr6kQHwg8xkXp_AAHe8a3nJwbDmY5a4oTonzM,690
+xia_scw_forward-0.0.3.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_scw_forward-0.0.3.dist-info/top_level.txt,sha256=zSdl1uiLifiOddj8F4TdDzODhdXe_Ny7s_A4Dfprpw0,16
+xia_scw_forward-0.0.3.dist-info/RECORD,,
```

