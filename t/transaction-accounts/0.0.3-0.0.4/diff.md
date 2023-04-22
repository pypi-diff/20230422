# Comparing `tmp/transaction-accounts-0.0.3.tar.gz` & `tmp/transaction-accounts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.0.3.tar", last modified: Sat Apr 22 07:08:08 2023, max compression
+gzip compressed data, was "transaction-accounts-0.0.4.tar", last modified: Sat Apr 22 15:43:52 2023, max compression
```

## Comparing `transaction-accounts-0.0.3.tar` & `transaction-accounts-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 07:08:08.394096 transaction-accounts-0.0.3/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.3/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7023 2023-04-22 07:08:08.394235 transaction-accounts-0.0.3/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 07:08:08.391603 transaction-accounts-0.0.3/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.3/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)     8367 2023-04-22 06:04:52.000000 transaction-accounts-0.0.3/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    11888 2023-04-22 06:04:52.000000 transaction-accounts-0.0.3/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-22 07:08:08.394830 transaction-accounts-0.0.3/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7285 2023-04-22 07:07:37.000000 transaction-accounts-0.0.3/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 07:08:08.393794 transaction-accounts-0.0.3/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7023 2023-04-22 07:08:08.000000 transaction-accounts-0.0.3/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      311 2023-04-22 07:08:08.000000 transaction-accounts-0.0.3/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-22 07:08:08.000000 transaction-accounts-0.0.3/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       33 2023-04-22 07:08:08.000000 transaction-accounts-0.0.3/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-22 07:08:08.000000 transaction-accounts-0.0.3/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.161280 transaction-accounts-0.0.4/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.4/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7382 2023-04-22 15:43:52.161448 transaction-accounts-0.0.4/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.154827 transaction-accounts-0.0.4/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.4/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     8251 2023-04-22 13:55:27.000000 transaction-accounts-0.0.4/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    11134 2023-04-22 15:23:52.000000 transaction-accounts-0.0.4/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-22 15:43:52.162097 transaction-accounts-0.0.4/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7655 2023-04-22 15:43:43.000000 transaction-accounts-0.0.4/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.158023 transaction-accounts-0.0.4/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     3204 2023-04-22 13:49:23.000000 transaction-accounts-0.0.4/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      960 2023-04-22 14:02:47.000000 transaction-accounts-0.0.4/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1917 2023-04-22 14:06:37.000000 transaction-accounts-0.0.4/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2556 2023-04-22 15:20:57.000000 transaction-accounts-0.0.4/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3915 2023-04-22 15:27:27.000000 transaction-accounts-0.0.4/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.160676 transaction-accounts-0.0.4/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7382 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      429 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.0.3/LICENSE.txt` & `transaction-accounts-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.3/PKG-INFO` & `transaction-accounts-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,44 @@
-Metadata-Version: 2.1
-Name: transaction-accounts
-Version: 0.0.3
-Summary: Create configuration for transactional accounts and implement account runtime
-Home-page: https://github.com/igormusic/transaction-accounts
-Author: Igor Music
-Author-email: igormusich@gmail.com
-License: MIT
-Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.3.tar.gz
-Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE.txt
-
+from setuptools import setup, find_packages
 
+setup(
+    name='transaction-accounts',
+    version='0.0.4',
+    description='Create configuration for transactional accounts and implement account runtime',
+    long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction
 accounts.
 
 You can use it to make any type of transaction account, such as a
 savings account, a credit card, or a loan.
 
 Assume we would like to create simple Savings Account that has 3 types
-of balances: 
+of balances:
+ 
 - current balance 
 - interest accrued 
 - withholding tax
 
 We would like to have 4 types of transactions: 
+
 - deposit 
 - interest accrued 
 - interest capitalized 
 - withholding tax
 
 We would like to have 2 types of schedules: 
+
 - accrual schedule 
 - compounding schedule
 
 We would like to have interest rate with 3 tiers: 
+
 - 0 - 10000: 3% 
 - 10000 - 50000: 3.5% 
 - 50000+: 4%
 
 Deposit transaction will increase current balance, and it will be used
 to deposit money to the account. This transaction will be externally
 created and posted to the account.
@@ -80,89 +72,110 @@
 variables: - account: Account - transaction: Transaction - config:
 Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
-   def create_savings_account() -> Configuration:
-       config: Configuration = Configuration("v1")
-
-       current = config.add_position_type("current", "current balance")
-       interest_accrued = config.add_position_type("accrued", "interest accrued")
-       withholding = config.add_position_type("withholding", "withholding tax")
-
-       deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
-
-       interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
-       interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
-
-       capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
-           TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
-
-       withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
-           TransactionOperation.CREDIT, withholding)
-
-       savings_account = config.add_account_type("savingsAccount", "Savings Account")
-
-       savings_account.add_transaction_type(deposit)
-       savings_account.add_transaction_type(interest_accrued_tt)
-       savings_account.add_transaction_type(capitalized)
-       savings_account.add_transaction_type(withholding_txn)
-
-       accrual_schedule = ScheduleType("accrual", "Accrual Schedule", ScheduleFrequency.DAILY, ScheduleEndType.NO_END,
-                                       BusinessDayAdjustment.NO_ADJUSTMENT, "1", "account.start_date")
-
-       savings_account.add_schedule_type(accrual_schedule)
-
-       compounding_schedule = ScheduleType("compounding", "Compounding Schedule", ScheduleFrequency.MONTHLY,
-                                           ScheduleEndType.NO_END, BusinessDayAdjustment.NO_ADJUSTMENT, "1",
-                                           "account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
-
-       savings_account.add_schedule_type(compounding_schedule)
-
-       savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                 interest_accrued_tt,
-                                                 "account.current * config.interest.get_rate(account.current) / Decimal(365)")
+    def create_savings_account() -> Configuration:
+        config: Configuration = Configuration(version="v1")
+    
+        current = config.add_position_type("current", "current balance")
+        interest_accrued = config.add_position_type("accrued", "interest accrued")
+        withholding = config.add_position_type("withholding", "withholding tax")
+    
+        deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
+    
+        interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
+        interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+    
+        capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
+            TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+    
+        withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
+            TransactionOperation.CREDIT, withholding)
+    
+        savings_account = config.add_account_type("savingsAccount", "Savings Account")
+    
+        savings_account.add_transaction_type(deposit)
+        savings_account.add_transaction_type(interest_accrued_tt)
+        savings_account.add_transaction_type(capitalized)
+        savings_account.add_transaction_type(withholding_txn)
+    
+        accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+                                        end_type=ScheduleEndType.NO_END,
+                                        business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                        interval_expression="1", start_date_expression="account.start_date")
+    
+        savings_account.add_schedule_type(accrual_schedule)
+    
+        compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule", frequency=ScheduleFrequency.MONTHLY,
+                                            end_type=ScheduleEndType.NO_END,
+                                            business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                            interval_expression="1",
+                                            start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
+    
+        savings_account.add_schedule_type(compounding_schedule)
+    
+        savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                                  interest_accrued_tt,
+                                                  "account.current * config.interest.get_rate(account.current) / Decimal(365)")
+    
+        savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                                  capitalized, "account.accrued")
+    
+        interest_rate = config.add_rate_type("interest", "Interest Rate")
+    
+        interest_rate.add_tier(Decimal(10000), Decimal(0.03))
+        interest_rate.add_tier(Decimal(100000), Decimal(0.035))
+        interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+    
+        config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
+    
+        return config
 
-       savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                 capitalized, "account.accrued")
 
-       interest_rate = config.add_rate_type("interest", "Interest Rate")
+Given configuration, we can create an account:
 
-       interest_rate.add_tier(Decimal(10000), Decimal(0.03))
-       interest_rate.add_tier(Decimal(100000), Decimal(0.035))
-       interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+.. code:: python
 
-       config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
+       config: Configuration = create_savings_account()
 
-       return config
+        # account = create_account(config, "savingsAccount", date(2019, 1, 1))
+        account_type = config.get_account_type("savingsAccount")
+        account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
+                          config_version= config.version, config=config)
 
-Given configuration, we can create an account:
+        valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
 
-.. code:: python
+        deposit_transaction_type = config.get_transaction_type("deposit")
 
+        external_transactions = group_by_date([
+            ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
+                                amount= Decimal(1000), value_date=date(2019, 1, 1))])
 
-       config: Configuration = create_savings_account()
+        valuation.forecast(date(2020, 1, 1), external_transactions)
 
-       account_type = config.get_account_type("savingsAccount")
-       
-       # account will start on 1st of January 2019
-       account = Account(date(2019, 1, 1), account_type, config)
-       
-       # we will create account valuation on 1st of January 2020 (action date)
-       valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
-       
-       deposit_transaction_type = config.get_transaction_type("deposit")
-       
-       # we will deposit 1000 on 1st of January 2019 (backdated transaction so that we can test accruals)
-       external_transactions = group_by_date([
-           ExternalTransaction(deposit_transaction_type.name, Decimal(1000), date(2019, 1, 1))])
-       
-       # we will forecast balances and transactions as of 1st of January 2020
-       valuation.forecast(date(2020, 1, 1), external_transactions)
-       
-       self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-       self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
-    
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
     
+    ''',
+    author='Igor Music',
+    author_email='igormusich@gmail.com',
+    packages=find_packages(),
+    license='MIT',
+    url='https://github.com/igormusic/transaction-accounts',
+    download_url='https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz',
+    keywords=['TRANSACTION PROCESSING', 'LOANS', 'SAVINGS', 'ACCOUNTS', 'FINANCE', 'BANKING'],
+    install_requires=[
+        'python-dateutil',
+        'pydantic'
+    ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',  # Define that your audience are developers
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.9',
 
+    ],
+)
```

### Comparing `transaction-accounts-0.0.3/accounts/metadata.py` & `transaction-accounts-0.0.4/accounts/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from calendar import monthrange
 from dataclasses import dataclass, field
 from datetime import date
 from decimal import Decimal
 from enum import Enum
-from typing import List, Optional
-
-from dataclasses_json import dataclass_json
+from typing import List, Optional, Dict
+from pydantic import BaseModel
 
 
 class TransactionOperation(Enum):
     CREDIT = 'credit'
     DEBIT = 'debit'
     SET = 'set'
 
@@ -39,38 +38,32 @@
 
 
 class ScheduledTransactionTiming(Enum):
     START_OF_DAY = "start_of_day"
     END_OF_DAY = "end_of_day"
 
 
-@dataclass_json()
-@dataclass()
-class PositionType:
+class PositionType(BaseModel):
     name: str
     label: str
 
 
-@dataclass_json()
-@dataclass()
-class RateTier:
+class RateTier(BaseModel):
     from_amount: Decimal
     to_amount: Decimal
     rate: Decimal
 
 
-@dataclass_json()
-@dataclass()
-class RateType:
+class RateType(BaseModel):
     name: str
     label: str
-    rate_tiers: List[RateTier] = field(default_factory=list)
+    rate_tiers: List[RateTier] = []
 
     def add_tier(self, to_amount: Decimal, rate: Decimal):
-        rate_tier = RateTier(self.get_max_to_amount(), to_amount, rate)
+        rate_tier = RateTier(from_amount=self.get_max_to_amount(), to_amount=to_amount, rate=rate)
         self.rate_tiers.append(rate_tier)
 
     def get_max_to_amount(self):
         if len(self.rate_tiers) == 0:
             return Decimal(0)
 
         max_value = max(self.rate_tiers, key=lambda tier: tier.to_amount)
@@ -105,151 +98,139 @@
 
                 if exit_loop:
                     break
 
         return fee
 
 
-@dataclass_json()
-@dataclass()
-class PositionRule:
+class PositionRule(BaseModel):
     operation: TransactionOperation
     position_type_name: str
 
 
-@dataclass_json()
-@dataclass()
-class TransactionType:
+class TransactionType(BaseModel):
     name: str
     label: str
-    position_rules: List[PositionRule] = field(default_factory=list)
+    position_rules: List[PositionRule] = []
 
     def add_position_rule(self, transaction_operation: TransactionOperation, position_type: PositionType):
-        self.position_rules.append(PositionRule(transaction_operation, position_type.name))
+        self.position_rules.append(PositionRule(operation=transaction_operation, position_type_name=position_type.name))
         return self
 
 
-@dataclass_json()
-@dataclass()
-class ScheduleType:
+class ScheduleType(BaseModel):
     name: str
     label: str
     frequency: ScheduleFrequency
     end_type: ScheduleEndType
     business_day_adjustment: BusinessDayAdjustment
     interval_expression: str
     start_date_expression: str
-    end_date_expression: str = field(default=None)
-    number_of_repeats_expression: str = field(default=None)
-    include_dates_expression: str = field(default=None)
-    exclude_dates_expression: str = field(default=None)
+    end_date_expression: str = None
+    number_of_repeats_expression: str = None
+    include_dates_expression: str = None
+    exclude_dates_expression: str = None
 
 
-@dataclass_json()
-@dataclass()
-class ScheduledTransaction:
+class ScheduledTransaction(BaseModel):
     schedule_name: str
     timing: ScheduledTransactionTiming
     generated_transaction_type: str
     amount_expression: str
 
 
-@dataclass_json()
-@dataclass()
-class TriggeredTransaction:
+class TriggeredTransaction(BaseModel):
     trigger_transaction_type_name: str
     generated_transaction_type: str
     amount_expression: str
 
 
-@dataclass_json()
-@dataclass()
-class PropertyType:
+class PropertyType(BaseModel):
     name: str
     label: str
 
 
-@dataclass_json()
-@dataclass()
-class AccountType:
+class AccountType(BaseModel):
     name: str
     label: str
-    transaction_type_names: List[str] = field(default_factory=list)
-    schedule_types: List[ScheduleType] = field(default_factory=list)
-    property_types: List[PropertyType] = field(default_factory=list)
-    scheduled_transactions: List[ScheduledTransaction] = field(default_factory=list)
-    triggered_transactions: List[TriggeredTransaction] = field(default_factory=list)
+    transaction_type_names: List[str] = []
+    schedule_types: List[ScheduleType] = []
+    property_types: List[PropertyType] = []
+    scheduled_transactions: List[ScheduledTransaction] = []
+    triggered_transactions: List[TriggeredTransaction] = []
 
     def add_transaction_type(self, transaction_type: TransactionType):
         self.transaction_type_names.append(transaction_type.name)
 
     def add_schedule_type(self, schedule_type: ScheduleType):
         self.schedule_types.append(schedule_type)
 
     def add_scheduled_transaction(self, schedule_type: ScheduleType, timing: ScheduledTransactionTiming,
                                   generated_transaction_type: TransactionType, amount_expression: str):
-        scheduled_transaction = ScheduledTransaction(schedule_type.name, timing, generated_transaction_type.name,
-                                                     amount_expression)
+        scheduled_transaction = ScheduledTransaction(schedule_name=schedule_type.name, timing=timing,
+                                                     generated_transaction_type=generated_transaction_type.name,
+                                                     amount_expression=amount_expression)
         self.scheduled_transactions.append(scheduled_transaction)
 
     def add_trigger_transaction(self, trigger_transaction_type: TransactionType,
                                 generated_transaction_type: TransactionType, amount_expression: str):
-        triggered_transaction = TriggeredTransaction(trigger_transaction_type.name, generated_transaction_type.name,
-                                                     amount_expression)
+        triggered_transaction = TriggeredTransaction(name=trigger_transaction_type.name,
+                                                     generated_transaction_type=generated_transaction_type.name,
+                                                     amount_expression=amount_expression)
         self.triggered_transactions.append(triggered_transaction)
 
 
-@dataclass_json()
-@dataclass()
-class Configuration:
+class Configuration(BaseModel):
     version: str
-    transaction_types: List[TransactionType] = field(default_factory=list)
-    position_types: List[PositionType] = field(default_factory=list)
-    account_types: List[AccountType] = field(default_factory=list)
-    rate_types: dict[str,RateType] = field(default_factory=dict)
-    triggered_transactions: List[TriggeredTransaction] = field(default_factory=list)
+    transaction_types: List[TransactionType] = []
+    position_types: List[PositionType] = []
+    account_types: List[AccountType] = []
+    rate_types: Dict[str, RateType] = {}
+    triggered_transactions: List[TriggeredTransaction] = []
 
     def add_transaction_type(self, name: str, label: str) -> TransactionType:
-        transaction_type = TransactionType(name, label)
+        transaction_type = TransactionType(name=name, label=label)
         self.transaction_types.append(transaction_type)
         return transaction_type
 
     def add_position_type(self, name: str, label: str) -> PositionType:
-        position_type = PositionType(name, label)
+        position_type = PositionType(name=name, label=label)
         self.position_types.append(position_type)
         return position_type
 
     def add_account_type(self, name: str, label: str) -> AccountType:
-        account_type = AccountType(name, label)
+        account_type = AccountType(name=name, label=label)
         self.account_types.append(account_type)
         return account_type
 
     def add_rate_type(self, name: str, label: str) -> RateType:
-        rate_type = RateType(name, label)
+        rate_type = RateType(name=name, label=label)
         self.rate_types[name] = rate_type
         return rate_type
 
     def add_trigger_transaction(self, trigger_transaction_type: TransactionType,
                                 generated_transaction_type: TransactionType, amount_expression: str):
-        trigger_transaction = TriggeredTransaction(trigger_transaction_type.name, generated_transaction_type.name,
-                                                   amount_expression)
+        trigger_transaction = TriggeredTransaction(trigger_transaction_type_name=trigger_transaction_type.name,
+                                                   generated_transaction_type=generated_transaction_type.name,
+                                                   amount_expression=amount_expression)
         self.triggered_transactions.append(trigger_transaction)
 
     def get_transaction_type(self, transaction_type_name: str) -> TransactionType:
         return next(tt for tt in self.transaction_types if tt.name == transaction_type_name)
 
     def get_account_type(self, account_type_name: str):
         return next(at for at in self.account_types if at.name == account_type_name)
 
     def get_rate_type(self, rate_type_name: str):
         return next(rt for rt in self.rate_types if rt.name == rate_type_name)
 
-    def get_trigger_transaction(self, trigger_transaction_type_name: str)-> Optional[TriggeredTransaction]:
-        return next((tt for tt in self.triggered_transactions if tt.trigger_transaction_type_name == trigger_transaction_type_name), None)
+    def get_trigger_transaction(self, trigger_transaction_type_name: str) -> Optional[TriggeredTransaction]:
+        return next((tt for tt in self.triggered_transactions if
+                     tt.trigger_transaction_type_name == trigger_transaction_type_name), None)
 
     def __getattr__(self, method_name: str):
         # find rate type by method name
 
         if method_name in self.rate_types:
             return self.rate_types[method_name]
         else:
-            raise AttributeError(f'No such attribute: {method_name}')
+            raise AttributeError(f'No such attribute: {method_name}')
```

### Comparing `transaction-accounts-0.0.3/accounts/runtime.py` & `transaction-accounts-0.0.4/accounts/runtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from typing import Mapping, Any
 
 from dateutil.relativedelta import *
 
 from accounts.metadata import *
 
 
-class Position:
-    def __init__(self):
-        self.amount = Decimal(0)
+class Position(BaseModel):
+    amount: Decimal = Decimal(0)
 
     def apply_operation(self, operation: TransactionOperation, amount: Decimal):
         if operation == TransactionOperation.CREDIT:
             self.amount = self.amount + amount
         elif operation == TransactionOperation.DEBIT:
             self.amount = self.amount - amount
         else:  # Replace
@@ -20,48 +19,34 @@
 
     def copy(self):
         position = Position()
         position.amount = self.amount
         return position
 
 
-class Transaction:
+class Transaction(BaseModel):
     amount = Decimal(0)
-
-    def __init__(self, action_date: date, value_date: date, transaction_type: str, amount: Decimal,
-                 system_generated: bool):
-        self.action_date = action_date
-        self.value_date = value_date
-        self.transaction_type = transaction_type
-        self.amount = amount
-        self.system_generated = system_generated
-
-    def display(self):
-        print("actionDate = {0}, valueDate = {1}, transactionType = {2}, amount = {3}, system_generated = {4}".format(
-            self.action_date,
-            self.value_date,
-            self.transaction_type,
-            self.amount,
-            self.system_generated))
-
-
-class Schedule:
-    def __init__(self, start_date: date, end_type: ScheduleEndType, frequency: ScheduleFrequency, interval: int = 0,
-                 adjustment: BusinessDayAdjustment = BusinessDayAdjustment.NO_ADJUSTMENT,
-                 end_date: date = None, number_of_repeats: int = 0):
-        self.start_date = start_date
-        self.end_type = end_type
-        self.interval = interval
-        self.frequency = frequency
-        self.adjustment = adjustment
-        self.end_date = end_date
-        self.number_of_repeats = number_of_repeats
-        self.include_dates: list[date] = []
-        self.exclude_dates: list[date] = []
-        self.cached_dates: dict[date, list[date]] = {}
+    action_date: date
+    value_date: date
+    transaction_type: str
+    amount: Decimal
+    system_generated: bool
+
+
+class Schedule(BaseModel):
+    start_date: date
+    end_type: ScheduleEndType
+    frequency: ScheduleFrequency
+    interval: int = 0,
+    adjustment: BusinessDayAdjustment = BusinessDayAdjustment.NO_ADJUSTMENT
+    end_date: Optional[date]
+    number_of_repeats: int = 0
+    include_dates: list[date] = []
+    exclude_dates: list[date] = []
+    cached_dates: dict[date, list[date]] = {}
 
     def __is_simple_daily_schedule(self):
         return (self.frequency == ScheduleFrequency.DAILY and
                 self.interval == 1 and
                 self.adjustment == BusinessDayAdjustment.NO_ADJUSTMENT)
 
     def __last_date(self):
@@ -125,40 +110,45 @@
         if self.adjustment == BusinessDayAdjustment.NO_ADJUSTMENT:
             return test_date
 
         # TODO add calendar and call get_adjusted()
         return test_date
 
 
-class ExternalTransaction:
-    def __init__(self, transaction_type_name: str, amount: Decimal, value_date: date):
-        self.transaction_type_name = transaction_type_name
-        self.amount = amount
-        self.value_date = value_date
-
-
-class Account:
-    def __init__(self, start_date: date, account_type: AccountType, config: Configuration):
-        self.start_date = start_date
-        self.account_type_name: str = account_type.name
-        self.config_version: str = config.version
-        self.positions: dict[str, Position] = {}
-        self.schedules: dict[str, Schedule] = {}
-        self.transactions: list[Transaction] = []
-
-        self.__initialize_positions(account_type, config)
-        self.__initialize_schedules(account_type, config)
+class ExternalTransaction(BaseModel):
+    transaction_type_name: str
+    amount: Decimal
+    value_date: date
+
+
+class Account(BaseModel):
+    start_date: date
+    account_type_name: str
+    config_version: str
+    positions: dict[str, Position] = {}
+    schedules: dict[str, Schedule] = {}
+    transactions: list[Transaction] = []
+
+    def __init__(self, *a, **kw):
+        super().__init__(*a, **kw)
+
+        if "config" in kw:
+            config: Configuration = kw["config"]
+            account_type: AccountType = config.get_account_type(self.account_type_name)
+            self.__initialize_positions(account_type, config)
+            self.__initialize_schedules(account_type, config)
 
     def __initialize_schedules(self, account_type: AccountType, config: Configuration):
         for schedule_type in account_type.schedule_types:
-            schedule = Schedule(self.evaluate(schedule_type.start_date_expression, {"config": config, "account": self}),
-                                schedule_type.end_type,
-                                schedule_type.frequency,
-                                self.evaluate(schedule_type.interval_expression, {"config": config, "account": self}),
-                                schedule_type.business_day_adjustment)
+            schedule = Schedule(
+                start_date=self.evaluate(schedule_type.start_date_expression, {"config": config, "account": self}),
+                end_type=schedule_type.end_type,
+                frequency=schedule_type.frequency,
+                interval=self.evaluate(schedule_type.interval_expression, {"config": config, "account": self}),
+                adjustment=schedule_type.business_day_adjustment)
 
             if schedule_type.end_date_expression:
                 schedule.end_date = self.evaluate(schedule_type.end_date_expression,
                                                   {"config": config, "account": self})
 
             if schedule_type.number_of_repeats_expression:
                 schedule.number_of_repeats = self.evaluate(schedule_type.number_of_repeats_expression)
@@ -189,14 +179,17 @@
 
     def __getattr__(self, method_name):
         if method_name in self.positions:
             return self.positions[method_name].amount
         else:
             raise AttributeError(f'No such attribute: {method_name}')
 
+    class Config:
+        exclude = {"config"}
+
 
 def group_by_date(external_transactions):
     grouped = {}
 
     for external_transaction in external_transactions:
         if external_transaction.value_date not in grouped:
             grouped[external_transaction.value_date] = [external_transaction]
@@ -255,15 +248,16 @@
             raise Exception(f'Error evaluating expression: {amount_expression} {e.args}') from e
         else:
             if amount != Decimal(0):
                 self.__create_transaction(transaction_type, value_date, amount, True)
 
     def __create_transaction(self, transaction_type: TransactionType, value_date: date,
                              amount: Decimal, system_generated: bool):
-        transaction = Transaction(self.action_date, value_date, transaction_type.name, amount, system_generated)
+        transaction = Transaction(action_date= self.action_date, value_date=value_date, transaction_type=transaction_type.name,
+                                  amount=amount, system_generated=system_generated)
         self.account.add_transaction(transaction, transaction_type)
 
         triggered_transaction = self.configuration.get_trigger_transaction(transaction_type.name)
 
         if triggered_transaction:
             trigger_amount = self.account.evaluate(triggered_transaction.amount_expression,
                                                    {"transaction": transaction,
```

### Comparing `transaction-accounts-0.0.3/setup.py` & `transaction-accounts-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,55 @@
-from setuptools import setup, find_packages
+Metadata-Version: 2.1
+Name: transaction-accounts
+Version: 0.0.4
+Summary: Create configuration for transactional accounts and implement account runtime
+Home-page: https://github.com/igormusic/transaction-accounts
+Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz
+Author: Igor Music
+Author-email: igormusich@gmail.com
+License: MIT
+Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE.txt
+
 
-setup(
-    name='transaction-accounts',
-    version='0.0.3',
-    description='Create configuration for transactional accounts and implement account runtime',
-    long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction
 accounts.
 
 You can use it to make any type of transaction account, such as a
 savings account, a credit card, or a loan.
 
 Assume we would like to create simple Savings Account that has 3 types
-of balances: 
+of balances:
+ 
 - current balance 
 - interest accrued 
 - withholding tax
 
 We would like to have 4 types of transactions: 
+
 - deposit 
 - interest accrued 
 - interest capitalized 
 - withholding tax
 
 We would like to have 2 types of schedules: 
+
 - accrual schedule 
 - compounding schedule
 
 We would like to have interest rate with 3 tiers: 
+
 - 0 - 10000: 3% 
 - 10000 - 50000: 3.5% 
 - 50000+: 4%
 
 Deposit transaction will increase current balance, and it will be used
 to deposit money to the account. This transaction will be externally
 created and posted to the account.
@@ -68,108 +83,90 @@
 variables: - account: Account - transaction: Transaction - config:
 Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
-   def create_savings_account() -> Configuration:
-       config: Configuration = Configuration("v1")
-
-       current = config.add_position_type("current", "current balance")
-       interest_accrued = config.add_position_type("accrued", "interest accrued")
-       withholding = config.add_position_type("withholding", "withholding tax")
-
-       deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
-
-       interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
-       interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
-
-       capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
-           TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
-
-       withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
-           TransactionOperation.CREDIT, withholding)
-
-       savings_account = config.add_account_type("savingsAccount", "Savings Account")
-
-       savings_account.add_transaction_type(deposit)
-       savings_account.add_transaction_type(interest_accrued_tt)
-       savings_account.add_transaction_type(capitalized)
-       savings_account.add_transaction_type(withholding_txn)
-
-       accrual_schedule = ScheduleType("accrual", "Accrual Schedule", ScheduleFrequency.DAILY, ScheduleEndType.NO_END,
-                                       BusinessDayAdjustment.NO_ADJUSTMENT, "1", "account.start_date")
-
-       savings_account.add_schedule_type(accrual_schedule)
-
-       compounding_schedule = ScheduleType("compounding", "Compounding Schedule", ScheduleFrequency.MONTHLY,
-                                           ScheduleEndType.NO_END, BusinessDayAdjustment.NO_ADJUSTMENT, "1",
-                                           "account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
-
-       savings_account.add_schedule_type(compounding_schedule)
-
-       savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                 interest_accrued_tt,
-                                                 "account.current * config.interest.get_rate(account.current) / Decimal(365)")
-
-       savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                 capitalized, "account.accrued")
+    def create_savings_account() -> Configuration:
+        config: Configuration = Configuration(version="v1")
+    
+        current = config.add_position_type("current", "current balance")
+        interest_accrued = config.add_position_type("accrued", "interest accrued")
+        withholding = config.add_position_type("withholding", "withholding tax")
+    
+        deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
+    
+        interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
+        interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+    
+        capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
+            TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+    
+        withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
+            TransactionOperation.CREDIT, withholding)
+    
+        savings_account = config.add_account_type("savingsAccount", "Savings Account")
+    
+        savings_account.add_transaction_type(deposit)
+        savings_account.add_transaction_type(interest_accrued_tt)
+        savings_account.add_transaction_type(capitalized)
+        savings_account.add_transaction_type(withholding_txn)
+    
+        accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+                                        end_type=ScheduleEndType.NO_END,
+                                        business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                        interval_expression="1", start_date_expression="account.start_date")
+    
+        savings_account.add_schedule_type(accrual_schedule)
+    
+        compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule", frequency=ScheduleFrequency.MONTHLY,
+                                            end_type=ScheduleEndType.NO_END,
+                                            business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                            interval_expression="1",
+                                            start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
+    
+        savings_account.add_schedule_type(compounding_schedule)
+    
+        savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                                  interest_accrued_tt,
+                                                  "account.current * config.interest.get_rate(account.current) / Decimal(365)")
+    
+        savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                                  capitalized, "account.accrued")
+    
+        interest_rate = config.add_rate_type("interest", "Interest Rate")
+    
+        interest_rate.add_tier(Decimal(10000), Decimal(0.03))
+        interest_rate.add_tier(Decimal(100000), Decimal(0.035))
+        interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+    
+        config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
+    
+        return config
 
-       interest_rate = config.add_rate_type("interest", "Interest Rate")
 
-       interest_rate.add_tier(Decimal(10000), Decimal(0.03))
-       interest_rate.add_tier(Decimal(100000), Decimal(0.035))
-       interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+Given configuration, we can create an account:
 
-       config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
+.. code:: python
 
-       return config
+       config: Configuration = create_savings_account()
 
-Given configuration, we can create an account:
+        # account = create_account(config, "savingsAccount", date(2019, 1, 1))
+        account_type = config.get_account_type("savingsAccount")
+        account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
+                          config_version= config.version, config=config)
 
-.. code:: python
+        valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
 
+        deposit_transaction_type = config.get_transaction_type("deposit")
 
-       config: Configuration = create_savings_account()
+        external_transactions = group_by_date([
+            ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
+                                amount= Decimal(1000), value_date=date(2019, 1, 1))])
 
-       account_type = config.get_account_type("savingsAccount")
-       
-       # account will start on 1st of January 2019
-       account = Account(date(2019, 1, 1), account_type, config)
-       
-       # we will create account valuation on 1st of January 2020 (action date)
-       valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
-       
-       deposit_transaction_type = config.get_transaction_type("deposit")
-       
-       # we will deposit 1000 on 1st of January 2019 (backdated transaction so that we can test accruals)
-       external_transactions = group_by_date([
-           ExternalTransaction(deposit_transaction_type.name, Decimal(1000), date(2019, 1, 1))])
-       
-       # we will forecast balances and transactions as of 1st of January 2020
-       valuation.forecast(date(2020, 1, 1), external_transactions)
-       
-       self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-       self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
-    
-    ''',
-    author='Igor Music',
-    author_email='igormusich@gmail.com',
-    packages=find_packages(),
-    license='MIT',
-    url='https://github.com/igormusic/transaction-accounts',
-    download_url='https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.3.tar.gz',
-    keywords=['TRANSACTION PROCESSING', 'LOANS', 'SAVINGS', 'ACCOUNTS', 'FINANCE', 'BANKING'],
-    install_requires=[
-        'python-dateutil',
-        'dataclasses-json'
-    ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',  # Define that your audience are developers
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.9',
+        valuation.forecast(date(2020, 1, 1), external_transactions)
 
-    ],
-)
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
+    
+
```

### Comparing `transaction-accounts-0.0.3/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.0.4/transaction_accounts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
+Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
-Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.3.tar.gz
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
 
@@ -23,30 +22,34 @@
 This library provides basic functionality for working with transaction
 accounts.
 
 You can use it to make any type of transaction account, such as a
 savings account, a credit card, or a loan.
 
 Assume we would like to create simple Savings Account that has 3 types
-of balances: 
+of balances:
+ 
 - current balance 
 - interest accrued 
 - withholding tax
 
 We would like to have 4 types of transactions: 
+
 - deposit 
 - interest accrued 
 - interest capitalized 
 - withholding tax
 
 We would like to have 2 types of schedules: 
+
 - accrual schedule 
 - compounding schedule
 
 We would like to have interest rate with 3 tiers: 
+
 - 0 - 10000: 3% 
 - 10000 - 50000: 3.5% 
 - 50000+: 4%
 
 Deposit transaction will increase current balance, and it will be used
 to deposit money to the account. This transaction will be externally
 created and posted to the account.
@@ -80,89 +83,90 @@
 variables: - account: Account - transaction: Transaction - config:
 Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
-   def create_savings_account() -> Configuration:
-       config: Configuration = Configuration("v1")
-
-       current = config.add_position_type("current", "current balance")
-       interest_accrued = config.add_position_type("accrued", "interest accrued")
-       withholding = config.add_position_type("withholding", "withholding tax")
-
-       deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
-
-       interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
-       interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
-
-       capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
-           TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
-
-       withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
-           TransactionOperation.CREDIT, withholding)
-
-       savings_account = config.add_account_type("savingsAccount", "Savings Account")
-
-       savings_account.add_transaction_type(deposit)
-       savings_account.add_transaction_type(interest_accrued_tt)
-       savings_account.add_transaction_type(capitalized)
-       savings_account.add_transaction_type(withholding_txn)
-
-       accrual_schedule = ScheduleType("accrual", "Accrual Schedule", ScheduleFrequency.DAILY, ScheduleEndType.NO_END,
-                                       BusinessDayAdjustment.NO_ADJUSTMENT, "1", "account.start_date")
-
-       savings_account.add_schedule_type(accrual_schedule)
-
-       compounding_schedule = ScheduleType("compounding", "Compounding Schedule", ScheduleFrequency.MONTHLY,
-                                           ScheduleEndType.NO_END, BusinessDayAdjustment.NO_ADJUSTMENT, "1",
-                                           "account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
-
-       savings_account.add_schedule_type(compounding_schedule)
-
-       savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                 interest_accrued_tt,
-                                                 "account.current * config.interest.get_rate(account.current) / Decimal(365)")
+    def create_savings_account() -> Configuration:
+        config: Configuration = Configuration(version="v1")
+    
+        current = config.add_position_type("current", "current balance")
+        interest_accrued = config.add_position_type("accrued", "interest accrued")
+        withholding = config.add_position_type("withholding", "withholding tax")
+    
+        deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
+    
+        interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
+        interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+    
+        capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
+            TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+    
+        withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
+            TransactionOperation.CREDIT, withholding)
+    
+        savings_account = config.add_account_type("savingsAccount", "Savings Account")
+    
+        savings_account.add_transaction_type(deposit)
+        savings_account.add_transaction_type(interest_accrued_tt)
+        savings_account.add_transaction_type(capitalized)
+        savings_account.add_transaction_type(withholding_txn)
+    
+        accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+                                        end_type=ScheduleEndType.NO_END,
+                                        business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                        interval_expression="1", start_date_expression="account.start_date")
+    
+        savings_account.add_schedule_type(accrual_schedule)
+    
+        compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule", frequency=ScheduleFrequency.MONTHLY,
+                                            end_type=ScheduleEndType.NO_END,
+                                            business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                            interval_expression="1",
+                                            start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
+    
+        savings_account.add_schedule_type(compounding_schedule)
+    
+        savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                                  interest_accrued_tt,
+                                                  "account.current * config.interest.get_rate(account.current) / Decimal(365)")
+    
+        savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                                  capitalized, "account.accrued")
+    
+        interest_rate = config.add_rate_type("interest", "Interest Rate")
+    
+        interest_rate.add_tier(Decimal(10000), Decimal(0.03))
+        interest_rate.add_tier(Decimal(100000), Decimal(0.035))
+        interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+    
+        config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
+    
+        return config
 
-       savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                 capitalized, "account.accrued")
 
-       interest_rate = config.add_rate_type("interest", "Interest Rate")
+Given configuration, we can create an account:
 
-       interest_rate.add_tier(Decimal(10000), Decimal(0.03))
-       interest_rate.add_tier(Decimal(100000), Decimal(0.035))
-       interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+.. code:: python
 
-       config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
+       config: Configuration = create_savings_account()
 
-       return config
+        # account = create_account(config, "savingsAccount", date(2019, 1, 1))
+        account_type = config.get_account_type("savingsAccount")
+        account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
+                          config_version= config.version, config=config)
 
-Given configuration, we can create an account:
+        valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
 
-.. code:: python
+        deposit_transaction_type = config.get_transaction_type("deposit")
 
+        external_transactions = group_by_date([
+            ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
+                                amount= Decimal(1000), value_date=date(2019, 1, 1))])
 
-       config: Configuration = create_savings_account()
+        valuation.forecast(date(2020, 1, 1), external_transactions)
 
-       account_type = config.get_account_type("savingsAccount")
-       
-       # account will start on 1st of January 2019
-       account = Account(date(2019, 1, 1), account_type, config)
-       
-       # we will create account valuation on 1st of January 2020 (action date)
-       valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
-       
-       deposit_transaction_type = config.get_transaction_type("deposit")
-       
-       # we will deposit 1000 on 1st of January 2019 (backdated transaction so that we can test accruals)
-       external_transactions = group_by_date([
-           ExternalTransaction(deposit_transaction_type.name, Decimal(1000), date(2019, 1, 1))])
-       
-       # we will forecast balances and transactions as of 1st of January 2020
-       valuation.forecast(date(2020, 1, 1), external_transactions)
-       
-       self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-       self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
     
     
-
```

