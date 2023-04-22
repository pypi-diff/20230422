# Comparing `tmp/telegram_pay-0.1.2.tar.gz` & `tmp/telegram_pay-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_pay-0.1.2.tar", max compression
+gzip compressed data, was "telegram_pay-0.1.3.tar", max compression
```

## Comparing `telegram_pay-0.1.2.tar` & `telegram_pay-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2023-03-19 23:10:26.757609 telegram_pay-0.1.2/LICENSE
--rw-r--r--   0        0        0      447 2023-03-30 19:12:37.456276 telegram_pay-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      379 2023-03-20 06:37:34.725487 telegram_pay-0.1.2/README.md
--rw-r--r--   0        0        0       74 2023-03-20 06:22:24.533182 telegram_pay-0.1.2/telegram_pay/__init__.py
--rw-r--r--   0        0        0     1915 2023-03-20 01:17:31.849639 telegram_pay-0.1.2/telegram_pay/enums.py
--rw-r--r--   0        0        0     4083 2023-03-30 19:12:04.809832 telegram_pay-0.1.2/telegram_pay/models.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 telegram_pay-0.1.2/setup.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 telegram_pay-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-19 12:42:24.063222 telegram_pay-0.1.3/LICENSE
+-rw-r--r--   0        0        0      447 2023-04-22 15:59:09.736770 telegram_pay-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      379 2023-04-19 12:42:24.064220 telegram_pay-0.1.3/README.md
+-rw-r--r--   0        0        0       74 2023-04-19 12:42:24.066213 telegram_pay-0.1.3/telegram_pay/__init__.py
+-rw-r--r--   0        0        0     1915 2023-04-19 12:42:24.066213 telegram_pay-0.1.3/telegram_pay/enums.py
+-rw-r--r--   0        0        0     4528 2023-04-22 15:58:05.914989 telegram_pay-0.1.3/telegram_pay/models.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 telegram_pay-0.1.3/setup.py
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 telegram_pay-0.1.3/PKG-INFO
```

### Comparing `telegram_pay-0.1.2/LICENSE` & `telegram_pay-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_pay-0.1.2/telegram_pay/enums.py` & `telegram_pay-0.1.3/telegram_pay/enums.py`

 * *Files identical despite different names*

### Comparing `telegram_pay-0.1.2/telegram_pay/models.py` & `telegram_pay-0.1.3/telegram_pay/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,25 @@
             subscription_json[0]["client"] = self
             return Subscription(**(subscription_json[0]))
         
         return Subscription(client=self, subscription_id=subscription_id, exists=False, user_id=user_id)
 
     async def cancel_subscription(self, subscription_unique_id: str):
         endpoint = f"subscriptions/{subscription_unique_id}/cancel"
-        return await self.make_request(endpoint)
+        return await self.make_request_auth(endpoint)
+    
+    async def apply_promocode(self, subscription_id: str, user_id: int, promocode: str, sale: int):
+        endpoint = "promocodes/apply"
+        params = {
+            "subscription_id": subscription_id,
+            "user_id": user_id,
+            "promocode": promocode,
+            "sale": sale
+        }
+        return await self.make_request_auth(endpoint, params)
 
 class Subscription(BaseModel):
     client: TelegramPay
     subscription_id: str
     exists: bool
     test_mode: Optional[bool]
     user_id: int
@@ -69,14 +79,16 @@
     valid_until: Optional[datetime]
     amount: Optional[Decimal]
     currency: Optional[Currency]
     interval: Optional[Interval]
     status: Optional[SubscriptionStatus]
     description: Optional[str]
     start_date: Optional[datetime]
+    promocode: Optional[str]
+    sale: Optional[int]
 
     class Config:
         arbitrary_types_allowed = True
 
     @property
     def valid(self) -> bool:
         return self.exists and datetime.now(tz=pytz.UTC) < self.valid_until
```

### Comparing `telegram_pay-0.1.2/setup.py` & `telegram_pay-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'pydantic>=1.10.6,<2.0.0', 'pytz>=2022.7.1,<2023.0.0']
 
 setup_kwargs = {
     'name': 'telegram-pay',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Wrapper for api.pay.4u.studio',
     'long_description': '# Install\n`pip install telegram-pay`\n\n# Use\n```python\nfrom telegram_pay import TelegramPay\n\nasync def main():\n    \n    client = TelegramPay(shop_id=SHOP_ID, shop_token=SHOP_TOKEN)\n    subscription = await client.get_user_subscription(USER_ID, SUBSCRIPTION_ID)\n\n    if subscription.valid:\n        # User is subscribed\n    else:\n        # User is not subscribed\n```',
     'author': 'Snimshchikov Ilya',
     'author_email': 'snimshchikov.ilya@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `telegram_pay-0.1.2/PKG-INFO` & `telegram_pay-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-pay
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper for api.pay.4u.studio
 License: MIT
 Author: Snimshchikov Ilya
 Author-email: snimshchikov.ilya@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

