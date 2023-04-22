# Comparing `tmp/bitdust-0.1.7.233.tar.gz` & `tmp/bitdust-0.1.8.234.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitdust-0.1.7.233.tar", last modified: Fri Apr 21 14:01:38 2023, max compression
+gzip compressed data, was "dist/bitdust-0.1.8.234.tar", last modified: Sat Apr 22 20:43:16 2023, max compression
```

## Comparing `bitdust-0.1.7.233.tar` & `bitdust-0.1.8.234.tar`

### file list

```diff
@@ -1,482 +1,482 @@
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.258923 bitdust-0.1.7.233/
--rw-r--r--   0 veselin   (1000) veselin   (1001)    34520 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/LICENSE.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7712 2023-04-21 14:01:38.258923 bitdust-0.1.7.233/PKG-INFO
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6011 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/README.txt
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.190921 bitdust-0.1.7.233/bitdust/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.190921 bitdust-0.1.7.233/bitdust/access/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8145 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/group_access_donor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    69935 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/group_member.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    27158 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/groups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35302 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/key_ring.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    46155 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/shared_access_coordinator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16003 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/access/shared_access_donor.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/automats/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/automats/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    28621 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/automats/automat.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4035 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/automats/global_state.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/blockchain/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/blockchain/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/broadcast/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7494 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcast_listener.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4803 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcast_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14662 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcaster_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10000 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/broadcast/broadcasters_finder.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.194921 bitdust-0.1.7.233/bitdust/chat/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      876 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3306 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/kbhit.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    29641 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/message_database.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5675 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/message_keeper.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11276 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/nickname_holder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11315 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/nickname_observer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10358 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/chat/terminal_chat.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/coins/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16133 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/accountant_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10172 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/accountants_finder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13995 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_db.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7339 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6480 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_io.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17260 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/coins_miner.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10287 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/contract_chain_consumer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7023 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/contract_chain_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10444 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/customer_contract_executor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6104 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/mine_old.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5311 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/miner_old.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11275 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/coins/supplier_contract_executor.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/contacts/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    38445 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/contactsdb.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3829 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/friends.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    21012 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/identitycache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14809 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/contacts/identitydb.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/crypt/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5835 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/certificate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4029 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/cipher.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11851 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/encrypted.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/hashes.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13081 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/key.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39203 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/my_keys.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/number.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8811 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/rsa_key.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17628 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/crypt/signed.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/currency/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/currency/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7434 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/currency/geth_service.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.198921 bitdust-0.1.7.233/bitdust/customer/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    41073 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/fire_hire.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13849 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/list_files_orator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26487 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/supplier_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13424 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/customer/supplier_finder.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.202921 bitdust-0.1.7.233/bitdust/dht/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      954 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10289 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/dht_records.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14437 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/dht_relations.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    62442 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/dht_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4098 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/dht/known_nodes.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.202921 bitdust-0.1.7.233/bitdust/interface/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)   238439 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/api.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    53720 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/api_rest_http_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11461 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/api_web_socket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    57996 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/cmd_line_json.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7069 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/cmd_line_json_templates.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22207 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/interface/ftp_server.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.202921 bitdust-0.1.7.233/bitdust/lib/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      969 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7701 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/diskspace.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/getsizeof.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10243 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/jsn.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    40342 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/jsontemplate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11193 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/maths.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    31961 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/misc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8488 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/nameurl.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    31041 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/net_misc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16067 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/packetid.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15989 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/schedule.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3508 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/serialization.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2760 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/strng.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    23049 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/txws.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10343 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/udp.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2382 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/utime.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13150 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/lib/websock.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.206921 bitdust-0.1.7.233/bitdust/logs/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25640 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/lg.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3211 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/measure_it.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1890 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/memdebug.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8227 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/weblog.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10403 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/logs/webtraffic.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.206921 bitdust-0.1.7.233/bitdust/main/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      949 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    34709 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/bpmain.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14262 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/bptester.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20957 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12982 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config_defaults.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24970 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config_details.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10719 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/config_types.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1712 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/bitdust/main/default_network.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9443 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/events.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9615 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/help.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20827 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/initializer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5089 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/install_wizard.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15084 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/installer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6602 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/listeners.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2368 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/network_config.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    60704 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/settings.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11845 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/main/shutdowner.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.210922 bitdust-0.1.7.233/bitdust/p2p/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      925 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8983 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/commands.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17986 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/handshaker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    28281 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/id_rotator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22021 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/lookup.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    23837 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/network_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11849 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/network_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    29615 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/online_status.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    27694 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    37669 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17410 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_service_seeker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4556 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/p2p_stats.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    19004 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/propagate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8730 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/p2p/ratings.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.210922 bitdust-0.1.7.233/bitdust/raid/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      933 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24733 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/eccmap.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5943 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/make.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20051 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/raid_worker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2059 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/raidutils.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8614 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/read.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9178 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/rebuild.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5395 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/raid/worker.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.218922 bitdust-0.1.7.233/bitdust/services/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26507 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/driver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17419 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/local_service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4424 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_accountant.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1974 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_backup_db.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6595 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_backups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1486 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_blockchain.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9792 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_broadcasting.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2897 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_contract_chain.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5591 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2618 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_contracts.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11976 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_family.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2318 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_patrol.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4913 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_customer_support.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1618 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_data_disintegration.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5001 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_data_motion.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9743 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_employer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8193 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_entangled_dht.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2511 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_gateway.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2009 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_http_connections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4091 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_http_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5346 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_identity_propagate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1991 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_identity_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2390 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_ip_port_responder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3298 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_keys_registry.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11261 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_keys_storage.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_list_files.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8420 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_message_broker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_message_history.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2127 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_miner.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4100 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_my_data.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2935 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_my_ip_port.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4938 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_network.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2033 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_nodes_lookup.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10155 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_p2p_hookups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7449 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_p2p_notifications.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3981 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_personal_messages.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4318 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_private_groups.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4827 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_private_messages.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4590 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_proxy_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_proxy_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1577 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_rebuilding.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1565 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_restores.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3397 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_shared_data.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17790 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_supplier.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2452 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_supplier_contracts.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1994 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_tcp_connections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4431 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_tcp_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2962 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_udp_datagrams.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5040 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/services/service_udp_transport.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.222922 bitdust-0.1.7.233/bitdust/storage/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      958 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12346 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/accounting.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    21358 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/archive_reader.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14921 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/archive_writer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22859 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39695 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_control.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    77837 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_fs.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    75581 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_matrix.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16663 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_monitor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    32245 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_rebuilder.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12919 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_schedule.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8285 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/backup_tar.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20832 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/index_synchronizer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    16189 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/keys_synchronizer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9662 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/restore_monitor.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    33963 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/restore_worker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11658 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/storage/tar_file.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.222922 bitdust-0.1.7.233/bitdust/stream/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    34695 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/broker_negotiator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4688 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/data_receiver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    20254 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/data_sender.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11841 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/file_down.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12865 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/file_up.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    38717 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/io_throttle.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    29553 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/message.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    91952 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/message_peddler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    19432 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/message_producer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    43379 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/p2p_queue.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35334 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stream/queue_keeper.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.222922 bitdust-0.1.7.233/bitdust/stun/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1223 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stun/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    23168 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stun/stun_client.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6390 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/stun/stun_server.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.226922 bitdust-0.1.7.233/bitdust/supplier/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/customer_assistant.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35366 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/customer_space.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8938 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/customers_rejector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    51966 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/family_member.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10878 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/list_files.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6955 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/supplier/local_tester.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.226922 bitdust-0.1.7.233/bitdust/system/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      961 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    37906 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/bpio.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6797 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/child_process.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14220 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/deploy.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4405 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/dirsize.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6550 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/diskusage.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6110 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/local_fs.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8609 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/nonblocking.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11747 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/run_upnpc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11571 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/tmpfile.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8526 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/system/tray_icon.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.226922 bitdust-0.1.7.233/bitdust/transport/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1161 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9653 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/bandwidth.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13659 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/callback.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    45667 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/gateway.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/http/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8974 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/http_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14059 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/http_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      842 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/sum_client.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      633 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/sum_server.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)    12360 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/transport_http_old.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2216 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/http/twisted-web-ssl.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10153 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/network_transport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    21546 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/packet_in.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    55997 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/packet_out.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/proxy/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13162 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    40557 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_receiver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    68687 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_router.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24428 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/proxy/proxy_sender.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/tcp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    18570 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_connection.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13313 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15160 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22333 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/tcp/tcp_stream.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/transport/udp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_connector.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24562 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_file_queue.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13917 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_interface.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    19322 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26324 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_session.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    57234 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/transport/udp/udp_stream.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.230922 bitdust-0.1.7.233/bitdust/updates/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/updates/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12033 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/updates/git_proc.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.234922 bitdust-0.1.7.233/bitdust/userid/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15285 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/global_id.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25972 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_registrator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    15375 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_restorer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    18020 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39959 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/id_url.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    39644 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/identity.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4119 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/known_servers.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22377 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust/userid/my_id.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.190921 bitdust-0.1.7.233/bitdust.egg-info/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7712 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/PKG-INFO
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14699 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/SOURCES.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)        1 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/dependency_links.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)      120 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/requires.txt
--rw-r--r--   0 veselin   (1000) veselin   (1001)       22 2023-04-21 14:01:38.000000 bitdust-0.1.7.233/bitdust.egg-info/top_level.txt
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.234922 bitdust-0.1.7.233/bitdust_forks/
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.242922 bitdust-0.1.7.233/bitdust_forks/Bismuth/
--rw-r--r--   0 veselin   (1000) veselin   (1001)        0 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1699 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/aliases.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1567 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/aliasesv2.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    37606 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/apihandler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      116 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/application_directories.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      846 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/balance_nogui.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2403 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/check_tx.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1034 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_addpeers.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      906 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1086 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_reg_round.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14518 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/commands.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3421 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/connectionmanager.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4748 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/connections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    18284 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/dbhandler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1310 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getaddresssince.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1426 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getstatus.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4399 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/difficulty.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    26736 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/digest.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11146 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/essentials.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2255 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/fork.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9427 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/genesis.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      790 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/hmac_drbg.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      715 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1114 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane_asyncio.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9049 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/ledger_explorer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/log.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    32179 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/mempool.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2362 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/mining.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7396 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/mining_heavy3.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)   116112 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      561 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/node_stop.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6116 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/optiexplorer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8203 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/optihash.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6014 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/options.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25033 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/optipoolware.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    24519 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/peershandler.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6820 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/plugins.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      537 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/process_search.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/quantizer.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8159 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/regnet.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      636 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/rewards_reindex.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      446 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/rewards_test.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5812 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/rpcconnections.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2014 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/send_csv.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4611 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/send_nogui_noconf.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5625 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/simplecrypt.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9408 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/staking.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9526 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/tokensv2.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1164 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_keys.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11108 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_server.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6998 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_websocket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    14984 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/Bismuth/worker.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.246923 bitdust-0.1.7.233/bitdust_forks/CodernityDB/
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)      700 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/__init__.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)    42787 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1037 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_gevent.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     8184 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_safe_shared.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3992 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_super_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7835 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/debug_stuff.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/env.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)    33960 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/hash_index.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     4814 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25578 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/indexcreator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4860 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5547 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache_with_lock.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1370 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/migrate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1011 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/misc.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     2851 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/patch.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3756 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4115 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache_with_lock.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     5125 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_hash.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3863 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_index.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3806 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/storage.py
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)   107565 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB/tree_index.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.246923 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    43644 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1040 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_gevent.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_safe_shared.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3973 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_super_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_thread_safe.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7915 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/debug_stuff.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/env.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    40383 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/hash_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4958 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25451 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/indexcreator.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5435 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6221 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1371 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/migrate.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1010 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/misc.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2852 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/patch.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4376 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4639 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache_with_lock.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6030 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_hash.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3714 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/storage.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)   111785 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/CodernityDB3/tree_index.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/entangled/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1474 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    25438 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/dtuple.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2008 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2181 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/constants.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3401 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/contact.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    12393 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/datastore.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8793 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/encoding.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5867 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/kbucket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6548 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgformat.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3471 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgtypes.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    89776 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/node.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    33799 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/protocol.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    22400 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/routingtable.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13052 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/entangled/node.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/parallelp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)      885 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/
--rw-r--r--   0 veselin   (1000) veselin   (1001)    36502 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4764 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppauto.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    11913 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppserver.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6981 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/pptransport.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5046 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppworker.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.250923 bitdust-0.1.7.233/bitdust_forks/txrestapi/
--rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/__init__.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/
--rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7447 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/json_resource.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1472 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/methods.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2941 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/resource.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)      169 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/service.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     9470 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/tests.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/bitdust_forks/websocket/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1022 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/__init__.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13641 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_abnf.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13508 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_app.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1758 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_cookiejar.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    17675 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_core.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2404 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_exceptions.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6436 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_handshake.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    10842 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_http.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2156 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_logging.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4757 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_socket.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     1797 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_ssl_compat.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4707 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_url.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6951 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/bitdust_forks/websocket/_utils.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/scripts/
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1918 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/scripts/bitdust
--rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1833 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/scripts/bitdust_worker
--rw-r--r--   0 veselin   (1000) veselin   (1001)       38 2023-04-21 14:01:38.258923 bitdust-0.1.7.233/setup.cfg
--rw-r--r--   0 veselin   (1000) veselin   (1001)     5284 2023-04-21 14:01:37.000000 bitdust-0.1.7.233/setup.py
-drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-21 14:01:38.254923 bitdust-0.1.7.233/tests/
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7089 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_backup_fs.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7938 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_backup_restore.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4064 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_codernity_db.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     8271 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_crypt_signed.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    35543 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_id_url.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     4942 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_identity.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     7730 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_my_keys.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3024 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_raid_make_read.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     3560 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_raid_manager.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)    13735 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_raid_worker.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     2299 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_rsa_key.py
--rw-r--r--   0 veselin   (1000) veselin   (1001)     6347 2023-04-21 10:30:35.000000 bitdust-0.1.7.233/tests/test_serialize.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.209024 bitdust-0.1.8.234/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    34520 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/LICENSE.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7712 2023-04-22 20:43:16.209024 bitdust-0.1.8.234/PKG-INFO
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6011 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/README.txt
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.125022 bitdust-0.1.8.234/bitdust/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.129022 bitdust-0.1.8.234/bitdust/access/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8145 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/group_access_donor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    69936 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/group_member.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    27158 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/groups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35302 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/key_ring.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    46155 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/shared_access_coordinator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16003 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/access/shared_access_donor.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.129022 bitdust-0.1.8.234/bitdust/automats/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/automats/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    28621 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/automats/automat.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4035 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/automats/global_state.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.129022 bitdust-0.1.8.234/bitdust/blockchain/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/blockchain/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.129022 bitdust-0.1.8.234/bitdust/broadcast/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/broadcast/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7494 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/broadcast/broadcast_listener.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4803 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/broadcast/broadcast_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14662 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/broadcast/broadcaster_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10000 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/broadcast/broadcasters_finder.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.129022 bitdust-0.1.8.234/bitdust/chat/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      876 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3306 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/kbhit.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    29560 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/message_database.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5675 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/message_keeper.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11276 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/nickname_holder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11315 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/nickname_observer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10358 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/chat/terminal_chat.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.133022 bitdust-0.1.8.234/bitdust/coins/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16133 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/accountant_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10172 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/accountants_finder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13995 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/coins_db.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7339 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/coins_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6480 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/coins_io.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17260 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/coins_miner.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10287 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/contract_chain_consumer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7023 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/contract_chain_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10444 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/customer_contract_executor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6104 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/mine_old.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5311 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/miner_old.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11275 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/coins/supplier_contract_executor.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.133022 bitdust-0.1.8.234/bitdust/contacts/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/contacts/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    38445 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/contacts/contactsdb.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3829 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/contacts/friends.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    21012 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/contacts/identitycache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14809 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/contacts/identitydb.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.133022 bitdust-0.1.8.234/bitdust/crypt/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5835 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/certificate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4029 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/cipher.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11851 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/encrypted.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/hashes.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13081 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/key.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39464 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/my_keys.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/number.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8811 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/rsa_key.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17628 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/crypt/signed.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.133022 bitdust-0.1.8.234/bitdust/currency/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/currency/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7434 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/currency/geth_service.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.137022 bitdust-0.1.8.234/bitdust/customer/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/customer/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    41073 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/customer/fire_hire.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13849 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/customer/list_files_orator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26487 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/customer/supplier_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13424 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/customer/supplier_finder.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.137022 bitdust-0.1.8.234/bitdust/dht/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      954 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/dht/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10289 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/dht/dht_records.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14437 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/dht/dht_relations.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    62442 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/dht/dht_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4098 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/dht/known_nodes.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.137022 bitdust-0.1.8.234/bitdust/interface/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)   238439 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/api.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    53720 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/api_rest_http_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11461 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/api_web_socket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    57996 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/cmd_line_json.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7069 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/cmd_line_json_templates.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22207 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/interface/ftp_server.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.141022 bitdust-0.1.8.234/bitdust/lib/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      969 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7701 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/diskspace.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2799 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/getsizeof.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10243 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/jsn.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    40342 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/jsontemplate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11193 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/maths.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    31961 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/misc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8488 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/nameurl.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    31041 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/net_misc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16067 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/packetid.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15989 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/schedule.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3508 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/serialization.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2760 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/strng.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    23049 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/txws.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10343 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/udp.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2382 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/utime.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13150 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/lib/websock.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.141022 bitdust-0.1.8.234/bitdust/logs/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/logs/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25640 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/logs/lg.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3211 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/logs/measure_it.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1890 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/logs/memdebug.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8227 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/logs/weblog.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10403 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/logs/webtraffic.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.145022 bitdust-0.1.8.234/bitdust/main/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      949 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    34709 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/bpmain.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14262 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/bptester.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20957 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/config.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12982 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/config_defaults.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24970 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/config_details.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10719 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/config_types.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1428 2023-04-22 20:43:15.000000 bitdust-0.1.8.234/bitdust/main/default_network.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9443 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/events.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9615 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/help.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20827 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/initializer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5089 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/install_wizard.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15084 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/installer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6602 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/listeners.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2368 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/network_config.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    60704 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/settings.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11845 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/main/shutdowner.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.145022 bitdust-0.1.8.234/bitdust/p2p/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      925 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8983 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/commands.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17986 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/handshaker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    28300 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/id_rotator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22021 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/lookup.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    23837 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/network_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11849 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/network_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    29615 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/online_status.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    27694 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/p2p_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    37669 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/p2p_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17410 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/p2p_service_seeker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4556 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/p2p_stats.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    19004 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/propagate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8730 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/p2p/ratings.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.149022 bitdust-0.1.8.234/bitdust/raid/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      933 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24733 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/eccmap.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5943 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/make.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20051 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/raid_worker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2059 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/raidutils.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8614 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/read.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9178 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/rebuild.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5395 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/raid/worker.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.157023 bitdust-0.1.8.234/bitdust/services/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      884 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26507 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/driver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17419 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/local_service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4424 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_accountant.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1974 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_backup_db.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6595 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_backups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1486 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_blockchain.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9792 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_broadcasting.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2897 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_contract_chain.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5591 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_customer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2618 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_customer_contracts.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11976 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_customer_family.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2318 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_customer_patrol.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4913 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_customer_support.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1618 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_data_disintegration.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5001 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_data_motion.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9743 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_employer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8193 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_entangled_dht.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2511 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_gateway.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2009 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_http_connections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4091 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_http_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5346 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_identity_propagate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1991 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_identity_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2390 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_ip_port_responder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3298 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_keys_registry.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11261 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_keys_storage.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3253 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_list_files.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8420 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_message_broker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4322 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_message_history.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2127 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_miner.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4100 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_my_data.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2935 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_my_ip_port.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4938 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_network.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2033 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_nodes_lookup.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10155 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_p2p_hookups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7449 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_p2p_notifications.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3981 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_personal_messages.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4318 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_private_groups.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4827 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_private_messages.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4590 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_proxy_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_proxy_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1577 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_rebuilding.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1565 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_restores.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3397 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_shared_data.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17790 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_supplier.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2452 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_supplier_contracts.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1994 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_tcp_connections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4431 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_tcp_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2962 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_udp_datagrams.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5040 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/services/service_udp_transport.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.161023 bitdust-0.1.8.234/bitdust/storage/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      958 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12346 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/accounting.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    21358 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/archive_reader.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14921 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/archive_writer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22859 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39695 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_control.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    77837 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_fs.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    75581 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_matrix.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16663 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_monitor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    32245 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_rebuilder.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12919 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_schedule.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8285 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/backup_tar.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20832 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/index_synchronizer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    16189 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/keys_synchronizer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9662 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/restore_monitor.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    33963 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/restore_worker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11658 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/storage/tar_file.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.165023 bitdust-0.1.8.234/bitdust/stream/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      882 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    34695 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/broker_negotiator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4688 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/data_receiver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    20254 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/data_sender.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11841 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/file_down.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12865 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/file_up.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    38717 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/io_throttle.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    29553 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/message.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    91952 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/message_peddler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    19432 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/message_producer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    43379 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/p2p_queue.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35334 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stream/queue_keeper.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.165023 bitdust-0.1.8.234/bitdust/stun/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1223 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stun/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    23168 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stun/stun_client.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6390 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/stun/stun_server.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.165023 bitdust-0.1.8.234/bitdust/supplier/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      880 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/customer_assistant.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35366 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/customer_space.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8938 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/customers_rejector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    51966 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/family_member.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10878 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/list_files.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6955 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/supplier/local_tester.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.169023 bitdust-0.1.8.234/bitdust/system/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      961 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    37906 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/bpio.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6797 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/child_process.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14220 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/deploy.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4405 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/dirsize.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6550 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/diskusage.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6110 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/local_fs.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8609 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/nonblocking.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11747 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/run_upnpc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11571 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/tmpfile.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8526 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/system/tray_icon.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.173023 bitdust-0.1.8.234/bitdust/transport/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1161 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9653 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/bandwidth.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13659 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/callback.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    45667 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/gateway.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.173023 bitdust-0.1.8.234/bitdust/transport/http/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8974 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/http_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14059 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/http_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      842 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/sum_client.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      633 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/sum_server.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)    12360 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/transport_http_old.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2216 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/http/twisted-web-ssl.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10153 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/network_transport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    21546 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/packet_in.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    55997 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/packet_out.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.173023 bitdust-0.1.8.234/bitdust/transport/proxy/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      881 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/proxy/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13162 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/proxy/proxy_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    40557 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/proxy/proxy_receiver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    68687 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/proxy/proxy_router.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24428 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/proxy/proxy_sender.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.177023 bitdust-0.1.8.234/bitdust/transport/tcp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/tcp/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    18570 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/tcp/tcp_connection.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13313 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/tcp/tcp_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15160 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/tcp/tcp_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22333 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/tcp/tcp_stream.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.177023 bitdust-0.1.8.234/bitdust/transport/udp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11284 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/udp_connector.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24562 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/udp_file_queue.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13917 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/udp_interface.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    19322 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/udp_node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26324 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/udp_session.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    57234 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/transport/udp/udp_stream.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.177023 bitdust-0.1.8.234/bitdust/updates/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      879 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/updates/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12033 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/updates/git_proc.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.181023 bitdust-0.1.8.234/bitdust/userid/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      877 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15285 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/global_id.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25972 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/id_registrator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    15375 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/id_restorer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17980 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/id_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39959 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/id_url.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    39644 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/identity.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4119 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/known_servers.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22377 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust/userid/my_id.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.125022 bitdust-0.1.8.234/bitdust.egg-info/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7712 2023-04-22 20:43:16.000000 bitdust-0.1.8.234/bitdust.egg-info/PKG-INFO
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14699 2023-04-22 20:43:16.000000 bitdust-0.1.8.234/bitdust.egg-info/SOURCES.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        1 2023-04-22 20:43:16.000000 bitdust-0.1.8.234/bitdust.egg-info/dependency_links.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      120 2023-04-22 20:43:16.000000 bitdust-0.1.8.234/bitdust.egg-info/requires.txt
+-rw-r--r--   0 veselin   (1000) veselin   (1001)       22 2023-04-22 20:43:16.000000 bitdust-0.1.8.234/bitdust.egg-info/top_level.txt
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.181023 bitdust-0.1.8.234/bitdust_forks/
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.193024 bitdust-0.1.8.234/bitdust_forks/Bismuth/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        0 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1699 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/aliases.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1567 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/aliasesv2.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    37606 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/apihandler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      116 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/application_directories.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      846 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/balance_nogui.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2403 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/check_tx.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1034 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/cmd_addpeers.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      906 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1086 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/cmd_hn_reg_round.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14518 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/commands.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3421 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/connectionmanager.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4748 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/connections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    18284 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/dbhandler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1310 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/demo_getaddresssince.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1426 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/demo_getstatus.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4399 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/difficulty.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    26736 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/digest.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11146 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/essentials.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2255 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/fork.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9427 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/genesis.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      790 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/hmac_drbg.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      715 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/hyperlane.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1114 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/hyperlane_asyncio.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9049 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/ledger_explorer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1764 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/log.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    32179 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/mempool.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2362 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/mining.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7396 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/mining_heavy3.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)   116112 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      561 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/node_stop.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6116 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/optiexplorer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8203 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/optihash.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6014 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/options.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25033 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/optipoolware.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    24519 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/peershandler.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6820 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/plugins.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      537 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/process_search.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/quantizer.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8159 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/regnet.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      636 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/rewards_reindex.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      446 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/rewards_test.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5812 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/rpcconnections.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2014 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/send_csv.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4611 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/send_nogui_noconf.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5625 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/simplecrypt.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9408 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/staking.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9526 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/tokensv2.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1164 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/wallet_keys.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11108 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/wallet_server.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6998 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/wallet_websocket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    14984 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/Bismuth/worker.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.197024 bitdust-0.1.8.234/bitdust_forks/CodernityDB/
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)      700 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/__init__.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)    42787 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/database.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1037 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_gevent.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     8184 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_safe_shared.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3992 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_super_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7835 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/debug_stuff.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/env.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)    33960 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/hash_index.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     4814 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25578 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/indexcreator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4860 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/lfu_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5547 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/lfu_cache_with_lock.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1370 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/migrate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1011 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/misc.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     2851 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/patch.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3756 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/rr_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4115 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/rr_cache_with_lock.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     5125 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/sharded_hash.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3863 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/sharded_index.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     3806 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/storage.py
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)   107565 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB/tree_index.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.197024 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      700 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    43644 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1040 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_gevent.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8236 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_safe_shared.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3973 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_super_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1170 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_thread_safe.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7915 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/debug_stuff.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      764 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/env.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    40383 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/hash_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4958 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25451 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/indexcreator.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5435 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/lfu_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6221 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1371 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/migrate.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1010 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/misc.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2852 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/patch.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4376 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/rr_cache.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4639 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/rr_cache_with_lock.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6030 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/sharded_hash.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3714 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/sharded_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4261 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/storage.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)   111785 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/CodernityDB3/tree_index.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1803 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.201024 bitdust-0.1.8.234/bitdust_forks/entangled/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1474 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    25438 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/dtuple.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.201024 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2008 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2181 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/constants.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3401 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/contact.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    12393 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/datastore.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8793 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/encoding.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5867 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/kbucket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6548 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/msgformat.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3471 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/msgtypes.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    89776 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/node.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    33799 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/protocol.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    22400 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/routingtable.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13052 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/entangled/node.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.201024 bitdust-0.1.8.234/bitdust_forks/parallelp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      885 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/parallelp/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.201024 bitdust-0.1.8.234/bitdust_forks/parallelp/pp/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    36502 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/parallelp/pp/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4764 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/parallelp/pp/ppauto.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    11913 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/parallelp/pp/ppserver.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6981 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/parallelp/pp/pptransport.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5046 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/parallelp/pp/ppworker.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.201024 bitdust-0.1.8.234/bitdust_forks/txrestapi/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/__init__.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.201024 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)        2 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7447 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/json_resource.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1472 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/methods.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2941 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/resource.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)      169 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/service.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     9470 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/tests.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.205024 bitdust-0.1.8.234/bitdust_forks/websocket/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1022 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/__init__.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13641 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_abnf.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13508 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_app.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1758 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_cookiejar.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    17675 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_core.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2404 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_exceptions.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6436 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_handshake.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    10842 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_http.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2156 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_logging.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4757 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_socket.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     1797 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_ssl_compat.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4707 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_url.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6951 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/bitdust_forks/websocket/_utils.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.205024 bitdust-0.1.8.234/scripts/
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1918 2023-04-22 20:43:15.000000 bitdust-0.1.8.234/scripts/bitdust
+-rwxr-xr-x   0 veselin   (1000) veselin   (1001)     1833 2023-04-22 20:43:15.000000 bitdust-0.1.8.234/scripts/bitdust_worker
+-rw-r--r--   0 veselin   (1000) veselin   (1001)       38 2023-04-22 20:43:16.209024 bitdust-0.1.8.234/setup.cfg
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     5284 2023-04-22 20:43:15.000000 bitdust-0.1.8.234/setup.py
+drwxr-xr-x   0 veselin   (1000) veselin   (1001)        0 2023-04-22 20:43:16.209024 bitdust-0.1.8.234/tests/
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7089 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_backup_fs.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7938 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_backup_restore.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4064 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_codernity_db.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     8271 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_crypt_signed.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    35543 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_id_url.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     4942 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_identity.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     7730 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_my_keys.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3024 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_raid_make_read.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     3560 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_raid_manager.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)    13735 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_raid_worker.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     2299 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_rsa_key.py
+-rw-r--r--   0 veselin   (1000) veselin   (1001)     6347 2023-04-22 19:32:08.000000 bitdust-0.1.8.234/tests/test_serialize.py
```

### Comparing `bitdust-0.1.7.233/LICENSE.txt` & `bitdust-0.1.8.234/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/PKG-INFO` & `bitdust-0.1.8.234/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitdust
-Version: 0.1.7.233
+Version: 0.1.8.234
 Summary: p2p secure distributed storage and communication engine
 Home-page: https://bitdust.io
 Download-URL: https://bitdust.io
 Author: Veselin Penev, BitDust
 Author-email: bitdust.io@gmail.com
 Maintainer: Veselin Penev, BitDust
 Maintainer-email: veselin@bitdust.io
```

### Comparing `bitdust-0.1.7.233/README.txt` & `bitdust-0.1.8.234/README.txt`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/__init__.py` & `bitdust-0.1.8.234/bitdust/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/access/__init__.py` & `bitdust-0.1.8.234/bitdust/access/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/access/group_access_donor.py` & `bitdust-0.1.8.234/bitdust/access/group_access_donor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/access/group_member.py` & `bitdust-0.1.8.234/bitdust/access/group_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,19 +821,14 @@
         """
         Action method.
         """
         self.group_brokers_updated = False
         if event == 'leave':
             groups.set_group_active(self.group_key_id, False)
             groups.save_group_info(self.group_key_id)
-            if kwargs.get('erase_key', False):
-                if my_keys.is_key_registered(self.group_key_id):
-                    my_keys.erase_key(self.group_key_id)
-                else:
-                    lg.warn('key %r not registered, can not be erased' % self.group_key_id)
         else:
             groups.save_group_info(self.group_key_id)
 
     def doCancelService(self, event, *args, **kwargs):
         """
         Action method.
         """
@@ -842,14 +837,19 @@
                 if not broker_idurl:
                     continue
                 p2p_service.SendCancelService(
                     remote_idurl=broker_idurl,
                     service_name='service_message_broker',
                     json_payload=self._do_prepare_service_request_params(broker_idurl, action='queue-disconnect'),
                 )
+            if kwargs.get('erase_key', False):
+                if my_keys.is_key_registered(self.group_key_id):
+                    my_keys.erase_key(self.group_key_id)
+                else:
+                    lg.warn('key %r not registered, can not be erased' % self.group_key_id)
 
     def doDestroyMe(self, *args, **kwargs):
         """
         Remove all references to the state machine object to destroy it.
         """
         events.remove_subscriber(self._on_group_brokers_updated, 'group-brokers-updated')
         message.clear_consumer_callbacks(self.name)
@@ -1203,15 +1203,15 @@
         if _Debug:
             lg.args(_DebugLevel, broker=possible_broker_idurl, pos=desired_broker_position, action=action, owner=self.group_creator_id)
         group_key_info = {}
         # if not my_keys.is_key_registered(self.group_key_id):
         #     lg.warn('group key %r was not registered, checking all registered keys' % self.group_key_id)
         #     my_keys.check_rename_my_keys(prefix=self.group_key_id.split('@')[0])
         if not my_keys.is_key_registered(self.group_key_id):
-            lg.err('closing group_member %r because key %r is not registered' % (self, self.group_key_id))
+            lg.warn('closing group_member %r because key %r is not registered' % (self, self.group_key_id))
             lg.exc('group key %r is not registered' % self.group_key_id)
             self.automat('shutdown')
             return
         try:
             group_key_info = my_keys.get_key_info(
                 key_id=self.group_key_id,
                 include_private=False,
```

### Comparing `bitdust-0.1.7.233/bitdust/access/groups.py` & `bitdust-0.1.8.234/bitdust/access/groups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/access/key_ring.py` & `bitdust-0.1.8.234/bitdust/access/key_ring.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/access/shared_access_coordinator.py` & `bitdust-0.1.8.234/bitdust/access/shared_access_coordinator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/access/shared_access_donor.py` & `bitdust-0.1.8.234/bitdust/access/shared_access_donor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/automats/__init__.py` & `bitdust-0.1.8.234/bitdust/automats/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/automats/automat.py` & `bitdust-0.1.8.234/bitdust/automats/automat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/automats/global_state.py` & `bitdust-0.1.8.234/bitdust/automats/global_state.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/blockchain/__init__.py` & `bitdust-0.1.8.234/bitdust/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/broadcast/__init__.py` & `bitdust-0.1.8.234/bitdust/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/broadcast/broadcast_listener.py` & `bitdust-0.1.8.234/bitdust/broadcast/broadcast_listener.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/broadcast/broadcast_service.py` & `bitdust-0.1.8.234/bitdust/broadcast/broadcast_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/broadcast/broadcaster_node.py` & `bitdust-0.1.8.234/bitdust/broadcast/broadcaster_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/broadcast/broadcasters_finder.py` & `bitdust-0.1.8.234/bitdust/broadcast/broadcasters_finder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/chat/__init__.py` & `bitdust-0.1.8.234/bitdust/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/chat/kbhit.py` & `bitdust-0.1.8.234/bitdust/chat/kbhit.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/chat/message_database.py` & `bitdust-0.1.8.234/bitdust/chat/message_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,18 +200,15 @@
 
 def get_conversation_id(
     sender_local_key_id,
     recipient_local_key_id,
     payload_type,
 ):
     conversation_id = None
-    if payload_type in [
-        3,
-        4,
-    ]:
+    if payload_type in [3, 4]:
         conversation_id = '{}&{}'.format(recipient_local_key_id, recipient_local_key_id)
     elif payload_type == 2:
         if recipient_local_key_id < sender_local_key_id:
             conversation_id = '{}&{}'.format(recipient_local_key_id, sender_local_key_id)
         else:
             conversation_id = '{}&{}'.format(sender_local_key_id, recipient_local_key_id)
     else:
@@ -225,18 +222,15 @@
 
 def build_json_message(data, message_id, message_time=None, sender=None, recipient=None, message_type=None, direction=None, conversation_id=None):
     if not sender:
         sender = my_id.getGlobalID(key_alias='master')
     if not recipient:
         recipient = my_id.getGlobalID(key_alias='master')
     if direction is None:
-        if message_type in [
-            'private_message',
-            None,
-        ]:
+        if message_type in ['private_message', None]:
             direction = 'out' if sender == my_id.getGlobalID(key_alias='master') else 'in'
         else:
             direction = 'in'
     else:
         direction = direction.replace('incoming', 'in').replace('outgoing', 'out')
     new_json = {
         'payload': {
@@ -731,18 +725,15 @@
         new_local_key_id,
         new_public_key,
     ]
     cur().execute(sql, params)
     db().commit()
     if _Debug:
         lg.args(_DebugLevel, sql=sql, params=params)
-    if conversation_type in [
-        'group_message',
-        'personal_message',
-    ]:
+    if conversation_type in ['group_message', 'personal_message']:
         update_conversation(
             sender_local_key_id=new_local_key_id,
             recipient_local_key_id=new_local_key_id,
             payload_type=MESSAGE_TYPES.get(conversation_type, 1),
             payload_time=utime.utcnow_to_sec1970(),
             payload_message_id='',
         )
```

### Comparing `bitdust-0.1.7.233/bitdust/chat/message_keeper.py` & `bitdust-0.1.8.234/bitdust/chat/message_keeper.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/chat/nickname_holder.py` & `bitdust-0.1.8.234/bitdust/chat/nickname_holder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/chat/nickname_observer.py` & `bitdust-0.1.8.234/bitdust/chat/nickname_observer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/chat/terminal_chat.py` & `bitdust-0.1.8.234/bitdust/chat/terminal_chat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/__init__.py` & `bitdust-0.1.8.234/bitdust/coins/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/accountant_node.py` & `bitdust-0.1.8.234/bitdust/coins/accountant_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/accountants_finder.py` & `bitdust-0.1.8.234/bitdust/coins/accountants_finder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/coins_db.py` & `bitdust-0.1.8.234/bitdust/coins/coins_db.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/coins_index.py` & `bitdust-0.1.8.234/bitdust/coins/coins_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/coins_io.py` & `bitdust-0.1.8.234/bitdust/coins/coins_io.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/coins_miner.py` & `bitdust-0.1.8.234/bitdust/coins/coins_miner.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/contract_chain_consumer.py` & `bitdust-0.1.8.234/bitdust/coins/contract_chain_consumer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/contract_chain_node.py` & `bitdust-0.1.8.234/bitdust/coins/contract_chain_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/customer_contract_executor.py` & `bitdust-0.1.8.234/bitdust/coins/customer_contract_executor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/mine_old.py` & `bitdust-0.1.8.234/bitdust/coins/mine_old.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/miner_old.py` & `bitdust-0.1.8.234/bitdust/coins/miner_old.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/coins/supplier_contract_executor.py` & `bitdust-0.1.8.234/bitdust/coins/supplier_contract_executor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/contacts/__init__.py` & `bitdust-0.1.8.234/bitdust/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/contacts/contactsdb.py` & `bitdust-0.1.8.234/bitdust/contacts/contactsdb.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/contacts/friends.py` & `bitdust-0.1.8.234/bitdust/contacts/friends.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/contacts/identitycache.py` & `bitdust-0.1.8.234/bitdust/contacts/identitycache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/contacts/identitydb.py` & `bitdust-0.1.8.234/bitdust/contacts/identitydb.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/__init__.py` & `bitdust-0.1.8.234/bitdust/crypt/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/certificate.py` & `bitdust-0.1.8.234/bitdust/crypt/certificate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/cipher.py` & `bitdust-0.1.8.234/bitdust/crypt/cipher.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/encrypted.py` & `bitdust-0.1.8.234/bitdust/crypt/encrypted.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/hashes.py` & `bitdust-0.1.8.234/bitdust/crypt/hashes.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/key.py` & `bitdust-0.1.8.234/bitdust/crypt/key.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/my_keys.py` & `bitdust-0.1.8.234/bitdust/crypt/my_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -558,14 +558,15 @@
     key_object.active = active
     known_keys()[key_id] = key_object
     if _Debug:
         lg.out(_DebugLevel, '    key %r registered' % key_id)
     save_key(key_id, keys_folder=keys_folder)
     events.send('key-registered', data=dict(
         key_id=key_id,
+        local_key_id=new_local_key_id,
         label=label,
         key_size=key_object.size(),
     ))
     listeners.push_snapshot(
         'key', snap_id=key_id, data=make_key_info(
             key_object=key_object,
             key_id=key_id,
@@ -595,24 +596,26 @@
         is_private = True
     try:
         os.remove(key_filepath)
     except:
         lg.exc()
         return False
     k_obj = known_keys().pop(key_id)
+    erased_local_key_id = k_obj.local_key_id
     local_keys().pop(k_obj.local_key_id, None)
     local_keys_index().pop(k_obj.toPublicString(), None)
     gc.collect()
     if _Debug:
         lg.out(_DebugLevel, '    key %s removed, file %s deleted' % (key_id, key_filepath))
-    events.send('key-erased', data=dict(key_id=key_id, is_private=is_private))
+    events.send('key-erased', data=dict(key_id=key_id, local_key_id=erased_local_key_id, is_private=is_private))
     listeners.push_snapshot(
         'key', snap_id=key_id, deleted=True, data=make_key_info(
             key_object=None,
             key_id=key_id,
+            local_id=erased_local_key_id,
             event='key-erased',
             include_private=False,
             include_local_id=True,
             include_signature=True,
             include_label=True,
             include_state=True,
         )
@@ -943,15 +946,17 @@
     if hasattr(key.MyPrivateKeyObject(), 'size'):
         r['size'] = strng.to_text(key.MyPrivateKeyObject().size())
     else:
         r['size'] = '0'
     return r
 
 
-def make_key_info(key_object, key_id=None, key_alias=None, creator_idurl=None, include_private=False, generate_signature=False, include_signature=False, include_local_id=False, include_label=True, include_state=False, event=None):
+def make_key_info(
+    key_object, key_id=None, key_alias=None, creator_idurl=None, include_private=False, generate_signature=False, include_signature=False, include_local_id=False, include_label=True, include_state=False, event=None, local_id=None
+):
     if key_id:
         key_id = latest_key_id(key_id)
         key_alias, creator_idurl = split_key_id(key_id)
     else:
         key_id = make_key_id(alias=key_alias, creator_idurl=id_url.field(creator_idurl))
     r = {
         'key_id': key_id,
@@ -976,15 +981,18 @@
         if include_private:
             r['private'] = strng.to_text(key_object.toPrivateString()) if key_object else None
     if key_object and hasattr(key_object, 'size'):
         r['size'] = strng.to_text(key_object.size())
     else:
         r['size'] = '0'
     if include_local_id:
-        r['local_key_id'] = getattr(key_object, 'local_key_id', None) if key_object else None
+        if local_id:
+            r['local_key_id'] = local_id
+        else:
+            r['local_key_id'] = getattr(key_object, 'local_key_id', None) if key_object else None
     if key_object and generate_signature:
         r = sign_key_info(r)
     else:
         if include_signature and key_object and key_object.isSigned():
             r['signature'] = key_object.signed[0]
             r['signature_pubkey'] = key_object.signed[1]
     return r
```

### Comparing `bitdust-0.1.7.233/bitdust/crypt/number.py` & `bitdust-0.1.8.234/bitdust/crypt/number.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/rsa_key.py` & `bitdust-0.1.8.234/bitdust/crypt/rsa_key.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/crypt/signed.py` & `bitdust-0.1.8.234/bitdust/crypt/signed.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/currency/__init__.py` & `bitdust-0.1.8.234/bitdust/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/currency/geth_service.py` & `bitdust-0.1.8.234/bitdust/currency/geth_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/customer/__init__.py` & `bitdust-0.1.8.234/bitdust/customer/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/customer/fire_hire.py` & `bitdust-0.1.8.234/bitdust/customer/fire_hire.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/customer/list_files_orator.py` & `bitdust-0.1.8.234/bitdust/customer/list_files_orator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/customer/supplier_connector.py` & `bitdust-0.1.8.234/bitdust/customer/supplier_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/customer/supplier_finder.py` & `bitdust-0.1.8.234/bitdust/customer/supplier_finder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/dht/__init__.py` & `bitdust-0.1.8.234/bitdust/dht/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/dht/dht_records.py` & `bitdust-0.1.8.234/bitdust/dht/dht_records.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/dht/dht_relations.py` & `bitdust-0.1.8.234/bitdust/dht/dht_relations.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/dht/dht_service.py` & `bitdust-0.1.8.234/bitdust/dht/dht_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/dht/known_nodes.py` & `bitdust-0.1.8.234/bitdust/dht/known_nodes.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/__init__.py` & `bitdust-0.1.8.234/bitdust/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/api.py` & `bitdust-0.1.8.234/bitdust/interface/api.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/api_rest_http_server.py` & `bitdust-0.1.8.234/bitdust/interface/api_rest_http_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/api_web_socket.py` & `bitdust-0.1.8.234/bitdust/interface/api_web_socket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/cmd_line_json.py` & `bitdust-0.1.8.234/bitdust/interface/cmd_line_json.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/cmd_line_json_templates.py` & `bitdust-0.1.8.234/bitdust/interface/cmd_line_json_templates.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/interface/ftp_server.py` & `bitdust-0.1.8.234/bitdust/interface/ftp_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/__init__.py` & `bitdust-0.1.8.234/bitdust/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/diskspace.py` & `bitdust-0.1.8.234/bitdust/lib/diskspace.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/getsizeof.py` & `bitdust-0.1.8.234/bitdust/lib/getsizeof.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/jsn.py` & `bitdust-0.1.8.234/bitdust/lib/jsn.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/jsontemplate.py` & `bitdust-0.1.8.234/bitdust/lib/jsontemplate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/maths.py` & `bitdust-0.1.8.234/bitdust/lib/maths.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/misc.py` & `bitdust-0.1.8.234/bitdust/lib/misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/nameurl.py` & `bitdust-0.1.8.234/bitdust/lib/nameurl.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/net_misc.py` & `bitdust-0.1.8.234/bitdust/lib/net_misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/packetid.py` & `bitdust-0.1.8.234/bitdust/lib/packetid.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/schedule.py` & `bitdust-0.1.8.234/bitdust/lib/schedule.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/serialization.py` & `bitdust-0.1.8.234/bitdust/lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/strng.py` & `bitdust-0.1.8.234/bitdust/lib/strng.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/txws.py` & `bitdust-0.1.8.234/bitdust/lib/txws.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/udp.py` & `bitdust-0.1.8.234/bitdust/lib/udp.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/utime.py` & `bitdust-0.1.8.234/bitdust/lib/utime.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/lib/websock.py` & `bitdust-0.1.8.234/bitdust/lib/websock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/logs/__init__.py` & `bitdust-0.1.8.234/bitdust/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/logs/lg.py` & `bitdust-0.1.8.234/bitdust/logs/lg.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/logs/measure_it.py` & `bitdust-0.1.8.234/bitdust/logs/measure_it.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/logs/memdebug.py` & `bitdust-0.1.8.234/bitdust/logs/memdebug.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/logs/weblog.py` & `bitdust-0.1.8.234/bitdust/logs/weblog.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/logs/webtraffic.py` & `bitdust-0.1.8.234/bitdust/logs/webtraffic.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/__init__.py` & `bitdust-0.1.8.234/bitdust/main/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/bpmain.py` & `bitdust-0.1.8.234/bitdust/main/bpmain.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/bptester.py` & `bitdust-0.1.8.234/bitdust/main/bptester.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/config.py` & `bitdust-0.1.8.234/bitdust/main/config.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/config_defaults.py` & `bitdust-0.1.8.234/bitdust/main/config_defaults.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/config_details.py` & `bitdust-0.1.8.234/bitdust/main/config_details.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/config_types.py` & `bitdust-0.1.8.234/bitdust/main/config_types.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/default_network.py` & `bitdust-0.1.8.234/bitdust/main/default_network.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,34 +12,26 @@
         "udp_port": 14441
       },
       {
         "host": "bitdust.ai",
         "udp_port": 14441
       },
       {
-        "host": "bitrex.ai",
-        "udp_port": 14441
-      },
-      {
         "host": "root-node.ai",
         "udp_port": 14441
       },
       {
         "host": "bahamas.ai",
         "udp_port": 14441
       },
       {
         "host": "peer2peer.ai",
         "udp_port": 14441
       },
       {
-        "host": "webapp.ai",
-        "udp_port": 14441
-      },
-      {
         "host": "seed.bitdust.io",
         "udp_port": 14441
       }
     ],
     "max_age": 86400,
     "parallel_calls": 4,
     "refresh_timeout": 600,
@@ -59,34 +51,26 @@
         "http_port": 80
       },
       {
         "host": "bitdust.ai",
         "http_port": 80
       },
       {
-        "host": "bitrex.ai",
-        "http_port": 80
-      },
-      {
         "host": "root-node.ai",
         "http_port": 80
       },
       {
         "host": "bahamas.ai",
         "http_port": 80
       },
       {
         "host": "peer2peer.ai",
         "http_port": 80
       },
       {
-        "host": "webapp.ai",
-        "http_port": 80
-      },
-      {
         "host": "seed.bitdust.io",
         "http_port": 80
       }
     ],
     "whitelisted_servers": []
   }
 }
```

### Comparing `bitdust-0.1.7.233/bitdust/main/events.py` & `bitdust-0.1.8.234/bitdust/main/events.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/help.py` & `bitdust-0.1.8.234/bitdust/main/help.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/initializer.py` & `bitdust-0.1.8.234/bitdust/main/initializer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/install_wizard.py` & `bitdust-0.1.8.234/bitdust/main/install_wizard.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/installer.py` & `bitdust-0.1.8.234/bitdust/main/installer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/listeners.py` & `bitdust-0.1.8.234/bitdust/main/listeners.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/network_config.py` & `bitdust-0.1.8.234/bitdust/main/network_config.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/settings.py` & `bitdust-0.1.8.234/bitdust/main/settings.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/main/shutdowner.py` & `bitdust-0.1.8.234/bitdust/main/shutdowner.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/__init__.py` & `bitdust-0.1.8.234/bitdust/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/commands.py` & `bitdust-0.1.8.234/bitdust/p2p/commands.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/handshaker.py` & `bitdust-0.1.8.234/bitdust/p2p/handshaker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/id_rotator.py` & `bitdust-0.1.8.234/bitdust/p2p/id_rotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,15 +573,15 @@
                 if not remote_ident.Valid():
                     raise Exception('remote identity not valid at position %r' % pos)
                 if latest_revision == -1:
                     latest_revision = remote_ident.getRevisionValue()
                 if latest_revision <= remote_ident.getRevisionValue():
                     latest_revision = remote_ident.getRevisionValue()
             except:
-                lg.exc()
+                lg.exc(remote_identity_src)
                 self.alive_idurls.append(None)
                 continue
             if idurl_bin not in self.alive_idurls:
                 self.alive_idurls.append(idurl_bin)
         if not self.new_revision:
             self.new_revision = max(local_revision, latest_revision) + 1
         if _Debug:
```

### Comparing `bitdust-0.1.7.233/bitdust/p2p/lookup.py` & `bitdust-0.1.8.234/bitdust/p2p/lookup.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/network_connector.py` & `bitdust-0.1.8.234/bitdust/p2p/network_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/network_service.py` & `bitdust-0.1.8.234/bitdust/p2p/network_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/online_status.py` & `bitdust-0.1.8.234/bitdust/p2p/online_status.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/p2p_connector.py` & `bitdust-0.1.8.234/bitdust/p2p/p2p_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/p2p_service.py` & `bitdust-0.1.8.234/bitdust/p2p/p2p_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/p2p_service_seeker.py` & `bitdust-0.1.8.234/bitdust/p2p/p2p_service_seeker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/p2p_stats.py` & `bitdust-0.1.8.234/bitdust/p2p/p2p_stats.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/propagate.py` & `bitdust-0.1.8.234/bitdust/p2p/propagate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/p2p/ratings.py` & `bitdust-0.1.8.234/bitdust/p2p/ratings.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/__init__.py` & `bitdust-0.1.8.234/bitdust/raid/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/eccmap.py` & `bitdust-0.1.8.234/bitdust/raid/eccmap.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/make.py` & `bitdust-0.1.8.234/bitdust/raid/make.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/raid_worker.py` & `bitdust-0.1.8.234/bitdust/raid/raid_worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/raidutils.py` & `bitdust-0.1.8.234/bitdust/raid/raidutils.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/read.py` & `bitdust-0.1.8.234/bitdust/raid/read.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/rebuild.py` & `bitdust-0.1.8.234/bitdust/raid/rebuild.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/raid/worker.py` & `bitdust-0.1.8.234/bitdust/raid/worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/__init__.py` & `bitdust-0.1.8.234/bitdust/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/driver.py` & `bitdust-0.1.8.234/bitdust/services/driver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/local_service.py` & `bitdust-0.1.8.234/bitdust/services/local_service.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_accountant.py` & `bitdust-0.1.8.234/bitdust/services/service_accountant.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_backup_db.py` & `bitdust-0.1.8.234/bitdust/services/service_backup_db.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_backups.py` & `bitdust-0.1.8.234/bitdust/services/service_backups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_blockchain.py` & `bitdust-0.1.8.234/bitdust/services/service_blockchain.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_broadcasting.py` & `bitdust-0.1.8.234/bitdust/services/service_broadcasting.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_contract_chain.py` & `bitdust-0.1.8.234/bitdust/services/service_contract_chain.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_customer.py` & `bitdust-0.1.8.234/bitdust/services/service_customer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_customer_contracts.py` & `bitdust-0.1.8.234/bitdust/services/service_customer_contracts.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_customer_family.py` & `bitdust-0.1.8.234/bitdust/services/service_customer_family.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_customer_patrol.py` & `bitdust-0.1.8.234/bitdust/services/service_customer_patrol.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_customer_support.py` & `bitdust-0.1.8.234/bitdust/services/service_customer_support.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_data_disintegration.py` & `bitdust-0.1.8.234/bitdust/services/service_data_disintegration.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_data_motion.py` & `bitdust-0.1.8.234/bitdust/services/service_data_motion.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_employer.py` & `bitdust-0.1.8.234/bitdust/services/service_employer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_entangled_dht.py` & `bitdust-0.1.8.234/bitdust/services/service_entangled_dht.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_gateway.py` & `bitdust-0.1.8.234/bitdust/services/service_gateway.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_http_connections.py` & `bitdust-0.1.8.234/bitdust/services/service_http_connections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_http_transport.py` & `bitdust-0.1.8.234/bitdust/services/service_http_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_identity_propagate.py` & `bitdust-0.1.8.234/bitdust/services/service_identity_propagate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_identity_server.py` & `bitdust-0.1.8.234/bitdust/services/service_identity_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_ip_port_responder.py` & `bitdust-0.1.8.234/bitdust/services/service_ip_port_responder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_keys_registry.py` & `bitdust-0.1.8.234/bitdust/services/service_keys_registry.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_keys_storage.py` & `bitdust-0.1.8.234/bitdust/services/service_keys_storage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_list_files.py` & `bitdust-0.1.8.234/bitdust/services/service_list_files.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_message_broker.py` & `bitdust-0.1.8.234/bitdust/services/service_message_broker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_message_history.py` & `bitdust-0.1.8.234/bitdust/services/service_message_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,18 +89,18 @@
         self.do_check_create_rename_key(evt.data['key_id'])
 
     def on_key_renamed(self, evt):
         self.do_check_create_rename_key(evt.data['new_key_id'])
 
     def on_key_erased(self, evt):
         from bitdust.main import listeners
-        from bitdust.crypt import my_keys
+        from bitdust.chat import message_database
         if evt.data['key_id'].startswith('group_'):
-            local_key_id = my_keys.get_local_key_id(evt.data['key_id'])
-            listeners.push_snapshot('conversation', snap_id=local_key_id, deleted=True)
+            conversation_id = message_database.get_conversation_id(evt.data['local_key_id'], evt.data['local_key_id'], 3)
+            listeners.push_snapshot('conversation', snap_id=conversation_id, deleted=True)
 
     def do_check_create_rename_key(self, new_key_id):
         from bitdust.logs import lg
         from bitdust.crypt import my_keys
         from bitdust.chat import message_database
         try:
             new_public_key = my_keys.get_public_key_raw(new_key_id)
```

### Comparing `bitdust-0.1.7.233/bitdust/services/service_miner.py` & `bitdust-0.1.8.234/bitdust/services/service_miner.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_my_data.py` & `bitdust-0.1.8.234/bitdust/services/service_my_data.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_my_ip_port.py` & `bitdust-0.1.8.234/bitdust/services/service_my_ip_port.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_network.py` & `bitdust-0.1.8.234/bitdust/services/service_network.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_nodes_lookup.py` & `bitdust-0.1.8.234/bitdust/services/service_nodes_lookup.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_p2p_hookups.py` & `bitdust-0.1.8.234/bitdust/services/service_p2p_hookups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_p2p_notifications.py` & `bitdust-0.1.8.234/bitdust/services/service_p2p_notifications.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_personal_messages.py` & `bitdust-0.1.8.234/bitdust/services/service_personal_messages.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_private_groups.py` & `bitdust-0.1.8.234/bitdust/services/service_private_groups.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_private_messages.py` & `bitdust-0.1.8.234/bitdust/services/service_private_messages.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_proxy_server.py` & `bitdust-0.1.8.234/bitdust/services/service_proxy_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_proxy_transport.py` & `bitdust-0.1.8.234/bitdust/services/service_proxy_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_rebuilding.py` & `bitdust-0.1.8.234/bitdust/services/service_rebuilding.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_restores.py` & `bitdust-0.1.8.234/bitdust/services/service_restores.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_shared_data.py` & `bitdust-0.1.8.234/bitdust/services/service_shared_data.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_supplier.py` & `bitdust-0.1.8.234/bitdust/services/service_supplier.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_supplier_contracts.py` & `bitdust-0.1.8.234/bitdust/services/service_supplier_contracts.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_tcp_connections.py` & `bitdust-0.1.8.234/bitdust/services/service_tcp_connections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_tcp_transport.py` & `bitdust-0.1.8.234/bitdust/services/service_tcp_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_udp_datagrams.py` & `bitdust-0.1.8.234/bitdust/services/service_udp_datagrams.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/services/service_udp_transport.py` & `bitdust-0.1.8.234/bitdust/services/service_udp_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/__init__.py` & `bitdust-0.1.8.234/bitdust/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/accounting.py` & `bitdust-0.1.8.234/bitdust/storage/accounting.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/archive_reader.py` & `bitdust-0.1.8.234/bitdust/storage/archive_reader.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/archive_writer.py` & `bitdust-0.1.8.234/bitdust/storage/archive_writer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup.py` & `bitdust-0.1.8.234/bitdust/storage/backup.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_control.py` & `bitdust-0.1.8.234/bitdust/storage/backup_control.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_fs.py` & `bitdust-0.1.8.234/bitdust/storage/backup_fs.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_matrix.py` & `bitdust-0.1.8.234/bitdust/storage/backup_matrix.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_monitor.py` & `bitdust-0.1.8.234/bitdust/storage/backup_monitor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_rebuilder.py` & `bitdust-0.1.8.234/bitdust/storage/backup_rebuilder.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_schedule.py` & `bitdust-0.1.8.234/bitdust/storage/backup_schedule.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/backup_tar.py` & `bitdust-0.1.8.234/bitdust/storage/backup_tar.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/index_synchronizer.py` & `bitdust-0.1.8.234/bitdust/storage/index_synchronizer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/keys_synchronizer.py` & `bitdust-0.1.8.234/bitdust/storage/keys_synchronizer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/restore_monitor.py` & `bitdust-0.1.8.234/bitdust/storage/restore_monitor.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/restore_worker.py` & `bitdust-0.1.8.234/bitdust/storage/restore_worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/storage/tar_file.py` & `bitdust-0.1.8.234/bitdust/storage/tar_file.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/__init__.py` & `bitdust-0.1.8.234/bitdust/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/broker_negotiator.py` & `bitdust-0.1.8.234/bitdust/stream/broker_negotiator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/data_receiver.py` & `bitdust-0.1.8.234/bitdust/stream/data_receiver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/data_sender.py` & `bitdust-0.1.8.234/bitdust/stream/data_sender.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/file_down.py` & `bitdust-0.1.8.234/bitdust/stream/file_down.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/file_up.py` & `bitdust-0.1.8.234/bitdust/stream/file_up.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/io_throttle.py` & `bitdust-0.1.8.234/bitdust/stream/io_throttle.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/message.py` & `bitdust-0.1.8.234/bitdust/stream/message.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/message_peddler.py` & `bitdust-0.1.8.234/bitdust/stream/message_peddler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/message_producer.py` & `bitdust-0.1.8.234/bitdust/stream/message_producer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/p2p_queue.py` & `bitdust-0.1.8.234/bitdust/stream/p2p_queue.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stream/queue_keeper.py` & `bitdust-0.1.8.234/bitdust/stream/queue_keeper.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stun/__init__.py` & `bitdust-0.1.8.234/bitdust/stun/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stun/stun_client.py` & `bitdust-0.1.8.234/bitdust/stun/stun_client.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/stun/stun_server.py` & `bitdust-0.1.8.234/bitdust/stun/stun_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/__init__.py` & `bitdust-0.1.8.234/bitdust/supplier/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/customer_assistant.py` & `bitdust-0.1.8.234/bitdust/supplier/customer_assistant.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/customer_space.py` & `bitdust-0.1.8.234/bitdust/supplier/customer_space.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/customers_rejector.py` & `bitdust-0.1.8.234/bitdust/supplier/customers_rejector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/family_member.py` & `bitdust-0.1.8.234/bitdust/supplier/family_member.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/list_files.py` & `bitdust-0.1.8.234/bitdust/supplier/list_files.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/supplier/local_tester.py` & `bitdust-0.1.8.234/bitdust/supplier/local_tester.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/__init__.py` & `bitdust-0.1.8.234/bitdust/system/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/bpio.py` & `bitdust-0.1.8.234/bitdust/system/bpio.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/child_process.py` & `bitdust-0.1.8.234/bitdust/system/child_process.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/deploy.py` & `bitdust-0.1.8.234/bitdust/system/deploy.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/dirsize.py` & `bitdust-0.1.8.234/bitdust/system/dirsize.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/diskusage.py` & `bitdust-0.1.8.234/bitdust/system/diskusage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/local_fs.py` & `bitdust-0.1.8.234/bitdust/system/local_fs.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/nonblocking.py` & `bitdust-0.1.8.234/bitdust/system/nonblocking.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/run_upnpc.py` & `bitdust-0.1.8.234/bitdust/system/run_upnpc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/tmpfile.py` & `bitdust-0.1.8.234/bitdust/system/tmpfile.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/system/tray_icon.py` & `bitdust-0.1.8.234/bitdust/system/tray_icon.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/__init__.py` & `bitdust-0.1.8.234/bitdust/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/bandwidth.py` & `bitdust-0.1.8.234/bitdust/transport/bandwidth.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/callback.py` & `bitdust-0.1.8.234/bitdust/transport/callback.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/gateway.py` & `bitdust-0.1.8.234/bitdust/transport/gateway.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/__init__.py` & `bitdust-0.1.8.234/bitdust/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/http_interface.py` & `bitdust-0.1.8.234/bitdust/transport/http/http_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/http_node.py` & `bitdust-0.1.8.234/bitdust/transport/http/http_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/sum_client.py` & `bitdust-0.1.8.234/bitdust/transport/http/sum_client.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/sum_server.py` & `bitdust-0.1.8.234/bitdust/transport/http/sum_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/transport_http_old.py` & `bitdust-0.1.8.234/bitdust/transport/http/transport_http_old.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/http/twisted-web-ssl.py` & `bitdust-0.1.8.234/bitdust/transport/http/twisted-web-ssl.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/network_transport.py` & `bitdust-0.1.8.234/bitdust/transport/network_transport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/packet_in.py` & `bitdust-0.1.8.234/bitdust/transport/packet_in.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/packet_out.py` & `bitdust-0.1.8.234/bitdust/transport/packet_out.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/proxy/__init__.py` & `bitdust-0.1.8.234/bitdust/transport/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_interface.py` & `bitdust-0.1.8.234/bitdust/transport/proxy/proxy_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_receiver.py` & `bitdust-0.1.8.234/bitdust/transport/proxy/proxy_receiver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_router.py` & `bitdust-0.1.8.234/bitdust/transport/proxy/proxy_router.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/proxy/proxy_sender.py` & `bitdust-0.1.8.234/bitdust/transport/proxy/proxy_sender.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/tcp/__init__.py` & `bitdust-0.1.8.234/bitdust/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_connection.py` & `bitdust-0.1.8.234/bitdust/transport/tcp/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_interface.py` & `bitdust-0.1.8.234/bitdust/transport/tcp/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_node.py` & `bitdust-0.1.8.234/bitdust/transport/tcp/tcp_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/tcp/tcp_stream.py` & `bitdust-0.1.8.234/bitdust/transport/tcp/tcp_stream.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/__init__.py` & `bitdust-0.1.8.234/bitdust/transport/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/udp_connector.py` & `bitdust-0.1.8.234/bitdust/transport/udp/udp_connector.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/udp_file_queue.py` & `bitdust-0.1.8.234/bitdust/transport/udp/udp_file_queue.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/udp_interface.py` & `bitdust-0.1.8.234/bitdust/transport/udp/udp_interface.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/udp_node.py` & `bitdust-0.1.8.234/bitdust/transport/udp/udp_node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/udp_session.py` & `bitdust-0.1.8.234/bitdust/transport/udp/udp_session.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/transport/udp/udp_stream.py` & `bitdust-0.1.8.234/bitdust/transport/udp/udp_stream.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/updates/__init__.py` & `bitdust-0.1.8.234/bitdust/updates/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/updates/git_proc.py` & `bitdust-0.1.8.234/bitdust/updates/git_proc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/__init__.py` & `bitdust-0.1.8.234/bitdust/userid/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/global_id.py` & `bitdust-0.1.8.234/bitdust/userid/global_id.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/id_registrator.py` & `bitdust-0.1.8.234/bitdust/userid/id_registrator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/id_restorer.py` & `bitdust-0.1.8.234/bitdust/userid/id_restorer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/id_server.py` & `bitdust-0.1.8.234/bitdust/userid/id_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
     def doSetUp(self, *args, **kwargs):
         """
         Action method.
         """
         self.hostname = settings.getIdServerHost()
         if self.hostname == '':
-            self.hostname = strng.to_bin(misc.readExternalIP())  # bpio.ReadTextFile(settings.ExternalIPFilename())
+            self.hostname = strng.to_bin(misc.readExternalIP())
         if self.hostname == '':
             self.hostname = net_misc.getLocalIp()
         lg.out(4, 'id_server.doSetUp hostname=%s' % strng.to_text(self.hostname))
         if not os.path.isdir(settings.IdentityServerDir()):
             os.makedirs(settings.IdentityServerDir())
             lg.out(4, '            created a folder %s' % settings.IdentityServerDir())
         root = WebRoot()
@@ -232,20 +232,20 @@
             args[0][-1].callback(True)
 
     def _save_identity(self, inputfilename):
         """
         """
         lg.out(6, 'id_server._save_identity ' + inputfilename)
         if os.path.getsize(inputfilename) > 50000:
-            lg.warn('input file too big - ignoring ')
+            lg.warn('input file too big - ignoring')
             tmpfile.erase('idsrv', inputfilename, 'input file too big')
             return
         newxml = bpio.ReadTextFile(inputfilename)
-        if len(newxml.strip()) < 500:
-            lg.warn('input file too small - ignoring ')
+        if not newxml or len(newxml.strip()) < 500:
+            lg.warn('input file too small - ignoring')
             tmpfile.erase('idsrv', inputfilename, 'input file too small')
             return
         try:
             newidentity = identity.identity(xmlsrc=newxml)
         except:
             lg.warn('input file is wrong - ignoring ')
             tmpfile.erase('idsrv', inputfilename, 'input file is wrong')
```

### Comparing `bitdust-0.1.7.233/bitdust/userid/id_url.py` & `bitdust-0.1.8.234/bitdust/userid/id_url.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/identity.py` & `bitdust-0.1.8.234/bitdust/userid/identity.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/known_servers.py` & `bitdust-0.1.8.234/bitdust/userid/known_servers.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust/userid/my_id.py` & `bitdust-0.1.8.234/bitdust/userid/my_id.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust.egg-info/PKG-INFO` & `bitdust-0.1.8.234/bitdust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitdust
-Version: 0.1.7.233
+Version: 0.1.8.234
 Summary: p2p secure distributed storage and communication engine
 Home-page: https://bitdust.io
 Download-URL: https://bitdust.io
 Author: Veselin Penev, BitDust
 Author-email: bitdust.io@gmail.com
 Maintainer: Veselin Penev, BitDust
 Maintainer-email: veselin@bitdust.io
```

### Comparing `bitdust-0.1.7.233/bitdust.egg-info/SOURCES.txt` & `bitdust-0.1.8.234/bitdust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/aliases.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/aliases.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/aliasesv2.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/aliasesv2.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/apihandler.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/apihandler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/balance_nogui.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/balance_nogui.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/check_tx.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/check_tx.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_addpeers.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/cmd_addpeers.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/cmd_hn_last_block_ts.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/cmd_hn_reg_round.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/cmd_hn_reg_round.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/commands.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/commands.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/connectionmanager.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/connectionmanager.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/connections.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/connections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/dbhandler.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/dbhandler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getaddresssince.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/demo_getaddresssince.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/demo_getstatus.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/demo_getstatus.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/difficulty.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/difficulty.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/digest.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/digest.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/essentials.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/essentials.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/fork.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/fork.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/genesis.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/genesis.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/hmac_drbg.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/hmac_drbg.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/hyperlane.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/hyperlane_asyncio.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/hyperlane_asyncio.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/ledger_explorer.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/ledger_explorer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/log.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/log.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/mempool.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/mempool.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/mining.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/mining.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/mining_heavy3.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/mining_heavy3.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/node.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/node_stop.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/node_stop.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/optiexplorer.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/optiexplorer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/optihash.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/optihash.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/options.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/options.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/optipoolware.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/optipoolware.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/peershandler.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/peershandler.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/plugins.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/plugins.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/process_search.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/process_search.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/quantizer.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/quantizer.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/regnet.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/regnet.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/rewards_reindex.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/rewards_reindex.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/rpcconnections.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/rpcconnections.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/send_csv.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/send_csv.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/send_nogui_noconf.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/send_nogui_noconf.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/simplecrypt.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/simplecrypt.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/staking.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/staking.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/tokensv2.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/tokensv2.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_keys.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/wallet_keys.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_server.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/wallet_server.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/wallet_websocket.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/wallet_websocket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/Bismuth/worker.py` & `bitdust-0.1.8.234/bitdust_forks/Bismuth/worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/database.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_gevent.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_gevent.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_safe_shared.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_safe_shared.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_super_thread_safe.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_super_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/database_thread_safe.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/database_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/debug_stuff.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/debug_stuff.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/env.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/env.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/hash_index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/hash_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/indexcreator.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/indexcreator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/lfu_cache_with_lock.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/lfu_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/migrate.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/migrate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/misc.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/patch.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/patch.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/rr_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/rr_cache_with_lock.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/rr_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_hash.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/sharded_hash.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/sharded_index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/sharded_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/storage.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/storage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB/tree_index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB/tree_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_gevent.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_gevent.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_safe_shared.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_safe_shared.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_super_thread_safe.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_super_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/database_thread_safe.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/database_thread_safe.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/debug_stuff.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/debug_stuff.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/env.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/env.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/hash_index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/hash_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/indexcreator.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/indexcreator.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/lfu_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/migrate.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/migrate.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/misc.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/misc.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/patch.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/patch.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/rr_cache.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/rr_cache_with_lock.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/rr_cache_with_lock.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_hash.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/sharded_hash.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/sharded_index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/sharded_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/storage.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/storage.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/CodernityDB3/tree_index.py` & `bitdust-0.1.8.234/bitdust_forks/CodernityDB3/tree_index.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/dtuple.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/dtuple.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/constants.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/constants.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/contact.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/contact.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/datastore.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/datastore.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/encoding.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/encoding.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/kbucket.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/kbucket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgformat.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/msgformat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/msgtypes.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/msgtypes.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/node.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/protocol.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/protocol.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/kademlia/routingtable.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/kademlia/routingtable.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/entangled/node.py` & `bitdust-0.1.8.234/bitdust_forks/entangled/node.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/parallelp/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/parallelp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/parallelp/pp/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppauto.py` & `bitdust-0.1.8.234/bitdust_forks/parallelp/pp/ppauto.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppserver.py` & `bitdust-0.1.8.234/bitdust_forks/parallelp/pp/ppserver.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/pptransport.py` & `bitdust-0.1.8.234/bitdust_forks/parallelp/pp/pptransport.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/parallelp/pp/ppworker.py` & `bitdust-0.1.8.234/bitdust_forks/parallelp/pp/ppworker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/json_resource.py` & `bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/json_resource.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/methods.py` & `bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/methods.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/resource.py` & `bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/resource.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/txrestapi/txrestapi/tests.py` & `bitdust-0.1.8.234/bitdust_forks/txrestapi/txrestapi/tests.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/__init__.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_abnf.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_app.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_cookiejar.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_core.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_exceptions.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_handshake.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_http.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_logging.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_socket.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_ssl_compat.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_url.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/bitdust_forks/websocket/_utils.py` & `bitdust-0.1.8.234/bitdust_forks/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/scripts/bitdust` & `bitdust-0.1.8.234/scripts/bitdust`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/scripts/bitdust_worker` & `bitdust-0.1.8.234/scripts/bitdust_worker`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/setup.py` & `bitdust-0.1.8.234/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 # Please contact us if you have any questions at bitdust.io@gmail.com
 from __future__ import absolute_import
 from setuptools import setup
 
 setup(
     name='bitdust',
-    version='0.1.7.233',
+    version='0.1.8.234',
     author='Veselin Penev, BitDust',
     author_email='bitdust.io@gmail.com',
     maintainer='Veselin Penev, BitDust',
     maintainer_email='veselin@bitdust.io',
     url='https://bitdust.io',
     description='p2p secure distributed storage and communication engine',
     long_description=open('README.txt', 'r').read(),
```

### Comparing `bitdust-0.1.7.233/tests/test_backup_fs.py` & `bitdust-0.1.8.234/tests/test_backup_fs.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_backup_restore.py` & `bitdust-0.1.8.234/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_codernity_db.py` & `bitdust-0.1.8.234/tests/test_codernity_db.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_crypt_signed.py` & `bitdust-0.1.8.234/tests/test_crypt_signed.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_id_url.py` & `bitdust-0.1.8.234/tests/test_id_url.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_identity.py` & `bitdust-0.1.8.234/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_my_keys.py` & `bitdust-0.1.8.234/tests/test_my_keys.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_raid_make_read.py` & `bitdust-0.1.8.234/tests/test_raid_make_read.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_raid_manager.py` & `bitdust-0.1.8.234/tests/test_raid_manager.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_raid_worker.py` & `bitdust-0.1.8.234/tests/test_raid_worker.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_rsa_key.py` & `bitdust-0.1.8.234/tests/test_rsa_key.py`

 * *Files identical despite different names*

### Comparing `bitdust-0.1.7.233/tests/test_serialize.py` & `bitdust-0.1.8.234/tests/test_serialize.py`

 * *Files identical despite different names*

