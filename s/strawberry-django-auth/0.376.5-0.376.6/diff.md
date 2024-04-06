# Comparing `tmp/strawberry_django_auth-0.376.5.tar.gz` & `tmp/strawberry_django_auth-0.376.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_auth-0.376.5.tar", max compression
+gzip compressed data, was "strawberry_django_auth-0.376.6.tar", max compression
```

## Comparing `strawberry_django_auth-0.376.5.tar` & `strawberry_django_auth-0.376.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1075 2024-01-27 17:29:20.231302 strawberry_django_auth-0.376.5/LICENSE
--rw-r--r--   0        0        0     3820 2024-01-27 17:29:20.231302 strawberry_django_auth-0.376.5/README.md
--rw-r--r--   0        0        0       24 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/__init__.py
--rw-r--r--   0        0        0      168 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/admin.py
--rw-r--r--   0        0        0      215 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/apps.py
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/captcha/__init__.py
--rw-r--r--   0        0        0     1267 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/captcha/captcha_factorty.py
--rw-r--r--   0        0        0     6606 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/captcha/create.py
--rw-r--r--   0        0        0    16724 2024-01-27 17:29:20.271302 strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/Nehama.ttf
--rw-r--r--   0        0        0   221328 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
--rw-r--r--   0        0        0    45448 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/pltwide.ttf
--rwxr-xr-x   0        0        0    22768 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/stam.ttf
--rw-r--r--   0        0        0     3413 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/captcha/models.py
--rw-r--r--   0        0        0      549 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/captcha/types_.py
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/__init__.py
--rw-r--r--   0        0        0     1995 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/constants.py
--rw-r--r--   0        0        0      910 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/directives.py
--rw-r--r--   0        0        0     1093 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/exceptions.py
--rw-r--r--   0        0        0      231 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/interfaces.py
--rw-r--r--   0        0        0     3972 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/middlewares.py
--rw-r--r--   0        0        0     1453 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/mixins.py
--rw-r--r--   0        0        0     1516 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/scalars.py
--rw-r--r--   0        0        0      857 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/types_.py
--rw-r--r--   0        0        0     4062 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/core/utils.py
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/jwt/__init__.py
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/jwt/tools.py
--rw-r--r--   0        0        0     7646 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/jwt/types_.py
--rw-r--r--   0        0        0     2969 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/migrations/0001_initial.py
--rw-r--r--   0        0        0      355 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/migrations/0002_alter_userstatus_options.py
--rw-r--r--   0        0        0      301 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/migrations/0003_delete_captcha.py
--rw-r--r--   0        0        0     1062 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/migrations/0004_captcha.py
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/migrations/__init__.py
--rw-r--r--   0        0        0     7328 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/models.py
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/py.typed
--rw-r--r--   0        0        0      649 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/settings.py
--rw-r--r--   0        0        0     9870 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/settings_type.py
--rw-r--r--   0        0        0      171 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/templates/email/activation_email.html
--rw-r--r--   0        0        0       41 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/templates/email/activation_subject.txt
--rw-r--r--   0        0        0   176202 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
--rw-r--r--   0        0        0   100933 2024-01-27 17:29:20.275302 strawberry_django_auth-0.376.5/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
--rw-r--r--   0        0        0      162 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/templates/email/password_reset_email.html
--rw-r--r--   0        0        0       39 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/templates/email/password_reset_subject.txt
--rw-r--r--   0        0        0      160 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/templates/email/password_set_email.html
--rw-r--r--   0        0        0       37 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/templates/email/password_set_subject.txt
--rw-r--r--   0        0        0        0 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/__init__.py
--rw-r--r--   0        0        0     2177 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/arg_mutations.py
--rw-r--r--   0        0        0     1628 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/forms.py
--rw-r--r--   0        0        0     1281 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/helpers.py
--rw-r--r--   0        0        0     1111 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/queries.py
--rw-r--r--   0        0        0     2277 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/relay.py
--rw-r--r--   0        0        0    19506 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/resolvers.py
--rw-r--r--   0        0        0      450 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/signals.py
--rw-r--r--   0        0        0     2005 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/types_.py
--rw-r--r--   0        0        0      119 2024-01-27 17:29:20.279302 strawberry_django_auth-0.376.5/gqlauth/user/views.py
--rw-r--r--   0        0        0     3352 2024-01-27 17:29:34.447282 strawberry_django_auth-0.376.5/pyproject.toml
--rw-r--r--   0        0        0     5260 1970-01-01 00:00:00.000000 strawberry_django_auth-0.376.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-28 22:45:33.537304 strawberry_django_auth-0.376.6/LICENSE
+-rw-r--r--   0        0        0     3820 2024-03-28 22:45:33.537304 strawberry_django_auth-0.376.6/README.md
+-rw-r--r--   0        0        0       24 2024-03-28 22:45:33.577304 strawberry_django_auth-0.376.6/gqlauth/__init__.py
+-rw-r--r--   0        0        0      168 2024-03-28 22:45:33.577304 strawberry_django_auth-0.376.6/gqlauth/admin.py
+-rw-r--r--   0        0        0      215 2024-03-28 22:45:33.577304 strawberry_django_auth-0.376.6/gqlauth/apps.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.577304 strawberry_django_auth-0.376.6/gqlauth/captcha/__init__.py
+-rw-r--r--   0        0        0     1267 2024-03-28 22:45:33.577304 strawberry_django_auth-0.376.6/gqlauth/captcha/captcha_factorty.py
+-rw-r--r--   0        0        0     6606 2024-03-28 22:45:33.577304 strawberry_django_auth-0.376.6/gqlauth/captcha/create.py
+-rw-r--r--   0        0        0    16724 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/Nehama.ttf
+-rw-r--r--   0        0        0   221328 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
+-rw-r--r--   0        0        0    45448 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/pltwide.ttf
+-rwxr-xr-x   0        0        0    22768 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/stam.ttf
+-rw-r--r--   0        0        0     3488 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/captcha/models.py
+-rw-r--r--   0        0        0      549 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/captcha/types_.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/__init__.py
+-rw-r--r--   0        0        0     1995 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/constants.py
+-rw-r--r--   0        0        0     1134 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/directives.py
+-rw-r--r--   0        0        0     1093 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/exceptions.py
+-rw-r--r--   0        0        0      231 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/interfaces.py
+-rw-r--r--   0        0        0     3972 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/middlewares.py
+-rw-r--r--   0        0        0     1453 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/mixins.py
+-rw-r--r--   0        0        0     1516 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/scalars.py
+-rw-r--r--   0        0        0      857 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/types_.py
+-rw-r--r--   0        0        0     4128 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/core/utils.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/jwt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/jwt/tools.py
+-rw-r--r--   0        0        0     7646 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/jwt/types_.py
+-rw-r--r--   0        0        0     2969 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0      355 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/migrations/0002_alter_userstatus_options.py
+-rw-r--r--   0        0        0      301 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/migrations/0003_delete_captcha.py
+-rw-r--r--   0        0        0     1062 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/migrations/0004_captcha.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/migrations/__init__.py
+-rw-r--r--   0        0        0     7328 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/models.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/py.typed
+-rw-r--r--   0        0        0      649 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/settings.py
+-rw-r--r--   0        0        0     9870 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/settings_type.py
+-rw-r--r--   0        0        0      171 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/templates/email/activation_email.html
+-rw-r--r--   0        0        0       41 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/templates/email/activation_subject.txt
+-rw-r--r--   0        0        0   176202 2024-03-28 22:45:33.581304 strawberry_django_auth-0.376.6/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
+-rw-r--r--   0        0        0   100933 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
+-rw-r--r--   0        0        0      162 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/templates/email/password_reset_email.html
+-rw-r--r--   0        0        0       39 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/templates/email/password_reset_subject.txt
+-rw-r--r--   0        0        0      160 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/templates/email/password_set_email.html
+-rw-r--r--   0        0        0       37 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/templates/email/password_set_subject.txt
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/__init__.py
+-rw-r--r--   0        0        0     2177 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/arg_mutations.py
+-rw-r--r--   0        0        0     1628 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/forms.py
+-rw-r--r--   0        0        0     1281 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/helpers.py
+-rw-r--r--   0        0        0     1111 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/queries.py
+-rw-r--r--   0        0        0     2277 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/relay.py
+-rw-r--r--   0        0        0    19498 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/resolvers.py
+-rw-r--r--   0        0        0      450 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/signals.py
+-rw-r--r--   0        0        0     2005 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/types_.py
+-rw-r--r--   0        0        0      119 2024-03-28 22:45:33.585305 strawberry_django_auth-0.376.6/gqlauth/user/views.py
+-rw-r--r--   0        0        0     3218 2024-03-28 22:45:48.373351 strawberry_django_auth-0.376.6/pyproject.toml
+-rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 strawberry_django_auth-0.376.6/PKG-INFO
```

### Comparing `strawberry_django_auth-0.376.5/LICENSE` & `strawberry_django_auth-0.376.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/README.md` & `strawberry_django_auth-0.376.6/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/captcha_factorty.py` & `strawberry_django_auth-0.376.6/gqlauth/captcha/captcha_factorty.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/create.py` & `strawberry_django_auth-0.376.6/gqlauth/captcha/create.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/Nehama.ttf` & `strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/Nehama.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/OpenSans-Semibold.ttf` & `strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/OpenSans-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/pltwide.ttf` & `strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/pltwide.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/fonts/stam.ttf` & `strawberry_django_auth-0.376.6/gqlauth/captcha/fonts/stam.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/models.py` & `strawberry_django_auth-0.376.6/gqlauth/captcha/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib.util
 import io
 import uuid
 
 from django.db import models
 from django.utils import timezone
 
@@ -16,14 +18,17 @@
 
 class Captcha(models.Model):
     instance: CaptchaInstanceType
     uuid = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     text = models.CharField(max_length=50, editable=False)
     insert_time = models.DateTimeField(auto_now_add=True, editable=False)
     tries = models.IntegerField(default=0)
+
+    objects: models.Manager[Captcha]
+
     if PILLOW_INSTALLED:
         image = models.ImageField(
             blank=False,
             null=False,
             upload_to="captcha/%Y/%m/%d/",
             editable=False,
             help_text="url for the captcha image",
```

### Comparing `strawberry_django_auth-0.376.5/gqlauth/captcha/types_.py` & `strawberry_django_auth-0.376.6/gqlauth/captcha/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/constants.py` & `strawberry_django_auth-0.376.6/gqlauth/core/constants.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/directives.py` & `strawberry_django_auth-0.376.6/gqlauth/core/directives.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+from __future__ import annotations
+
 import dataclasses
-from typing import Any, Callable, final
+from typing import Any, Callable, cast, final
 
 import strawberry
+from graphql.pyutils import AwaitableOrValue
 from strawberry.schema_directive import Location
 from strawberry.types import Info
 from strawberry_django.permissions import DjangoNoPermission, DjangoPermissionExtension
+from strawberry_django.utils.typing import UserType
+from typing_extensions import override
 
 from gqlauth.core.utils import UserProto
 
 
 @strawberry.schema_directive(
     locations=[Location.FIELD_DEFINITION],
     description="Checks whether a user is verified",
 )
 @final
 class IsVerified(DjangoPermissionExtension):
     """Mark a field as only resolvable by authenticated users."""
 
     message: strawberry.Private[str] = dataclasses.field(default="User is not authenticated.")
 
+    @override
     def resolve_for_user(
-        self,
-        resolver: Callable,
-        user: UserProto,
-        *,
-        info: Info,
-        source: Any,
-    ):
+        self, resolver: Callable[..., Any], user: UserType | None, *, info: Info, source: Any
+    ) -> AwaitableOrValue:
+        user = cast(UserProto, user)
         if user.is_authenticated and user.status.verified:
             return resolver()
         raise DjangoNoPermission
```

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/exceptions.py` & `strawberry_django_auth-0.376.6/gqlauth/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/middlewares.py` & `strawberry_django_auth-0.376.6/gqlauth/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/mixins.py` & `strawberry_django_auth-0.376.6/gqlauth/core/mixins.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/scalars.py` & `strawberry_django_auth-0.376.6/gqlauth/core/scalars.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/types_.py` & `strawberry_django_auth-0.376.6/gqlauth/core/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/core/utils.py` & `strawberry_django_auth-0.376.6/gqlauth/core/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 from django.core import signing
 from strawberry.field import StrawberryField
 from strawberry.types import Info
 from strawberry.utils.str_converters import to_camel_case
 
 from gqlauth.core.exceptions import TokenScopeError
 
+# Without this it would cause django to complain about import ordering.
 if typing.TYPE_CHECKING:  # pragma: no cover
     from gqlauth.models import UserStatus
     from gqlauth.settings_type import GqlAuthSettings
 
     class UserProto(AbstractBaseUser):
         status: UserStatus
 
-
-UserProto: "UserProto" = "UserProto"  # type: ignore  # noqa: F811
+else:
+    UserProto = "Foobar to allow import me in runtime."
 
 USER_MODEL = get_user_model()
 USER_UNION = typing.Union["UserProto", AnonymousUser, AbstractBaseUser]
 app_settings: "GqlAuthSettings" = settings.GQL_AUTH
 
 
 def hide_args_kwargs(field):
```

### Comparing `strawberry_django_auth-0.376.5/gqlauth/jwt/types_.py` & `strawberry_django_auth-0.376.6/gqlauth/jwt/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/migrations/0001_initial.py` & `strawberry_django_auth-0.376.6/gqlauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/migrations/0004_captcha.py` & `strawberry_django_auth-0.376.6/gqlauth/migrations/0004_captcha.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/models.py` & `strawberry_django_auth-0.376.6/gqlauth/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/settings.py` & `strawberry_django_auth-0.376.6/gqlauth/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/settings_type.py` & `strawberry_django_auth-0.376.6/gqlauth/settings_type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg` & `strawberry_django_auth-0.376.6/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg` & `strawberry_django_auth-0.376.6/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/arg_mutations.py` & `strawberry_django_auth-0.376.6/gqlauth/user/arg_mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/forms.py` & `strawberry_django_auth-0.376.6/gqlauth/user/forms.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/helpers.py` & `strawberry_django_auth-0.376.6/gqlauth/user/helpers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/queries.py` & `strawberry_django_auth-0.376.6/gqlauth/user/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/relay.py` & `strawberry_django_auth-0.376.6/gqlauth/user/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/resolvers.py` & `strawberry_django_auth-0.376.6/gqlauth/user/resolvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,16 +456,15 @@
     """Update user model fields, defined on settings.
 
     User must be verified.
     """
 
     @strawberry.input
     @inject_fields(app_settings.UPDATE_MUTATION_FIELDS)
-    class UpdateAccountInput:
-        ...
+    class UpdateAccountInput: ...
 
     form = UpdateAccountForm
     REQUIRE_VERIFICATION = True
 
     @classmethod
     def resolve_mutation(cls, info, input_: UpdateAccountInput) -> MutationNormalOutput:
         user = get_user(info)
```

### Comparing `strawberry_django_auth-0.376.5/gqlauth/user/types_.py` & `strawberry_django_auth-0.376.6/gqlauth/user/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.376.5/pyproject.toml` & `strawberry_django_auth-0.376.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 [tool.poetry]
 name = "strawberry-django-auth"
-version = "0.376.5"
+version = "0.376.6"
 description = "Graphql authentication system with Strawberry for Django."
 license = "MIT"
 authors = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 readme = "README.md"
 classifiers = [
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Framework :: Django',
-    'Framework :: Django :: 3.2',
-    'Framework :: Django :: 4.1',
-    'Framework :: Django :: 4.2',
-    'Framework :: Django :: 5.0',
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 packages = [{ include = "gqlauth" }]
@@ -36,15 +32,15 @@
 captcha = ["pillow"]
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 coverage = "^7.2"
 pytest = "^7.2"
-pytest-cov = "^4.0"
+pytest-cov = ">=4,<6"
 types-cryptography = "^3.3.23"
 django-mock-queries = "^2.1.7"
 types-mock = "^5.0.0"
 types-jwt = "^0.1.0"
 types-pkg-resources = "^0.1.0"
 mkdocs = ">=1.3.0"
 mkdocs-markdownextradata-plugin = ">=0.2.5"
```

### Comparing `strawberry_django_auth-0.376.5/PKG-INFO` & `strawberry_django_auth-0.376.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: strawberry-django-auth
-Version: 0.376.5
+Version: 0.376.6
 Summary: Graphql authentication system with Strawberry for Django.
 License: MIT
 Author: Nir.J Benlulu
 Author-email: nrbnlulu@gmail.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

