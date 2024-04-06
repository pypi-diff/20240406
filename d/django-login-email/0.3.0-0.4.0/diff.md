# Comparing `tmp/django_login_email-0.3.0.tar.gz` & `tmp/django_login_email-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_login_email-0.3.0.tar", max compression
+gzip compressed data, was "django_login_email-0.4.0.tar", max compression
```

## Comparing `django_login_email-0.3.0.tar` & `django_login_email-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.3.0/django_login_email/__init__.py
--rw-r--r--   0        0        0       66 2024-04-04 13:03:53.315517 django_login_email-0.3.0/django_login_email/admin.py
--rw-r--r--   0        0        0      172 2024-04-04 13:48:39.145418 django_login_email-0.3.0/django_login_email/apps.py
--rw-r--r--   0        0        0     3280 2024-04-05 09:03:42.714709 django_login_email-0.3.0/django_login_email/email.py
--rw-r--r--   0        0        0       48 2024-04-04 14:10:43.064298 django_login_email-0.3.0/django_login_email/errors.py
--rw-r--r--   0        0        0      148 2024-04-04 13:39:37.730372 django_login_email-0.3.0/django_login_email/forms.py
--rw-r--r--   0        0        0      651 2024-04-05 07:43:16.485657 django_login_email-0.3.0/django_login_email/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.3.0/django_login_email/migrations/__init__.py
--rw-r--r--   0        0        0      644 2024-04-05 08:49:30.577058 django_login_email-0.3.0/django_login_email/models.py
--rw-r--r--   0        0        0      262 2024-04-04 13:13:26.017612 django_login_email-0.3.0/django_login_email/templates/login_email/base.html
--rw-r--r--   0        0        0        0 2024-04-05 07:10:27.427724 django_login_email-0.3.0/django_login_email/templates/login_email/components/mail_template.html
--rw-r--r--   0        0        0      264 2024-04-04 13:28:15.565466 django_login_email-0.3.0/django_login_email/templates/login_email/error.html
--rw-r--r--   0        0        0      303 2024-04-05 02:52:27.902145 django_login_email-0.3.0/django_login_email/templates/login_email/home.html
--rw-r--r--   0        0        0      262 2024-04-04 13:14:07.688691 django_login_email-0.3.0/django_login_email/templates/login_email/login.html
--rw-r--r--   0        0        0      166 2024-04-04 13:14:54.572437 django_login_email-0.3.0/django_login_email/templates/login_email/success.html
--rw-r--r--   0        0        0        0 2024-04-05 02:35:09.498191 django_login_email-0.3.0/django_login_email/tests/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-05 09:03:29.344879 django_login_email-0.3.0/django_login_email/tests/test_mixin.py
--rw-r--r--   0        0        0      455 2024-04-05 07:41:19.183970 django_login_email-0.3.0/django_login_email/tests/test_models.py
--rw-r--r--   0        0        0       85 2024-04-05 02:38:19.911927 django_login_email-0.3.0/django_login_email/tests/test_str.py
--rw-r--r--   0        0        0      130 2024-04-05 06:52:23.110227 django_login_email-0.3.0/django_login_email/tests/test_time.py
--rw-r--r--   0        0        0       63 2024-04-04 13:03:53.315517 django_login_email-0.3.0/django_login_email/tests.py
--rw-r--r--   0        0        0     2595 2024-04-05 07:28:51.167000 django_login_email-0.3.0/django_login_email/token.py
--rw-r--r--   0        0        0     3599 2024-04-05 09:06:32.403242 django_login_email-0.3.0/django_login_email/views.py
--rw-r--r--   0        0        0     1270 2024-04-04 14:30:21.236968 django_login_email-0.3.0/LICENSE
--rw-r--r--   0        0        0      854 2024-04-05 09:08:51.152655 django_login_email-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      769 2024-04-05 09:07:23.790007 django_login_email-0.3.0/README.md
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 django_login_email-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.4.0/django_login_email/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-04 13:03:53.315517 django_login_email-0.4.0/django_login_email/admin.py
+-rw-r--r--   0        0        0      172 2024-04-04 13:48:39.145418 django_login_email-0.4.0/django_login_email/apps.py
+-rw-r--r--   0        0        0     3806 2024-04-06 03:45:19.064227 django_login_email-0.4.0/django_login_email/email.py
+-rw-r--r--   0        0        0       48 2024-04-04 14:10:43.064298 django_login_email-0.4.0/django_login_email/errors.py
+-rw-r--r--   0        0        0      148 2024-04-04 13:39:37.730372 django_login_email-0.4.0/django_login_email/forms.py
+-rw-r--r--   0        0        0      651 2024-04-05 07:43:16.485657 django_login_email-0.4.0/django_login_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0      879 2024-04-06 03:07:29.243270 django_login_email-0.4.0/django_login_email/migrations/0002_emaillogin_sault_emaillogin_validated_and_more.py
+-rw-r--r--   0        0        0      433 2024-04-06 03:28:21.041236 django_login_email-0.4.0/django_login_email/migrations/0003_rename_last_time_emaillogin_expired_time.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.4.0/django_login_email/migrations/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-06 03:23:54.678449 django_login_email-0.4.0/django_login_email/models.py
+-rw-r--r--   0        0        0      262 2024-04-04 13:13:26.017612 django_login_email-0.4.0/django_login_email/templates/login_email/base.html
+-rw-r--r--   0        0        0        0 2024-04-05 07:10:27.427724 django_login_email-0.4.0/django_login_email/templates/login_email/components/mail_template.html
+-rw-r--r--   0        0        0      264 2024-04-04 13:28:15.565466 django_login_email-0.4.0/django_login_email/templates/login_email/error.html
+-rw-r--r--   0        0        0      303 2024-04-05 02:52:27.902145 django_login_email-0.4.0/django_login_email/templates/login_email/home.html
+-rw-r--r--   0        0        0      262 2024-04-04 13:14:07.688691 django_login_email-0.4.0/django_login_email/templates/login_email/login.html
+-rw-r--r--   0        0        0      166 2024-04-04 13:14:54.572437 django_login_email-0.4.0/django_login_email/templates/login_email/success.html
+-rw-r--r--   0        0        0        0 2024-04-05 02:35:09.498191 django_login_email-0.4.0/django_login_email/tests/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-06 03:16:34.959649 django_login_email-0.4.0/django_login_email/tests/test_email.py
+-rw-r--r--   0        0        0     1279 2024-04-06 03:26:37.811811 django_login_email-0.4.0/django_login_email/tests/test_mixin.py
+-rw-r--r--   0        0        0      464 2024-04-06 03:26:46.598384 django_login_email-0.4.0/django_login_email/tests/test_models.py
+-rw-r--r--   0        0        0      130 2024-04-05 06:52:23.110227 django_login_email-0.4.0/django_login_email/tests/test_time.py
+-rw-r--r--   0        0        0     3041 2024-04-06 03:43:58.849340 django_login_email-0.4.0/django_login_email/token.py
+-rw-r--r--   0        0        0     4909 2024-04-06 04:39:02.952231 django_login_email-0.4.0/django_login_email/views.py
+-rw-r--r--   0        0        0     1270 2024-04-04 14:30:21.236968 django_login_email-0.4.0/LICENSE
+-rw-r--r--   0        0        0      875 2024-04-06 04:39:35.582503 django_login_email-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      883 2024-04-06 04:39:15.410590 django_login_email-0.4.0/README.md
+-rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 django_login_email-0.4.0/PKG-INFO
```

### Comparing `django_login_email-0.3.0/django_login_email/email.py` & `django_login_email-0.4.0/django_login_email/email.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,82 +32,95 @@
 
 class TimeLimit(object):
     minutes: int = 10
 
 
 @dataclass
 class MailRecord(object):
-    last_time: t.Optional[datetime.datetime]
+    expired_time: t.Optional[datetime.datetime]
     email: str
+    validated: bool
+    sault: str
 
 
 class MailRecordMixin(abc.ABC):
 
     @abc.abstractmethod
     def get_mail_record(self, mail: str) -> MailRecord:
         # for easy to change. use a function.
         raise NotImplementedError("You must implement get_mail_record")
 
     @abc.abstractmethod
-    def set_mail_record(self, mail: str):
-        raise NotImplementedError("You must implement set_mail_record")
+    def save_token(self, token: token.TokenDict):
+        """to save token in the database or somewhere."""
+        raise NotImplementedError("You must implement save_token")
+
+    @abc.abstractmethod
+    def disable_token(self, token: token.TokenDict):
+        """Every token should only login once"""
+        raise NotImplementedError("")
 
 
 class EmailInfoMixin(MailRecordMixin):
     email_info_class: t.Type[EmailLoginInfo]
 
     tl: TimeLimit
 
     def check_user(self, email):
         User = get_user_model()
         u = User.objects.get(email=email)
         return u
 
     def check_could_send(self, email):
         re = self.get_mail_record(email)
-        if (re.last_time is None) or (
-            re.last_time + datetime.timedelta(minutes=self.tl.minutes) <= datetime.datetime.now(tz=timezone.utc)
-        ):
+        # TODO: if other user send email, the current user could not sign in.
+        if (re.expired_time is None) or (re.expired_time <= datetime.datetime.now(tz=timezone.utc)):
             return True
         return False
 
     def send_valid(self, email: str):
         e = self.email_info_class()
         m = token.TokenManager(self.tl.minutes)
 
-        token_v = m.encrypt_mail(email)
-        e.set_token(token_v)
+        encrypt_token = m.encrypt_mail(email, self.save_token)
+        e.set_token(encrypt_token)
 
         msg = EmailMessage(e.subject, e.message, e.from_email, [email])
         msg.content_subtype = "html"
         msg.send()
 
     def send_login_mail(self, email: str):
         self.check_user(email)
         if not self.check_could_send(email=email):
             raise Exception(f"Cannot send. Wait {self.tl.minutes} minutes.")
 
         self.send_valid(email)
-        self.set_mail_record(email)
 
 
-class EmailValidateMixin(object):
+class EmailValidateMixin(MailRecordMixin):
     tl: TimeLimit
 
     def verify_login_mail(self, request, token_v: str):
         m = token.TokenManager(self.tl.minutes)
-        emailAndSalt = m.decrypt_token(token=token_v)
-        token_d = m.check_token(emailAndSalt)
+        token_str = m.decrypt_token(token=token_v)
+        token_d = m.transform_token(token_str)
+
+        mr = self.get_mail_record(m.get_mail(token_d))
+        if mr.validated:
+            raise Exception("Already validated.")
+
+        token_d = m.check_token(token_d, lambda: mr.sault)
         if token_d is None:
             raise Exception("Invalid token.")
 
         User = get_user_model()
         u = User.objects.get(email=m.get_mail(token_d))
         if not u.is_active:
             raise Exception("Inactive user, disallow login.")
 
+        self.disable_token(token=token_d)
         login(request, u)
 
 
 class EmailLogoutMixin(object):
     def logout(self, request):
         logout(request)
```

### Comparing `django_login_email-0.3.0/django_login_email/migrations/0001_initial.py` & `django_login_email-0.4.0/django_login_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_login_email-0.3.0/django_login_email/models.py` & `django_login_email-0.4.0/django_login_email/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from django.db import models
 
 # Create your models here.
 
 
 class EmailLogin(models.Model):
-    last_time = models.DateTimeField(auto_now_add=True, verbose_name="Last login request time")
+    expired_time = models.DateTimeField(auto_now_add=True, verbose_name="Last login request time")
+    validated = models.BooleanField(default=False, verbose_name="Login Token validated")
+    sault = models.CharField(max_length=100, verbose_name="Sault")
     email = models.EmailField(verbose_name="Email", unique=True, null=False)
 
     @classmethod
-    def set_email_last_time(cls, email, datetime) -> "EmailLogin":
+    def set_email_expired_time(cls, email, datetime) -> "EmailLogin":
         obj, _ = cls.objects.get_or_create(email=email)
-        obj.set_last_time(datetime)
+        obj.set_expired_time(datetime)
         return obj
 
-    def set_last_time(self, datetime):
-        self.last_time = datetime
+    def set_expired_time(self, datetime):
+        self.expired_time = datetime
+        self.validated = False
         self.save()
 
     def __str__(self) -> str:
         return f"Email: {self.email}"
```

### Comparing `django_login_email-0.3.0/django_login_email/tests/test_mixin.py` & `django_login_email-0.4.0/django_login_email/tests/test_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import pytest
 import datetime
-from django_login_email import models
 from django_login_email.email import EmailInfoMixin, MailRecord, TimeLimit
+from django_login_email.token import TokenDict
 
 
 class MyTimeLit(TimeLimit):
     minutes = 10
 
 
 class Mixin(EmailInfoMixin):
     tl = MyTimeLit()
 
     def get_mail_record(self, mail: str) -> MailRecord:
         r1 = MailRecord(
             email="svtter@163.com",
-            last_time=datetime.datetime.now(tz=datetime.timezone.utc) - datetime.timedelta(minutes=10),
+            expired_time=datetime.datetime.now(tz=datetime.timezone.utc) - datetime.timedelta(minutes=10),
+            validated=False,
+            sault="",
         )
-        # r2 = MailRecord(email="svtter@163.com", last_time=datetime.datetime.now(tz=datetime.timezone.utc))
         return r1
 
-    def set_mail_record(self, mail: str):
+    def save_token(self, token: TokenDict):
         pass
 
 
 @pytest.mark.django_db
 def test_mixin():
     mail = "svtter@163.com"
     e = Mixin()
     re = e.get_mail_record(mail)
-    assert re.last_time
-    # assert re.last_time + datetime.timedelta(minutes=10) <= datetime.datetime.now(tz=datetime.timezone.utc)
+    assert re.expired_time
     assert e.check_could_send(email=mail)
 
 
 class Mixin2(EmailInfoMixin):
     tl = MyTimeLit()
 
     def get_mail_record(self, mail: str) -> MailRecord:
-        r2 = MailRecord(email="svtter@163.com", last_time=None)
+        r2 = MailRecord(email="svtter@163.com", expired_time=None, validated=False, sault="")
         return r2
 
-    def set_mail_record(self, mail: str):
+    def save_token(self, token: TokenDict):
         pass
 
 
 def test_none_of_mixin():
     mail = "svtter@163.com"
     e = Mixin2()
     re = e.get_mail_record(mail=mail)
-    assert re.last_time is None
+    assert re.expired_time is None
```

### Comparing `django_login_email-0.3.0/django_login_email/token.py` & `django_login_email-0.4.0/django_login_email/token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 # Handle email token
+import os
 import base64
 import json
 import urllib.parse
 import typing as t
 
 from Crypto.Cipher import AES
 from django.conf import settings
 import datetime
 
 Token = str
 EmailAndSalt = str
 Email = str
 
-TokenDict = t.TypedDict("TokenDict", {"email": Email, "expire_time": int, "salt": str})
+TokenDict = t.TypedDict("TokenDict", {"email": Email, "expired_time": int, "salt": str})
 
 
 class TokenGenerator(object):
     def __init__(self, minutes: int) -> None:
         self.minutes = minutes
 
-    def get_expire_time(self) -> int:
+    def get_expired_time(self) -> int:
         return int((datetime.datetime.now() + datetime.timedelta(minutes=self.minutes)).timestamp())
 
-    def gen(self, email, salt):
-        return json.dumps(
-            {
-                "email": email,
-                "expire_time": self.get_expire_time(),
-                "salt": salt,
-            }
-        )
+    def gen_salt(self, email) -> str:
+        return email + str(base64.b64encode(os.urandom(16)))
+
+    def gen(self, email, save_token: t.Callable[[TokenDict], None]) -> str:
+        """call save_token to save token in database or somewhere"""
+        token: TokenDict = {
+            "email": email,
+            "expired_time": self.get_expired_time(),
+            "salt": self.gen_salt(email),
+        }
+        save_token(token)
+        token_str = json.dumps(token)
+        return token_str
 
 
 class TokenManager(object):
-    salt: str = "randomsalt"
     key: bytes
     generator: TokenGenerator
 
     def __init__(self, minutes: int) -> None:
         self.key = settings.SECRET_KEY[:32].encode("utf-8")
         self.generator: TokenGenerator = TokenGenerator(minutes)
 
-    def check_token(self, token_uncrypt: str) -> t.Optional[TokenDict]:
-        """check salt and expire-time"""
+    def transform_token(self, token_uncrypt: Token) -> TokenDict:
         token_dict: TokenDict = json.loads(token_uncrypt)
-        if token_dict["salt"] == self.salt and token_dict["expire_time"] > int(datetime.datetime.now().timestamp()):
+        return token_dict
+
+    def check_token(self, token_dict: TokenDict, get_salt: t.Callable[[], str]) -> t.Optional[TokenDict]:
+        """check salt and expire-time"""
+        if token_dict["salt"] == get_salt() and token_dict["expired_time"] > int(datetime.datetime.now().timestamp()):
             return token_dict
         return None
 
     def get_mail(self, token_uncrypt: TokenDict) -> Email:
         return token_uncrypt["email"]
 
     def encrypt(self, plaintext, key):
@@ -61,18 +69,18 @@
         nonce = ciphertext[:16]
         tag = ciphertext[-16:]
         ciphertext = ciphertext[16:-16]
         cipher = AES.new(key, AES.MODE_EAX, nonce)
         plaintext = cipher.decrypt_and_verify(ciphertext, tag)
         return plaintext
 
-    def encrypt_mail(self, email: Email) -> str:
+    def encrypt_mail(self, email: Email, save_token: t.Callable[[TokenDict], None]) -> str:
         """email -> token -> base64 -> utf-8 -> urlquote"""
         # add salt.
-        content = self.generator.gen(email, self.salt)
+        content = self.generator.gen(email, save_token)
         content = content.encode("utf-8")
         return urllib.parse.quote(base64.b64encode(self.encrypt(content, self.key)).decode("utf-8"))
 
     def decrypt_token(self, token: Token) -> str:
         t = urllib.parse.unquote(token).encode("utf-8")
         print(t)
         t = base64.b64decode(t)
```

### Comparing `django_login_email-0.3.0/django_login_email/views.py` & `django_login_email-0.4.0/django_login_email/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,66 +5,94 @@
 from django.urls import reverse
 from django.views.generic.edit import FormView
 from django.views.generic import TemplateView
 from django.contrib.auth import get_user_model
 from . import forms
 from . import email
 from . import models
+from . import token
 
 # Create your views here.
 
 
 class TimeLimit(email.TimeLimit):
     minutes = 10
 
 
 class MailRecordModelMixin(email.EmailInfoMixin):
     """Here is an example for MailRecord, using django model. You could implement yourself."""
 
-    def set_mail_record(self, mail: str):
-        models.EmailLogin.set_email_last_time(mail, datetime.datetime.now(tz=datetime.timezone.utc))
-
     def reset_mail(self, mail: str):
         # models.EmailLogin.objects.filter(email=mail).delete()
         e = models.EmailLogin.objects.get(email=mail)
-        e.last_time = e.last_time - datetime.timedelta(minutes=self.tl.minutes)
+        e.expired_time = e.expired_time - datetime.timedelta(minutes=self.tl.minutes)
+        e.validated = False
         e.save()
 
     def get_mail_record(self, mail: str) -> email.MailRecord:
+        """get mail record to validate the sault, and validated status."""
         # for easy to change. use a function.
         try:
             e = models.EmailLogin.objects.get(email=mail)
+            return email.MailRecord(email=e.email, expired_time=e.expired_time, validated=e.validated, sault=e.sault)
+        except models.EmailLogin.DoesNotExist:
+            return email.MailRecord(email=mail, expired_time=None, validated=False, sault="")
+
+    def transform_timestamp(self, ts: int) -> datetime.datetime:
+        return datetime.datetime.fromtimestamp(ts, tz=datetime.timezone.utc)
+
+    def save_token(self, token: token.TokenDict):
+        """When generate new token, should call this method."""
+        try:
+            models.EmailLogin.objects.filter(email=token["email"]).update(
+                sault=token["salt"], expired_time=self.transform_timestamp(token["expired_time"])
+            )
         except models.EmailLogin.DoesNotExist:
-            return email.MailRecord(email=mail, last_time=None)
-        return email.MailRecord(email=e.email, last_time=e.last_time)
+            models.EmailLogin.objects.create(
+                email=token["email"],
+                sault=token["salt"],
+                expired_time=self.transform_timestamp(token["expired_time"]),
+            )
+
+    def disable_token(self, token: token.TokenDict):
+        models.EmailLogin.objects.filter(sault=token["salt"]).update(validated=True)
 
 
 class EmailLoginView(FormView, MailRecordModelMixin):
     template_name = "login_email/login.html"
     form_class = forms.LoginForm
     email_info_class = email.EmailLoginInfo
     tl = TimeLimit()
 
+    def get(self, request: HttpRequest, *args: str, **kwargs: Any) -> HttpResponse:
+        if self.request.user.is_authenticated:
+            return redirect("home")
+        return super().get(request, *args, **kwargs)
+
     def form_valid(self, form):
         """check the email"""
+
+        # Not allow to login if the user is already authenticated.
+        if self.request.user.is_authenticated:
+            return redirect("home")
+
         User = get_user_model()
         try:
             self.send_login_mail(form.cleaned_data["email"])
         except User.DoesNotExist as e:
             # ignore user missing problem.
             print(e, form.cleaned_data["email"])
             return render(self.request, "login_email/success.html", {"form": form})
         except Exception as e:
-            # raise Exception(e)
             print(e)
             return render(self.request, "login_email/error.html", {"error": e})
         return render(self.request, "login_email/success.html", {"form": form})
 
 
-class EmailVerifyView(TemplateView, email.EmailValidateMixin):
+class EmailVerifyView(TemplateView, email.EmailValidateMixin, MailRecordModelMixin):
     tl = TimeLimit()
 
     def post(self, request: HttpRequest, *args: str, **kwargs: Any) -> HttpResponse:
         raise Http404("Invalid Request.")
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         token = request.GET.get("token", None)
```

### Comparing `django_login_email-0.3.0/LICENSE` & `django_login_email-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_login_email-0.3.0/pyproject.toml` & `django_login_email-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "django-login-email"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["svtter <svtter@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 django = "^5.0.4"
 pycryptodome = "^3.20.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 pytest-django = "^4.8.0"
 psycopg2 = "^2.9.9"
+ipython = "^8.23.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 homepage = "https://github.com/Svtter/django-login-email"
```

### Comparing `django_login_email-0.3.0/README.md` & `django_login_email-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 - `/account/verify` for email verify.
 
 ## Feature
 
 - [x] The developer could define their own `User` model.
 - [x] Time-limited of login link.
 - [x] limited of sending email. Using TimeLimt to set minutes.
+- [x] The link could be used for Login once.
+- [ ] Ban IP to frequently ask to send mail.
+- [ ] Multiple user.
 - [ ] More easier and customizable login link.
 
 ## Future
 
 - Academically prove the safety of this method.
 
 ## Related project
```

### Comparing `django_login_email-0.3.0/PKG-INFO` & `django_login_email-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-login-email
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: svtter
 Author-email: svtter@qq.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -32,14 +32,17 @@
 - `/account/verify` for email verify.
 
 ## Feature
 
 - [x] The developer could define their own `User` model.
 - [x] Time-limited of login link.
 - [x] limited of sending email. Using TimeLimt to set minutes.
+- [x] The link could be used for Login once.
+- [ ] Ban IP to frequently ask to send mail.
+- [ ] Multiple user.
 - [ ] More easier and customizable login link.
 
 ## Future
 
 - Academically prove the safety of this method.
 
 ## Related project
```

