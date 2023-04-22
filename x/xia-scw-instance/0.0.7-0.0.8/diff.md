# Comparing `tmp/xia_scw_instance-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.0.8-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 103461 bytes, number of entries: 12
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-21 21:25 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   241152 b- defN 23-Apr-21 21:30 xia_scw_instance/instance.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/backend.tf
--rw-rw-rw-  2.0 unx      243 b- defN 23-Apr-21 21:25 xia_scw_instance/templates/ScwInstance/main.tf
--rw-rw-rw-  2.0 unx      396 b- defN 23-Apr-21 21:25 xia_scw_instance/templates/ScwInstance/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/provider.tf
--rw-rw-rw-  2.0 unx     1063 b- defN 23-Apr-21 16:02 xia_scw_instance/templates/ScwInstance/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 21:30 xia_scw_instance-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-21 21:30 xia_scw_instance-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 21:30 xia_scw_instance-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 21:30 xia_scw_instance-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1144 b- defN 23-Apr-21 21:30 xia_scw_instance-0.0.7.dist-info/RECORD
-12 files, 245484 bytes uncompressed, 101479 bytes compressed:  58.7%
+Zip file size: 93400 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      133 b- defN 23-Apr-22 12:38 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   252312 b- defN 23-Apr-22 12:39 xia_scw_instance/instance.cpython-310-darwin.so
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-21 13:45 xia_scw_instance/templates/ScwInstance/backend.tf
+-rw-r--r--  2.0 unx     3026 b- defN 23-Apr-22 12:38 xia_scw_instance/templates/ScwInstance/main.tf
+-rw-r--r--  2.0 unx      766 b- defN 23-Apr-22 12:38 xia_scw_instance/templates/ScwInstance/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 13:45 xia_scw_instance/templates/ScwInstance/provider.tf
+-rw-r--r--  2.0 unx     4173 b- defN 23-Apr-22 12:38 xia_scw_instance/templates/ScwInstance/variables.tf
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-22 12:39 xia_scw_instance-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      662 b- defN 23-Apr-22 12:39 xia_scw_instance-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-22 12:39 xia_scw_instance-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-22 12:39 xia_scw_instance-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1149 b- defN 23-Apr-22 12:39 xia_scw_instance-0.0.8.dist-info/RECORD
+12 files, 262910 bytes uncompressed, 91412 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: xia_scw_instance/__init__.py
 Comment: 
 
-Filename: xia_scw_instance/instance.cp39-win_amd64.pyd
+Filename: xia_scw_instance/instance.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/backend.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/main.tf
 Comment: 
@@ -15,23 +15,23 @@
 
 Filename: xia_scw_instance/templates/ScwInstance/provider.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/variables.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.7.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.7.dist-info/METADATA
+Filename: xia_scw_instance-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.0.7.dist-info/WHEEL
+Filename: xia_scw_instance-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.0.7.dist-info/top_level.txt
+Filename: xia_scw_instance-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.7.dist-info/RECORD
+Filename: xia_scw_instance-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
-from xia_scw_instance.instance import ScwInstance
+from xia_scw_instance.instance import ScwInstance, ScwForward
 
 
 __all__ = [
-    "ScwInstance"
+    "ScwInstance", "ScwForward"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

## xia_scw_instance/templates/ScwInstance/main.tf

```diff
@@ -5,7 +5,101 @@
 resource "scaleway_instance_server" "instance" {
   name = var.name
   type = var.type
   image = data.scaleway_instance_image.my_image.id
   tags = var.tags
   state = var.state
 }
+
+
+data "scaleway_vpc_public_gateway" "main" {
+  name = var.vpc_name
+}
+
+data scaleway_vpc_private_network "service" {
+  name = var.lan_name
+}
+
+data scaleway_vpc_gateway_network "service_net" {
+    gateway_id = data.scaleway_vpc_public_gateway.main.id
+    private_network_id = data.scaleway_vpc_private_network.service.id
+}
+
+resource "scaleway_instance_private_nic" "service_nic" {
+  count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+  server_id = scaleway_instance_server.instance.id
+  private_network_id = data.scaleway_vpc_private_network.service.id
+}
+
+resource "time_sleep" "wait_5_seconds_after_service_nic" {
+  count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+  depends_on = [scaleway_instance_private_nic.service_nic]
+  create_duration = "5s"
+}
+
+resource scaleway_vpc_public_gateway_dhcp_reservation main {
+    count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+
+    gateway_network_id = data.scaleway_vpc_gateway_network.service_net.id
+    mac_address = scaleway_instance_private_nic.service_nic[0].mac_address
+    ip_address = var.lan_ip
+    depends_on = [time_sleep.wait_5_seconds_after_service_nic]
+}
+
+locals {
+  ufw_ssh = length(var.ssh_hosts) > 0 ? [
+    for ip in var.ssh_hosts : "ufw allow from ${ip} to any port 22 proto tcp"
+  ] : [
+    "ufw allow ssh"
+  ]
+  ufw_commands = flatten([
+    for rule in var.forwards : [
+      for ip in rule.allowed_ips : "ufw allow from ${ip} to any port ${rule.lan_port} proto ${rule.protocol}"
+    ]
+  ])
+}
+
+resource scaleway_vpc_public_gateway_pat_rule service_pat {
+    for_each = { for i, item in var.forwards : i => item }
+
+    gateway_id = data.scaleway_vpc_public_gateway.main.id
+    private_ip = var.lan_ip
+    private_port = each.value["lan_port"]
+    public_port = each.value["wan_port"]
+    protocol = each.value["protocol"]
+    depends_on = [scaleway_vpc_public_gateway_dhcp_reservation.main]
+}
+
+resource "null_resource" "ufw_status" {
+  count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+
+  triggers = {
+    ssh_status = jsonencode(local.ufw_ssh)
+    app_status = jsonencode(local.ufw_commands)
+  }
+
+  provisioner "remote-exec" {
+    inline = concat(
+      ["ufw --force reset"],
+      local.ufw_ssh,
+      local.ufw_commands,
+      ["ufw --force enable"]
+    )
+
+    connection {
+      type        = "ssh"
+      user        = "root"
+      private_key = file(var.ssh_private_key)
+      host        = var.lan_ip
+
+      bastion_host        = var.wan_ip
+      bastion_port        = 59999
+      bastion_user        = "bastion"
+      bastion_private_key = file(var.ssh_private_key)
+
+      timeout              = "5m"   # Maximum time to wait for the connection to become available
+    }
+  }
+
+  depends_on = [scaleway_vpc_public_gateway_dhcp_reservation.main]
+}
+
```

## xia_scw_instance/templates/ScwInstance/output.tf

```diff
@@ -17,7 +17,39 @@
 output "state" {
   value = scaleway_instance_server.instance.state
 }
 
 output "tags" {
   value = scaleway_instance_server.instance.tags
 }
+
+output "vpc_name" {
+  value = var.vpc_name
+}
+
+output "wan_ip" {
+  value = var.wan_ip
+}
+
+output "lan_ip" {
+  value = var.wan_ip
+}
+
+output "lan_name" {
+  value = var.lan_name
+}
+
+output "ssh_hosts" {
+  value = var.ssh_hosts
+}
+
+output "forwards" {
+  value = var.forwards
+}
+
+output "ufw_rules" {
+  value = local.ufw_commands
+}
+
+output "ssh_rules" {
+  value = local.ufw_ssh
+}
```

## xia_scw_instance/templates/ScwInstance/variables.tf

```diff
@@ -34,7 +34,98 @@
 }
 
 variable "tags" {
     type = list(string)
     default = null  #xia#
     #xia# default = [{% for v in tags %}{% if loop.index > 1 %}, {% endif %}{% if v is not none %}"{{ v }}"{% else %}null{% endif %}{% endfor %}]
 }
+
+variable "vpc_name" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if vpc_name is defined and vpc_name is not none %}"{{ vpc_name }}"{% else %}null{% endif %}
+
+}
+
+variable "wan_ip" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if wan_ip is defined and wan_ip is not none %}"{{ wan_ip }}"{% else %}null{% endif %}
+
+}
+
+variable "lan_ip" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if lan_ip is defined and lan_ip is not none %}"{{ lan_ip }}"{% else %}null{% endif %}
+
+}
+
+variable "lan_name" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if lan_name is defined and lan_name is not none %}"{{ lan_name }}"{% else %}null{% endif %}
+
+}
+
+variable "ssh_hosts" {
+    type = list(string)
+    default = null  #xia#
+    #xia# default = [{% for v in ssh_hosts %}{% if loop.index > 1 %}, {% endif %}{% if v is not none %}"{{ v }}"{% else %}null{% endif %}{% endfor %}]
+
+    validation {
+    condition = (
+      alltrue([
+        for ip in var.ssh_hosts: (
+          can(regex("^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$", ip)) ||
+          can(regex("^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)/(?:3[0-2]|[12]?[0-9])$", ip))
+        )
+      ])
+    )
+    error_message = "Each element of the allowed_ip variable must be a valid IPv4 address or an IPv4 address with a subnet mask."
+  }
+}
+
+variable "forwards" {
+    type = list(object({
+      protocol = string
+      wan_port = number
+      lan_port = number
+      allowed_ips = list(string)
+    }))
+    default = null  #xia#
+#xia#     default = [{% for v in forwards %}
+#xia#             {% if loop.index > 1 %},{% endif %}{
+#xia#             {% for w, x in v.items() %}
+#xia#                 {% if x is boolean %}
+#xia#         {{ w }} = {% if x is none %}null{% elif x %}true{% else %}false{% endif %}
+
+#xia#                 {% elif x is string %}
+#xia#         {{ w }} = {% if x is not none %}"{{ x }}"{% else %}null{% endif %}
+
+#xia#                 {% elif x is number %}
+#xia#         {{ w }} = {% if x is not none %}{{ x }}{% else %}null{% endif %}
+
+#xia#                 {% elif x is sequence and x is not string %}
+#xia#         {{ w }} = [{% for y in x %}{% if loop.index > 1 %}, {% endif %}{% if y is not none %}"{{ y }}"{% else %}null{% endif %}{% endfor %}]
+
+#xia#                 {% endif %}
+#xia#             {% endfor %}
+#xia#     }{% endfor %}]
+    validation {
+      condition = alltrue([
+         for rule in var.forwards : alltrue([
+           for ip in rule.allowed_ips: (
+             can(regex("^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$", ip)) ||
+             can(regex("^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)/(?:3[0-2]|[12]?[0-9])$", ip))
+           )
+         ])
+      ])
+
+      error_message = "Each element of the allowed_ips variable must be a valid IPv4 address or an IPv4 address with a subnet mask."
+    }
+}
+
+variable "ssh_private_key" {
+  type = string
+  default = null
+}
```

## Comparing `xia_scw_instance-0.0.7.dist-info/METADATA` & `xia_scw_instance-0.0.8.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.7
+Version: 0.0.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine-terraform
 Requires-Dist: xia-scw-vpc
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-instance.svg?color=blue
@@ -27,9 +25,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

## Comparing `xia_scw_instance-0.0.7.dist-info/RECORD` & `xia_scw_instance-0.0.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_scw_instance/__init__.py,sha256=z0kzipNk7TFrxvmzt9k3maCiR8i4oEMKs0BXpNRzQ94,107
-xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=yc_C5R1_n5tbkUATQpzHEz7qYkRWe3KKs6BQfhNGkjA,241152
+xia_scw_instance/__init__.py,sha256=xE9u2A2lBfr7FX2xDzAx2VAtHRy8_vMNeDY7TqCRv-k,133
+xia_scw_instance/instance.cpython-310-darwin.so,sha256=HfAJetR28wJXF8fjV7HGJiw8cwWJgBNXoijZFFC1RKA,252312
 xia_scw_instance/templates/ScwInstance/backend.tf,sha256=E6fgAX-nMcTt9oErRKvK67uJPdB-O77YJpzAvf06zgs,69
-xia_scw_instance/templates/ScwInstance/main.tf,sha256=JVqPHsgfV9EhIIxk11sQ-Po2s47MziWljrrqIQyg8v4,243
-xia_scw_instance/templates/ScwInstance/output.tf,sha256=0-ExjDDABoitkjoegeosrS50oo57VhNmicg17NR7KE4,396
+xia_scw_instance/templates/ScwInstance/main.tf,sha256=4AT2qTq0fYZBzJBJXvWxktIvoqWY6Qlgs-6Wf1PXeQE,3026
+xia_scw_instance/templates/ScwInstance/output.tf,sha256=3xDrNiAsa1jY_YqxmeTH2aJDtGPboK-5MnJwtIH4Yi8,766
 xia_scw_instance/templates/ScwInstance/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
-xia_scw_instance/templates/ScwInstance/variables.tf,sha256=tjh2NHOT-v9dTpc0c4FTaGrE8y9Gfm4ME8eVbI2To1g,1063
-xia_scw_instance-0.0.7.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
-xia_scw_instance-0.0.7.dist-info/METADATA,sha256=z8JRQfvHNtsKDEUWIkS1ERcFKbKnyPVA6t3ep11_b6E,699
-xia_scw_instance-0.0.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_instance-0.0.7.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
-xia_scw_instance-0.0.7.dist-info/RECORD,,
+xia_scw_instance/templates/ScwInstance/variables.tf,sha256=qkzRe_c7wVjYF89AqoJQcYPu0kyxRgo1Q0QrlUuxgsQ,4173
+xia_scw_instance-0.0.8.dist-info/LICENSE.txt,sha256=CgeJ1rTURAK7GLPD_GW3lyXH8ZFFrBDM0ekl9JHZR2s,152
+xia_scw_instance-0.0.8.dist-info/METADATA,sha256=E4sdNyhqg_DJOaPjY1E7HeFBPb_O-QhoJ1vpVG1fpFA,662
+xia_scw_instance-0.0.8.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_scw_instance-0.0.8.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
+xia_scw_instance-0.0.8.dist-info/RECORD,,
```

