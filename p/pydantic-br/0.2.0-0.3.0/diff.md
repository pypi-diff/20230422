# Comparing `tmp/pydantic_br-0.2.0.tar.gz` & `tmp/pydantic_br-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_br-0.2.0.tar", max compression
+gzip compressed data, was "pydantic_br-0.3.0.tar", max compression
```

## Comparing `pydantic_br-0.2.0.tar` & `pydantic_br-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1090 2023-03-27 13:26:17.201060 pydantic_br-0.2.0/LICENSE
--rw-r--r--   0        0        0      364 2023-04-06 02:17:02.183549 pydantic_br-0.2.0/pydantic_br/__init__.py
--rw-r--r--   0        0        0      718 2023-04-01 15:44:31.545140 pydantic_br-0.2.0/pydantic_br/field_erros.py
--rw-r--r--   0        0        0     1267 2023-04-05 01:51:03.317952 pydantic_br-0.2.0/pydantic_br/fields/cnh_field.py
--rw-r--r--   0        0        0     2322 2023-04-05 01:51:03.317952 pydantic_br-0.2.0/pydantic_br/fields/cnpj_field.py
--rw-r--r--   0        0        0     2196 2023-04-04 02:11:01.668037 pydantic_br-0.2.0/pydantic_br/fields/cpf_field.py
--rw-r--r--   0        0        0     1213 2023-04-06 02:14:03.591570 pydantic_br-0.2.0/pydantic_br/fields/te_field.py
--rw-r--r--   0        0        0     1204 2023-04-05 01:51:03.318953 pydantic_br-0.2.0/pydantic_br/validators/cnh_validator.py
--rw-r--r--   0        0        0     1586 2023-04-04 03:12:14.745595 pydantic_br-0.2.0/pydantic_br/validators/cnpj_validator.py
--rw-r--r--   0        0        0     1195 2023-04-04 02:34:51.015838 pydantic_br-0.2.0/pydantic_br/validators/cpf_validator.py
--rw-r--r--   0        0        0     1883 2023-04-06 02:39:58.028378 pydantic_br-0.2.0/pydantic_br/validators/te_validator.py
--rw-r--r--   0        0        0     1740 2023-04-06 02:44:56.299138 pydantic_br-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3965 2023-04-06 02:19:38.210322 pydantic_br-0.2.0/README.md
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 pydantic_br-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-03-27 13:26:17.201060 pydantic_br-0.3.0/LICENSE
+-rw-r--r--   0        0        0      452 2023-04-22 02:05:24.594119 pydantic_br-0.3.0/pydantic_br/__init__.py
+-rw-r--r--   0        0        0      718 2023-04-01 15:44:31.545140 pydantic_br-0.3.0/pydantic_br/field_erros.py
+-rw-r--r--   0        0        0     1970 2023-04-22 02:48:54.995154 pydantic_br-0.3.0/pydantic_br/fields/base_field.py
+-rw-r--r--   0        0        0      307 2023-04-22 02:55:17.245254 pydantic_br-0.3.0/pydantic_br/fields/cnh_field.py
+-rw-r--r--   0        0        0      786 2023-04-22 02:55:17.245254 pydantic_br-0.3.0/pydantic_br/fields/cnpj_field.py
+-rw-r--r--   0        0        0      778 2023-04-22 02:55:17.245254 pydantic_br-0.3.0/pydantic_br/fields/cpf_field.py
+-rw-r--r--   0        0        0      733 2023-04-22 02:28:55.870250 pydantic_br-0.3.0/pydantic_br/fields/pis_field.py
+-rw-r--r--   0        0        0      308 2023-04-22 02:55:17.246262 pydantic_br-0.3.0/pydantic_br/fields/te_field.py
+-rw-r--r--   0        0        0      226 2023-04-22 02:40:51.452781 pydantic_br-0.3.0/pydantic_br/validators/base_validator.py
+-rw-r--r--   0        0        0     1266 2023-04-22 02:55:17.246262 pydantic_br-0.3.0/pydantic_br/validators/cnh_validator.py
+-rw-r--r--   0        0        0     1715 2023-04-22 02:55:17.246262 pydantic_br-0.3.0/pydantic_br/validators/cnpj_validator.py
+-rw-r--r--   0        0        0     1318 2023-04-22 02:55:17.247269 pydantic_br-0.3.0/pydantic_br/validators/cpf_validator.py
+-rw-r--r--   0        0        0     1151 2023-04-22 02:49:26.506208 pydantic_br-0.3.0/pydantic_br/validators/pis_validator.py
+-rw-r--r--   0        0        0     1945 2023-04-22 02:55:17.247269 pydantic_br-0.3.0/pydantic_br/validators/te_validator.py
+-rw-r--r--   0        0        0     1740 2023-04-22 02:01:05.454342 pydantic_br-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3957 2023-04-22 01:45:04.888335 pydantic_br-0.3.0/README.md
+-rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 pydantic_br-0.3.0/PKG-INFO
```

### Comparing `pydantic_br-0.2.0/LICENSE` & `pydantic_br-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.2.0/pydantic_br/field_erros.py` & `pydantic_br-0.3.0/pydantic_br/field_erros.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.2.0/pydantic_br/fields/cnh_field.py` & `pydantic_br-0.3.0/pydantic_br/fields/base_field.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,81 @@
-from typing import Any, Callable, Dict, Generator
-
-from ..field_erros import FieldDigitError, FieldInvalidError, FieldTypeError
-from ..validators.cnh_validator import CNHValidator
-
-__all__ = ["CNH"]
-
-
-AnyCallable = Callable[..., Any]
-CallableGenerator = Generator[AnyCallable, None, None]
-
-
-class CNH(str):
-    __slots__ = ["number"]
-
-    def __init__(self, number: str) -> None:
-        self.number = number
-
-    @classmethod
-    def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
-        field_schema.update(type="string", format="cnh")
-
-    @classmethod
-    def __get_validators__(cls) -> CallableGenerator:
-        yield cls.validate_type
-        yield cls.validate_numbers
-        yield cls.validate
-
-    @classmethod
-    def validate_type(cls, value: str) -> str:
-        if not isinstance(value, str):
-            raise FieldTypeError()
-        return value
-
-    @classmethod
-    def validate_numbers(cls, value: str) -> str:
-        if not value.isdigit():
-            raise FieldDigitError()
-        return value
-
-    @classmethod
-    def validate(cls, value: str) -> str:
-        cnh = CNHValidator(value)
-        if not cnh.validate():
-            raise FieldInvalidError()
-        return value
+from typing import Any, Callable, Dict, Generator
+
+from ..field_erros import (
+    FieldDigitError,
+    FieldInvalidError,
+    FieldMaskError,
+    FieldTypeError,
+)
+from ..validators.base_validator import FieldMaskValidator, FieldValidator
+
+__all__ = [
+    "Base",
+    "BaseMask",
+    "BaseDigits",
+]
+
+AnyCallable = Callable[..., Any]
+CallableGenerator = Generator[AnyCallable, None, None]
+
+
+class Base:
+    format: str
+    Validator: Callable[..., FieldValidator]
+
+    __slots__ = ["number"]
+
+    def __init__(self, number: str) -> None:
+        self.number = number
+
+    @classmethod
+    def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
+        field_schema.update(type="string", format=cls.format)
+
+    @classmethod
+    def __get_validators__(cls) -> CallableGenerator:
+        yield cls.validate_type
+        yield cls.validate
+
+    @classmethod
+    def validate_type(cls, value: str) -> str:
+        if not isinstance(value, str):
+            raise FieldTypeError()
+        return value
+
+    @classmethod
+    def validate(cls, value: str) -> str:
+        doc = cls.Validator(value)
+        if not doc.validate():
+            raise FieldInvalidError()
+        return value
+
+
+class BaseMask(Base):
+    Validator: Callable[..., FieldMaskValidator]
+
+    @classmethod
+    def __get_validators__(cls) -> CallableGenerator:
+        yield cls.validate_type
+        yield cls.validate_mask
+        yield cls.validate
+
+    @classmethod
+    def validate_mask(cls, value: str) -> str:
+        doc = cls.Validator(value)
+        if not doc.validate_mask():
+            raise FieldMaskError()
+        return value
+
+
+class BaseDigits(Base):
+    @classmethod
+    def __get_validators__(cls) -> CallableGenerator:
+        yield cls.validate_type
+        yield cls.validate_numbers
+        yield cls.validate
+
+    @classmethod
+    def validate_numbers(cls, value: str) -> str:
+        if not value.isdigit():
+            raise FieldDigitError()
+        return value
```

### Comparing `pydantic_br-0.2.0/pydantic_br/validators/cnh_validator.py` & `pydantic_br-0.3.0/pydantic_br/validators/cnh_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 
+from .base_validator import FieldValidator
+
 __all__ = ["CNHValidator"]
 
 
-class CNHValidator:
+class CNHValidator(FieldValidator):
     def __init__(self, cnh: str) -> None:
         self.cnh = cnh
 
     def validate(self) -> bool:
         cnh = re.sub("[^0-9]", "", str(self.cnh))
 
         if len(set(cnh)) == 1:
```

### Comparing `pydantic_br-0.2.0/pydantic_br/validators/cnpj_validator.py` & `pydantic_br-0.3.0/pydantic_br/validators/cnpj_validator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-import re
-
-__all__ = ["CNPJValidator"]
-
-
-class CNPJValidator:
-    def __init__(self, cnpj) -> None:
-        self.cnpj = cnpj
-
-    def validate_mask(self) -> bool:
-        if len(self.cnpj) == 18:
-            if (
-                self.cnpj[2:3] == "."
-                and self.cnpj[6:7] == "."
-                and self.cnpj[10:11] == "/"
-                and self.cnpj[15:16] == "-"
-            ):
-                return True
-        return False
-
-    def validate(self) -> bool:
-        cnpj = re.sub("[^0-9]", "", self.cnpj)
-
-        if len(cnpj) != 14:
-            return False
-        first_digit = self._validate_first_digit(cnpj)
-        second_digit = self._validate_second_digit(cnpj)
-        return cnpj[12] == first_digit and cnpj[13] == second_digit
-
-    def _validate_first_digit(self, cnpj) -> str:
-        sum = 0
-        weight = [5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
-
-        """ Valida o primeiro digito """
-        for n in range(12):
-            value = int(cnpj[n]) * weight[n]
-            sum = sum + value
-
-        check_digit = sum % 11
-
-        if check_digit < 2:
-            first_digit = 0
-        else:
-            first_digit = 11 - check_digit
-        return str(first_digit)
-
-    def _validate_second_digit(self, cnpj) -> str:
-        sum = 0
-        weight = [6, 5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
-        for n in range(13):
-            sum = sum + int(cnpj[n]) * weight[n]
-
-        check_digit = sum % 11
-
-        if check_digit < 2:
-            second_digit = 0
-        else:
-            second_digit = 11 - check_digit
-        return str(second_digit)
+import re
+
+from .base_validator import FieldMaskValidator
+
+__all__ = ["CNPJValidator"]
+
+
+class CNPJValidator(FieldMaskValidator):
+    def __init__(self, cnpj) -> None:
+        self.cnpj = cnpj
+
+    def validate_mask(self) -> bool:
+        if len(self.cnpj) == 18:
+            if (
+                self.cnpj[2:3] == "."
+                and self.cnpj[6:7] == "."
+                and self.cnpj[10:11] == "/"
+                and self.cnpj[15:16] == "-"
+            ):
+                return True
+        return False
+
+    def validate(self) -> bool:
+        cnpj = re.sub("[^0-9]", "", self.cnpj)
+
+        if len(cnpj) != 14:
+            return False
+        first_digit = self._validate_first_digit(cnpj)
+        second_digit = self._validate_second_digit(cnpj)
+        return cnpj[12] == first_digit and cnpj[13] == second_digit
+
+    def _validate_first_digit(self, cnpj) -> str:
+        sum = 0
+        weight = [5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
+
+        """ Valida o primeiro digito """
+        for n in range(12):
+            value = int(cnpj[n]) * weight[n]
+            sum = sum + value
+
+        check_digit = sum % 11
+
+        if check_digit < 2:
+            first_digit = 0
+        else:
+            first_digit = 11 - check_digit
+        return str(first_digit)
+
+    def _validate_second_digit(self, cnpj) -> str:
+        sum = 0
+        weight = [6, 5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
+        for n in range(13):
+            sum = sum + int(cnpj[n]) * weight[n]
+
+        check_digit = sum % 11
+
+        if check_digit < 2:
+            second_digit = 0
+        else:
+            second_digit = 11 - check_digit
+        return str(second_digit)
```

### Comparing `pydantic_br-0.2.0/pydantic_br/validators/te_validator.py` & `pydantic_br-0.3.0/pydantic_br/validators/te_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 from typing import List
 
+from .base_validator import FieldValidator
+
 __all__ = ["TEValidator"]
 
 
-class TEValidator:
+class TEValidator(FieldValidator):
     def __init__(self, te: str) -> None:
         self.te = te
         self.first_check_digit_weights = list(range(2, 10))
         self.second_check_digit_weights = list(range(7, 10))
         self.first_check_digit_doc_slice = slice(0, 8)
         self.second_check_digit_doc_slice = slice(8, 10)
```

### Comparing `pydantic_br-0.2.0/pyproject.toml` & `pydantic_br-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-br"
-version = "0.2.0"
+version = "0.3.0"
 description = "Pydantic library extension with Brazilian fields"
 license = "MIT"
 authors = ["Jorge Silva <jorgesilva.ti@hotmail.com>"]
 maintainers = ["Jorge Silva <jorgesilva.ti@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/scjorge/pydantic_br"
 documentation = "https://pydantic-br.readthedocs.io"
```

### Comparing `pydantic_br-0.2.0/README.md` & `pydantic_br-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 | Campo | Grupo de Documentos | Nome do Documento | Método de validação | Situação
 |---|---|---|---|---|
 | CNPJ | Pessoa Jurídica | Carteira Nacional de Pessoas Jurídicas | Digito Verificador | Concluído
 | CPF | Pessoa física | Cadastro de Pessoa Física | Digito Verificador | Concluído
 | CNH | Pessoa física | Carteira Nacional de Habilitação | Digito Verificador | Concluído
 | TE | Pessoa física  | Título de Eleitor | Digito Verificador | Concluído
-| PIS | Pessoa física  | Programa de Integração Social | Digito Verificador | Em desenvolvimento
+| PIS | Pessoa física  | Programa de Integração Social | Digito Verificador | Concluído
 | CERT | Pessoa física  | Certidão (Nascimento/Casamento/Óbito) | Digito Verificador | Em desenvolvimento
 | CNS | Pessoa física  | Cartão Nacional de Saúde | Digito Verificador | Em desenvolvimento
 | RNVAM | Veículos | Registro Nacional de Veículos Automotores | RegExr | Em desenvolvimento
 | PLACA | Veículos | Placa do Veículo | RegExr | Em desenvolvimento
 | ISBN | Livros | Padrão Internacional de Numeração de Livro | Digito Verificador | Em desenvolvimento
```

### Comparing `pydantic_br-0.2.0/PKG-INFO` & `pydantic_br-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-br
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pydantic library extension with Brazilian fields
 Home-page: https://github.com/scjorge/pydantic_br
 License: MIT
 Keywords: pydantic,json,json-schema,hints,parsin,brasil,documentos,br,fastapi,doc,documento
 Author: Jorge Silva
 Author-email: jorgesilva.ti@hotmail.com
 Maintainer: Jorge Silva
@@ -56,15 +56,15 @@
 
 | Campo | Grupo de Documentos | Nome do Documento | Método de validação | Situação
 |---|---|---|---|---|
 | CNPJ | Pessoa Jurídica | Carteira Nacional de Pessoas Jurídicas | Digito Verificador | Concluído
 | CPF | Pessoa física | Cadastro de Pessoa Física | Digito Verificador | Concluído
 | CNH | Pessoa física | Carteira Nacional de Habilitação | Digito Verificador | Concluído
 | TE | Pessoa física  | Título de Eleitor | Digito Verificador | Concluído
-| PIS | Pessoa física  | Programa de Integração Social | Digito Verificador | Em desenvolvimento
+| PIS | Pessoa física  | Programa de Integração Social | Digito Verificador | Concluído
 | CERT | Pessoa física  | Certidão (Nascimento/Casamento/Óbito) | Digito Verificador | Em desenvolvimento
 | CNS | Pessoa física  | Cartão Nacional de Saúde | Digito Verificador | Em desenvolvimento
 | RNVAM | Veículos | Registro Nacional de Veículos Automotores | RegExr | Em desenvolvimento
 | PLACA | Veículos | Placa do Veículo | RegExr | Em desenvolvimento
 | ISBN | Livros | Padrão Internacional de Numeração de Livro | Digito Verificador | Em desenvolvimento
```

