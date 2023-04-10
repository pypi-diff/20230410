# Comparing `tmp/fastapi_all_out-0.1.1.tar.gz` & `tmp/fastapi_all_out-0.1.2.tar.gz`

## Comparing `fastapi_all_out-0.1.1.tar` & `fastapi_all_out-0.1.2.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/app.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/code_responses.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/enums.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/lazy.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/mailing.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/models.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/responses.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/schemas.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/base.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/router.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/schemas.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/jwt/__init__.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/jwt/backend.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/jwt/schemas.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/jwt/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/roles/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/roles/router.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/auth/roles/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/conntection.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/repository.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/repository_meta.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/user_repository.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/user_service.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/fields/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/fk.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/int.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/simple.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/str.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/__init__.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/base.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/base_user.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/content_type.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/permissions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/management/__init__.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/management/command.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/camel_model.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/comma_separated.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/field_in_related_model.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/password.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/phonenumber.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/related_list.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/username.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/__init__.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/base_repository.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/base_repository_meta.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/crud_router.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/exceptions.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/utils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/bool.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/fk.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/int.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/int_btw.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/str.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/templates/activation.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/fastapi_all_out/templates/password_reset.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/LICENSE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/README.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/app.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/code_responses.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/enums.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/lazy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/mailing.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/models.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/responses.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/schemas.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/__init__.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/base.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/router.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/schemas.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/jwt/__init__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/jwt/backend.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/jwt/schemas.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/jwt/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/roles/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/roles/router.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/auth/roles/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/conntection.py
+-rw-r--r--   0        0        0    33364 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/repository.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/repository_meta.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/user_repository.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/user_service.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/fields/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/fk.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/int.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/simple.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/str.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/base.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/base_user.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/content_type.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/permissions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/management/__init__.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/management/command.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/camel_model.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/comma_separated.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/field_in_related_model.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/password.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/phonenumber.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/related_list.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/username.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/__init__.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/base_repository.py
+-rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/crud_router.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/exceptions.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/utils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/bool.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/fk.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/int.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/int_btw.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/str.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/templates/activation.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/fastapi_all_out/templates/password_reset.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.1.2/PKG-INFO
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/app.py` & `fastapi_all_out-0.1.2/fastapi_all_out/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from typing import Literal
-
-from fastapi import FastAPI, APIRouter
+from fastapi import FastAPI, APIRouter, Depends
 
 from fastapi_all_out.responses import \
     default_exception_handlers, \
     change_openapi_validation_error_schema
+from fastapi_all_out.lazy import get_auth_backend
 from fastapi_all_out.settings import MainDB
 
 
 class ExFastAPI(FastAPI):
     router: APIRouter
 
     def __init__(
             self,
             *,
             db_provider: MainDB = None,
             db_config: dict = None,
+            add_auth_dependency: bool = True,
             **kwargs
     ) -> None:
         kwargs.setdefault('swagger_ui_parameters', {"operationsSorter": "method", "docExpansion": "none"})
         exception_handlers = kwargs.get('exception_handlers', {})
         kwargs['exception_handlers'] = {**default_exception_handlers, **exception_handlers}
+        if add_auth_dependency:
+            dependencies = kwargs.get('dependencies', [])
+            kwargs['dependencies'] = [Depends(get_auth_backend().authenticate()), *dependencies]
         super().__init__(**kwargs)
 
         if db_config:
             match db_provider:
                 case MainDB.tortoise:
                     from fastapi_all_out.contrib.tortoise import conntection
                     db_on_start = conntection.on_start(config=db_config)
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/code_responses.py` & `fastapi_all_out-0.1.2/fastapi_all_out/code_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from enum import Enum
 from itertools import groupby
 from types import DynamicClassAttribute
-from typing import Any
+from typing import Any, Type
 
 from fastapi import BackgroundTasks
 
 from fastapi_all_out.pydantic import CamelModel, lower_camel
 from fastapi_all_out.responses import BgHTTPException
 
 
@@ -50,21 +50,25 @@
     def resp(self) -> dict[str, Any]:
         return {'code': lower_camel(self.name), 'message': self.message}
 
     def format_resp(self, values: str | tuple[str]):
         values = (values,) if isinstance(values, str) else values
         return {'code': lower_camel(self.name), 'message': self.message.format(*values)}
 
+    @property
+    def error_class(self) -> Type[BgHTTPException]:
+        return BgHTTPException
+
     def err(self, details: dict[str, Any] = None, background: BackgroundTasks = None) -> BgHTTPException:
         resp = {**self.resp, **details} if details else self.resp
-        return BgHTTPException(self.status, detail=resp, headers=self.headers, background=background)
+        return self.error_class(self.status, detail=resp, headers=self.headers, background=background)
 
     def format_err(self, values: str | tuple[str], details: dict[str, Any] = None, background: BackgroundTasks = None):
         resp = {**self.format_resp(values), **details} if details else self.format_resp(values)
-        return BgHTTPException(self.status, detail=resp, headers=self.headers, background=background)
+        return self.error_class(self.status, detail=resp, headers=self.headers, background=background)
 
     def resp_detail(self, **kwargs) -> dict[str, Any]:
         return {**self.resp, **kwargs}
 
     @classmethod
     def responses(
             cls,
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/lazy.py` & `fastapi_all_out-0.1.2/fastapi_all_out/lazy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from fastapi_all_out.settings import MainDB, BaseSettings,\
     MAIN_DB, USER_MODEL, REPOSITORY, USER_REPOSITORY, USER_SERVICE, MAIL_SENDER, CODES, AUTH
 
 if TYPE_CHECKING:
     from fastapi_all_out.code_responses import DefaultCodes
     from fastapi_all_out.routers.base_repository import BaseRepository
+    from fastapi_all_out.auth.user_service import BaseUserService
     from fastapi_all_out.mailing import MailSender
     from fastapi_all_out.auth.base import AuthBackend
-    from fastapi_all_out.auth.user_service import BaseUserService
 
 
 _T = TypeVar('_T')
 
 
 def get_settings(var: str, default: Any = '__undefined__') -> Any:
     settings = import_module('settings')
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/mailing.py` & `fastapi_all_out-0.1.2/fastapi_all_out/mailing.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,12 +61,11 @@
             'uuid': uuid,
             'temp_code': temp_code,
             'duration': duration,
             'host': host,
         })
 
 
-
 try:
     mail_sender = MailSender(MailingConfig())
 except ValidationError:
     mail_sender = None
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/models.py` & `fastapi_all_out-0.1.2/fastapi_all_out/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/responses.py` & `fastapi_all_out-0.1.2/fastapi_all_out/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/settings.py` & `fastapi_all_out-0.1.2/fastapi_all_out/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/router.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/router.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from uuid import uuid4, UUID
 
-from fastapi import Request, BackgroundTasks, Depends, Body, Query
+from fastapi import Request, BackgroundTasks, Response, Depends, Body, Query
 
 from fastapi_all_out.enums import TempCodeTriggers
 from fastapi_all_out.lazy import get_user_repository, get_user_service, get_schema, get_codes, get_auth_backend
 from fastapi_all_out.routers import CRUDRouter
 from fastapi_all_out.routers.exceptions import ObjectErrors, ItemNotFound
 from fastapi_all_out.schemas import UserRead, UserMeRead, UserEdit, UserMeEdit, UserCreate, UserRegistration
 
@@ -33,83 +33,93 @@
     kwargs.setdefault('read_list_item_schema', UserRead)
     kwargs.setdefault('create_schema', UserCreate)
     kwargs.setdefault('edit_schema', UserEdit)
 
     router = CRUDRouter(repo=UserRepository, complete_auto_routes=False, **kwargs)
 
     if add_get_me_route:
-        @router.get('/me', response_model=UserMeRead, responses=Codes.responses(*Codes.auth_errors()))
-        async def get_me(user_service: UserService = Depends(auth_backend.get_auth())):
-            return UserMeRead.from_orm(user_service.user)
+        @router.get(
+            '/me', response_model=UserMeRead, responses=Codes.responses(*Codes.auth_errors()),
+            dependencies=[Depends(auth_backend.with_permissions())]
+        )
+        async def get_me(request: Request):
+            return UserMeRead.from_orm(request.user)
 
     if add_edit_me_route:
-        @router.patch('/me', response_model=UserMeRead, responses=Codes.responses(
-            *Codes.auth_errors(),
-            router.field_errors_response_example()
-        ))
+        @router.patch(
+            '/me', response_model=UserMeRead, responses=Codes.responses(
+                *Codes.auth_errors(),
+                router.field_errors_response_example()
+            ),
+            dependencies=[Depends(auth_backend.with_permissions())]
+        )
         async def edit_me(
                 request: Request,
                 background_tasks: BackgroundTasks,
-                user_service: UserService = Depends(),
+                response: Response,
                 data: UserMeEdit = Body(...),
         ):
-            repository = router.repo(request=request, background_tasks=background_tasks)
             try:
-                instance = await repository.edit(user_service.user, data)
+                instance = await router.repo(request=request, background_tasks=background_tasks, response=response)\
+                    .edit(request.user, data.dict(exclude_unset=True))
             except ObjectErrors as e:
                 raise router.field_errors(e)
             return UserMeRead.from_orm(instance)
 
     if add_registration_route:
         @router.post('/registration', status_code=201, responses=Codes.responses(
             (Codes.activation_email, {'uuid': uuid4()}),
             router.field_errors_response_example()
         ))
         async def registration(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 data: get_schema(UserRegistration) = Body(...)
         ):
             try:
-                repository = router.repo(request=request, background_tasks=background_tasks)
-                user = await repository.create(data)
+                user = await router.repo(request=request, background_tasks=background_tasks, response=response)\
+                    .create(data.dict(exclude_unset=True))
             except ObjectErrors as e:
                 raise router.field_errors(e)
             user_service = UserService(user)
             await user_service.post_registration(request=request, background_tasks=background_tasks)
-            return Codes.activation_email.resp_detail(uuid=user_service.uuid)
+            return Codes.activation_email.resp_detail(uuid=user_service.user.uuid)
 
     if add_account_activation_route:
-        @router.get('/activation', response_model=auth_backend.strategy.authorize_response_model, responses=Codes.responses(
-            router.not_found_error_instance(),
-            Codes.activation_email_resend,
-            Codes.activation_email_code_incorrect,
-            Codes.already_active,
-        ))
+        @router.get(
+            '/activation', response_model=auth_backend.strategy.authorize_response_model, responses=Codes.responses(
+                router.not_found_error_instance(),
+                Codes.activation_email_resend,
+                Codes.activation_email_code_incorrect,
+                Codes.already_active,
+            )
+        )
         async def activate_account(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 uuid: UUID = Query(...),
                 code: str = Query(..., min_length=6, max_length=6)
         ):
             try:
-                repository = router.repo(request=request, background_tasks=background_tasks)
-                user = await repository.get_one(uuid, field_name='uuid')
+                user = await router.repo(request=request, background_tasks=background_tasks, response=response)\
+                    .get_one(uuid, field_name='uuid')
             except ItemNotFound:
                 raise router.not_found_error()
             user_service = UserService(user)
-            if user_service.is_user_active:
+            if user_service.user.is_active:
                 raise Codes.already_active.err()
             temp_code_error = user_service.check_temp_code_error(code, trigger=TempCodeTriggers.EmailActivation)
             if temp_code_error:
                 if temp_code_error == 'expired':
-                    user_service.add_send_activation_email_task(background_tasks=background_tasks)
+                    background_tasks.add_task(user_service.send_activation_email)
                     raise Codes.activation_email_resend.err(background=background_tasks)
                 if temp_code_error == 'incorrect':
                     raise Codes.activation_email_code_incorrect.err()
             await user_service.activate()
-            return auth_backend.strategy.authorize(user_service.user)
+            return auth_backend.authorize(user_service.user)
 
     if complete_auto_routes:
         router.complete_auto_routes()
 
     return router
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/schemas.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/user_service.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/user_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,62 @@
-from datetime import datetime
-from typing import Protocol, Optional, TypeVar, Any, Generic, Literal
+from typing import TypeVar, Any, Generic, Literal
 from abc import ABC, abstractmethod
-from uuid import UUID
 
 from passlib.context import CryptContext
 from fastapi import Request, BackgroundTasks
 
 from fastapi_all_out.enums import TempCodeTriggers
-from fastapi_all_out.schemas import PasswordsPair
+from .base import BaseUser
 
 
-class UserInterface(Protocol):
-    id: int
-    uuid: UUID
-    username: Optional[str]
-    email: Optional[str]
-    password_hash: str
-    password_change_dt: datetime
-    password_salt: str
-    is_superuser: bool
-    is_active: bool
-    created_at: datetime
-    EMAIL_FIELD: str
-    AUTH_FIELDS: tuple[str, ...]
-
-
-USER_MODEL = TypeVar("USER_MODEL", bound=UserInterface)
+USER_MODEL = TypeVar("USER_MODEL", bound=BaseUser)
+UNUSED_PASSWORD_PREFIX = '!'
 
 
 class BaseUserService(Generic[USER_MODEL], ABC):
 
     user: USER_MODEL
-    pwd_context = CryptContext(schemes=["md5_crypt"])
+    pwd_context = CryptContext(schemes=["md5_crypt"], deprecated="auto")
 
     def __init__(self, user: USER_MODEL):
         self.user = user
 
-    @classmethod
-    @abstractmethod
-    async def create_user(
-            cls,
-            data: PasswordsPair,
-            should_exclude: set[str] = None,
-            defaults: dict[str, Any] = None
-    ) -> USER_MODEL: ...
-
-    @abstractmethod
-    async def post_registration(self, request: Request, background_tasks: BackgroundTasks) -> None: ...
-
-    @property
-    @abstractmethod
-    def pk(self) -> int | UUID: ...
-
-    @property
-    @abstractmethod
-    def is_user_active(self) -> bool: ...
-
     def can_login(self) -> bool:
-        return self.is_user_active
+        return self.user.is_active
 
-    @property
-    @abstractmethod
-    def is_superuser(self) -> bool: ...
-
-    @property
-    @abstractmethod
-    def uuid(self) -> UUID: ...
-
-    @abstractmethod
-    def token_expired(self, iat: int) -> bool: ...
+    def token_expired(self, iat: int) -> bool:
+        return self.user.password_change_dt.timestamp() > iat
 
     @abstractmethod
     def set_password(self, password: str) -> None: ...
 
-    @abstractmethod
-    def get_fake_password(self, password: str) -> str: ...
+    def get_fake_password(self, password: str) -> str:
+        return password + str(self.user.password_change_dt.timestamp()) + self.user.password_salt
 
     def get_password_hash(self, password: str) -> str:
         return self.pwd_context.hash(self.get_fake_password(password))
 
-    @abstractmethod
-    def verify_password(self, password: str) -> bool: ...
-
-    @abstractmethod
-    def get_permissions(self) -> tuple[tuple[int, str], ...]: ...
-
-    @abstractmethod
-    def has_permissions(self, *permissions: tuple[str, str]) -> bool: ...
+    def verify_password(self, password: str) -> bool:
+        if self.user.password_hash.startswith(UNUSED_PASSWORD_PREFIX):
+            return False
+        return self.pwd_context.verify(self.get_fake_password(password), self.user.password_hash)
 
     @abstractmethod
     async def get_or_create_temp_code(self, trigger: TempCodeTriggers) -> Any: ...
 
     @abstractmethod
     async def update_or_create_temp_code(self, trigger: TempCodeTriggers) -> None: ...
 
     @abstractmethod
     async def send_activation_email(self) -> None: ...
 
     @abstractmethod
     async def send_password_reset_email(self) -> None: ...
 
-    def add_send_activation_email_task(self, background_tasks: BackgroundTasks) -> None:
+    async def post_registration(self, request: Request, background_tasks: BackgroundTasks) -> None:
         background_tasks.add_task(self.send_activation_email)
 
     @abstractmethod
     def check_temp_code_error(self, code: str, trigger: TempCodeTriggers) -> Literal['expired', 'incorrect'] | None: ...
 
     @abstractmethod
     async def activate(self) -> None: ...
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/jwt/backend.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/jwt/backend.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,101 @@
 from typing import Callable, Coroutine, Any
 
-from fastapi import APIRouter, Request, BackgroundTasks, Body, Header, Depends
+from fastapi import APIRouter, Request, BackgroundTasks, Response, Body, Depends
+from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
 
-from fastapi_all_out.lazy import get_schema, get_user_model, get_user_repository, get_user_service, get_codes
+from fastapi_all_out.lazy import get_schema, get_user_model, get_user_repository, get_user_service, get_codes,\
+    get_settings_obj
 from fastapi_all_out.routers.exceptions import ItemNotFound
 from fastapi_all_out.schemas import LoginPasswordSchema, UserMeRead
-from ..base import AuthBackend
+from ..base import AuthBackend, BaseUser, SimpleUser, UnauthenticatedUser
 from .schemas import JWTTokenUser
 from .strategy import JWTAuthStrategy
 
 
 LoginPasswordSchema = get_schema(LoginPasswordSchema)
 UserMeRead = get_schema(UserMeRead)
 JWTTokenUser = get_schema(JWTTokenUser)
 UserModel = get_user_model()
 UserRepository = get_user_repository()
 UserService = get_user_service()
 Codes = get_codes()
+settings = get_settings_obj()
+oauth2_default = OAuth2PasswordBearer(
+    tokenUrl=settings.API_PREFIX + '/auth/jwt/login',
+    scheme_name='Bearer',
+    auto_error=False,
+)
 
 
 class JWTAuthBackend(AuthBackend):
 
     strategy: "JWTAuthStrategy"
+    oauth: OAuth2PasswordBearer
+    _authenticate: Callable[[], Coroutine[Any, Any, None]]
+    _auth_required: Callable[[], Coroutine[Any, Any, None]]
 
-    def __init__(self, strategy: "JWTAuthStrategy"):
+    def __init__(self, strategy: "JWTAuthStrategy", oauth: OAuth2PasswordBearer = oauth2_default):
         assert isinstance(strategy, JWTAuthStrategy)
         self.strategy = strategy
+        self.oauth = oauth
 
-    def check_auth(self) -> Callable[[], Coroutine[Any, Any, bool]]:
-        async def wrapper(token: str = Header(default=None, alias='Token')) -> bool:
-            return self.strategy.get_auth(token) is not None
+    def authorize(self, user: BaseUser) -> Any:
+        return self.strategy.authorize(user)
 
-        return wrapper
+    def authenticate(self) -> Callable[[], Coroutine[Any, Any, None]]:
+        if not hasattr(self, '_authenticate'):
+            oauth_schema = self.oauth
+            authenticate_handler = self.strategy.authenticate
+
+            async def wrapper(request: Request, token: str = Depends(oauth_schema)) -> None:
+                token_data = await authenticate_handler(token)
+                if token_data is None:
+                    request.scope['auth'] = None
+                    request.scope['user'] = UnauthenticatedUser()
+                else:
+                    user = token_data.user
+                    request.scope['auth'] = token_data
+                    request.scope['user'] = SimpleUser(pk=user.get_pk(), username=user.username)
+
+            self._authenticate = wrapper
+
+        return self._authenticate
+
+    def auth_required(self) -> Callable[[], Coroutine[Any, Any, None]]:
+        if not hasattr(self, '_auth_required'):
+            async def wrapper(request: Request) -> None:
+                user: BaseUser = request.user
+                if not user.is_authenticated:
+                    raise Codes.not_authenticated.err()
+
+            self._auth_required = wrapper
+        return self._auth_required
 
-    def get_auth(self) -> Callable[[], Coroutine[Any, Any, UserService]]:
+    def with_permissions(self, *permissions: tuple[str, str]) -> Callable[[], Coroutine[Any, Any, None]]:
         async def wrapper(
                 request: Request,
                 background_tasks: BackgroundTasks,
-                token: str = Header(default=None, alias='Token')
-        ) -> UserService:
-            token = self.strategy.get_auth(token)
-            try:
-                user = await UserRepository(request=request, background_tasks=background_tasks)\
-                    .get_one(token.user.id)
-            except ItemNotFound:
-                raise Codes.not_authenticated.err()
-            user_service = UserService(user)
-            if user_service.token_expired(token.iat):
-                raise Codes.not_authenticated.err()
-            return user_service
+                response: Response,
+        ) -> None:
+            user: BaseUser = request.user
+            if not user.is_authenticated:
+                raise Codes.not_authenticated.err()
+            if user.is_simple:
+                user: SimpleUser
+                try:
+                    user_db = await UserRepository(
+                        request=request, background_tasks=background_tasks, response=response
+                    ).get_one(user.pk)
+                    request.scope['user'] = user = user_db
+                except ItemNotFound:
+                    raise Codes.not_authenticated.err()
 
-        return wrapper
-
-    def get_auth_with_permissions(
-            self, *permissions: tuple[str, str]
-    ) -> Callable[[], Coroutine[Any, Any, UserService]]:
-        async def wrapper(user_service: UserService = Depends(self.get_auth())) -> UserService:
-            if not (user_service.is_superuser or user_service.has_permissions(*permissions)):
+            if not (user.is_superuser or user.has_permissions(*permissions)):
                 raise Codes.permission_denied.err()
-            return user_service
 
         return wrapper
 
     def create_router(self, **kwargs) -> APIRouter:
         kwargs.setdefault('prefix', '/auth/jwt')
         kwargs.setdefault('tags', ['auth'])
         router = APIRouter(**kwargs)
@@ -70,25 +103,28 @@
         self.add_login_route(router)
         self.add_logout_route(router)
         self.add_refresh_route(router)
 
         return router
 
     def add_login_route(self, router: APIRouter) -> None:
-        @router.post('/login', response_model=self.strategy.authorize_response_model, responses=Codes.responses(
-            Codes.not_authenticated
-        ))
+        @router.post(
+            '/login', response_model=self.strategy.authorize_response_model, response_model_by_alias=False,
+            responses=Codes.responses(Codes.not_authenticated)
+        )
         async def wrapper(
                 request: Request,
                 background_tasks: BackgroundTasks,
-                login_password: LoginPasswordSchema = Body(...)
+                response: Response,
+                form: OAuth2PasswordRequestForm = Depends(),
         ):
+            login_password = LoginPasswordSchema(login=form.username, password=form.password)
             field, value = login_password.get_auth_field_and_value()
             try:
-                user = await UserRepository(request=request, background_tasks=background_tasks)\
+                user = await UserRepository(request=request, background_tasks=background_tasks, response=response)\
                     .get_one(value, field_name=field)
             except ItemNotFound:
                 raise Codes.not_authenticated.err()
 
             user_service = UserService(user)
             if not user_service.verify_password(password=login_password.password):
                 raise Codes.not_authenticated.err()
@@ -97,23 +133,26 @@
                 raise Codes.not_authenticated.err()
             return self.strategy.authorize(user)
 
     def add_logout_route(self, router: APIRouter) -> None:
         pass
 
     def add_refresh_route(self, router: APIRouter) -> None:
-        @router.post('/refresh', response_model=self.strategy.authorize_response_model, responses=Codes.responses(
-            Codes.not_authenticated
-        ))
+        @router.post(
+            '/refresh', response_model=self.strategy.authorize_response_model, response_model_by_alias=False,
+            responses=Codes.responses(Codes.not_authenticated)
+        )
         async def wrapper(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 token: str = Body(..., alias='refreshToken')
         ):
             token = self.strategy.get_refresh_token(token)
             try:
-                user = await UserRepository(request=request, background_tasks=background_tasks).get_one(token.user.id)
+                user = await UserRepository(request=request, background_tasks=background_tasks, response=response)\
+                    .get_one(token.user.id)
             except ItemNotFound:
                 raise Codes.not_authenticated.err()
             if UserService(user).token_expired(token.iat):
                 raise Codes.not_authenticated.err()
             return self.strategy.authorize(user)
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/jwt/strategy.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/jwt/strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from abc import abstractmethod
 from datetime import timedelta, datetime
-from typing import Any
+from typing import Any, Optional
 
 from jwt import PyJWT, InvalidSignatureError, DecodeError, ExpiredSignatureError
 
 from fastapi_all_out.pydantic import CamelModel
 from fastapi_all_out.responses import DefaultJSONEncoder
 from fastapi_all_out.lazy import get_schema, get_codes
 from fastapi_all_out.enums import JWTTokenTypes
 from fastapi_all_out.schemas import UserMeRead
-from ..base import AuthStrategy
+from ..base import AuthStrategy, BaseUser
 from .schemas import JWTToken, JWTTokenIssue
 
 
 LIFETIME = dict[JWTTokenTypes, int]
 DEFAULT_LIFETIME: LIFETIME = {
     JWTTokenTypes.access: int(timedelta(minutes=5).total_seconds()),
     JWTTokenTypes.refresh: int(timedelta(days=10).total_seconds()),
@@ -25,14 +25,15 @@
 Codes = get_codes()
 
 
 class TokenPair(CamelModel):
     access_token: str
     refresh_token: str
     user: UserMeRead
+    token_type: str = 'bearer'
 
 
 class JWTAuthStrategy(AuthStrategy):
     jwt = PyJWT()
     json_encoder = DefaultJSONEncoder
 
     authorize_response_model = TokenPair
@@ -65,26 +66,27 @@
                 user=user,
                 type=token_type,
                 iat=iat or self.now(),
                 seconds=self.lifetime[token_type]
             ).dict()
         )
 
-    def create_access_token(self, user, iat: int = None) -> str:
+    def create_access_token(self, user: BaseUser, iat: int = None) -> str:
         return self.create_token(user, JWTTokenTypes.access, iat=iat)
 
-    def create_refresh_token(self, user, iat: int = None) -> str:
+    def create_refresh_token(self, user: BaseUser, iat: int = None) -> str:
         return self.create_token(user, JWTTokenTypes.refresh, iat=iat)
 
-    def authorize(self, user) -> TokenPair:
+    def authorize(self, user: BaseUser) -> TokenPair:
         now = self.now()
         return TokenPair(
             access_token=self.create_access_token(user, iat=now),
             refresh_token=self.create_refresh_token(user, iat=now),
             user=user,
+            token_type=self.SCHEMA.lower()
         )
 
     def get_token_payload(self, token: str):
         try:
             payload = self.decode(token)
         except (InvalidSignatureError, DecodeError):
             raise Codes.invalid_token.err()
@@ -94,23 +96,21 @@
 
     def parse_token(self, token: str, token_type: JWTTokenTypes) -> JWTToken:
         payload = self.get_token_payload(token)
         if payload.type != token_type:
             raise Codes.not_authenticated.err()
         return payload
 
-    def get_access_token(self, token: str) -> JWTToken:
-        if token is None:
-            raise Codes.not_authenticated.err()
-        schema, _, token = token.partition(" ")
-        if schema.lower() != self.SCHEMA:
-            raise Codes.not_authenticated.err()
+    def get_access_token(self, token: Optional[str]) -> JWTToken:
         return self.parse_token(token, token_type=JWTTokenTypes.access)
 
-    get_auth = get_access_token
+    async def authenticate(self, token: Optional[str]) -> Optional[JWTToken]:
+        if token is None:
+            return None
+        return self.get_access_token(token)
 
     def get_refresh_token(self, token: str) -> JWTToken:
         return self.parse_token(token, token_type=JWTTokenTypes.refresh)
 
 
 class RS256JWTAuthStrategy(JWTAuthStrategy):
     ALGORITHM = 'RS256'
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/roles/router.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/roles/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/auth/roles/schemas.py` & `fastapi_all_out-0.1.2/fastapi_all_out/auth/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/conntection.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/conntection.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/repository.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from collections import defaultdict
-from typing import Any, Optional, TypeVar, TYPE_CHECKING, Type, Self
+from typing import Any, Optional, TypeVar, TYPE_CHECKING, Type
 
 from tortoise.models import MetaInfo
-from tortoise.fields import ManyToManyRelation
+from tortoise.fields import ManyToManyRelation, Field, DateField, DatetimeField, TimeField
 from tortoise.queryset import QuerySet
 from tortoise.transactions import in_transaction
 
-from fastapi_all_out.pydantic import CamelModel
-from fastapi_all_out.routers.base_repository import BaseRepository, PK, ModelPrefix, CreateHandler, EditHandler, \
-    FKGetInstance
+from fastapi_all_out.routers.base_repository import BaseRepository, PK, ModelPrefix, Updated
 from fastapi_all_out.routers.exceptions import ItemNotFound, ObjectErrors, NotUnique, ListFieldError, NotFoundFK, \
     FieldRequired
 from .repository_meta import TortoiseRepositoryMeta
 from .models import BaseModel
 
 if TYPE_CHECKING:
     from fastapi_all_out.routers.filters import BaseFilter
@@ -24,18 +22,24 @@
 class TortoiseRepository(BaseRepository[DB_MODEL], metaclass=TortoiseRepositoryMeta):
     opts: MetaInfo
     node_key = 'parent_id'
 
     select_related: tuple[str]
     prefetch_related: tuple[str]
 
+    root_instance: Optional[DB_MODEL]
+    BFK_REMOVE_FIELDS_PATTERN = '_{}_remove'
+    M2M_REMOVE_FIELDS_PATTERN = '_{}_remove'
+    M2M_ADD_FIELDS_PATTERN = '_{}_add'
+
     def __init__(self, *args, select_related: tuple[str] = (), prefetch_related: tuple[str] = (), **kwargs):
         super().__init__(*args, **kwargs)
         self.select_related = select_related
         self.prefetch_related = prefetch_related
+        self.root_instance = None
 
     def get_queryset(self):
         if self.request is None:
             path, method = '', ''
         else:
             path, method = self.request.scope['route'].path, self.request.method
 
@@ -91,535 +95,738 @@
     def _get_many_queryset(self, item_ids: list[PK]) -> QuerySet[DB_MODEL]:
         return self.get_queryset().filter(pk__in=item_ids)
 
     async def get_many(self, item_ids: list[PK]) -> list[DB_MODEL]:
         return await self._get_many_queryset(item_ids)
 
     async def get_one(self, item_id: PK, *, field_name: str = 'pk') -> Optional[DB_MODEL]:
+        if field_name in self.model.IEXACT_FIELDS:
+            field_name = field_name + '__iexact'
         instance = await self.get_queryset()\
             .get_or_none(**{field_name: item_id})
         if instance is None:
             raise ItemNotFound()
         return instance
 
     async def get_tree_node(self, node_id: Optional[PK]) -> list[DB_MODEL]:
         return await self.get_queryset().filter(**{self.node_key: node_id})
 
     async def create(
             self,
-            data: CamelModel,
+            data: dict[str, Any],
             *,
-            model: Type[BaseModel] = None,
+            model: Type[DB_MODEL] = None,
             exclude: set[str] = None,
             defaults: dict[str, Any] = None,
             inside_transaction: bool = False,
             prefix: ModelPrefix = ModelPrefix(),
     ) -> DB_MODEL:
-        model: Type[BaseModel] = model or self.model
+        model: Type[DB_MODEL] = model or self.model
         fk_fields, bfk_fields, o2o_fields, bo2o_fields, m2m_fields = exclude_fk_bfk_o2o_bo2o_m2m(model, data)
         exclude_dict = get_exclude_dict(exclude or set())
         errors = ObjectErrors()
         defaults = defaults or {}
 
         async def get_new_instance() -> DB_MODEL:
-            not_unique = await model.check_unique(data.dict(include=model._meta.db_fields))
-            for field_name in not_unique:
-                errors.add(field_name, NotUnique)
+            await self.clean_data(
+                model=model, data=data, prefix=prefix, create=True,
+                fk_fields=fk_fields,
+                bfk_fields=bfk_fields,
+                o2o_fields=o2o_fields,
+                bo2o_fields=bo2o_fields,
+                m2m_fields=m2m_fields,
+            )
+            try:
+                await self.check_unique(data=data, model=model, prefix=prefix)
+            except ObjectErrors as e:
+                errors.merge(e)
 
             # Сначала создаём o2o и fk, потому что они могут быть not null, из-за этого вылетает ошибка.
             created_o2o, picked_fks = {}, {}
 
             for o2o_field_name in o2o_fields:
                 try:
-                    o2o_instance = await self.create_o2o(
+                    created_o2o[o2o_field_name] = await self.create_o2o(
                         model=model,
                         field_name=o2o_field_name,
                         data=data,
                         exclude=exclude_dict[o2o_field_name],
-                        prefix=prefix
+                        prefix=prefix.plus(o2o_field_name),
                     )
-                    created_o2o[o2o_field_name] = o2o_instance
                 except ObjectErrors as e:
                     errors.add(o2o_field_name, e)
 
             try:
                 picked_fks = await self.pick_fks(model=model, fk_fields=fk_fields, data=data, prefix=prefix)
             except ObjectErrors as e:
                 errors.merge(e)
 
             if errors:
                 raise errors
+
             try:
-                instance: DB_MODEL = await self.handle_create(prefix, model=model)(
+                instance: Optional[DB_MODEL] = await self.handle_create(
+                    model=model,
                     data=data,
                     exclude={*exclude_dict['__root__'], *fk_fields},
-                    defaults={**self.get_defaults(prefix), **defaults, **created_o2o, **picked_fks}
+                    prefix=prefix,
+                    defaults={**self.get_defaults(prefix), **defaults, **created_o2o, **picked_fks},
                 )
             except ObjectErrors as e:
                 raise errors.merge(e)
 
             for bo2o_field_name in bo2o_fields:
                 try:
                     await self.create_backward_o2o(
                         instance=instance,
                         field_name=bo2o_field_name,
                         data=data,
                         exclude=exclude_dict[bo2o_field_name],
-                        prefix=prefix
+                        prefix=prefix.plus(bo2o_field_name)
                     )
                 except ObjectErrors as e:
                     errors.add(bo2o_field_name, e)
 
             for bfk_field_name in bfk_fields:
                 try:
                     await self.create_backward_fk(
                         instance=instance,
                         field_name=bfk_field_name,
                         data=data,
                         exclude=exclude_dict[bfk_field_name],
-                        prefix=prefix,
+                        prefix=prefix.plus(bfk_field_name),
                     )
                 except ListFieldError as e:
                     errors.add(bfk_field_name, e)
 
+            if errors:
+                raise errors
+
             for m2m_field_name in m2m_fields:
                 await self.save_m2m(
                     instance=instance,
                     data=data,
                     field_name=m2m_field_name,
-                    prefix=prefix,
+                    prefix=prefix.plus(m2m_field_name),
                 )
 
-            if errors:
-                raise errors
             return instance
 
         if inside_transaction:
             return await get_new_instance()
         else:
             async with in_transaction():
                 new_instance = await get_new_instance()
+            await self.post_create(new_instance)
+            if self.background_tasks:
+                self.background_tasks.add_task(self.post_create_background, new_instance)
             return await self.get_one(new_instance.pk)
 
     async def create_o2o(
             self,
             model: Type[DB_MODEL],
             field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> Optional[DB_MODEL]:
-        o2o_data = getattr(data, field_name)
+        o2o_data = data.get(field_name)
         if o2o_data is None:
             return None
-        o2o_model: Type[BaseModel] = model._meta.fields_map[field_name].related_model
+        o2o_model: Type[DB_MODEL] = model._meta.fields_map[field_name].related_model
         return await self.create(
             data=o2o_data,
             model=o2o_model,
             exclude=exclude,
             inside_transaction=True,
-            prefix=prefix.plus(field_name)
+            prefix=prefix,
         )
 
     async def create_backward_o2o(
             self,
-            instance: BaseModel,
+            instance: DB_MODEL,
             field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> None:
-        back_o2o_data = getattr(data, field_name)
+        back_o2o_data = data.get(field_name)
         if back_o2o_data is None:
             return
         back_o2o_field = instance._meta.fields_map[field_name]
-        back_o2o_model: Type[BaseModel] = back_o2o_field.related_model
+        back_o2o_model: Type[DB_MODEL] = back_o2o_field.related_model
         back_o2o_source_field = back_o2o_model._meta\
             .fields_map[back_o2o_field.relation_source_field]\
             .reference.model_field_name
         await self.create(
             data=back_o2o_data,
             model=back_o2o_model,
             exclude=exclude,
             defaults={back_o2o_source_field: instance},
             inside_transaction=True,
-            prefix=prefix.plus(field_name)
+            prefix=prefix
         )
 
     async def create_backward_fk(
             self,
-            instance: BaseModel,
+            instance: DB_MODEL,
             field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> None:
         list_errors = ListFieldError()
         back_fk_field = instance._meta.fields_map[field_name]
-        back_fk_model: Type[BaseModel] = back_fk_field.related_model
+        back_fk_model: Type[DB_MODEL] = back_fk_field.related_model
         back_fk_source_field = back_fk_model._meta \
             .fields_map[back_fk_field.relation_source_field] \
             .reference.model_field_name
-        next_prefix = prefix.plus(field_name)
-        for index, back_fk_data in enumerate(getattr(data, field_name)):
+        for index, back_fk_data in enumerate(data.get(field_name)):
             try:
                 await self.create(
                     data=back_fk_data,
                     model=back_fk_model,
                     exclude=exclude,
                     defaults={back_fk_source_field: instance},
                     inside_transaction=True,
-                    prefix=next_prefix,
+                    prefix=prefix,
                 )
             except ObjectErrors as e:
                 list_errors.append(index, e)
         if list_errors:
             raise list_errors
 
     async def edit(
             self,
             instance: DB_MODEL,
-            data: CamelModel,
+            data: dict[str, Any],
             *,
             exclude: set[str] = None,
             defaults: dict[str, Any] = None,
             inside_transaction: bool = False,
             prefix: ModelPrefix = ModelPrefix(),
     ) -> DB_MODEL:
-        model: Type[BaseModel] = instance.__class__
+        model: Type[DB_MODEL] = instance.__class__
         fk_fields, bfk_fields, o2o_fields, bo2o_fields, m2m_fields = exclude_fk_bfk_o2o_bo2o_m2m(model, data)
         exclude_dict = get_exclude_dict(exclude or set())
         errors = ObjectErrors()
         defaults = defaults or {}
 
         async def get_changed_instance() -> DB_MODEL:
-            not_unique = await model.check_unique(data.dict(include=model._meta.db_fields, exclude_unset=True))
-            for field_name in not_unique:
-                errors.add(field_name, NotUnique)
+            await self.clean_data(
+                model=model, data=data, prefix=prefix, instance=instance, create=False,
+                fk_fields=fk_fields,
+                bfk_fields=bfk_fields,
+                o2o_fields=o2o_fields,
+                bo2o_fields=bo2o_fields,
+                m2m_fields=m2m_fields,
+            )
+            try:
+                await self.check_unique(data=data, model=model, prefix=prefix)
+            except ObjectErrors as e:
+                errors.merge(e)
 
             created_o2o, picked_fks = {}, {}
             for o2o_field_name in o2o_fields:
                 try:
                     o2o_instance = await self.edit_o2o(
                         instance=instance,
                         field_name=o2o_field_name,
                         data=data,
                         exclude=exclude_dict[o2o_field_name],
-                        prefix=prefix,
+                        prefix=prefix.plus(o2o_field_name),
                     )
                     if o2o_instance:
                         created_o2o[o2o_field_name] = o2o_instance
                 except ObjectErrors as e:
                     errors.add(o2o_field_name, e)
 
             try:
                 picked_fks = await self.pick_fks(model=model, fk_fields=fk_fields, data=data, prefix=prefix)
             except ObjectErrors as e:
                 errors.merge(e)
 
             if errors:
                 raise errors
 
-            await self.handle_edit(prefix, model=model)(
+            await self.handle_edit(
                 instance=instance,
                 data=data,
                 exclude={*exclude_dict['__root__'], *fk_fields},
-                defaults={**defaults, **created_o2o, **picked_fks}
+                prefix=prefix,
+                defaults={**defaults, **created_o2o, **picked_fks},
             )
 
             for bo2o_field_name in bo2o_fields:
                 try:
                     await self.edit_backward_o2o(
                         instance=instance,
                         field_name=bo2o_field_name,
                         data=data,
                         exclude=exclude_dict[bo2o_field_name],
-                        prefix=prefix
+                        prefix=prefix.plus(bo2o_field_name)
                     )
                 except ObjectErrors as e:
                     errors.add(bo2o_field_name, e)
 
             for bfk_source_field_name in bfk_fields:
                 try:
                     await self.edit_backward_fk(
                         instance=instance,
                         field_name=bfk_source_field_name,
                         data=data,
                         exclude=exclude_dict[bfk_source_field_name],
-                        prefix=prefix
+                        prefix=prefix.plus(bfk_source_field_name)
                     )
                 except ListFieldError as e:
                     errors.add(bfk_source_field_name, e)
 
             for m2m_field_name in m2m_fields:
                 await self.save_m2m(
                     instance=instance,
                     data=data,
                     field_name=m2m_field_name,
-                    prefix=prefix,
+                    prefix=prefix.plus(m2m_field_name),
                     clear=True,
                 )
 
             if errors:
                 raise errors
+
             return instance
 
         if inside_transaction:
             return await get_changed_instance()
         else:
+            self.root_instance = instance
+            self.updated = {}
             async with in_transaction():
                 changed_instance = await get_changed_instance()
+            await self.post_edit(self.updated)
+            if self.background_tasks:
+                self.background_tasks.add_task(self.post_edit_background, self.updated)
             return await self.get_one(changed_instance.pk)
 
     async def edit_o2o(
             self,
             instance: DB_MODEL,
             field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
-    ) -> Optional[BaseModel]:
-        o2o_instance: Optional[BaseModel] = getattr(instance, field_name)
-        o2o_data = getattr(data, field_name)
+    ) -> Optional[DB_MODEL]:
+        o2o_instance: Optional[DB_MODEL] = getattr(instance, field_name)
+        o2o_data = data.get(field_name)
         if o2o_data is None:
             if o2o_instance is not None:
                 await o2o_instance.delete()
             return None
         if o2o_instance is not None:
             await self.edit(
                 instance=o2o_instance,
                 data=o2o_data,
                 exclude=exclude,
                 inside_transaction=True,
-                prefix=prefix.plus(field_name),
+                prefix=prefix,
             )
         else:
             return await self.create(
                 data=o2o_data,
                 exclude=exclude,
                 model=instance._meta.fields_map[field_name].related_model,
                 inside_transaction=True,
-                prefix=prefix.plus(field_name),
+                prefix=prefix,
             )
 
     async def edit_backward_o2o(
             self,
             instance: DB_MODEL,
             field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> None:
         back_o2o_instance = getattr(instance, field_name)
-        back_o2o_data = getattr(data, field_name)
+        back_o2o_data = data.get(field_name)
         back_o2o_field = instance._meta.fields_map[field_name]
-        back_o2o_model: Type[BaseModel] = back_o2o_field.related_model
+        back_o2o_model: Type[DB_MODEL] = back_o2o_field.related_model
         back_o2o_source_field = back_o2o_model._meta \
             .fields_map[back_o2o_field.relation_source_field] \
             .reference.model_field_name
         if back_o2o_instance is not None:
             await self.edit(
                 instance=back_o2o_instance,
                 data=back_o2o_data,
                 exclude=exclude,
                 inside_transaction=True,
-                prefix=prefix.plus(field_name),
+                prefix=prefix,
             )
         else:
             await self.create(
                 data=back_o2o_data,
                 model=back_o2o_model,
                 exclude=exclude,
                 defaults={back_o2o_source_field: instance},
                 inside_transaction=True,
-                prefix=prefix.plus(field_name),
+                prefix=prefix,
             )
 
     async def edit_backward_fk(
             self,
             instance: DB_MODEL,
             field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> None:
-        def get_fk_instance(instances: list[BaseModel], pk_value) -> BaseModel | None:
+        def get_fk_instance(instances: list[DB_MODEL], pk_value) -> DB_MODEL | None:
             for i in instances:
                 if i.pk == pk_value:
                     return i
 
         list_errors = ListFieldError()
-        back_fk_instances: list[BaseModel] = getattr(instance, field_name)
+        back_fk_instances: list[DB_MODEL] = getattr(instance, field_name)
         back_fk_field = instance._meta.fields_map[field_name]
-        back_fk_model: Type[BaseModel] = back_fk_field.related_model
+        back_fk_model: Type[DB_MODEL] = back_fk_field.related_model
         back_fk_source_field = back_fk_model._meta \
             .fields_map[back_fk_field.relation_source_field] \
             .reference.model_field_name
-        back_pk_attr = back_fk_model._meta.pk_attr
-        for index, back_fk_data in enumerate(getattr(data, field_name)):
-            if pk := getattr(back_fk_data, back_pk_attr, None):
+        back_pk_attr = self._get_pk_attr(back_fk_model)
+        for index, back_fk_data in enumerate(data.get(field_name)):
+            back_fk_data: dict[str, Any]
+            if pk := back_fk_data.get(back_pk_attr):
                 fk_instance = get_fk_instance(back_fk_instances, pk)
                 if fk_instance:
                     coro = self.edit(
                         instance=fk_instance,
                         data=back_fk_data,
                         exclude=exclude,
                         inside_transaction=True,
-                        prefix=prefix.plus(field_name),
+                        prefix=prefix.plus(index),
                     )
                 else:
                     list_errors.append(index, NotFoundFK)
                     continue
             else:
                 coro = self.create(
                     data=back_fk_data,
                     model=back_fk_model,
                     exclude=exclude,
                     defaults={back_fk_source_field: instance},
                     inside_transaction=True,
-                    prefix=prefix.plus(field_name),
+                    prefix=prefix.plus(index),
                 )
             try:
                 await coro
             except ObjectErrors as e:
                 list_errors.append(index, e)
 
         if list_errors:
             raise list_errors
 
+        remove_pks = data.get(self.BFK_REMOVE_FIELDS_PATTERN.format(field_name))
+        if remove_pks:
+            await back_fk_model.filter(pk__in=remove_pks).delete()
+
     async def pick_fk(
             self,
             model: Type[DB_MODEL],
             fk_source_field_name: str,
-            data: CamelModel,
+            data: dict[str, Any],
             prefix: ModelPrefix,
     ) -> tuple[str, Optional[DB_MODEL]]:
         opts = model._meta
         rel_model, field_name = None, None
         for field in opts.fk_fields:
             if (f_opts := opts.fields_map[field]).source_field == fk_source_field_name:
                 rel_model = f_opts.related_model
                 field_name = field
 
-        value = getattr(data, fk_source_field_name, None)
+        value = data.get(fk_source_field_name)
         if value is None:
             return field_name, None
 
-        get_rel_instance_func = self.get_fk_get_instance(prefix=prefix.plus(fk_source_field_name), model=rel_model)
-        rel_instance = await get_rel_instance_func(self, pk=value)
+        fk_get_func = getattr(self, f'fk_get_{prefix}', self._fk_get_default)
+        rel_instance = await fk_get_func(model=rel_model, pk=value)
         if rel_instance is None:
             raise NotFoundFK
         return field_name, rel_instance
 
     async def pick_fks(
             self,
             model: Type[DB_MODEL],
             fk_fields: set[str],
-            data: CamelModel,
+            data: dict[str, Any],
             prefix: ModelPrefix,
     ) -> dict[str, Optional[DB_MODEL]]:
         picked_fks = {}
         errors = ObjectErrors()
         for fk_source_field_name in fk_fields:
             try:
                 fk_field_name, fk_instance = await self.pick_fk(
                     model=model,
                     fk_source_field_name=fk_source_field_name,
                     data=data,
-                    prefix=prefix
+                    prefix=prefix.plus(fk_source_field_name)
                 )
                 picked_fks[fk_field_name] = fk_instance
             except NotFoundFK:
                 errors.add(fk_source_field_name, NotFoundFK)
         if errors:
             raise errors
         return picked_fks
 
+    async def save_m2m(
+            self,
+            instance: DB_MODEL,
+            data: dict[str, Any],
+            field_name: str,
+            prefix: ModelPrefix,
+            clear=False,
+    ) -> None:
+        rel: ManyToManyRelation = getattr(instance, field_name)
+        ids: list[PK] = data.get(field_name)
+        if ids is None:
+            return
+        if clear:
+            await rel.clear()
+        if ids:
+            await rel.add(*(await rel.remote_model.filter(pk__in=ids)))
+
     async def delete_many(self, item_ids: list[PK]) -> int:
         return await self._get_many_queryset(item_ids).delete()
 
-    async def delete_one(self, item_id: PK) -> None:
-        item = await self.get_one(item_id)
-        await item.delete()
-
-    def handle_create(self, prefix: ModelPrefix, model: Type[DB_MODEL]) -> CreateHandler[DB_MODEL]:
-        if handler := self.create_handlers.get(prefix):
-            return handler
-
-        async def base_handler(
-                data: CamelModel,
-                exclude: set[str],
-                defaults: dict[str, Any] = None,
-        ) -> DB_MODEL:
-            errors = ObjectErrors()
-            include_fields = model._meta.db_fields.difference(exclude)
-            data_dict = data.dict(include=include_fields, exclude_unset=True)
-            if defaults is not None:
-                data_dict.update(defaults)
-            instance = model(**data_dict)
-            opts = model._meta
-            for field_name in (*opts.db_fields, *opts.fk_fields, *opts.o2o_fields):
-                f_opts = opts.fields_map[field_name]
-                if (
-                        f_opts.null is False
-                        and f_opts.pk is False
-                        and getattr(instance, field_name) is None
-                ):
-                    errors.add(field_name, FieldRequired)
-            if errors:
-                raise errors
-            await instance.save(force_create=True)
-            return instance
+    async def delete_one(self, instance: DB_MODEL) -> None:
+        await instance.delete()
 
-        self.create_handlers[prefix] = base_handler
-        return base_handler
+    async def handle_create(
+            self,
+            model: Type[DB_MODEL],
+            data: dict[str, Any],
+            exclude: set[str],
+            prefix: ModelPrefix,
+            defaults: dict[str, Any] = None,
+    ) -> DB_MODEL:
+        if hasattr(self, f'handle_create_{prefix}'):
+            handler = getattr(self, f'handle_create_{prefix}')
+        else:
+            handler = self._handle_create_default
+        return await handler(
+            model=model,
+            data=data,
+            exclude=exclude,
+            prefix=prefix,
+            defaults=defaults,
+        )
 
-    def handle_edit(self, prefix: ModelPrefix, model: Type[DB_MODEL]) -> EditHandler[DB_MODEL]:
-        if handler := self.edit_handlers.get(prefix):
-            return handler
-
-        async def base_handler(
-                instance: DB_MODEL,
-                data: CamelModel,
-                exclude: set[str],
-                defaults: dict[str, Any] = None,
-        ) -> DB_MODEL:
-            include_fields = model._meta.db_fields.difference(exclude)
-            data_dict = data.dict(include=include_fields, exclude_unset=True)
-            if defaults is not None:
-                data_dict.update(defaults)
-            instance.update_from_dict(data_dict)
-            await instance.save(force_update=True)
-            return instance
+    async def _handle_create_default(
+            self,
+            model: Type[DB_MODEL],
+            data: dict[str, Any],
+            exclude: set[str],
+            prefix: ModelPrefix,
+            defaults: dict[str, Any] = None,
+            commit: bool = True,
+    ) -> DB_MODEL:
+        errors = ObjectErrors()
+        include_fields = model._meta.db_fields.difference(exclude)
+        final_data = {field: value for field, value in data.items() if field in include_fields}
+        if defaults is not None:
+            final_data.update(defaults)
+        instance = model(**final_data)
+        opts = model._meta
+        pass_check_required = self.get_pass_check_required(prefix)
+        for field_name in opts.db_fields:
+            if field_name in pass_check_required:
+                continue
+            if field_is_required(opts.fields_map[field_name]) and getattr(instance, field_name) is None:
+                errors.add(field_name, FieldRequired)
+        if errors:
+            raise errors
+        if commit:
+            await instance.save(force_create=True)
+        return instance
 
-        self.edit_handlers[prefix] = base_handler
-        return base_handler
+    async def handle_edit(
+            self,
+            instance: DB_MODEL,
+            data: dict[str, Any],
+            exclude: set[str],
+            prefix: ModelPrefix,
+            defaults: dict[str, Any] = None,
+    ) -> None:
+        if hasattr(self, f'handle_edit_{prefix}'):
+            handler = getattr(self, f'handle_edit_{prefix}')
+        else:
+            handler = self._handle_edit_default
+        await handler(
+            instance=instance,
+            data=data,
+            exclude=exclude,
+            prefix=prefix,
+            defaults=defaults,
+        )
 
-    async def save_m2m(
+    async def _handle_edit_default(
             self,
             instance: DB_MODEL,
-            data: CamelModel,
-            field_name: str,
+            data: dict[str, Any],
+            exclude: set[str],
             prefix: ModelPrefix,
-            clear=False,
+            defaults: dict[str, Any] = None,
     ) -> None:
-        rel: ManyToManyRelation = getattr(instance, field_name)
-        ids: list[PK] = getattr(data, field_name)
-        if clear:
-            await rel.clear()
-        await rel.add(*(await rel.remote_model.filter(pk__in=ids)))
+        errors = ObjectErrors()
+        include_fields = instance._meta.db_fields.difference(exclude)
+        final_data = {field: value for field, value in data.items() if field in include_fields}
+        if defaults is not None:
+            final_data.update(defaults)
+        instance.update_from_dict(final_data)
+        opts = instance._meta
+        for field_name in opts.db_fields:
+            if field_is_required(opts.fields_map[field_name]) and getattr(instance, field_name) is None:
+                errors.add(field_name, FieldRequired)
+        if errors:
+            raise errors
+        if final_data:
+            await instance.save(force_update=True)
+            self.updated[prefix] = Updated(instance=instance, fields=set(final_data.keys()))
+
+    async def clean_data(
+            self,
+            model: Type[DB_MODEL],
+            data: dict[str, Any],
+            prefix: ModelPrefix,
+            fk_fields: set[str],
+            bfk_fields: set[str],
+            o2o_fields: set[str],
+            bo2o_fields: set[str],
+            m2m_fields: set[str],
+            instance: Optional[DB_MODEL] = None,
+            create: bool = True,
+    ) -> dict[str, Any]:
+        related_fields = {*model._meta.db_fields, *fk_fields, *bfk_fields, *o2o_fields, *bo2o_fields, *m2m_fields}
+        for field_name in related_fields:
+            if field_name not in data:
+                continue
+            func_name = f'clean_field_{prefix.plus(field_name)}'
+            if hasattr(self, func_name):
+                func = getattr(self, func_name)
+            elif field_name in fk_fields:
+                func = self._clean_fk_field_default
+            elif field_name in bfk_fields:
+                func = self._clean_bfk_field_default
+            elif field_name in o2o_fields:
+                func = self._clean_o2o_field_default
+            elif field_name in bo2o_fields:
+                func = self._clean_bo2o_field_default
+            elif field_name in m2m_fields:
+                func = self._clean_m2m_field_default
+            else:
+                func = self._clean_field_default
+            should_remove = await func(
+                model=model, data=data, field_name=field_name, instance=instance, create=create
+            )
+            if should_remove:
+                for set_ in (fk_fields, bfk_fields, o2o_fields, bo2o_fields, m2m_fields):
+                    if field_name in set_:
+                        set_.remove(field_name)
+                try:
+                    del data[field_name]
+                except KeyError:
+                    pass
+        return data
+
+    async def _clean_field_default(
+            self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
+            instance: Optional[DB_MODEL], create: bool
+    ) -> bool:
+        if create:
+            return False
+        return getattr(instance, field_name) == data[field_name]
+
+    async def _clean_fk_field_default(
+            self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
+            instance: Optional[DB_MODEL], create: bool
+    ) -> bool:
+        return await self._clean_field_default(
+            model=model, data=data, field_name=field_name,
+            instance=instance, create=create
+        )
+
+    async def _clean_bfk_field_default(
+            self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
+            instance: Optional[DB_MODEL], create: bool
+    ) -> bool:
+        if not create:
+            value: list[dict[str, Any]] = data[field_name]
+            bfk_model = self._get_bfk_model(model=model, field_name=field_name)
+            bfk_pk_attr = self._get_pk_attr(bfk_model)
+            data_before: list[DB_MODEL] = await getattr(instance, field_name).all()
+            remove_pks = []
+            current_pks = [item_pk for item in value if (item_pk := item.get(bfk_pk_attr)) is not None]
+            for item in data_before:
+                if item.pk not in current_pks:
+                    remove_pks.append(item.pk)
+            if remove_pks:
+                data[self.BFK_REMOVE_FIELDS_PATTERN.format(field_name)] = remove_pks
+        return False
+
+    async def _clean_o2o_field_default(
+            self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
+            instance: Optional[DB_MODEL], create: bool
+    ) -> bool:
+        return False
+
+    async def _clean_bo2o_field_default(
+            self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
+            instance: Optional[DB_MODEL], create: bool
+    ) -> bool:
+        return False
+
+    async def _clean_m2m_field_default(
+            self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
+            instance: Optional[DB_MODEL], create: bool
+    ) -> bool:
+        return False
+
+    async def check_unique(self, data: dict[str, Any], model: Type[DB_MODEL], prefix: ModelPrefix) -> None:
+        errors = ObjectErrors()
+        for field_name in model._meta.db_fields:
+            field = model._meta.fields_map[field_name]
+            if not field.unique or field.generated:
+                continue
+            if value := data.get(field_name) is not None:
+                if hasattr(self, f'check_unique_{prefix.plus(field_name)}'):
+                    check_unique_func = getattr(self, f'check_unique_{prefix.plus(field_name)}')
+                else:
+                    check_unique_func = self._check_unique_default
+                if await check_unique_func(model=model, field_name=field_name, value=value):
+                    errors.add(field_name, NotUnique)
+        if errors:
+            raise errors
+
+    async def _check_unique_default(self, model: Type[DB_MODEL], field_name: str, value: Any) -> bool:
+        if field_name in model.IEXACT_FIELDS:
+            field_name = field_name + '__iexact'
+        return await model.filter(**{field_name: value}).exists()
+
+    @classmethod
+    def _get_bfk_model(cls, model: Type[BaseModel], field_name: str) -> Type[BaseModel]:
+        return model._meta.fields_map[field_name].related_model
+
+    @classmethod
+    def _get_pk_attr(cls, model: Type[BaseModel]) -> str:
+        return model._meta.pk_attr
 
     @classmethod
     def get_default_sort_fields(cls) -> set[str]:
         return {*cls.opts.db_fields}
 
-    def _default_fk_get_instance(self, model: Type[DB_MODEL]) -> FKGetInstance[PK, DB_MODEL]:
-        async def func(repository: Self, pk: PK) -> Optional[DB_MODEL]:
-            return await model.get_or_none(pk=pk)
-        return func
+    async def _fk_get_default(self, model: Type[DB_MODEL], pk: PK) -> DB_MODEL:
+        return await model.get_or_none(pk=pk)
 
 
 def get_exclude_dict(fields: set[str]) -> dict[str, set[str]]:
     """
     Из {a, b, c.d, c.e, f.g.h, f.g.i} делает
     {
         '__root__': {'a', 'b'},
@@ -634,25 +841,33 @@
         else:
             base, _, field_in_related = field.partition('.')
             exclude_dict[base].add(field_in_related)
     return exclude_dict
 
 
 def exclude_fk_bfk_o2o_bo2o_m2m(
-        model: Type[BaseModel], data: CamelModel
+        model: Type[DB_MODEL], data: dict[str, Any]
 ) -> tuple[set[str], set[str], set[str], set[str], set[str]]:
     opts = model._meta
     return (
         exclude_fields_from_data(data, *(opts.fields_map[f].source_field for f in opts.fk_fields)),
         exclude_fields_from_data(data, *opts.backward_fk_fields),
         exclude_fields_from_data(data, *opts.o2o_fields),
         exclude_fields_from_data(data, *opts.backward_o2o_fields),
         exclude_fields_from_data(data, *opts.m2m_fields)
     )
 
 
-def exclude_fields_from_data(data: CamelModel, *fields: str) -> set[str]:
+def exclude_fields_from_data(data: dict[str, Any], *fields: str) -> set[str]:
     return_fields: set[str] = set()
     for field_name in fields:
-        if field_name in data.__fields_set__:
+        if field_name in data:
             return_fields.add(field_name)
     return return_fields
+
+
+def field_is_required(field: Field) -> bool:
+    if isinstance(field, (DateField, DatetimeField, TimeField)) and (field.auto_now or field.auto_now_add):
+        return False
+    if field.required:
+        return True
+    return False
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/simple.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/simple.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/filters/str.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/base.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from collections.abc import Callable
 from typing import Any, Type
 
 from tortoise import Model as DefaultModel
 
 
 class BaseModel(DefaultModel):
+    IEXACT_FIELDS: set[str] = ()
 
     class Meta:
         abstract = True
-
-    @classmethod
-    async def check_unique(cls, data: dict[str, Any]) -> list[str]:
-        # TODO: self.__class__._meta.unique_together
-        not_unique = []
-        query = cls.all()
-        for key, value in cls._meta.fields_map.items():
-            if (
-                    not value.generated
-                    and value.unique
-                    and (current_value := data.get(key)) is not None
-            ):
-                if await query.filter(**{key: current_value}).exists():
-                    not_unique.append(key)
-        return not_unique
+    #
+    # @classmethod
+    # async def check_unique(cls, data: dict[str, Any]) -> list[str]:
+    #     # TODO: self.__class__._meta.unique_together
+    #     not_unique = []
+    #     query = cls.all()
+    #     for key, value in cls._meta.fields_map.items():
+    #         if (
+    #                 not value.generated
+    #                 and value.unique
+    #                 and (current_value := data.get(key)) is not None
+    #         ):
+    #             if await query.filter(**{key: current_value}).exists():
+    #                 not_unique.append(key)
+    #     return not_unique
 
 
 def get_field_param(model: Type[BaseModel], field_name: str, field_param: str):
     return getattr(model._meta.fields_map[field_name], field_param)
 
 
 def max_len_of(model: Type[BaseModel]) -> Callable[[str], int]:
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/base_user.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/base_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime, timedelta
 from uuid import UUID, uuid4
 
 from tortoise import fields, timezone
 
 from fastapi_all_out.lazy import get_user_model_path
 from fastapi_all_out.enums import TempCodeTriggers
-from . import BaseModel, PermissionMixin, max_len_of
+from . import BaseModel, PermissionMixin, max_len_of, ContentType
 
 
 USER_GET_BY_FIELDS = Literal['id', 'email', 'username', 'phone']
 
 
 class BaseUser(BaseModel):
     id: int
@@ -32,14 +32,26 @@
     created_at: datetime = fields.DatetimeField(auto_now_add=True)
 
     temp_code: Union["BaseTempCode", fields.BackwardOneToOneRelation["BaseTempCode"]]
 
     class Meta:
         abstract = True
 
+    @property
+    def is_authenticated(self) -> bool:
+        return True
+
+    @property
+    def display_name(self) -> str:
+        return self.username
+
+    @property
+    def is_simple(self) -> bool:
+        return True
+
 
 class UserWithPermissions(BaseUser, PermissionMixin):
     class Meta:
         abstract = True
 
 
 def get_random_tempcode(code_len: int) -> Callable[[], str]:
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/content_type.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/content_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/contrib/tortoise/models/permissions.py` & `fastapi_all_out-0.1.2/fastapi_all_out/contrib/tortoise/models/permissions.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,7 +47,22 @@
 
     class Meta:
         abstract = True
 
     @property
     def all_permissions(self) -> set[Permission]:
         return {*self.permissions, *(p for g in self.groups for p in g.permissions)}
+
+    def get_permissions_as_tuples(self) -> tuple[tuple[int, str], ...]:
+        return tuple((perm.content_type_id, perm.name) for perm in self.all_permissions)
+
+    def has_permissions(self, *permissions: tuple[str, str]) -> bool:
+        if not permissions:
+            return True
+        user_perms = self.get_permissions_as_tuples()
+        has = True
+        for model_name, perm_name in permissions:
+            content_type_id = ContentType.get_by_name(model_name).id
+            if (content_type_id, perm_name) not in user_perms:
+                has = False
+                break
+        return has
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/management/command.py` & `fastapi_all_out-0.1.2/fastapi_all_out/management/command.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/camel_model.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/camel_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/comma_separated.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/comma_separated.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/field_in_related_model.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/field_in_related_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/password.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/phonenumber.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/phonenumber.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/related_list.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/related_list.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/pydantic/fields/username.py` & `fastapi_all_out-0.1.2/fastapi_all_out/pydantic/fields/username.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/base_repository.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/base_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,60 @@
-from abc import ABC, abstractmethod
-from typing import Type, Any, TypeVar, Generic, Optional, Protocol, Callable, Coroutine
+from abc import abstractmethod
+from typing import Type, Any, TypeVar, Generic, Optional, Callable, Coroutine, TypedDict
 from uuid import UUID
 
-from fastapi import Request, BackgroundTasks
+from fastapi import Request, BackgroundTasks, Response
 
-from fastapi_all_out.pydantic import CamelModel
 from fastapi_all_out.lazy import get_auth_backend
-from .base_repository_meta import BaseRepositoryMeta
 from .filters import BaseFilter
 
 
 SERVICE = TypeVar('SERVICE', bound="BaseCRUDService")
 PK = TypeVar('PK', int, UUID)
 DB_MODEL = TypeVar('DB_MODEL')
 
 
-class CreateHandler(Protocol[DB_MODEL]):
-    async def __call__(
-            self,
-            data: CamelModel,
-            exclude: set[str],
-            defaults: dict[str, Any] = None
-    ) -> DB_MODEL: ...
-
-
-class EditHandler(Protocol[DB_MODEL]):
-    async def __call__(
-            self,
-            instance: DB_MODEL,
-            data: CamelModel,
-            exclude: set[str],
-            defaults: dict[str, Any] = None
-    ) -> DB_MODEL: ...
-
-
-class FKGetInstance(Protocol[PK, DB_MODEL]):
-    async def __call__(self, repository: "BaseRepository", pk: PK) -> Optional[DB_MODEL]: ...
-
-
 class ModelPrefix(str):
-    def plus(self, field_name: str):
+    def plus(self, field_name: str | int):
         if self == '':
             return self.__class__(field_name)
         else:
             return self.__class__(f'{self}__{field_name}')
 
 
-class BaseRepository(Generic[DB_MODEL], ABC, metaclass=BaseRepositoryMeta):
+class Updated(Generic[DB_MODEL], TypedDict):
+    instance: DB_MODEL
+    fields: set[str]
+
+
+class BaseRepository(Generic[DB_MODEL]):
     model: Type[DB_MODEL]
     pk_attr: str
     node_key: str
     pk_field_type: Type[PK]
 
-    create_handlers: dict[str, CreateHandler[DB_MODEL]]
-    edit_handlers: dict[str, EditHandler[DB_MODEL]]
-    fk_get_instance_map: dict[str, FKGetInstance[PK, DB_MODEL]]
-    defaults: dict[str, dict[str, Any]]
+    defaults: dict[str, dict[str, Any]] = None  # {"field": value, "o2o": {"field": "value"}}
+    pass_check_required: dict[str, set[str]] = None  # {"": {'a', 'b'}, "submodel__subsubmodel": {'a', 'b'}}
 
     request: Optional[Request]
     background_tasks: Optional[BackgroundTasks]
+    response: Optional[Response]
+
+    updated: dict[str, Updated]
 
-    def __init__(self, *, request: Request = None, background_tasks: BackgroundTasks = None):
+    def __init__(
+            self,
+            *,
+            request: Optional[Request] = None,
+            background_tasks: Optional[BackgroundTasks] = None,
+            response: Optional[Response] = None
+    ):
         self.request = request
         self.background_tasks = background_tasks
+        self.response = response
 
     @abstractmethod
     def get_queryset(self): ...
 
     @abstractmethod
     async def get_all(
             self,
@@ -84,73 +72,82 @@
 
     @abstractmethod
     async def get_tree_node(self, node_id: Optional[PK]) -> list[DB_MODEL]: ...
 
     @abstractmethod
     async def create(
             self,
-            data: CamelModel,
+            data: dict[str, Any],
             *,
             model: Type[DB_MODEL] = None,
             exclude: set[str] = None,
             defaults: dict[str, Any] = None,
             inside_transaction: bool = False,
             prefix: ModelPrefix = ModelPrefix(),
     ) -> DB_MODEL: ...
 
+    async def post_create(self, instance: DB_MODEL) -> None:
+        pass
+
+    async def post_create_background(self, instance: DB_MODEL) -> None:
+        pass
+
     @abstractmethod
     async def edit(
             self,
             instance: DB_MODEL,
-            data: CamelModel,
+            data: dict[str, Any],
             *,
             exclude: set[str] = None,
             defaults: dict[str, Any] = None,
             inside_transaction: bool = False,
             prefix: ModelPrefix = ModelPrefix(),
     ) -> DB_MODEL: ...
 
-    @abstractmethod
-    async def delete_many(self, item_ids: list[PK]) -> int: ...
+    async def post_edit(self, updated: dict[str, Updated[DB_MODEL]]) -> None:
+        pass
+
+    async def post_edit_background(self, updated: dict[str, Updated[DB_MODEL]]) -> None:
+        pass
 
     @abstractmethod
-    async def delete_one(self, item_id: PK) -> None: ...
+    async def delete_many(self, instances: list[PK]) -> int: ...
 
-    @classmethod
-    def with_model_permissions(cls, name: str) -> Callable[[...], Coroutine]:
-        return get_auth_backend().get_auth_with_permissions((cls.model.__name__, name))
+    @abstractmethod
+    async def delete_one(self, instance: DB_MODEL) -> None: ...
 
     @classmethod
-    def check_auth(cls) -> Callable[[...], Coroutine]:
-        return get_auth_backend().check_auth()
+    def with_model_permissions(cls, name: str) -> Callable[[...], Coroutine[Any, Any, None]]:
+        return get_auth_backend().with_permissions((cls.model.__name__, name))
 
     @classmethod
-    def with_create_permissions(cls) -> Callable[[...], Coroutine]:
+    def with_create_permissions(cls) -> Callable[[...], Coroutine[Any, Any, None]]:
         return cls.with_model_permissions('create')
 
     @classmethod
-    def with_get_permissions(cls) -> Callable[[...], Coroutine]:
+    def with_get_permissions(cls) -> Callable[[...], Coroutine[Any, Any, None]]:
         return cls.with_model_permissions('get')
 
     @classmethod
-    def with_edit_permissions(cls) -> Callable[[...], Coroutine]:
+    def with_edit_permissions(cls) -> Callable[[...], Coroutine[Any, Any, None]]:
         return cls.with_model_permissions('edit')
 
     @classmethod
-    def with_delete_permissions(cls) -> Callable[[...], Coroutine]:
+    def with_delete_permissions(cls) -> Callable[[...], Coroutine[Any, Any, None]]:
         return cls.with_model_permissions('delete')
 
     @classmethod
     @abstractmethod
     def get_default_sort_fields(cls) -> set[str]: ...
 
     def get_defaults(self, prefix: ModelPrefix) -> dict[str, Any]:
-        return self.defaults.get(prefix, {})
+        if self.defaults:
+            return self.defaults.get(prefix, {})
+        return {}
 
-    def get_fk_get_instance(self, prefix: ModelPrefix, model: Type[DB_MODEL]) -> FKGetInstance[PK, DB_MODEL]:
-        func = self.fk_get_instance_map.get(prefix)
-        if func is None:
-            func = self.fk_get_instance_map[prefix] = self._default_fk_get_instance(model=model)
-        return func
+    def get_pass_check_required(self, prefix: ModelPrefix) -> set[str]:
+        if self.pass_check_required:
+            return self.pass_check_required.get(prefix, set())
+        return set()
 
     @abstractmethod
-    def _default_fk_get_instance(self, model: Type[DB_MODEL]) -> FKGetInstance[PK, DB_MODEL]: ...
+    def _fk_get_default(self, model: Type[DB_MODEL], pk: PK) -> DB_MODEL: ...
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/crud_router.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/crud_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 
 from fastapi import Response, Request, APIRouter, Body, Path, Query, params, Depends, BackgroundTasks
 from fastapi.exceptions import RequestValidationError
 from pydantic.error_wrappers import ErrorWrapper
 
 from fastapi_all_out.code_responses import BaseCodes
 from fastapi_all_out.pydantic import CommaSeparatedOf, lower_camel, CamelModel
-from fastapi_all_out.lazy import get_codes
+from fastapi_all_out.lazy import get_codes, get_auth_backend
 from fastapi_all_out.responses import BgHTTPException
 from fastapi_all_out.routers import BaseRepository
 from .exceptions import ItemNotFound, ObjectErrors
 from .filters import BaseFilter
 from .utils import pagination_factory, PAGINATION, get_filters, sort_factory
 
 
 DISPLAY_FIELDS = tuple[str, ...]
 REPO = TypeVar('REPO', bound=BaseRepository)
 DEPENDENCIES = Optional[Sequence[params.Depends]]
 ROUTES_KWARGS = dict[str, bool | dict[str, Any]]
 
-
 Codes = get_codes()
 
 
 class CRUDRouter(Generic[REPO], APIRouter):
     repo: Type[BaseRepository]
     max_items_get_many_routes: Optional[int]
     max_items_delete_many_routes: Optional[int]
@@ -136,15 +135,15 @@
                 response: Response,
                 pagination: PAGINATION = pagination_factory(self.max_page_size),
                 sort: set[str] = Depends(sort_factory(self.available_sort)),
                 applied_filters: list[BaseFilter] = Depends(get_filters(self.filters))
         ):
             raise_if_error_in_filters(applied_filters)
             skip, limit = pagination
-            repository = self.repo(request=request, background_tasks=background_tasks)
+            repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             result, total = await repository.get_all(
                 skip=skip,
                 limit=limit,
                 sort=sort,
                 filters=applied_filters,
             )
             response.headers.append('X-Total-Count', str(total))
@@ -156,33 +155,35 @@
         pk_field_type = self.repo.pk_field_type
         max_items = self.max_items_get_many_routes
         read_many_schema = self.get_read_many_schema()
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 item_ids: CommaSeparatedOf(pk_field_type, max_items=max_items, in_query=True) = Query(..., alias='ids')
         ):
-            repository = self.repo(request=request, background_tasks=background_tasks)
+            repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             results = await repository.get_many(item_ids)
             return [read_many_schema.from_orm(r) for r in results]
 
         return route
 
     def _get_one_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         read_schema = self.get_read_schema()
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 item_id: pk_field_type = Path(...),
         ):
             try:
-                repository = self.repo(request=request, background_tasks=background_tasks)
+                repository = self.repo(request=request, background_tasks=background_tasks, response=response)
                 item = await repository.get_one(item_id)
             except ItemNotFound:
                 raise self.not_found_error()
             return read_schema.from_orm(item)
 
         return route
 
@@ -190,91 +191,97 @@
         pk_field_type = self.repo.pk_field_type
         get_list_item_schema = self.get_read_list_item_schema()
         alias = lower_camel(self.repo.node_key)
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 node_id: Optional[pk_field_type] = Query(None, alias=alias)
         ):
-            repository = self.repo(request=request, background_tasks=background_tasks)
+            repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             return [get_list_item_schema.from_orm(item) for item in await repository.get_tree_node(node_id)]
 
         return route
 
     def _create_route(self) -> Callable[..., Any]:
         create_schema = self.get_create_schema()
         read_schema = self.get_read_schema()
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 data: create_schema = Body(...)
         ):
             try:
-                repository = self.repo(request=request, background_tasks=background_tasks)
-                instance = await repository.create(data)
+                instance = await self.repo(request=request, background_tasks=background_tasks, response=response)\
+                    .create(data.dict(exclude_unset=True))
             except ObjectErrors as e:
                 raise self.field_errors(e)
             return read_schema.from_orm(instance)
 
         return route
 
     def _edit_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         read_schema = self.get_read_schema()
         edit_schema = self.get_edit_schema()
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 item_id: pk_field_type = Path(...),
                 data: edit_schema = Body(...)
         ):
-            repository = self.repo(request=request, background_tasks=background_tasks)
+            repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             try:
                 instance = await repository.get_one(item_id)
             except ItemNotFound:
                 raise self.not_found_error()
             try:
-                instance = await repository.edit(instance, data)
+                instance = await repository.edit(instance, data.dict(exclude_unset=True))
             except ObjectErrors as e:
                 raise self.field_errors(e)
             return read_schema.from_orm(instance)
 
         return route
 
     def _delete_many_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         max_items = self.max_items_get_many_routes
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 item_ids: CommaSeparatedOf(pk_field_type, max_items=max_items, in_query=True) = Query(..., alias='ids')
         ):
-            repository = self.repo(request=request, background_tasks=background_tasks)
+            repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             deleted_items_count = await repository.delete_many(item_ids)
             return self.ok_response(count=deleted_items_count)
 
         return route
 
     def _delete_one_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
 
         async def route(
                 request: Request,
                 background_tasks: BackgroundTasks,
+                response: Response,
                 item_id: pk_field_type = Path(...)
         ):
+            repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             try:
-                repository = self.repo(request=request, background_tasks=background_tasks)
-                await repository.delete_one(item_id)
+                instance = await repository.get_one(item_id)
             except ItemNotFound:
                 raise self.not_found_error()
+            await repository.delete_one(instance=instance)
             return self.ok_response(item=item_id)
 
         return route
 
     @classmethod
     def _ok_response_instance(cls) -> BaseCodes:
         return Codes.OK
@@ -320,15 +327,15 @@
             route_name: str,
             route_kwargs: dict[str, Any],
     ) -> None:
         responses = {}
         response_model = None
         status = 200
         openapi_extra = None
-        route_kwargs = {**self.routes_kwargs.get('all', {}), ** route_kwargs}
+        route_kwargs = {**self.routes_kwargs.get('all', {}), **route_kwargs}
         match route_name:
             case 'get_all':
                 path = '/all'
                 method = ["GET"]
                 response_model = list[self.get_read_list_item_schema()]
                 check_perms_dependency = Depends(self.repo.with_get_permissions())
                 openapi_extra = {'parameters': [f.query_openapi_desc() for f in self.filters]}
@@ -379,44 +386,43 @@
             case _:
                 raise Exception(f'Unknown name of route: {route_name}.\n'
                                 f'Available are {", ".join(self.default_routes_names())}')
         summary = f"{route_name.title().replace('_', ' ')} {self.repo.model.__name__}"
 
         if route_kwargs.get('check_perms', True):
             dependencies = [*self.auto_routes_dependencies, check_perms_dependency]
-        elif route_kwargs.get('check_auth', True):
-            dependencies = [*self.auto_routes_dependencies, Depends(self.repo.check_auth())]
+        elif route_kwargs.get('auth_required', True):
+            dependencies = [*self.auto_routes_dependencies, Depends(get_auth_backend().auth_required())]
         else:
             dependencies = [*self.auto_routes_dependencies]
-        route_kwargs = get_route_kwargs(route_kwargs, dependencies, responses)
 
         self.add_api_route(
             path=path,
             endpoint=getattr(self, f'_{route_name}_route')(),
             methods=method,
             response_model=response_model,
             summary=summary,
             status_code=status,
             openapi_extra=openapi_extra,
-            **route_kwargs,
+            **get_route_kwargs(route_kwargs, dependencies, responses),
         )
 
-    def get_read_schema(self):
+    def get_read_schema(self) -> Type[CamelModel]:
         return self.read_schema
 
-    def get_read_many_schema(self):
+    def get_read_many_schema(self) -> Type[CamelModel]:
         return self.read_many_schema
 
-    def get_read_list_item_schema(self):
+    def get_read_list_item_schema(self) -> Type[CamelModel]:
         return self.read_list_item_schema
 
-    def get_create_schema(self):
+    def get_create_schema(self) -> Type[CamelModel]:
         return self.create_schema
 
-    def get_edit_schema(self):
+    def get_edit_schema(self) -> Type[CamelModel]:
         return self.edit_schema
 
 
 def get_route_kwargs(
         route_data: dict[str, Any],
         dependencies: DEPENDENCIES,
         responses: dict[str, Any],
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/exceptions.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,27 +32,30 @@
         super().__init__(*args)
         self.objects_map = {}
 
     def append(self, index: int, err: Union[Type["FieldError"], "FieldError", "ObjectErrors"]):
         self.objects_map[index] = err
 
     def to_error(self):
-        return {key: error.to_error() for key, error in self.objects_map.items()}
+        return {index: error.to_error() for index, error in self.objects_map.items()}
 
     def __bool__(self):
         return not not self.objects_map
 
 
 class ObjectErrors(Exception):
     errors: dict[str, Union[Type["FieldError"], "FieldError", "ObjectErrors"]]
 
     def __init__(self, *args):
         super().__init__(*args)
         self.errors = {}
 
+    def __str__(self):
+        return str(self.to_error())
+
     def to_error(self):
         return {key: error.to_error() for key, error in self.errors.items()}
 
     def add(self, field: str, error: Union[Type["FieldError"], "FieldError", "ObjectErrors"]):
         self.errors[field] = error
 
     def merge(self, obj_error: "ObjectErrors") -> Self:
```

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/utils.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/base.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/bool.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/int.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/int.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/int_btw.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/int_btw.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/routers/filters/str.py` & `fastapi_all_out-0.1.2/fastapi_all_out/routers/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/templates/activation.html` & `fastapi_all_out-0.1.2/fastapi_all_out/templates/activation.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/fastapi_all_out/templates/password_reset.html` & `fastapi_all_out-0.1.2/fastapi_all_out/templates/password_reset.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/LICENSE.md` & `fastapi_all_out-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.1.1/pyproject.toml` & `fastapi_all_out-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["fastapi_all_out"]
 
 [project]
 name = "fastapi-all-out"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 maintainers = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "WEB", "Architecture", "Backend"]
-description = "Makes fastapi much easier, then Django"
+description = "Makes fastapi much easier and stronger, then Django"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python=">=3.11"
 dependencies = [
     'fastapi[all]>=0.89',
     'passlib>=1.7.4',
     'PyJWT>=2.6.0',
```

### Comparing `fastapi_all_out-0.1.1/PKG-INFO` & `fastapi_all_out-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastapi-all-out
-Version: 0.1.1
-Summary: Makes fastapi much easier, then Django
+Version: 0.1.2
+Summary: Makes fastapi much easier and stronger, then Django
 Project-URL: Github, https://github.com/alta7700/fastapi_all_out/
 Author-email: Alexandr Tamrazov <alta77@mail.ru>
 Maintainer-email: Alexandr Tamrazov <alta77@mail.ru>
 License: Copyright © 2023 Alexandr Tamrazov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

