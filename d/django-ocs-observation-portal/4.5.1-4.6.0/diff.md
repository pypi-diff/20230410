# Comparing `tmp/django-ocs-observation-portal-4.5.1.tar.gz` & `tmp/django_ocs_observation_portal-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ocs-observation-portal-4.5.1.tar", max compression
+gzip compressed data, was "django_ocs_observation_portal-4.6.0.tar", max compression
```

## Comparing `django-ocs-observation-portal-4.5.1.tar` & `django_ocs_observation_portal-4.6.0.tar`

### file list

```diff
@@ -1,203 +1,202 @@
--rw-r--r--   0        0        0    35149 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/LICENSE
--rw-r--r--   0        0        0    39207 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/README.md
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/admin.py
--rw-r--r--   0        0        0      224 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/apps.py
--rw-r--r--   0        0        0      651 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/backends.py
--rw-r--r--   0        0        0     2008 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/forms.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/__init__.py
--rw-r--r--   0        0        0     1970 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/create_application.py
--rw-r--r--   0        0        0     2027 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/create_user.py
--rw-r--r--   0        0        0      802 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/generateschema_mocked.py
--rw-r--r--   0        0        0     2416 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/init_e2e_credentials.py
--rw-r--r--   0        0        0     1403 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/updateclientusers.py
--rw-r--r--   0        0        0     1276 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/migrations/0002_profile_terms_accepted.py
--rw-r--r--   0        0        0      835 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/migrations/0003_bulk_create_users_api.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/migrations/__init__.py
--rw-r--r--   0        0        0     3589 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/models.py
--rw-r--r--   0        0        0     5648 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/0001_initial.py
--rw-r--r--   0        0        0     3266 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py
--rw-r--r--   0        0        0     1714 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/__init__.py
--rw-r--r--   0        0        0     1841 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/permissions.py
--rw-r--r--   0        0        0     9168 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/serializers.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.139541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/signals/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/signals/handlers.py
--rw-r--r--   0        0        0     2065 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/tasks.py
--rw-r--r--   0        0        0      197 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/auth/logged_in_state.html
--rw-r--r--   0        0        0      170 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/base.html
--rw-r--r--   0        0        0      330 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/bulkapi-account-created-email.txt
--rw-r--r--   0        0        0      638 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/redoc.html
--rw-r--r--   0        0        0      589 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/registration/activation_complete.html
--rw-r--r--   0        0        0     2131 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/registration/activation_email.html
--rwxr-xr-x   0        0        0      483 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/registration/login.html
--rw-r--r--   0        0        0      327 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/registration/registration_form.html
--rw-r--r--   0        0        0      974 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/test_utils.py
--rw-r--r--   0        0        0     9376 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/test_views.py
--rw-r--r--   0        0        0    28161 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/tests.py
--rw-r--r--   0        0        0      281 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/throttling.py
--rw-r--r--   0        0        0      964 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/urls.py
--rw-r--r--   0        0        0     6522 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/accounts/views.py
--rw-r--r--   0        0        0       23 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/__init__.py
--rw-r--r--   0        0        0    35076 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/configdb.py
--rw-r--r--   0        0        0    26068 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/doc_examples.py
--rw-r--r--   0        0        0     3622 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/downtimedb.py
--rw-r--r--   0        0        0     1283 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/middleware.py
--rw-r--r--   0        0        0     2984 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/mixins.py
--rw-r--r--   0        0        0    15015 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/rise_set_utils.py
--rw-r--r--   0        0        0     8137 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/schema.py
--rw-r--r--   0        0        0    17629 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/state_changes.py
--rw-r--r--   0        0        0    14532 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/telescope_states.py
--rw-r--r--   0        0        0     2012 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_configdb.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/__init__.py
--rw-r--r--   0        0        0   106356 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/configdb.json
--rw-r--r--   0        0        0    14960 2023-04-04 23:01:40.143541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/doc_configdb.json
--rw-r--r--   0        0        0 10749196 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/es_telescope_states_data.txt
--rw-r--r--   0        0        0     4932 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_helpers.py
--rw-r--r--   0        0        0    54539 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_state_changes.py
--rw-r--r--   0        0        0    27685 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/common/test_telescope_states.py
--rw-r--r--   0        0        0     1773 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/common/utils.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/__init__.py
--rw-r--r--   0        0        0     2470 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/admin.py
--rw-r--r--   0        0        0      236 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/apps.py
--rw-r--r--   0        0        0     4596 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/filters.py
--rw-r--r--   0        0        0      614 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/forms.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.167541 django-ocs-observation-portal-4.5.1/observation_portal/observations/management/commands/__init__.py
--rw-r--r--   0        0        0     1661 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/management/commands/populate_time_charged.py
--rw-r--r--   0        0        0     6658 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/management/commands/time_accounting.py
--rw-r--r--   0        0        0     5063 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0001_initial.py
--rw-r--r--   0        0        0      399 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0002_auto_20190408_1908.py
--rw-r--r--   0        0        0      550 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0003_auto_20190514_0005.py
--rw-r--r--   0        0        0      473 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0004_observation_priority.py
--rw-r--r--   0        0        0     1069 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0005_auto_20210116_0033.py
--rw-r--r--   0        0        0      484 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0006_alter_summary_events.py
--rw-r--r--   0        0        0      358 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0007_alter_configurationstatus_unique_together.py
--rw-r--r--   0        0        0      542 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/__init__.py
--rw-r--r--   0        0        0    13134 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/models.py
--rw-r--r--   0        0        0    21866 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/serializers.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/signals/__init__.py
--rw-r--r--   0        0        0      981 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/signals/handlers.py
--rw-r--r--   0        0        0      443 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/tasks.py
--rw-r--r--   0        0        0      425 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/templates/observations/observation_changeform.html
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/test/__init__.py
--rw-r--r--   0        0        0   128718 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/test/tests.py
--rw-r--r--   0        0        0     5676 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/time_accounting.py
--rw-r--r--   0        0        0     2260 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/views.py
--rw-r--r--   0        0        0    11820 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/observations/viewsets.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/__init__.py
--rw-r--r--   0        0        0     4110 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/admin.py
--rw-r--r--   0        0        0      227 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/apps.py
--rw-r--r--   0        0        0     2867 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/filters.py
--rw-r--r--   0        0        0     4731 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/forms.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/management/commands/__init__.py
--rw-r--r--   0        0        0     4286 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/management/commands/create_proposal.py
--rw-r--r--   0        0        0     1445 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/management/commands/create_semester.py
--rw-r--r--   0        0        0     6532 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0001_initial.py
--rw-r--r--   0        0        0     1172 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0002_auto_20190815_1942.py
--rw-r--r--   0        0        0      461 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0003_auto_20210203_0022.py
--rw-r--r--   0        0        0      690 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0004_auto_20210617_0908.py
--rw-r--r--   0        0        0      733 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0005_auto_20210604_2154.py
--rw-r--r--   0        0        0      631 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0006_auto_20210604_2155.py
--rw-r--r--   0        0        0      595 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py
--rw-r--r--   0        0        0      910 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0008_auto_20210708_1623.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/__init__.py
--rw-r--r--   0        0        0    13225 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/models.py
--rw-r--r--   0        0        0     2597 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/notifications.py
--rw-r--r--   0        0        0     2784 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/serializers.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/signals/__init__.py
--rw-r--r--   0        0        0      654 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/signals/handlers.py
--rw-r--r--   0        0        0      726 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/tasks.py
--rw-r--r--   0        0        0      280 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/added.txt
--rw-r--r--   0        0        0      309 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/invitation.txt
--rw-r--r--   0        0        0      750 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/requestfailurelimit.txt
--rw-r--r--   0        0        0      527 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt
--rw-r--r--   0        0        0     1380 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/timeallocationreminder.html
--rw-r--r--   0        0        0    45521 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/test_api.py
--rw-r--r--   0        0        0    18777 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/tests.py
--rw-r--r--   0        0        0    13908 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/proposals/viewsets.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/__init__.py
--rw-r--r--   0        0        0     5060 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/admin.py
--rw-r--r--   0        0        0      239 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/apps.py
--rw-r--r--   0        0        0     2053 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/cadence.py
--rw-r--r--   0        0        0     8095 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/contention.py
--rw-r--r--   0        0        0    16127 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/duration_utils.py
--rw-r--r--   0        0        0     3126 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/filters.py
--rw-r--r--   0        0        0      766 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/forms.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/management/commands/__init__.py
--rw-r--r--   0        0        0    14120 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/management/commands/create_example_requests.py
--rw-r--r--   0        0        0    25262 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0001_initial.py
--rw-r--r--   0        0        0     2533 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py
--rw-r--r--   0        0        0      594 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py
--rw-r--r--   0        0        0      575 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py
--rw-r--r--   0        0        0      385 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0005_auto_20190501_2103.py
--rw-r--r--   0        0        0      926 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py
--rw-r--r--   0        0        0      922 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py
--rw-r--r--   0        0        0      589 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py
--rw-r--r--   0        0        0      977 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py
--rw-r--r--   0        0        0     2180 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py
--rw-r--r--   0        0        0      536 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py
--rw-r--r--   0        0        0     1488 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py
--rw-r--r--   0        0        0     1158 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py
--rw-r--r--   0        0        0     1036 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py
--rw-r--r--   0        0        0     1072 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py
--rw-r--r--   0        0        0      456 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0016_auto_20210525_0643.py
--rw-r--r--   0        0        0      546 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0017_request_extra_params.py
--rw-r--r--   0        0        0     2512 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py
--rw-r--r--   0        0        0      731 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py
--rw-r--r--   0        0        0      681 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py
--rw-r--r--   0        0        0      586 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0021_request_optimization_type.py
--rw-r--r--   0        0        0      577 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py
--rw-r--r--   0        0        0      632 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/__init__.py
--rw-r--r--   0        0        0    36336 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/models.py
--rw-r--r--   0        0        0     8037 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/pattern_expansion.py
--rw-r--r--   0        0        0     7545 2023-04-04 23:01:40.171541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/request_utils.py
--rw-r--r--   0        0        0    53248 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/serializers.py
--rw-r--r--   0        0        0       23 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/signals/__init__.py
--rw-r--r--   0        0        0     1538 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/signals/handlers.py
--rw-r--r--   0        0        0     4344 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/target_helpers.py
--rw-r--r--   0        0        0      296 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/tasks.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/__init__.py
--rw-r--r--   0        0        0   595296 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/data/blocks.json
--rw-r--r--   0        0        0    37647 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test.py
--rw-r--r--   0        0        0   188357 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_api.py
--rw-r--r--   0        0        0     3346 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_cadence.py
--rw-r--r--   0        0        0     2596 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_helpers.py
--rw-r--r--   0        0        0    42192 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_request_utils.py
--rw-r--r--   0        0        0     4295 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_views.py
--rw-r--r--   0        0        0    10712 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/views.py
--rw-r--r--   0        0        0    19248 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/viewsets.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/__init__.py
--rw-r--r--   0        0        0     4712 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/admin.py
--rw-r--r--   0        0        0      124 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/apps.py
--rw-r--r--   0        0        0     1718 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/filters.py
--rw-r--r--   0        0        0     5775 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0001_initial.py
--rw-r--r--   0        0        0      450 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0002_timerequest_instrument_types.py
--rw-r--r--   0        0        0      620 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py
--rw-r--r--   0        0        0      346 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0004_remove_timerequest_instrument.py
--rw-r--r--   0        0        0      728 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py
--rw-r--r--   0        0        0        0 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/__init__.py
--rw-r--r--   0        0        0    10686 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/models.py
--rw-r--r--   0        0        0    13642 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/serializers.py
--rw-r--r--   0        0        0      375 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/templates/sciapplications/approved.txt
--rw-r--r--   0        0        0      318 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/templates/sciapplications/ddt_submitted.txt
--rw-r--r--   0        0        0    11505 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/test_admin.py
--rw-r--r--   0        0        0    54563 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/test_api.py
--rw-r--r--   0        0        0     7046 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/tests.py
--rw-r--r--   0        0        0     6480 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/viewsets.py
--rw-r--r--   0        0        0    23236 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/settings.py
--rw-r--r--   0        0        0      920 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/task_scheduler.py
--rw-r--r--   0        0        0      601 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/test_runner.py
--rw-r--r--   0        0        0     1776 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/test_settings.py
--rw-r--r--   0        0        0     5507 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/urls.py
--rw-r--r--   0        0        0      413 2023-04-04 23:01:40.175541 django-ocs-observation-portal-4.5.1/observation_portal/wsgi.py
--rw-r--r--   0        0        0     2037 2023-04-04 23:01:40.179541 django-ocs-observation-portal-4.5.1/pyproject.toml
--rw-r--r--   0        0        0    42581 2023-04-04 23:01:50.689923 django-ocs-observation-portal-4.5.1/setup.py
--rw-r--r--   0        0        0    41472 2023-04-04 23:01:50.692334 django-ocs-observation-portal-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 19:41:27.990839 django_ocs_observation_portal-4.6.0/LICENSE
+-rw-r--r--   0        0        0    39207 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/__init__.py
+-rw-r--r--   0        0        0     1187 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/admin.py
+-rw-r--r--   0        0        0      224 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/apps.py
+-rw-r--r--   0        0        0      651 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/backends.py
+-rw-r--r--   0        0        0     2008 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/forms.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/__init__.py
+-rw-r--r--   0        0        0     1970 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_application.py
+-rw-r--r--   0        0        0     2027 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_user.py
+-rw-r--r--   0        0        0      802 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/generateschema_mocked.py
+-rw-r--r--   0        0        0     2416 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/init_e2e_credentials.py
+-rw-r--r--   0        0        0     1403 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/updateclientusers.py
+-rw-r--r--   0        0        0     1276 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0002_profile_terms_accepted.py
+-rw-r--r--   0        0        0      835 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0003_bulk_create_users_api.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/__init__.py
+-rw-r--r--   0        0        0     3589 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/models.py
+-rw-r--r--   0        0        0     5648 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0001_initial.py
+-rw-r--r--   0        0        0     3266 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py
+-rw-r--r--   0        0        0     1714 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/__init__.py
+-rw-r--r--   0        0        0     1841 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/permissions.py
+-rw-r--r--   0        0        0     9168 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/signals/__init__.py
+-rw-r--r--   0        0        0     1272 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/signals/handlers.py
+-rw-r--r--   0        0        0     2065 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/tasks.py
+-rw-r--r--   0        0        0      197 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/auth/logged_in_state.html
+-rw-r--r--   0        0        0      170 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/base.html
+-rw-r--r--   0        0        0      330 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/bulkapi-account-created-email.txt
+-rw-r--r--   0        0        0      638 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/redoc.html
+-rw-r--r--   0        0        0      589 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_complete.html
+-rw-r--r--   0        0        0     2131 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_email.html
+-rwxr-xr-x   0        0        0      483 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/login.html
+-rw-r--r--   0        0        0      327 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/registration_form.html
+-rw-r--r--   0        0        0      974 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_utils.py
+-rw-r--r--   0        0        0     9376 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_views.py
+-rw-r--r--   0        0        0    28161 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/tests.py
+-rw-r--r--   0        0        0      281 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/throttling.py
+-rw-r--r--   0        0        0      964 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/urls.py
+-rw-r--r--   0        0        0     6522 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/accounts/views.py
+-rw-r--r--   0        0        0       23 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/__init__.py
+-rw-r--r--   0        0        0    35076 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/configdb.py
+-rw-r--r--   0        0        0    26068 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/doc_examples.py
+-rw-r--r--   0        0        0     3622 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/downtimedb.py
+-rw-r--r--   0        0        0     1283 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/middleware.py
+-rw-r--r--   0        0        0     2984 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/mixins.py
+-rw-r--r--   0        0        0    15015 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/rise_set_utils.py
+-rw-r--r--   0        0        0     8137 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/schema.py
+-rw-r--r--   0        0        0    17629 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/state_changes.py
+-rw-r--r--   0        0        0    14532 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/telescope_states.py
+-rw-r--r--   0        0        0     2012 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/test_configdb.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:27.994839 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/__init__.py
+-rw-r--r--   0        0        0   106356 2023-04-10 19:41:27.998840 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/configdb.json
+-rw-r--r--   0        0        0    14960 2023-04-10 19:41:27.998840 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/doc_configdb.json
+-rw-r--r--   0        0        0 10749196 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/es_telescope_states_data.txt
+-rw-r--r--   0        0        0     4932 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_helpers.py
+-rw-r--r--   0        0        0    54539 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_state_changes.py
+-rw-r--r--   0        0        0    27685 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/test_telescope_states.py
+-rw-r--r--   0        0        0     1773 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/common/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/__init__.py
+-rw-r--r--   0        0        0     2470 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/admin.py
+-rw-r--r--   0        0        0      236 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/apps.py
+-rw-r--r--   0        0        0     4596 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/filters.py
+-rw-r--r--   0        0        0      614 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/forms.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1661 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/populate_time_charged.py
+-rw-r--r--   0        0        0     6658 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/time_accounting.py
+-rw-r--r--   0        0        0     5063 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0001_initial.py
+-rw-r--r--   0        0        0      399 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0002_auto_20190408_1908.py
+-rw-r--r--   0        0        0      550 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0003_auto_20190514_0005.py
+-rw-r--r--   0        0        0      473 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0004_observation_priority.py
+-rw-r--r--   0        0        0     1069 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0005_auto_20210116_0033.py
+-rw-r--r--   0        0        0      484 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0006_alter_summary_events.py
+-rw-r--r--   0        0        0      358 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0007_alter_configurationstatus_unique_together.py
+-rw-r--r--   0        0        0      542 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/__init__.py
+-rw-r--r--   0        0        0    13134 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/models.py
+-rw-r--r--   0        0        0    21866 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.026842 django_ocs_observation_portal-4.6.0/observation_portal/observations/signals/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/signals/handlers.py
+-rw-r--r--   0        0        0      443 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/tasks.py
+-rw-r--r--   0        0        0      425 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/templates/observations/observation_changeform.html
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/test/__init__.py
+-rw-r--r--   0        0        0   128718 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/test/tests.py
+-rw-r--r--   0        0        0     5676 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/time_accounting.py
+-rw-r--r--   0        0        0     2260 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/views.py
+-rw-r--r--   0        0        0    11820 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/observations/viewsets.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/__init__.py
+-rw-r--r--   0        0        0     4401 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/admin.py
+-rw-r--r--   0        0        0      227 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/apps.py
+-rw-r--r--   0        0        0     2867 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/filters.py
+-rw-r--r--   0        0        0     4731 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/forms.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/__init__.py
+-rw-r--r--   0        0        0     4286 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_proposal.py
+-rw-r--r--   0        0        0     1445 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_semester.py
+-rw-r--r--   0        0        0     6532 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1172 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0002_auto_20190815_1942.py
+-rw-r--r--   0        0        0      461 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0003_auto_20210203_0022.py
+-rw-r--r--   0        0        0      690 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0004_auto_20210617_0908.py
+-rw-r--r--   0        0        0      733 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0005_auto_20210604_2154.py
+-rw-r--r--   0        0        0      631 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0006_auto_20210604_2155.py
+-rw-r--r--   0        0        0      595 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py
+-rw-r--r--   0        0        0      910 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0008_auto_20210708_1623.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/__init__.py
+-rw-r--r--   0        0        0    13225 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/models.py
+-rw-r--r--   0        0        0     2597 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/notifications.py
+-rw-r--r--   0        0        0     2784 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/signals/__init__.py
+-rw-r--r--   0        0        0      654 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/signals/handlers.py
+-rw-r--r--   0        0        0      726 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/tasks.py
+-rw-r--r--   0        0        0      280 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/added.txt
+-rw-r--r--   0        0        0      309 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/invitation.txt
+-rw-r--r--   0        0        0      750 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestfailurelimit.txt
+-rw-r--r--   0        0        0      527 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt
+-rw-r--r--   0        0        0     1380 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/timeallocationreminder.html
+-rw-r--r--   0        0        0    45521 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/test_api.py
+-rw-r--r--   0        0        0    18777 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/tests.py
+-rw-r--r--   0        0        0    13908 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/proposals/viewsets.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/__init__.py
+-rw-r--r--   0        0        0     5060 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/admin.py
+-rw-r--r--   0        0        0      239 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/apps.py
+-rw-r--r--   0        0        0     2053 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/cadence.py
+-rw-r--r--   0        0        0     8095 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/contention.py
+-rw-r--r--   0        0        0    16127 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/duration_utils.py
+-rw-r--r--   0        0        0     3126 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/filters.py
+-rw-r--r--   0        0        0      766 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/forms.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/commands/__init__.py
+-rw-r--r--   0        0        0    14120 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/commands/create_example_requests.py
+-rw-r--r--   0        0        0    25262 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2533 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py
+-rw-r--r--   0        0        0      594 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py
+-rw-r--r--   0        0        0      575 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py
+-rw-r--r--   0        0        0      385 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0005_auto_20190501_2103.py
+-rw-r--r--   0        0        0      926 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py
+-rw-r--r--   0        0        0      922 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py
+-rw-r--r--   0        0        0      589 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py
+-rw-r--r--   0        0        0      977 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py
+-rw-r--r--   0        0        0     2180 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py
+-rw-r--r--   0        0        0      536 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py
+-rw-r--r--   0        0        0     1488 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py
+-rw-r--r--   0        0        0     1158 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py
+-rw-r--r--   0        0        0     1036 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py
+-rw-r--r--   0        0        0     1072 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py
+-rw-r--r--   0        0        0      456 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0016_auto_20210525_0643.py
+-rw-r--r--   0        0        0      546 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0017_request_extra_params.py
+-rw-r--r--   0        0        0     2512 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py
+-rw-r--r--   0        0        0      731 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py
+-rw-r--r--   0        0        0      681 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py
+-rw-r--r--   0        0        0      586 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0021_request_optimization_type.py
+-rw-r--r--   0        0        0      577 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py
+-rw-r--r--   0        0        0      632 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/__init__.py
+-rw-r--r--   0        0        0    36336 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/models.py
+-rw-r--r--   0        0        0     8037 2023-04-10 19:41:28.030842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/pattern_expansion.py
+-rw-r--r--   0        0        0     7545 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/request_utils.py
+-rw-r--r--   0        0        0    53248 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/serializers.py
+-rw-r--r--   0        0        0       23 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/signals/__init__.py
+-rw-r--r--   0        0        0     1538 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/signals/handlers.py
+-rw-r--r--   0        0        0     4344 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/target_helpers.py
+-rw-r--r--   0        0        0      296 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/__init__.py
+-rw-r--r--   0        0        0   595296 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/data/blocks.json
+-rw-r--r--   0        0        0    37647 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test.py
+-rw-r--r--   0        0        0   188357 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_api.py
+-rw-r--r--   0        0        0     3346 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_cadence.py
+-rw-r--r--   0        0        0     2596 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_helpers.py
+-rw-r--r--   0        0        0    42192 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_request_utils.py
+-rw-r--r--   0        0        0     4295 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_views.py
+-rw-r--r--   0        0        0    10712 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/views.py
+-rw-r--r--   0        0        0    19248 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/viewsets.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/__init__.py
+-rw-r--r--   0        0        0     4712 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/admin.py
+-rw-r--r--   0        0        0      124 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/apps.py
+-rw-r--r--   0        0        0     1718 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/filters.py
+-rw-r--r--   0        0        0     5775 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0001_initial.py
+-rw-r--r--   0        0        0      450 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0002_timerequest_instrument_types.py
+-rw-r--r--   0        0        0      620 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py
+-rw-r--r--   0        0        0      346 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0004_remove_timerequest_instrument.py
+-rw-r--r--   0        0        0      728 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py
+-rw-r--r--   0        0        0        0 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/__init__.py
+-rw-r--r--   0        0        0    10686 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/models.py
+-rw-r--r--   0        0        0    13642 2023-04-10 19:41:28.034842 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/serializers.py
+-rw-r--r--   0        0        0      375 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/templates/sciapplications/approved.txt
+-rw-r--r--   0        0        0      318 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/templates/sciapplications/ddt_submitted.txt
+-rw-r--r--   0        0        0    11505 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_admin.py
+-rw-r--r--   0        0        0    54563 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_api.py
+-rw-r--r--   0        0        0     7046 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/tests.py
+-rw-r--r--   0        0        0     6480 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/viewsets.py
+-rw-r--r--   0        0        0    23236 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/settings.py
+-rw-r--r--   0        0        0      920 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/task_scheduler.py
+-rw-r--r--   0        0        0      601 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/test_runner.py
+-rw-r--r--   0        0        0     1776 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/test_settings.py
+-rw-r--r--   0        0        0     5507 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/urls.py
+-rw-r--r--   0        0        0      413 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/observation_portal/wsgi.py
+-rw-r--r--   0        0        0     2043 2023-04-10 19:41:28.038843 django_ocs_observation_portal-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0    41514 1970-01-01 00:00:00.000000 django_ocs_observation_portal-4.6.0/PKG-INFO
```

### Comparing `django-ocs-observation-portal-4.5.1/LICENSE` & `django_ocs_observation_portal-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/README.md` & `django_ocs_observation_portal-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/admin.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/backends.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/backends.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/forms.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/forms.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/create_application.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_application.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/create_user.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/create_user.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/generateschema_mocked.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/generateschema_mocked.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/init_e2e_credentials.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/init_e2e_credentials.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/management/commands/updateclientusers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/management/commands/updateclientusers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/migrations/0001_initial.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/migrations/0003_bulk_create_users_api.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/migrations/0003_bulk_create_users_api.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/models.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/models.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/0001_initial.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0002_auto_20210715_0630.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/oauth2_migrations/0003_alter_accesstoken_user_alter_application_user_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/permissions.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/permissions.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/serializers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/signals/handlers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/tasks.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/redoc.html` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/registration/activation_complete.html` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/templates/registration/activation_email.html` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/templates/registration/activation_email.html`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/test_utils.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/test_views.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/test_views.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/tests.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/urls.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/accounts/views.py` & `django_ocs_observation_portal-4.6.0/observation_portal/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/configdb.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/configdb.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/doc_examples.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/doc_examples.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/downtimedb.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/downtimedb.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/middleware.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/middleware.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/mixins.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/rise_set_utils.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/rise_set_utils.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/schema.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/schema.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/state_changes.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/state_changes.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/telescope_states.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/telescope_states.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_configdb.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_configdb.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/configdb.json` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/configdb.json`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/doc_configdb.json` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/doc_configdb.json`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_data/es_telescope_states_data.txt` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_data/es_telescope_states_data.txt`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_helpers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_state_changes.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_state_changes.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/test_telescope_states.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/test_telescope_states.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/common/utils.py` & `django_ocs_observation_portal-4.6.0/observation_portal/common/utils.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/admin.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/admin.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/filters.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/filters.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/forms.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/forms.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/management/commands/populate_time_charged.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/populate_time_charged.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/management/commands/time_accounting.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/management/commands/time_accounting.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0001_initial.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0003_auto_20190514_0005.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0003_auto_20190514_0005.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0005_auto_20210116_0033.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0005_auto_20210116_0033.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/migrations/0008_configurationstatus_time_charged.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/models.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/models.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/serializers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/signals/handlers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/test/tests.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/test/tests.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/time_accounting.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/time_accounting.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/views.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/views.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/observations/viewsets.py` & `django_ocs_observation_portal-4.6.0/observation_portal/observations/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/admin.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,25 +77,30 @@
         'modified'
     )
     list_filter = ('active', ProposalTagListFilter, 'sca', 'public')
     raw_id_fields = ('users',)
     inlines = [TimeAllocationAdminInline]
     search_fields = ['id', 'title', 'abstract']
     readonly_fields = []
-    actions = ['activate_selected']
+    actions = ['activate_selected', 'deactivate_selected']
 
     def semesters(self, obj):
         return [semester.id for semester in obj.semester_set.all().distinct()]
     semesters.ordering = ''
 
     def activate_selected(self, request, queryset):
         activated = queryset.filter(active=False).update(active=True)
         self.message_user(request, 'Successfully activated {} proposal(s)'.format(activated))
     activate_selected.short_description = 'Activate selected inactive proposals'
 
+    @admin.action(description='Deactivate selected proposals')
+    def deactivate_selected(self, request, queryset):
+        deactivated = queryset.update(active=False)
+        self.message_user(request, 'Successfully deactivated {} proposal(s)'.format(deactivated))
+
     def get_readonly_fields(self, request, obj=None):
         if obj:
             return self.readonly_fields + ['id']
         else:
             return self.readonly_fields
 
     def get_actions(self, request):
```

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/filters.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/filters.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/forms.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/forms.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/management/commands/create_proposal.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_proposal.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/management/commands/create_semester.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/management/commands/create_semester.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0001_initial.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0002_auto_20190815_1942.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0002_auto_20190815_1942.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0004_auto_20210617_0908.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0004_auto_20210617_0908.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0005_auto_20210604_2154.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0005_auto_20210604_2154.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0006_auto_20210604_2155.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0006_auto_20210604_2155.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0007_remove_timeallocation_instrument_type.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/migrations/0008_auto_20210708_1623.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/migrations/0008_auto_20210708_1623.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/models.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/models.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/notifications.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/notifications.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/serializers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/signals/handlers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/tasks.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/tasks.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/requestfailurelimit.txt` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestfailurelimit.txt`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/requestgroupcomplete.txt`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/templates/proposals/timeallocationreminder.html` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/templates/proposals/timeallocationreminder.html`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/test_api.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/test_api.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/tests.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/tests.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/proposals/viewsets.py` & `django_ocs_observation_portal-4.6.0/observation_portal/proposals/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/admin.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/admin.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/cadence.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/cadence.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/contention.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/contention.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/duration_utils.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/duration_utils.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/filters.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/filters.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/forms.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/forms.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/management/commands/create_example_requests.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/management/commands/create_example_requests.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0001_initial.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0002_auto_20190319_1814.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0003_acquisitionconfig_exposure_time.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0004_auto_20190410_0103.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0006_auto_20190514_0005.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0007_auto_20190516_1713.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0008_auto_20190516_2055.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0009_auto_20190518_0023.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0010_auto_20190612_0048.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0011_auto_20190702_2014.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0012_auto_20191123_0233.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0013_auto_20191220_0711.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0014_auto_20210123_0715.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0015_auto_20210323_0635.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0017_request_extra_params.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0017_request_extra_params.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0018_alter_acquisitionconfig_extra_params_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0019_request_configuration_repeats.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0020_alter_constraints_max_lunar_phase.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0021_request_optimization_type.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0021_request_optimization_type.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0022_alter_constraints_max_seeing.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/migrations/0023_alter_target_epochofperih.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/models.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/models.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/pattern_expansion.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/pattern_expansion.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/request_utils.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/request_utils.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/serializers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/signals/handlers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/target_helpers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/target_helpers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/data/blocks.json` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/data/blocks.json`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_api.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_api.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_cadence.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_cadence.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_helpers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_request_utils.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_request_utils.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/test/test_views.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/test/test_views.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/views.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/views.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/requestgroups/viewsets.py` & `django_ocs_observation_portal-4.6.0/observation_portal/requestgroups/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/admin.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/admin.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/filters.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/filters.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0001_initial.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0003_auto_20210604_2155.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/migrations/0005_auto_20210708_1623.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/models.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/models.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/serializers.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/serializers.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/test_admin.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/test_api.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/test_api.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/tests.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/tests.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/sciapplications/viewsets.py` & `django_ocs_observation_portal-4.6.0/observation_portal/sciapplications/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/settings.py` & `django_ocs_observation_portal-4.6.0/observation_portal/settings.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/task_scheduler.py` & `django_ocs_observation_portal-4.6.0/observation_portal/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/test_runner.py` & `django_ocs_observation_portal-4.6.0/observation_portal/test_runner.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/test_settings.py` & `django_ocs_observation_portal-4.6.0/observation_portal/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/observation_portal/urls.py` & `django_ocs_observation_portal-4.6.0/observation_portal/urls.py`

 * *Files identical despite different names*

### Comparing `django-ocs-observation-portal-4.5.1/pyproject.toml` & `django_ocs_observation_portal-4.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ocs-observation-portal"
-version = "4.5.1"
+version = "4.6.0"
 description = "The Observatory Control System (OCS) Observation Portal django apps"
 license = "GPL-3.0-only"
 authors = ["Observatory Control System Project <ocs@lco.global>"]
 readme = "README.md"
 homepage = "https://observatorycontrolsystem.github.io"
 repository = "https://github.com/observatorycontrolsystem/observation-portal"
 keywords = [
@@ -27,15 +27,15 @@
     { include = "observation_portal" }
 ]
 
 [tool.poetry.scripts]
 ocs-django-manage = "manage:main"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.11"
 apscheduler = ">=3.7,<3.8"
 boto3 = "<2.0"
 cerberus = ">1.0,<2.0"
 django = "^4"
 djangorestframework = "^3.13"
 django-bootstrap4 = "<4.0"
 django-cors-headers = "^3.11"
@@ -48,15 +48,15 @@
 django-storages = "^1.12"
 dramatiq = { version = "^1.12", extras = [ "redis", "watch" ] }
 drf-yasg = "^1.20"
 opensearch-py = ">=1.0,<2.0"
 gunicorn = { version = "^20.1", extras = [ "gevent" ] }
 lcogt-logging = "0.3.2"
 numpy = "^1.16"
-ocs-rise-set = "^0.5.2"
+ocs-rise-set = "0.6.2"
 psycopg2-binary = "^2.9.3"
 PyPDF2 = ">=1.26,<1.28"
 redis = "^3"
 requests = "^2.27.1"
 time_intervals = "^1"
 uritemplate = "^4.1.1"
 PyYAML = "^6.0"
```

### Comparing `django-ocs-observation-portal-4.5.1/setup.py` & `django_ocs_observation_portal-4.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,235 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-ocs-observation-portal
+Version: 4.6.0
+Summary: The Observatory Control System (OCS) Observation Portal django apps
+Home-page: https://observatorycontrolsystem.github.io
+License: GPL-3.0-only
+Keywords: observations,astronomy,astrophysics,cosmology,science
+Author: Observatory Control System Project
+Author-email: ocs@lco.global
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: PyPDF2 (>=1.26,<1.28)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: apscheduler (>=3.7,<3.8)
+Requires-Dist: boto3 (<2.0)
+Requires-Dist: cerberus (>1.0,<2.0)
+Requires-Dist: django (>=4,<5)
+Requires-Dist: django-bootstrap4 (<4.0)
+Requires-Dist: django-cors-headers (>=3.11,<4.0)
+Requires-Dist: django-dramatiq (>=0.10,<0.11)
+Requires-Dist: django-extensions (>=3.1,<4.0)
+Requires-Dist: django-filter (==21.1)
+Requires-Dist: django-oauth-toolkit (>=1.6,<1.7)
+Requires-Dist: django-redis-cache (>=3,<4)
+Requires-Dist: django-registration-redux (>=2.9,<3.0)
+Requires-Dist: django-storages (>=1.12,<2.0)
+Requires-Dist: djangorestframework (>=3.13,<4.0)
+Requires-Dist: dramatiq[redis,watch] (>=1.12,<2.0)
+Requires-Dist: drf-yasg (>=1.20,<2.0)
+Requires-Dist: gunicorn[gevent] (>=20.1,<21.0)
+Requires-Dist: lcogt-logging (==0.3.2)
+Requires-Dist: numpy (>=1.16,<2.0)
+Requires-Dist: ocs-rise-set (==0.6.2)
+Requires-Dist: opensearch-py (>=1.0,<2.0)
+Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
+Requires-Dist: redis (>=3,<4)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: time_intervals (>=1,<2)
+Requires-Dist: uritemplate (>=4.1.1,<5.0.0)
+Project-URL: Repository, https://github.com/observatorycontrolsystem/observation-portal
+Description-Content-Type: text/markdown
+
+# Observation Portal
+
+![Build](https://github.com/observatorycontrolsystem/observation-portal/workflows/Build/badge.svg)
+[![Coverage Status](https://coveralls.io/repos/github/observatorycontrolsystem/observation-portal/badge.svg?branch=master)](https://coveralls.io/github/observatorycontrolsystem/observation-portal?branch=master)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/9846cee7c4904cae8864525101030169)](https://www.codacy.com/gh/observatorycontrolsystem/observation-portal?utm_source=github.com&utm_medium=referral&utm_content=observatorycontrolsystem/observation-portal&utm_campaign=Badge_Grade)
+
+## An API for Astronomical Observation Management
+
+Within an observatory control system, the observation portal provides modules for:
+
+-   **Proposal management**: Calls for proposals, proposal creation, and time allocation
+-   **Request management**: Observation request validation, submission, and cancellation, as well as views providing ancillary information about them
+-   **Observation management**: Store and provide the telescope schedule, update observations, and update observation requests on observation update
+-   **User identity management**: Oauth2 authenticated user management that can be used in other applications
+
+## Prerequisites
+
+Optional prerequisites can be skipped for reduced functionality.
+
+-   Python >= 3.8
+-   PostgreSQL >= 10
+-   A running [Configuration Database](https://github.com/observatorycontrolsystem/configdb) 
+-   (Optional) A running [Downtime Database](https://github.com/observatorycontrolsystem/downtime)
+-   (Optional) A running Elasticsearch
+
+
+
+## Environment Variables
+
+|                        | Variable                         | Description                                                                                                                                                                 | Default                                                 |
+| ---------------------- | -------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |
+| General                | `DEBUG`                          | Whether the application should run using Django's debug mode                                                                                                                | `False`                                                 |
+|                        | `SECRET_KEY`                     | The secret key used for sessions                                                                                                                                            | _`random characters`_                                   |
+|                        | `ALLOWED_HOSTS`                     | Override for Django's ALLOWED_HOSTS setting                                                                                                                                            | `*`                                   |
+|                        | `CSRF_TRUSTED_ORIGINS`           | Comma separated list of trusted origins allowed for CSRF                                                                                                                    | `None`
+|                        | `MAX_FAILURES_PER_REQUEST` | Maximum number of times an Observation can fail per Request before the Request is marked as FAILURE_LIMIT_REACHED. 0 means there is no max. | `0` |
+|                        | `MAX_IPP_VALUE` | The maximum value to be used for ipp scaling. Should be greater than 1 (1 would be no scaling) | `2.0` |
+|                        | `MIN_IPP_VALUE` | The minimum value to be used for ipp scaling. Should be less than 1 but greater than 0 | `0.5` |
+|                        | `PROPOSAL_TIME_OVERUSE_ALLOWANCE` | The amount of leeway in a proposals timeallocation before rejecting that request for scheduling. For example, a value of 1.1 results in allows over-scheduling by up to 10% of the total time_allocation. It is useful to allow some over-scheduling since it is likely some in progress observations will use less time then allocated, due to conservative overheads, failing, or cancelling.                | `1.1` |
+| Database               | `DB_NAME`                        | The name of the database                                                                                                                                                    | `observation_portal`                                    |
+|                        | `DB_USER`                        | The database user                                                                                                                                                           | `postgres`                                              |
+|                        | `DB_PASSWORD`                    | The database password                                                                                                                                                       | _`Empty string`_                                        |
+|                        | `DB_HOST`                        | The database host                                                                                                                                                           | `127.0.0.1`                                             |
+|                        | `DB_PORT`                        | The database port                                                                                                                                                           | `5432`                                                  |
+| Cache                  | `CACHE_BACKEND`                  | The remote Django cache backend                                                                                                                                             | `django.core.cache.backends.locmem.LocMemCache`         |
+|                        | `CACHE_LOCATION`                 | The cache location or connection string                                                                                                                                     | `unique-snowflake`                                      |
+|                        | `LOCAL_CACHE_BACKEND`            | The local Django cache backend to use                                                                                                                                       | `django.core.cache.backends.locmem.LocMemCache`         |
+| Static and Media Files | `AWS_BUCKET_NAME`                | The name of the AWS bucket in which to store static and media files                                                                                                         | `observation-portal-test-bucket`                        |
+|                        | `AWS_REGION`                     | The AWS region                                                                                                                                                              | `us-west-2`                                             |
+|                        | `AWS_ACCESS_KEY_ID`              | The AWS user access key with read/write priveleges on the s3 bucket                                                                                                         | `None`                                                  |
+|                        | `AWS_SECRET_ACCESS_KEY`          | The AWS user secret key to use with the access key                                                                                                                          | `None`                                                  |
+|                        | `MEDIA_STORAGE`                  | The Django media files storage backend                                                                                                                                      | `django.core.files.storage.FileSystemStorage`           |
+|                        | `MEDIAFILES_DIR`                 | The directory in which to store media files                                                                                                                                 | `media`                                                 |
+|                        | `STATIC_STORAGE`                 | The Django static files storage backend                                                                                                                                     | `django.contrib.staticfiles.storage.StaticFilesStorage` |
+| Email                  | `EMAIL_BACKEND`                  | The Django SMTP backend to use                                                                                                                                              | `django.core.mail.backends.console.EmailBackend`        |
+|                        | `EMAIL_HOST`                     | The SMTP host                                                                                                                                                               | `localhost`                                             |
+|                        | `EMAIL_HOST_USER`                | The SMTP user                                                                                                                                                               | _`Empty string`_                                        |
+|                        | `EMAIL_HOST_PASSWORD`            | The SMTP password                                                                                                                                                           | _`Empty string`_                                        |
+|                        | `EMAIL_PORT`                     | The SMTP port                                                                                                                                                               | `587`                                                   |
+|                        | `ORGANIZATION_EMAIL`             | The reply-to email for outgoing messages                                                                                                                                                           | _`Empty string`_                                                    |
+|                        | `ORGANIZATION_DDT_EMAIL`             | Email to receive ddt science application submission messages                                                                                                                                                           | _`Empty string`_                                                    |
+|                        | `ORGANIZATION_ADMIN_EMAIL`             | The Django Admin email to receive http 500 reports.                                                                                                                                                           | _`Empty string`_                                                    |
+|                        | `ORGANIZATION_SUPPORT_EMAIL`             | Email to receive account removal requests                                                                                                                                                            | _`Empty string`_                                                    |
+|                        | `ORGANIZATION_NAME`              | The name of your organization, used within email templates                                                                                                                                                           | _`Empty string`_                                                    |
+|                        | `OBSERVATION_PORTAL_BASE_URL`    | The base url of your deployed Observation Portal code, used within email templates to provide links to pages                                                                                                                                                          | `http://localhost`                                                    |
+|                        | `REQUESTGROUP_DATA_DOWNLOAD_URL` | The url where a user can download requestgroup data. Optionally include `{requestgroup_id}` in the string which will be filled in with the ID of the specific requestgroup. | _`Empty string`_ |
+|                        | `REQUEST_DETAIL_URL` | The url to frontend detail page for a Request. Optionally include `{request_id}` in the string which will be filled in with the ID of the specific request. | _`Empty string`_ |
+|                        | `SCIENCE_APPLICATION_DETAIL_URL` | The url to frontend science application detail page. Optionally include `{sciapp_id}` in the string which will be filled in with the ID of the specific science application. | _`Empty string`_ |
+| External Services      | `CONFIGDB_URL`                   | The url to the configuration database                                                                                                                                       | `http://localhost`                                      |
+|                        | `DOWNTIMEDB_URL`                 | The url to the downtime database                                                                                                                                            | `http://localhost`                                      |
+|                        | `OPENSEARCH_URL`                 | The url to the OpenSearch cluster                                                                                                                                           | `http://localhost`                                      |
+| Authentication         | `OAUTH_SERVER_KEY`               | The secret key for client applications to verify against for authentication calls                                                                                                                                              | _`Empty string`_                                        |
+|                        | `OAUTH_CLIENT_APPS_BASE_URLS`    | Comma delimited set of base urls for client applications. This server will update those clients on any change in user accounts or api tokens.                                                                                                                                                               | _`Empty string`_                                |
+| Task Scheduling        | `DRAMATIQ_BROKER_URL`            | The url to the dramatiq broker (if set takes precedence over `DRAMATIQ_BROKER_HOST` & `DRAMATIQ_BROKER_PORT`                                                                | `redis://redis:6379/0`                                  |
+|                        | `DRAMATIQ_BROKER_HOST`           | The broker host for dramatiq (deprecated)                                                                                                                                   | `redis`                                                 |
+|                        | `DRAMATIQ_BROKER_PORT`           | The broker port for dramatiq (deprecated)                                                                                                                                   | `6379`                                                  |
+| Throttle Overrides     | `REQUESTGROUPS_CANCEL_DEFAULT_THROTTLE`           | Default django rest framework throttle rate string for the RequestGroups cancel endpoint                                                                                                                                              | `2000/day`                                                 |
+|                        | `REQUESTGROUPS_CREATE_DEFAULT_THROTTLE`           | Default django rest framework throttle rate string for the RequestGroups create endpoint                                                                                                                                              | `5000/day`                                                 |
+|                        | `REQUESTGROUPS_VALIDATE_DEFAULT_THROTTLE`           | Default django rest framework throttle rate string for the RequestGroups validate endpoint                                                                                                                                             | `20000/day`                                                 |
+| Serializer Overrides   | `OBSERVATIONS_SUMMARY_SERIALIZER`           | Class dotpath for Observation's Summary serializer override                                                                                                                                             | `observation_portal.observations.serializers.SummarySerializer`                                                 |
+|                        | `OBSERVATIONS_CONFIGURATIONSTATUS_SERIALIZER`           | Class dotpath for Observation's ConfigurationStatus serializer override                                                                                                                                             | `observation_portal.observations.serializers.ConfigurationStatusSerializer`                                                 |
+|                        | `OBSERVATIONS_TARGET_SERIALIZER`           | Class dotpath for Observation's Target serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObservationTargetSerializer`                                              |
+|                        | `OBSERVATIONS_CONFIGURATION_SERIALIZER`           | Class dotpath for Observation's Configuration serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObservationConfigurationSerializer`                                              |
+|                        | `OBSERVATIONS_REQUEST_SERIALIZER`           | Class dotpath for Observation's Request serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObserveRequestSerializer`                                              |
+|                        | `OBSERVATIONS_REQUESTGROUP_SERIALIZER`           | Class dotpath for Observation's RequestGroup serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObserveRequestGroupSerializer`                                              |
+|                        | `OBSERVATIONS_SCHEDULE_SERIALIZER`           | Class dotpath for Observation's Schedule serializer override                                                                                                                                             | `observation_portal.observations.serializers.ScheduleSerializer`                                              |
+|                        | `OBSERVATIONS_OBSERVATION_SERIALIZER`           | Class dotpath for Observation's Observation serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObservationSerializer`                                              |
+|                        | `OBSERVATIONS_CANCEL_SERIALIZER`           | Class dotpath for Observation's Cancel Observation serializer override                                                                                                                                             | `observation_portal.observations.serializers.CancelObservationsSerializer`                                              |
+|                        | `REQUESTGROUPS_CADENCE_SERIALIZER`           | Class dotpath for RequestGroups's Cadence serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.CadenceSerializer`                                              |
+|                        | `REQUESTGROUPS_CADENCEREQUEST_SERIALIZER`         | Class dotpath for RequestGroups's Cadence Request serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.CadenceRequestSerializer`                                              |
+|                        | `REQUESTGROUPS_CONSTRAINTS_SERIALIZER`           | Class dotpath for RequestGroups's Constraints serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.ConstraintsSerializer`                                              |
+|                        | `REQUESTGROUPS_REGIONOFINTEREST_SERIALIZER`           | Class dotpath for RequestGroups's Instrument Config ROI serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.RegionOfInterestSerializer`                                              |
+|                        | `REQUESTGROUPS_INSTRUMENTCONFIG_SERIALIZER`           | Class dotpath for RequestGroups's Instrument Config serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.InstrumentConfigSerializer`                                              |
+|                        | `REQUESTGROUPS_ACQUISITIONCONFIG_SERIALIZER`           | Class dotpath for RequestGroups's Acquisition Config serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.AcquisitionConfigSerializer`                                              |
+|                        | `REQUESTGROUPS_GUIDINGCONFIG_SERIALIZER`           | Class dotpath for RequestGroups's Guiding Config serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.GuidingConfigSerializer`                                              |
+|                        | `REQUESTGROUPS_TARGET_SERIALIZER`           | Class dotpath for RequestGroups's Target serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.TargetSerializer`                                              |
+|                        | `REQUESTGROUPS_CONFIGURATION_SERIALIZER`           | Class dotpath for RequestGroups's Configuration serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.ConfigurationSerializer`                                              |
+|                        | `REQUESTGROUPS_LOCATION_SERIALIZER`           | Class dotpath for RequestGroups's Location serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.LocationSerializer`                                              |
+|                        | `REQUESTGROUPS_WINDOW_SERIALIZER`           | Class dotpath for RequestGroups's Window serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.WindowSerializer`                                              |
+|                        | `REQUESTGROUPS_REQUEST_SERIALIZER`           | Class dotpath for RequestGroups's Request serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.RequestSerializer`                                              |
+|                        | `REQUESTGROUPS_REQUESTGROUP_SERIALIZER`           | Class dotpath for RequestGroups's RequestGroup serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.RequestGroupSerializer`                                              |
+|                        | `REQUESTGROUPS_DRAFTREQUESTGROUP_SERIALIZER`           | Class dotpath for RequestGroups's Draft RequestGroup serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.DraftRequestGroupSerializer`                                              |
+|                        | `PROPOSALS_PROPOSAL_SERIALIZER`           | Class dotpath for Proposal's Proposal serializer override                                                                                                                                             | `observation_portal.proposals.serializers.ProposalSerializer`                                              |
+|                        | `PROPOSALS_PROPOSALINVITE_SERIALIZER`           | Class dotpath for Proposal's ProposalInvite serializer override                                                                                                                                             | `observation_portal.proposals.serializers.ProposalInviteSerializer`                                              |
+|                        | `PROPOSALS_SEMESTER_SERIALIZER`           | Class dotpath for Proposal's Semester serializer override                                                                                                                                             | `observation_portal.proposals.serializers.SemesterSerialzer`                                              |
+|                        | `PROPOSALS_MEMBERSHIP_SERIALIZER`           | Class dotpath for Proposal's Membership serializer override                                                                                                                                             | `observation_portal.proposals.serializers.MembershipSerializer`                                              |
+|                        | `PROPOSALS_PROPOSALNOTIFICATION_SERIALIZER`           | Class dotpath for Proposal's ProposalNotification serializer override                                                                                                                                             | `observation_portal.proposals.serializers.ProposalNotificationSerializer`                                              |
+|                        | `PROPOSALS_TIMELIMIT_SERIALIZER`           | Class dotpath for Proposal's Proposal serializer override                                                                                                                                             | `observation_portal.proposals.serializers.TimeLimitSerializer`                                              |
+|                        | `ACCOUNTS_PROFILE_SERIALIZER`           | Class dotpath for Accounts's Profile serializer override                                                                                                                                             | `observation_portal.accounts.serializers.ProfileSerializer`                                              |
+|                        | `ACCOUNTS_USER_SERIALIZER`           | Class dotpath for Accounts's User serializer override                                                                                                                                             | `observation_portal.accounts.serializers.UserSerializer`                                              |
+|                        | `ACCOUNTS_ACCOUNTREMOVAL_SERIALIZER`           | Class dotpath for Accounts's Account Removal serializer override                                                                                                                                             | `observation_portal.accounts.serializers.AccountRemovalSerializer`                                              |
+|                        | `SCIAPPLICATIONS_CALL_SERIALIZER`           | Class dotpath for SciApplications's Call serializer override                                                                                                                                             | `observation_portal.sciapplications.serializers.CallSerializer`                                              |
+|                        | `SCIAPPLICATIONS_SCIENCEAPPLICATION_SERIALIZER`           | Class dotpath for SciApplications's Science Application serializer override                                                                                                                                             | `observation_portal.sciapplications.serializers.ScienceApplicationSerializer`                                              |
+| as_dict Overrides   | `OBSERVATIONS_SUMMARY_AS_DICT`           | Class dotpath for Observation's Summary as_dict override                                                                                                                                             | `observation_portal.observations.models.summary_as_dict`                                                 |
+|                        | `OBSERVATIONS_CONFIGURATIONSTATUS_AS_DICT`           | Class dotpath for Observation's ConfigurationStatus as_dict override                                                                                                                                             | `observation_portal.observations.models.configurationstatus_as_dict`                                                 |
+|                        | `OBSERVATIONS_OBSERVATION_AS_DICT`           | Class dotpath for Observation's Observation as_dict override                                                                                                                                             | `observation_portal.observations.models.observation_as_dict`                                              |
+|                        | `REQUESTGROUPS_CONSTRAINTS_AS_DICT`           | Class dotpath for RequestGroups's Constraints as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.constraints_as_dict`                                              |
+|                        | `REQUESTGROUPS_REGIONOFINTEREST_AS_DICT`           | Class dotpath for RequestGroups's Instrument Config ROI as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.regionofinterest_as_dict`                                              |
+|                        | `REQUESTGROUPS_INSTRUMENTCONFIG_AS_DICT`           | Class dotpath for RequestGroups's Instrument Config as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.instrumentconfig_as_dict`                                              |
+|                        | `REQUESTGROUPS_ACQUISITIONCONFIG_AS_DICT`           | Class dotpath for RequestGroups's Acquisition Config as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.acquisitionconfig_as_dict`                                              |
+|                        | `REQUESTGROUPS_GUIDINGCONFIG_AS_DICT`           | Class dotpath for RequestGroups's Guiding Config as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.guidingconfig_as_dict`                                              |
+|                        | `REQUESTGROUPS_TARGET_AS_DICT`           | Class dotpath for RequestGroups's Target as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.target_as_dict`                                              |
+|                        | `REQUESTGROUPS_CONFIGURATION_AS_DICT`           | Class dotpath for RequestGroups's Configuration as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.configuration_as_dict`                                              |
+|                        | `REQUESTGROUPS_LOCATION_AS_DICT`           | Class dotpath for RequestGroups's Location as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.location_as_dict`                                              |
+|                        | `REQUESTGROUPS_WINDOW_AS_DICT`           | Class dotpath for RequestGroups's Window as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.window_as_dict`                                              |
+|                        | `REQUESTGROUPS_REQUEST_AS_DICT`           | Class dotpath for RequestGroups's Request as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.request_as_dict`                                              |
+|                        | `REQUESTGROUPS_REQUESTGROUP_AS_DICT`           | Class dotpath for RequestGroups's RequestGroup as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.requestgroup_as_dict`                                              |
+|                        | `PROPOSALS_PROPOSAL_AS_DICT`           | Class dotpath for Proposal's Proposal as_dict override                                                                                                                                             | `observation_portal.proposals.models.proposal_as_dict`                                              |
+|                        | `PROPOSALS_TIMEALLOCATION_AS_DICT`           | Class dotpath for Proposal's TimeAllocation as_dict override                                                                                                                                             | `observation_portal.proposals.models.timeallocation_as_dict`                                              |
+|                        | `PROPOSALS_MEMBERSHIP_AS_DICT`           | Class dotpath for Proposal's Membership as_dict override                                                                                                                                             | `observation_portal.proposals.models.membership_as_dict`                                              |
+| duration Overrides   | `INSTRUMENT_CONFIGURATION_PER_EXPOSURE_DURATION`           | Class dotpath for duration_per_exposure method override                                                                                                                                             | `observation_portal.requestgroups.duration_utils.get_instrument_configuration_duration_per_exposure`                                                 |
+
+
+## Local Development
+
+### **Set up external services**
+
+Please refer to the [Configuration Database](https://github.com/observatorycontrolsystem/configdb) and [Downtime Database](https://github.com/observatorycontrolsystem/downtime) projects for instructions on how to get those running, as well as the [Elasticsearch documentation](https://www.elastic.co/guide/en/elasticsearch/reference/5.6/install-elasticsearch.html) for options on how to run Elasticsearch.
+
+
+### **Poetry**
+
+We use Poetry for package management. If you already have Poetry installed, you
+can skip this section.
+
+You can install Poetry using one of the many options listed at https://python-poetry.org/docs/#installation.
+One simple option is using Pipx:
+
+    python3 -m pip install --user pipx
+    python3 -m pipx ensurepath
+    pipx install poetry
+
+### **Install**
+
+Install the project and its Python dependencies:
+
+    poetry install
+
+This will install the project in a Poetry managed virtual environment. To run
+commands in that environment either use `poetry run ...` or start a shell in
+that environment with `poetry shell`
+
+### **Set up the database**
+
+This example uses the [PostgreSQL Docker image](https://hub.docker.com/_/postgres) to create a database. Make sure that the options that you use to set up your database correspond with your configured database settings.
+
+    docker run --name observation-portal-postgres -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=observation_portal -v/var/lib/postgresql/data -p5432:5432 -d postgres:11.1
+
+After creating the database, migrations must be applied to set up the tables in the database.
+
+    poetry run python manage.py migrate
+
+### **Run the tests**
 
-packages = \
-['observation_portal',
- 'observation_portal.accounts',
- 'observation_portal.accounts.management',
- 'observation_portal.accounts.management.commands',
- 'observation_portal.accounts.migrations',
- 'observation_portal.accounts.oauth2_migrations',
- 'observation_portal.accounts.signals',
- 'observation_portal.common',
- 'observation_portal.common.test_data',
- 'observation_portal.observations',
- 'observation_portal.observations.management',
- 'observation_portal.observations.management.commands',
- 'observation_portal.observations.migrations',
- 'observation_portal.observations.signals',
- 'observation_portal.observations.test',
- 'observation_portal.proposals',
- 'observation_portal.proposals.management',
- 'observation_portal.proposals.management.commands',
- 'observation_portal.proposals.migrations',
- 'observation_portal.proposals.signals',
- 'observation_portal.requestgroups',
- 'observation_portal.requestgroups.management',
- 'observation_portal.requestgroups.management.commands',
- 'observation_portal.requestgroups.migrations',
- 'observation_portal.requestgroups.signals',
- 'observation_portal.requestgroups.test',
- 'observation_portal.sciapplications',
- 'observation_portal.sciapplications.migrations']
-
-package_data = \
-{'': ['*'],
- 'observation_portal.accounts': ['templates/*',
-                                 'templates/auth/*',
-                                 'templates/registration/*'],
- 'observation_portal.observations': ['templates/observations/*'],
- 'observation_portal.proposals': ['templates/proposals/*'],
- 'observation_portal.requestgroups.test': ['data/*'],
- 'observation_portal.sciapplications': ['templates/sciapplications/*']}
-
-install_requires = \
-['PyPDF2>=1.26,<1.28',
- 'PyYAML>=6.0,<7.0',
- 'apscheduler>=3.7,<3.8',
- 'boto3<2.0',
- 'cerberus>1.0,<2.0',
- 'django-bootstrap4<4.0',
- 'django-cors-headers>=3.11,<4.0',
- 'django-dramatiq>=0.10,<0.11',
- 'django-extensions>=3.1,<4.0',
- 'django-filter==21.1',
- 'django-oauth-toolkit>=1.6,<1.7',
- 'django-redis-cache>=3,<4',
- 'django-registration-redux>=2.9,<3.0',
- 'django-storages>=1.12,<2.0',
- 'django>=4,<5',
- 'djangorestframework>=3.13,<4.0',
- 'dramatiq[redis,watch]>=1.12,<2.0',
- 'drf-yasg>=1.20,<2.0',
- 'gunicorn[gevent]>=20.1,<21.0',
- 'lcogt-logging==0.3.2',
- 'numpy>=1.16,<2.0',
- 'ocs-rise-set>=0.5.2,<0.6.0',
- 'opensearch-py>=1.0,<2.0',
- 'psycopg2-binary>=2.9.3,<3.0.0',
- 'redis>=3,<4',
- 'requests>=2.27.1,<3.0.0',
- 'time_intervals>=1,<2',
- 'uritemplate>=4.1.1,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['ocs-django-manage = manage:main']}
-
-setup_kwargs = {
-    'name': 'django-ocs-observation-portal',
-    'version': '4.5.1',
-    'description': 'The Observatory Control System (OCS) Observation Portal django apps',
-    'long_description': "# Observation Portal\n\n![Build](https://github.com/observatorycontrolsystem/observation-portal/workflows/Build/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/observatorycontrolsystem/observation-portal/badge.svg?branch=master)](https://coveralls.io/github/observatorycontrolsystem/observation-portal?branch=master)\n[![Codacy Badge](https://api.codacy.com/project/badge/Grade/9846cee7c4904cae8864525101030169)](https://www.codacy.com/gh/observatorycontrolsystem/observation-portal?utm_source=github.com&utm_medium=referral&utm_content=observatorycontrolsystem/observation-portal&utm_campaign=Badge_Grade)\n\n## An API for Astronomical Observation Management\n\nWithin an observatory control system, the observation portal provides modules for:\n\n-   **Proposal management**: Calls for proposals, proposal creation, and time allocation\n-   **Request management**: Observation request validation, submission, and cancellation, as well as views providing ancillary information about them\n-   **Observation management**: Store and provide the telescope schedule, update observations, and update observation requests on observation update\n-   **User identity management**: Oauth2 authenticated user management that can be used in other applications\n\n## Prerequisites\n\nOptional prerequisites can be skipped for reduced functionality.\n\n-   Python >= 3.8\n-   PostgreSQL >= 10\n-   A running [Configuration Database](https://github.com/observatorycontrolsystem/configdb) \n-   (Optional) A running [Downtime Database](https://github.com/observatorycontrolsystem/downtime)\n-   (Optional) A running Elasticsearch\n\n\n\n## Environment Variables\n\n|                        | Variable                         | Description                                                                                                                                                                 | Default                                                 |\n| ---------------------- | -------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |\n| General                | `DEBUG`                          | Whether the application should run using Django's debug mode                                                                                                                | `False`                                                 |\n|                        | `SECRET_KEY`                     | The secret key used for sessions                                                                                                                                            | _`random characters`_                                   |\n|                        | `ALLOWED_HOSTS`                     | Override for Django's ALLOWED_HOSTS setting                                                                                                                                            | `*`                                   |\n|                        | `CSRF_TRUSTED_ORIGINS`           | Comma separated list of trusted origins allowed for CSRF                                                                                                                    | `None`\n|                        | `MAX_FAILURES_PER_REQUEST` | Maximum number of times an Observation can fail per Request before the Request is marked as FAILURE_LIMIT_REACHED. 0 means there is no max. | `0` |\n|                        | `MAX_IPP_VALUE` | The maximum value to be used for ipp scaling. Should be greater than 1 (1 would be no scaling) | `2.0` |\n|                        | `MIN_IPP_VALUE` | The minimum value to be used for ipp scaling. Should be less than 1 but greater than 0 | `0.5` |\n|                        | `PROPOSAL_TIME_OVERUSE_ALLOWANCE` | The amount of leeway in a proposals timeallocation before rejecting that request for scheduling. For example, a value of 1.1 results in allows over-scheduling by up to 10% of the total time_allocation. It is useful to allow some over-scheduling since it is likely some in progress observations will use less time then allocated, due to conservative overheads, failing, or cancelling.                | `1.1` |\n| Database               | `DB_NAME`                        | The name of the database                                                                                                                                                    | `observation_portal`                                    |\n|                        | `DB_USER`                        | The database user                                                                                                                                                           | `postgres`                                              |\n|                        | `DB_PASSWORD`                    | The database password                                                                                                                                                       | _`Empty string`_                                        |\n|                        | `DB_HOST`                        | The database host                                                                                                                                                           | `127.0.0.1`                                             |\n|                        | `DB_PORT`                        | The database port                                                                                                                                                           | `5432`                                                  |\n| Cache                  | `CACHE_BACKEND`                  | The remote Django cache backend                                                                                                                                             | `django.core.cache.backends.locmem.LocMemCache`         |\n|                        | `CACHE_LOCATION`                 | The cache location or connection string                                                                                                                                     | `unique-snowflake`                                      |\n|                        | `LOCAL_CACHE_BACKEND`            | The local Django cache backend to use                                                                                                                                       | `django.core.cache.backends.locmem.LocMemCache`         |\n| Static and Media Files | `AWS_BUCKET_NAME`                | The name of the AWS bucket in which to store static and media files                                                                                                         | `observation-portal-test-bucket`                        |\n|                        | `AWS_REGION`                     | The AWS region                                                                                                                                                              | `us-west-2`                                             |\n|                        | `AWS_ACCESS_KEY_ID`              | The AWS user access key with read/write priveleges on the s3 bucket                                                                                                         | `None`                                                  |\n|                        | `AWS_SECRET_ACCESS_KEY`          | The AWS user secret key to use with the access key                                                                                                                          | `None`                                                  |\n|                        | `MEDIA_STORAGE`                  | The Django media files storage backend                                                                                                                                      | `django.core.files.storage.FileSystemStorage`           |\n|                        | `MEDIAFILES_DIR`                 | The directory in which to store media files                                                                                                                                 | `media`                                                 |\n|                        | `STATIC_STORAGE`                 | The Django static files storage backend                                                                                                                                     | `django.contrib.staticfiles.storage.StaticFilesStorage` |\n| Email                  | `EMAIL_BACKEND`                  | The Django SMTP backend to use                                                                                                                                              | `django.core.mail.backends.console.EmailBackend`        |\n|                        | `EMAIL_HOST`                     | The SMTP host                                                                                                                                                               | `localhost`                                             |\n|                        | `EMAIL_HOST_USER`                | The SMTP user                                                                                                                                                               | _`Empty string`_                                        |\n|                        | `EMAIL_HOST_PASSWORD`            | The SMTP password                                                                                                                                                           | _`Empty string`_                                        |\n|                        | `EMAIL_PORT`                     | The SMTP port                                                                                                                                                               | `587`                                                   |\n|                        | `ORGANIZATION_EMAIL`             | The reply-to email for outgoing messages                                                                                                                                                           | _`Empty string`_                                                    |\n|                        | `ORGANIZATION_DDT_EMAIL`             | Email to receive ddt science application submission messages                                                                                                                                                           | _`Empty string`_                                                    |\n|                        | `ORGANIZATION_ADMIN_EMAIL`             | The Django Admin email to receive http 500 reports.                                                                                                                                                           | _`Empty string`_                                                    |\n|                        | `ORGANIZATION_SUPPORT_EMAIL`             | Email to receive account removal requests                                                                                                                                                            | _`Empty string`_                                                    |\n|                        | `ORGANIZATION_NAME`              | The name of your organization, used within email templates                                                                                                                                                           | _`Empty string`_                                                    |\n|                        | `OBSERVATION_PORTAL_BASE_URL`    | The base url of your deployed Observation Portal code, used within email templates to provide links to pages                                                                                                                                                          | `http://localhost`                                                    |\n|                        | `REQUESTGROUP_DATA_DOWNLOAD_URL` | The url where a user can download requestgroup data. Optionally include `{requestgroup_id}` in the string which will be filled in with the ID of the specific requestgroup. | _`Empty string`_ |\n|                        | `REQUEST_DETAIL_URL` | The url to frontend detail page for a Request. Optionally include `{request_id}` in the string which will be filled in with the ID of the specific request. | _`Empty string`_ |\n|                        | `SCIENCE_APPLICATION_DETAIL_URL` | The url to frontend science application detail page. Optionally include `{sciapp_id}` in the string which will be filled in with the ID of the specific science application. | _`Empty string`_ |\n| External Services      | `CONFIGDB_URL`                   | The url to the configuration database                                                                                                                                       | `http://localhost`                                      |\n|                        | `DOWNTIMEDB_URL`                 | The url to the downtime database                                                                                                                                            | `http://localhost`                                      |\n|                        | `OPENSEARCH_URL`                 | The url to the OpenSearch cluster                                                                                                                                           | `http://localhost`                                      |\n| Authentication         | `OAUTH_SERVER_KEY`               | The secret key for client applications to verify against for authentication calls                                                                                                                                              | _`Empty string`_                                        |\n|                        | `OAUTH_CLIENT_APPS_BASE_URLS`    | Comma delimited set of base urls for client applications. This server will update those clients on any change in user accounts or api tokens.                                                                                                                                                               | _`Empty string`_                                |\n| Task Scheduling        | `DRAMATIQ_BROKER_URL`            | The url to the dramatiq broker (if set takes precedence over `DRAMATIQ_BROKER_HOST` & `DRAMATIQ_BROKER_PORT`                                                                | `redis://redis:6379/0`                                  |\n|                        | `DRAMATIQ_BROKER_HOST`           | The broker host for dramatiq (deprecated)                                                                                                                                   | `redis`                                                 |\n|                        | `DRAMATIQ_BROKER_PORT`           | The broker port for dramatiq (deprecated)                                                                                                                                   | `6379`                                                  |\n| Throttle Overrides     | `REQUESTGROUPS_CANCEL_DEFAULT_THROTTLE`           | Default django rest framework throttle rate string for the RequestGroups cancel endpoint                                                                                                                                              | `2000/day`                                                 |\n|                        | `REQUESTGROUPS_CREATE_DEFAULT_THROTTLE`           | Default django rest framework throttle rate string for the RequestGroups create endpoint                                                                                                                                              | `5000/day`                                                 |\n|                        | `REQUESTGROUPS_VALIDATE_DEFAULT_THROTTLE`           | Default django rest framework throttle rate string for the RequestGroups validate endpoint                                                                                                                                             | `20000/day`                                                 |\n| Serializer Overrides   | `OBSERVATIONS_SUMMARY_SERIALIZER`           | Class dotpath for Observation's Summary serializer override                                                                                                                                             | `observation_portal.observations.serializers.SummarySerializer`                                                 |\n|                        | `OBSERVATIONS_CONFIGURATIONSTATUS_SERIALIZER`           | Class dotpath for Observation's ConfigurationStatus serializer override                                                                                                                                             | `observation_portal.observations.serializers.ConfigurationStatusSerializer`                                                 |\n|                        | `OBSERVATIONS_TARGET_SERIALIZER`           | Class dotpath for Observation's Target serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObservationTargetSerializer`                                              |\n|                        | `OBSERVATIONS_CONFIGURATION_SERIALIZER`           | Class dotpath for Observation's Configuration serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObservationConfigurationSerializer`                                              |\n|                        | `OBSERVATIONS_REQUEST_SERIALIZER`           | Class dotpath for Observation's Request serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObserveRequestSerializer`                                              |\n|                        | `OBSERVATIONS_REQUESTGROUP_SERIALIZER`           | Class dotpath for Observation's RequestGroup serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObserveRequestGroupSerializer`                                              |\n|                        | `OBSERVATIONS_SCHEDULE_SERIALIZER`           | Class dotpath for Observation's Schedule serializer override                                                                                                                                             | `observation_portal.observations.serializers.ScheduleSerializer`                                              |\n|                        | `OBSERVATIONS_OBSERVATION_SERIALIZER`           | Class dotpath for Observation's Observation serializer override                                                                                                                                             | `observation_portal.observations.serializers.ObservationSerializer`                                              |\n|                        | `OBSERVATIONS_CANCEL_SERIALIZER`           | Class dotpath for Observation's Cancel Observation serializer override                                                                                                                                             | `observation_portal.observations.serializers.CancelObservationsSerializer`                                              |\n|                        | `REQUESTGROUPS_CADENCE_SERIALIZER`           | Class dotpath for RequestGroups's Cadence serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.CadenceSerializer`                                              |\n|                        | `REQUESTGROUPS_CADENCEREQUEST_SERIALIZER`         | Class dotpath for RequestGroups's Cadence Request serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.CadenceRequestSerializer`                                              |\n|                        | `REQUESTGROUPS_CONSTRAINTS_SERIALIZER`           | Class dotpath for RequestGroups's Constraints serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.ConstraintsSerializer`                                              |\n|                        | `REQUESTGROUPS_REGIONOFINTEREST_SERIALIZER`           | Class dotpath for RequestGroups's Instrument Config ROI serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.RegionOfInterestSerializer`                                              |\n|                        | `REQUESTGROUPS_INSTRUMENTCONFIG_SERIALIZER`           | Class dotpath for RequestGroups's Instrument Config serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.InstrumentConfigSerializer`                                              |\n|                        | `REQUESTGROUPS_ACQUISITIONCONFIG_SERIALIZER`           | Class dotpath for RequestGroups's Acquisition Config serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.AcquisitionConfigSerializer`                                              |\n|                        | `REQUESTGROUPS_GUIDINGCONFIG_SERIALIZER`           | Class dotpath for RequestGroups's Guiding Config serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.GuidingConfigSerializer`                                              |\n|                        | `REQUESTGROUPS_TARGET_SERIALIZER`           | Class dotpath for RequestGroups's Target serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.TargetSerializer`                                              |\n|                        | `REQUESTGROUPS_CONFIGURATION_SERIALIZER`           | Class dotpath for RequestGroups's Configuration serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.ConfigurationSerializer`                                              |\n|                        | `REQUESTGROUPS_LOCATION_SERIALIZER`           | Class dotpath for RequestGroups's Location serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.LocationSerializer`                                              |\n|                        | `REQUESTGROUPS_WINDOW_SERIALIZER`           | Class dotpath for RequestGroups's Window serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.WindowSerializer`                                              |\n|                        | `REQUESTGROUPS_REQUEST_SERIALIZER`           | Class dotpath for RequestGroups's Request serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.RequestSerializer`                                              |\n|                        | `REQUESTGROUPS_REQUESTGROUP_SERIALIZER`           | Class dotpath for RequestGroups's RequestGroup serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.RequestGroupSerializer`                                              |\n|                        | `REQUESTGROUPS_DRAFTREQUESTGROUP_SERIALIZER`           | Class dotpath for RequestGroups's Draft RequestGroup serializer override                                                                                                                                             | `observation_portal.requestgroups.serializers.DraftRequestGroupSerializer`                                              |\n|                        | `PROPOSALS_PROPOSAL_SERIALIZER`           | Class dotpath for Proposal's Proposal serializer override                                                                                                                                             | `observation_portal.proposals.serializers.ProposalSerializer`                                              |\n|                        | `PROPOSALS_PROPOSALINVITE_SERIALIZER`           | Class dotpath for Proposal's ProposalInvite serializer override                                                                                                                                             | `observation_portal.proposals.serializers.ProposalInviteSerializer`                                              |\n|                        | `PROPOSALS_SEMESTER_SERIALIZER`           | Class dotpath for Proposal's Semester serializer override                                                                                                                                             | `observation_portal.proposals.serializers.SemesterSerialzer`                                              |\n|                        | `PROPOSALS_MEMBERSHIP_SERIALIZER`           | Class dotpath for Proposal's Membership serializer override                                                                                                                                             | `observation_portal.proposals.serializers.MembershipSerializer`                                              |\n|                        | `PROPOSALS_PROPOSALNOTIFICATION_SERIALIZER`           | Class dotpath for Proposal's ProposalNotification serializer override                                                                                                                                             | `observation_portal.proposals.serializers.ProposalNotificationSerializer`                                              |\n|                        | `PROPOSALS_TIMELIMIT_SERIALIZER`           | Class dotpath for Proposal's Proposal serializer override                                                                                                                                             | `observation_portal.proposals.serializers.TimeLimitSerializer`                                              |\n|                        | `ACCOUNTS_PROFILE_SERIALIZER`           | Class dotpath for Accounts's Profile serializer override                                                                                                                                             | `observation_portal.accounts.serializers.ProfileSerializer`                                              |\n|                        | `ACCOUNTS_USER_SERIALIZER`           | Class dotpath for Accounts's User serializer override                                                                                                                                             | `observation_portal.accounts.serializers.UserSerializer`                                              |\n|                        | `ACCOUNTS_ACCOUNTREMOVAL_SERIALIZER`           | Class dotpath for Accounts's Account Removal serializer override                                                                                                                                             | `observation_portal.accounts.serializers.AccountRemovalSerializer`                                              |\n|                        | `SCIAPPLICATIONS_CALL_SERIALIZER`           | Class dotpath for SciApplications's Call serializer override                                                                                                                                             | `observation_portal.sciapplications.serializers.CallSerializer`                                              |\n|                        | `SCIAPPLICATIONS_SCIENCEAPPLICATION_SERIALIZER`           | Class dotpath for SciApplications's Science Application serializer override                                                                                                                                             | `observation_portal.sciapplications.serializers.ScienceApplicationSerializer`                                              |\n| as_dict Overrides   | `OBSERVATIONS_SUMMARY_AS_DICT`           | Class dotpath for Observation's Summary as_dict override                                                                                                                                             | `observation_portal.observations.models.summary_as_dict`                                                 |\n|                        | `OBSERVATIONS_CONFIGURATIONSTATUS_AS_DICT`           | Class dotpath for Observation's ConfigurationStatus as_dict override                                                                                                                                             | `observation_portal.observations.models.configurationstatus_as_dict`                                                 |\n|                        | `OBSERVATIONS_OBSERVATION_AS_DICT`           | Class dotpath for Observation's Observation as_dict override                                                                                                                                             | `observation_portal.observations.models.observation_as_dict`                                              |\n|                        | `REQUESTGROUPS_CONSTRAINTS_AS_DICT`           | Class dotpath for RequestGroups's Constraints as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.constraints_as_dict`                                              |\n|                        | `REQUESTGROUPS_REGIONOFINTEREST_AS_DICT`           | Class dotpath for RequestGroups's Instrument Config ROI as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.regionofinterest_as_dict`                                              |\n|                        | `REQUESTGROUPS_INSTRUMENTCONFIG_AS_DICT`           | Class dotpath for RequestGroups's Instrument Config as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.instrumentconfig_as_dict`                                              |\n|                        | `REQUESTGROUPS_ACQUISITIONCONFIG_AS_DICT`           | Class dotpath for RequestGroups's Acquisition Config as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.acquisitionconfig_as_dict`                                              |\n|                        | `REQUESTGROUPS_GUIDINGCONFIG_AS_DICT`           | Class dotpath for RequestGroups's Guiding Config as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.guidingconfig_as_dict`                                              |\n|                        | `REQUESTGROUPS_TARGET_AS_DICT`           | Class dotpath for RequestGroups's Target as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.target_as_dict`                                              |\n|                        | `REQUESTGROUPS_CONFIGURATION_AS_DICT`           | Class dotpath for RequestGroups's Configuration as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.configuration_as_dict`                                              |\n|                        | `REQUESTGROUPS_LOCATION_AS_DICT`           | Class dotpath for RequestGroups's Location as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.location_as_dict`                                              |\n|                        | `REQUESTGROUPS_WINDOW_AS_DICT`           | Class dotpath for RequestGroups's Window as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.window_as_dict`                                              |\n|                        | `REQUESTGROUPS_REQUEST_AS_DICT`           | Class dotpath for RequestGroups's Request as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.request_as_dict`                                              |\n|                        | `REQUESTGROUPS_REQUESTGROUP_AS_DICT`           | Class dotpath for RequestGroups's RequestGroup as_dict override                                                                                                                                             | `observation_portal.requestgroups.models.requestgroup_as_dict`                                              |\n|                        | `PROPOSALS_PROPOSAL_AS_DICT`           | Class dotpath for Proposal's Proposal as_dict override                                                                                                                                             | `observation_portal.proposals.models.proposal_as_dict`                                              |\n|                        | `PROPOSALS_TIMEALLOCATION_AS_DICT`           | Class dotpath for Proposal's TimeAllocation as_dict override                                                                                                                                             | `observation_portal.proposals.models.timeallocation_as_dict`                                              |\n|                        | `PROPOSALS_MEMBERSHIP_AS_DICT`           | Class dotpath for Proposal's Membership as_dict override                                                                                                                                             | `observation_portal.proposals.models.membership_as_dict`                                              |\n| duration Overrides   | `INSTRUMENT_CONFIGURATION_PER_EXPOSURE_DURATION`           | Class dotpath for duration_per_exposure method override                                                                                                                                             | `observation_portal.requestgroups.duration_utils.get_instrument_configuration_duration_per_exposure`                                                 |\n\n\n## Local Development\n\n### **Set up external services**\n\nPlease refer to the [Configuration Database](https://github.com/observatorycontrolsystem/configdb) and [Downtime Database](https://github.com/observatorycontrolsystem/downtime) projects for instructions on how to get those running, as well as the [Elasticsearch documentation](https://www.elastic.co/guide/en/elasticsearch/reference/5.6/install-elasticsearch.html) for options on how to run Elasticsearch.\n\n\n### **Poetry**\n\nWe use Poetry for package management. If you already have Poetry installed, you\ncan skip this section.\n\nYou can install Poetry using one of the many options listed at https://python-poetry.org/docs/#installation.\nOne simple option is using Pipx:\n\n    python3 -m pip install --user pipx\n    python3 -m pipx ensurepath\n    pipx install poetry\n\n### **Install**\n\nInstall the project and its Python dependencies:\n\n    poetry install\n\nThis will install the project in a Poetry managed virtual environment. To run\ncommands in that environment either use `poetry run ...` or start a shell in\nthat environment with `poetry shell`\n\n### **Set up the database**\n\nThis example uses the [PostgreSQL Docker image](https://hub.docker.com/_/postgres) to create a database. Make sure that the options that you use to set up your database correspond with your configured database settings.\n\n    docker run --name observation-portal-postgres -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=observation_portal -v/var/lib/postgresql/data -p5432:5432 -d postgres:11.1\n\nAfter creating the database, migrations must be applied to set up the tables in the database.\n\n    poetry run python manage.py migrate\n\n### **Run the tests**\n\n    poetry run python manage.py test --settings=observation_portal.test_settings\n\n### **Run the portal**\n\n    poetry run python manage.py runserver\n\nThe observation portal should now be accessible from <http://127.0.0.1:8000>!\n",
-    'author': 'Observatory Control System Project',
-    'author_email': 'ocs@lco.global',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://observatorycontrolsystem.github.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+    poetry run python manage.py test --settings=observation_portal.test_settings
 
+### **Run the portal**
+
+    poetry run python manage.py runserver
+
+The observation portal should now be accessible from <http://127.0.0.1:8000>!
 
-setup(**setup_kwargs)
```

