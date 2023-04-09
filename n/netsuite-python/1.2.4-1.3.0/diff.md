# Comparing `tmp/netsuite_python-1.2.4.tar.gz` & `tmp/netsuite_python-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.2.4.tar", last modified: Thu Apr  6 19:33:55 2023, max compression
+gzip compressed data, was "netsuite_python-1.3.0.tar", last modified: Sun Apr  9 23:07:45 2023, max compression
```

## Comparing `netsuite_python-1.2.4.tar` & `netsuite_python-1.3.0.tar`

### file list

```diff
@@ -1,99 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.221751 netsuite_python-1.2.4/
--rw-rw-rw-   0        0        0    11792 2023-04-06 19:33:55.221751 netsuite_python-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    11461 2023-02-01 21:44:48.000000 netsuite_python-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.079815 netsuite_python-1.2.4/netsuite/
--rw-rw-rw-   0        0        0     6813 2023-04-06 19:31:47.000000 netsuite_python-1.2.4/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/__init__.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.082815 netsuite_python-1.2.4/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     5255 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     5387 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.088815 netsuite_python-1.2.4/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.099815 netsuite_python-1.2.4/netsuite/swagger_client/
--rw-rw-rw-   0        0        0     7078 2023-04-06 19:32:28.000000 netsuite_python-1.2.4/netsuite/swagger_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.110816 netsuite_python-1.2.4/netsuite/swagger_client/api/
--rw-rw-rw-   0        0        0      350 2023-04-06 19:32:00.000000 netsuite_python-1.2.4/netsuite/swagger_client/api/__init__.py
--rw-rw-rw-   0        0        0    39267 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/api/contact_api.py
--rw-rw-rw-   0        0        0    68525 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/api/customer_api.py
--rw-rw-rw-   0        0        0    40005 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/api/message_api.py
--rw-rw-rw-   0        0        0     5582 2023-02-27 17:54:28.000000 netsuite_python-1.2.4/netsuite/swagger_client/api/query_api.py
--rw-rw-rw-   0        0        0     2289 2023-04-06 18:45:16.000000 netsuite_python-1.2.4/netsuite/swagger_client/api/restlet_api.py
--rw-rw-rw-   0        0        0    25621 2023-02-17 17:39:39.000000 netsuite_python-1.2.4/netsuite/swagger_client/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.215750 netsuite_python-1.2.4/netsuite/swagger_client/models/
--rw-rw-rw-   0        0        0     6150 2023-02-13 16:56:23.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/__init__.py
--rw-rw-rw-   0        0        0   124906 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/contact.py
--rw-rw-rw-   0        0        0     6811 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/contact_collection.py
--rw-rw-rw-   0        0        0     4007 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/contact_custom_form.py
--rw-rw-rw-   0        0        0   499116 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer.py
--rw-rw-rw-   0        0        0    15732 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_address_book_address_book_address.py
--rw-rw-rw-   0        0        0     6914 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_address_book_collection.py
--rw-rw-rw-   0        0        0    11388 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_address_book_element.py
--rw-rw-rw-   0        0        0     4156 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_alcohol_recipient_type.py
--rw-rw-rw-   0        0        0     6852 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_campaigns_collection.py
--rw-rw-rw-   0        0        0     3925 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_campaigns_element.py
--rw-rw-rw-   0        0        0     6842 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_collection.py
--rw-rw-rw-   0        0        0     6945 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_contact_roles_collection.py
--rw-rw-rw-   0        0        0     9153 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_contact_roles_element.py
--rw-rw-rw-   0        0        0     4090 2023-02-25 18:03:44.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_custom_form.py
--rw-rw-rw-   0        0        0     4098 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_email_preference.py
--rw-rw-rw-   0        0        0     4200 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_global_subscription_status.py
--rw-rw-rw-   0        0        0     6945 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_group_pricing_collection.py
--rw-rw-rw-   0        0        0     5317 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_group_pricing_element.py
--rw-rw-rw-   0        0        0     6914 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_item_pricing_collection.py
--rw-rw-rw-   0        0        0     6011 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_item_pricing_element.py
--rw-rw-rw-   0        0        0     4558 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_language.py
--rw-rw-rw-   0        0        0     4142 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_negative_number_format.py
--rw-rw-rw-   0        0        0     4066 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_number_format.py
--rw-rw-rw-   0        0        0     4089 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_shipping_carrier.py
--rw-rw-rw-   0        0        0     4082 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_symbol_placement.py
--rw-rw-rw-   0        0        0     4120 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customer_third_party_carrier.py
--rw-rw-rw-   0        0        0     5848 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/customeraddress_bookaddress_book_address_country.py
--rw-rw-rw-   0        0        0    22360 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/message.py
--rw-rw-rw-   0        0        0     7064 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/message_collection.py
--rw-rw-rw-   0        0        0     5678 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/ns_error.py
--rw-rw-rw-   0        0        0     8174 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/ns_error_oerror_details.py
--rw-rw-rw-   0        0        0     3563 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/ns_link.py
--rw-rw-rw-   0        0        0     4994 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/ns_resource.py
--rw-rw-rw-   0        0        0     6614 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/ns_resource_collection.py
--rw-rw-rw-   0        0        0     2531 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_company.py
--rw-rw-rw-   0        0        0     2599 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_course_attended.py
--rw-rw-rw-   0        0        0     2611 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_energy_eff_attended.py
--rw-rw-rw-   0        0        0     2627 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_hitachi_course_attended.py
--rw-rw-rw-   0        0        0     2607 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_hp_course_attended.py
--rw-rw-rw-   0        0        0     2611 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_pv_course_atteneded.py
--rw-rw-rw-   0        0        0     2611 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_sol_course_attended.py
--rw-rw-rw-   0        0        0     2607 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_unvent_hot_water_g3.py
--rw-rw-rw-   0        0        0     2623 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcontact_custentity_water_regulations1999.py
--rw-rw-rw-   0        0        0     2603 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_course_attended.py
--rw-rw-rw-   0        0        0     2615 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_energy_eff_attended.py
--rw-rw-rw-   0        0        0     2631 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_hitachi_course_attended.py
--rw-rw-rw-   0        0        0     2611 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_hp_course_attended.py
--rw-rw-rw-   0        0        0     2615 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_pv_course_atteneded.py
--rw-rw-rw-   0        0        0     2615 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_sol_course_attended.py
--rw-rw-rw-   0        0        0     2611 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_unvent_hot_water_g3.py
--rw-rw-rw-   0        0        0     2627 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_custentity_water_regulations1999.py
--rw-rw-rw-   0        0        0     2595 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofcustomer_item_pricing_element_item.py
--rw-rw-rw-   0        0        0     2622 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofmessage_author.py
--rw-rw-rw-   0        0        0     2622 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofmessage_entity.py
--rw-rw-rw-   0        0        0     2662 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofmessage_primary_recipient.py
--rw-rw-rw-   0        0        0     2634 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/models/one_ofmessage_recipient.py
--rw-rw-rw-   0        0        0    13258 2023-02-12 19:28:31.000000 netsuite_python-1.2.4/netsuite/swagger_client/rest.py
--rw-rw-rw-   0        0        0     1823 2023-02-25 19:42:59.000000 netsuite_python-1.2.4/netsuite/swagger_client/rest_client.py
--rw-rw-rw-   0        0        0     1098 2023-04-06 18:22:16.000000 netsuite_python-1.2.4/netsuite/swagger_client/restlet_client.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:33:55.220750 netsuite_python-1.2.4/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    11792 2023-04-06 19:33:54.000000 netsuite_python-1.2.4/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4752 2023-04-06 19:33:54.000000 netsuite_python-1.2.4/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 19:33:54.000000 netsuite_python-1.2.4/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-06 19:33:54.000000 netsuite_python-1.2.4/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-06 19:33:54.000000 netsuite_python-1.2.4/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 19:33:54.000000 netsuite_python-1.2.4/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 19:33:55.221751 netsuite_python-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-06 19:32:57.000000 netsuite_python-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.325083 netsuite_python-1.3.0/
+-rw-rw-rw-   0        0        0    11966 2023-04-09 23:07:45.325083 netsuite_python-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11635 2023-04-09 23:07:01.000000 netsuite_python-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.297084 netsuite_python-1.3.0/netsuite/
+-rw-rw-rw-   0        0        0    10514 2023-04-09 23:00:48.000000 netsuite_python-1.3.0/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.305083 netsuite_python-1.3.0/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.0/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.310083 netsuite_python-1.3.0/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.0/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.0/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.0/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.0/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.0/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.0/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.312083 netsuite_python-1.3.0/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     5255 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     5387 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.319083 netsuite_python-1.3.0/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.0/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 23:07:45.324083 netsuite_python-1.3.0/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    11966 2023-04-09 23:07:45.000000 netsuite_python-1.3.0/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-09 23:07:45.000000 netsuite_python-1.3.0/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 23:07:45.000000 netsuite_python-1.3.0/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-09 23:07:45.000000 netsuite_python-1.3.0/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-04-09 23:07:45.000000 netsuite_python-1.3.0/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 23:07:45.000000 netsuite_python-1.3.0/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 23:07:45.326083 netsuite_python-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-04-09 23:07:22.000000 netsuite_python-1.3.0/setup.py
```

### Comparing `netsuite_python-1.2.4/PKG-INFO` & `netsuite_python-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: netsuite_python
-Version: 1.2.4
-Summary: Python SDK for Netsuite API with Django Integration
-Home-page: https://bitbucket.org/theapiguys/netsuite_python
-Author: Will @ TheAPIGuys
-Author-email: will@theapiguys.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # README #
 
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
@@ -51,14 +40,20 @@
 * On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
 * Click `Create-New` button
     * Entity: The User created for TAG
     * ROLE: Role created for this integration
     * Application: Application Created for this integration
     * Certificate: Click "Choose A File" and upload the PUBLIC Cert (NOT PRIVATE KEY)
 * Copy the Certificate ID
+
+## Generate Netsuite Client ##
+* Run command to generate sdk using openapi 3.0 
+* method is generate_swagger_client
+* visit link returned from method and download result 
+* unzip the file and copy the "netsuite_client" folder from the directory into the projects root folder
 ## Setting up Netsuite SDK in a project ##
 * Run `netsuite generate-client-config`
     * It will ask you for information obtained above: You can use all the defaults
         * Client ID
         * Netsuite Certificate ID
         * Netsuite Key File
         * Netsuite Application Name
@@ -83,28 +78,23 @@
 ## Usage ##
 
 
 It is pretty simple to get started using the SDK once you have a valid token.
 
 ### Setup Netsuite ###
 ```
-import pathlib
 from netsuite import Netsuite
+import netsuite_client
+from netsuite_client.api.customer_api import CustomerApi
 
-#Include config file, config dict, or leave empty to use default setup
+netsuite = Netsuite(config_file=settings.NS_CREDENTIALS_PATH)
 
-# w/ config file 
-# netsuite = Netsuite(config_file=pathlib.Path('./netsuite-credentials.json'))
+customer_api = CustomerApi(netsuite.REST_CLIENT)
 
-# using default 
-netsuite = Netsuite()
-
-#initialize apis
-ns_contact_api = netsuite.REST_CLIENT.contact_api
-ns_customer_api = netsuite.REST_CLIENT.customer_api
+print(customer_api.customer_id_get(id=1617260))
 ```
 
 ## Example Usage ##
  ```
  print(ns_contact_api.contact_id_get(id=1413220))
  ```
 
@@ -179,9 +169,8 @@
  - [OneOfcustomerCustentityEnergyEffAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityEnergyEffAttended.md)
  - [OneOfcustomerCustentityHitachiCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHitachiCourseAttended.md)
  - [OneOfcustomerCustentityHpCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHpCourseAttended.md)
  - [OneOfcustomerCustentityPvCourseAtteneded](netsuite/swagger_client/docs/OneOfcustomerCustentityPvCourseAtteneded.md)
  - [OneOfcustomerCustentitySolCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentitySolCourseAttended.md)
  - [OneOfcustomerCustentityUnventHotWaterG3](netsuite/swagger_client/docs/OneOfcustomerCustentityUnventHotWaterG3.md)
  - [OneOfcustomerCustentityWaterRegulations1999](netsuite/swagger_client/docs/OneOfcustomerCustentityWaterRegulations1999.md)
- - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
-
+ - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
```

### Comparing `netsuite_python-1.2.4/README.md` & `netsuite_python-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: netsuite_python
+Version: 1.3.0
+Summary: Python SDK for Netsuite API with Django Integration
+Home-page: https://bitbucket.org/theapiguys/netsuite_python
+Author: Will @ TheAPIGuys
+Author-email: will@theapiguys.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # README #
 
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
@@ -40,14 +51,20 @@
 * On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
 * Click `Create-New` button
     * Entity: The User created for TAG
     * ROLE: Role created for this integration
     * Application: Application Created for this integration
     * Certificate: Click "Choose A File" and upload the PUBLIC Cert (NOT PRIVATE KEY)
 * Copy the Certificate ID
+
+## Generate Netsuite Client ##
+* Run command to generate sdk using openapi 3.0 
+* method is generate_swagger_client
+* visit link returned from method and download result 
+* unzip the file and copy the "netsuite_client" folder from the directory into the projects root folder
 ## Setting up Netsuite SDK in a project ##
 * Run `netsuite generate-client-config`
     * It will ask you for information obtained above: You can use all the defaults
         * Client ID
         * Netsuite Certificate ID
         * Netsuite Key File
         * Netsuite Application Name
@@ -72,28 +89,23 @@
 ## Usage ##
 
 
 It is pretty simple to get started using the SDK once you have a valid token.
 
 ### Setup Netsuite ###
 ```
-import pathlib
 from netsuite import Netsuite
+import netsuite_client
+from netsuite_client.api.customer_api import CustomerApi
 
-#Include config file, config dict, or leave empty to use default setup
+netsuite = Netsuite(config_file=settings.NS_CREDENTIALS_PATH)
 
-# w/ config file 
-# netsuite = Netsuite(config_file=pathlib.Path('./netsuite-credentials.json'))
+customer_api = CustomerApi(netsuite.REST_CLIENT)
 
-# using default 
-netsuite = Netsuite()
-
-#initialize apis
-ns_contact_api = netsuite.REST_CLIENT.contact_api
-ns_customer_api = netsuite.REST_CLIENT.customer_api
+print(customer_api.customer_id_get(id=1617260))
 ```
 
 ## Example Usage ##
  ```
  print(ns_contact_api.contact_id_get(id=1413220))
  ```
 
@@ -168,8 +180,9 @@
  - [OneOfcustomerCustentityEnergyEffAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityEnergyEffAttended.md)
  - [OneOfcustomerCustentityHitachiCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHitachiCourseAttended.md)
  - [OneOfcustomerCustentityHpCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentityHpCourseAttended.md)
  - [OneOfcustomerCustentityPvCourseAtteneded](netsuite/swagger_client/docs/OneOfcustomerCustentityPvCourseAtteneded.md)
  - [OneOfcustomerCustentitySolCourseAttended](netsuite/swagger_client/docs/OneOfcustomerCustentitySolCourseAttended.md)
  - [OneOfcustomerCustentityUnventHotWaterG3](netsuite/swagger_client/docs/OneOfcustomerCustentityUnventHotWaterG3.md)
  - [OneOfcustomerCustentityWaterRegulations1999](netsuite/swagger_client/docs/OneOfcustomerCustentityWaterRegulations1999.md)
- - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
+ - [OneOfcustomerItemPricingElementItem](netsuite/swagger_client/docs/OneOfcustomerItemPricingElementItem.md)
+
```

### Comparing `netsuite_python-1.2.4/netsuite/Netsuite.py` & `netsuite_python-1.3.0/netsuite/Netsuite.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import json
 import pathlib
 import jwt
 from datetime import datetime, timedelta
 from pathlib import Path
 import requests
 from netsuite.NetsuiteToken import NetsuiteToken
-from netsuite.swagger_client.rest_client import RestClient, QueryClient
-from netsuite.swagger_client.restlet_client import RestletClient
+# from netsuite.swagger_client.restlet_client import RestletClient
 from netsuite.settings import APISettings
 from netsuite.storages import BaseStorage, JSONStorage
+from netsuite import api_clients
+
+
+client_exists = False
+try:
+    import netsuite_client
+    from netsuite_client.api import *
+    client_exists = True
+except ModuleNotFoundError or ImportError as err:
+    print('Rest Client needs to be generated')
 
 
 class Netsuite:
     app_name: str = None
     storage: BaseStorage = None
     api_settings: APISettings
     rest_client = None
@@ -28,25 +37,27 @@
         if config is None and config_file is None:
             try:
                 with open(pathlib.Path(APISettings().defaults.get("CREDENTIALS_PATH")), 'r') as f:
                     config = json.load(f)
             except Exception as e:
                 raise Exception("No Configuration Present. Try Generating one.")
 
+
         self.api_settings = APISettings(config)
         if not self.api_settings.CLIENT_ID:
             raise Exception("Missing Client Id")
         if not self.api_settings.NETSUITE_APP_NAME:
             raise Exception("Missing Netsuite App Name")
         if not self.api_settings.NETSUITE_KEY_FILE:
             raise Exception("Missing Netsuite Certificate path.")
         if not self.api_settings.CERT_ID:
             raise Exception("Missing Netsuite Certificate ID.")
 
         self.app_name = self.api_settings.APP_NAME
+
         self.netsuite_app_name = self.api_settings.NETSUITE_APP_NAME
         self.netsuite_key_path = self.api_settings.NETSUITE_KEY_FILE
         self.netsuite_cert_id = self.api_settings.CERT_ID
         # self.field_map = None
         # if self.api_settings.NETSUITE_FIELD_MAP:
         #     self.field_map = self.api_settings.NETSUITE_FIELD_MAP
 
@@ -57,31 +68,39 @@
             self.storage.storage_path = self.api_settings.JSON_STORAGE_PATH
         self.rest_url = f"https://{self.api_settings.NETSUITE_APP_NAME}.suitetalk.api.netsuite.com/services/rest" \
                         f"/record/v1/ "
         self.access_token_url = f"https://{self.api_settings.NETSUITE_APP_NAME}.suitetalk.api.netsuite.com/services/rest/auth/oauth2/v1/token",
 
     @property
     def REST_CLIENT(self):
-        if not self.rest_client:
-            self.rest_client = RestClient(self)
-        return self.rest_client
+        try:
+            if not self.rest_client:
+                if client_exists:
+                    self.rest_client = self.get_rest_client()
+                    return self.rest_client
+            else:
+                print('Client needs to be generated.')
+        except Exception as e:
+            print(e)
+
 
     @property
     def QUERY_CLIENT(self):
         if not self.query_client:
-            self.query_client = QueryClient(self)
+            self.query_client = self.QueryClient(self)
             # if self.token.access_token is not None:
                 # self.get_customer_categories()
                 # self.get_status_dict()
         return self.query_client
 
+
     @property
     def RESTLET_CLIENT(self):
         if not self.restlet_client:
-            self.restlet_client = RestletClient(self)
+            self.restlet_client = self.RestletClient(self)
         return self.restlet_client
 
     @property
     def token(self) -> NetsuiteToken:
         return self.storage.get_token(self.app_name)
 
     def save_token(self, token):
@@ -125,27 +144,93 @@
         token = NetsuiteToken(**response.json())
         self.save_token(token)
         # if token.access_token is not None:
         #     self.get_customer_categories()
         #     self.get_status_dict()
         return self.token
 
-    def change_app(self, app_name):
-        self.app_name = app_name
-        if not self.token.access_token:
-            raise Exception(f"{app_name} does not have a token in storage, please authenticate")
-        # self.rest_v1 = REST_V1(self)
-        self.rest_client = RestClient(self)
+    def generate_swagger_client(self):
+        token = self.storage.get_token(self.app_name)
+        url = f"https://{self.app_name}.suitetalk.api.netsuite.com/services/rest/record/v1/metadata-catalog"
+        params = {
+            'select': 'customer'
+        }
+        headers = {
+            'Accept': 'application/swagger+json',
+            'Authorization': f'Bearer {token.access_token}'
+        }
+        response = requests.get(url, headers=headers, params=params)
+        # print(token.access_token)
+        # print(response.json())
+        data = {
+            'options': {
+                'packageName': 'netsuite_client'
+            },
+            'generateSourceCodeOnly': 'True',
+            'spec': response.json()
+        }
+        headers2 = {
+            'Content-Type': 'application/json'
+        }
+        result = requests.post('https://api-latest-master.openapi-generator.tech/api/gen/clients/python',headers=headers2, json=data)
+        print(result.json())
+        # with open("./client_schema.json", "w") as outfile:
+        #     outfile.write(json.dumps(response.json()))
 
     def get_token(self):
         if not self.token.is_expired:
             return self.token
         else:
             return self.request_access_token()
 
+
+    def get_rest_client(self):
+        configuration = netsuite_client.configuration.Configuration(
+            host="https://472052.suitetalk.api.netsuite.com/services/rest/record/v1"
+        )
+        configuration.api_key['OAuth_1.0_authorization'] = self.get_token().access_token
+        configuration.api_key_prefix['OAuth_1.0_authorization'] = 'Bearer'
+        api_client = netsuite_client.api_client.ApiClient(configuration=configuration)
+        return api_client
+
+
+    class QueryClient:
+        def __init__(self, netsuite):
+            self.netsuite = netsuite
+            self.configuration = api_clients.Configuration()
+            self.configuration.token = netsuite.storage.get_token(netsuite.app_name)
+            self.configuration.token_refresh_hook = self.refresh_token
+            self.configuration.app_name = netsuite.netsuite_app_name
+            self.configuration.host = f"https://{self.configuration.app_name}.suitetalk.api.netsuite.com/services/rest/query/v1/suiteql"
+            self.query_api_client = api_clients.ApiClient(configuration=self.configuration)
+            self.query_api = api_clients.QueryApi(api_client=self.query_api_client)
+
+        def refresh_token(self):
+            self.configuration.token = self.netsuite.get_token()
+            return self.configuration.token
+
+    class RestletClient:
+        def __init__(self, netsuite):
+            self.netsuite = netsuite
+            self.configuration = api_clients.Configuration()
+            self.configuration.token = netsuite.storage.get_token(netsuite.app_name)
+            self.configuration.token_refresh_hook = self.refresh_token
+            self.configuration.app_name = netsuite.netsuite_app_name
+            self.configuration.host = f"https://{self.configuration.app_name}.restlets.api.netsuite.com/app/site/hosting/restlet.nl"
+            self.api_client = api_clients.ApiClient(configuration=self.configuration)
+            self.restlet_api = api_clients.RestletApi(api_client=self.api_client)
+
+            # self.contact_api = swagger_client.ContactApi(api_client=self.api_client)
+            # self.customer_api = swagger_client.CustomerApi(api_client=self.api_client)
+            # self.message_api = swagger_client.MessageApi(api_client=self.api_client)
+
+        def refresh_token(self):
+            self.configuration.token = self.netsuite.get_token()
+            return self.configuration.token
+
     # def get_status_dict(self):
     #     if self.token.access_token is None:
     #         return None
     #     if self.status_dict is None:
     #         query = "SELECT * FROM EntityStatus WHERE inactive = 'F'"
     #         statuses = self.QUERY_CLIENT.query_api.execute_query(query=query)
     #         status_dict = {}
```

### Comparing `netsuite_python-1.2.4/netsuite/module_loading.py` & `netsuite_python-1.3.0/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.2.4/netsuite/scripts/cli.py` & `netsuite_python-1.3.0/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.2.4/netsuite/settings.py` & `netsuite_python-1.3.0/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.2.4/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.3.0/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.2.4/netsuite/storages/JSONStorage.py` & `netsuite_python-1.3.0/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.2.4/netsuite/swagger_client/api/query_api.py` & `netsuite_python-1.3.0/netsuite/api_clients/api/query_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 import json
 
-from netsuite.swagger_client.api_client import ApiClient
-import netsuite.swagger_client.models
+from netsuite.api_clients.api_client import ApiClient
 
 
 class QueryApi(object):
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def execute_query(self, query, **kwargs):
-        all_params = ['prefer', 'response_type', 'limit', 'offset']  # noqa: E
+        all_params = ['prefer', 'response_type', 'limit', 'offset']  # noqa: E501
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method customer_get" % key
                 )
@@ -39,41 +38,40 @@
         query_params = {}
         if 'prefer' in params:
             header_params['Prefer'] = params['prefer']  # noqa: E501
         else:
             header_params['Prefer'] = 'transient'
 
         if 'limit' in params:
-            print(params['limit'])
             if params['limit'] is not None:
-                print('set')
                 query_params['limit'] = params['limit']
             else:
                 query_params['limit'] = 500
 
         if 'offset' in params:
             if params['offset'] is not None:
                 query_params['offset'] = params['offset']
             else:
                 query_params['offset'] = 0
 
-        if 'response_type' in params:
-            if params['response_type'] is not None:
-                if hasattr(netsuite.swagger_client.models, params['response_type']):
-                    response_type = params['response_type']
-                else:
-                    response_type = None
-                    raise TypeError(f"{params['response_type']} is not a valid response type")
-            return_http_only_data = True
-            _preload_content = True
-            # print(params['response_type'])
-        else:
-            response_type = None
-            return_http_only_data = True
-            _preload_content = False
+
+        # if 'response_type' in params:
+        #     if params['response_type'] is not None:
+        #         if hasattr(netsuite.swagger_client.models, params['response_type']):
+        #             response_type = params['response_type']
+        #         else:
+        #             response_type = None
+        #             raise TypeError(f"{params['response_type']} is not a valid response type")
+        #     return_http_only_data = True
+        #     _preload_content = True
+        #     # print(params['response_type'])
+        # else:
+        response_type = None
+        return_http_only_data = True
+        _preload_content = False
 
         # Authentication setting
         auth_settings = ['oAuth2ClientCredentials']
         response = self.api_client.call_api('',
                                             'POST',
                                             header_params=header_params,
                                             query_params=query_params,
```

### Comparing `netsuite_python-1.2.4/netsuite/swagger_client/api/restlet_api.py` & `netsuite_python-1.3.0/netsuite/api_clients/api/restlet_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 import json
 
-from netsuite.swagger_client.api_client import ApiClient
-import netsuite.swagger_client.models
+from netsuite.api_clients.api_client import ApiClient
+
 
 
 class RestletApi(object):
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
```

### Comparing `netsuite_python-1.2.4/netsuite/swagger_client/api_client.py` & `netsuite_python-1.3.0/netsuite/api_clients/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 import re
 import tempfile
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
-from netsuite.swagger_client.configuration import Configuration
-import netsuite.swagger_client.models
-from netsuite.swagger_client import rest
+from netsuite.api_clients.configuration import Configuration
+from netsuite.api_clients import rest
 
 
 class ApiClient(object):
     """Generic API client for Swagger client library builds.
 
     Swagger generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
```

### Comparing `netsuite_python-1.2.4/netsuite/swagger_client/configuration.py` & `netsuite_python-1.3.0/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.2.4/netsuite/swagger_client/rest.py` & `netsuite_python-1.3.0/netsuite/api_clients/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
                 key_file=configuration.key_file,
                 **addition_pool_args
             )
 
     def request(self, method, url, query_params=None, headers=None,
                 body=None, post_params=None, _preload_content=True,
                 _request_timeout=None):
+
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param query_params: query parameters in the url
         :param headers: http request headers
         :param body: request json body, for `application/json`
@@ -121,14 +122,15 @@
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         """
+
         method = method.upper()
         assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
                           'PATCH', 'OPTIONS']
 
         if post_params and body:
             raise ValueError(
                 "body parameter cannot be used with post_params parameter."
@@ -147,15 +149,14 @@
                     connect=_request_timeout[0], read=_request_timeout[1])
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/json'
 
         if headers.get("Accept") == "application/vnd.oracle.resource+json; type=error":
             headers["Accept"] = "application/vnd.oracle.resource+json; type=singular"
-
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
                 if query_params:
                     url += '?' + urlencode(query_params)
                 if re.search('json', headers['Content-Type'], re.IGNORECASE):
                     request_body = '{}'
```

### Comparing `netsuite_python-1.2.4/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.3.0/netsuite_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.2.4
+Version: 1.3.0
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -51,14 +51,20 @@
 * On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
 * Click `Create-New` button
     * Entity: The User created for TAG
     * ROLE: Role created for this integration
     * Application: Application Created for this integration
     * Certificate: Click "Choose A File" and upload the PUBLIC Cert (NOT PRIVATE KEY)
 * Copy the Certificate ID
+
+## Generate Netsuite Client ##
+* Run command to generate sdk using openapi 3.0 
+* method is generate_swagger_client
+* visit link returned from method and download result 
+* unzip the file and copy the "netsuite_client" folder from the directory into the projects root folder
 ## Setting up Netsuite SDK in a project ##
 * Run `netsuite generate-client-config`
     * It will ask you for information obtained above: You can use all the defaults
         * Client ID
         * Netsuite Certificate ID
         * Netsuite Key File
         * Netsuite Application Name
@@ -83,28 +89,23 @@
 ## Usage ##
 
 
 It is pretty simple to get started using the SDK once you have a valid token.
 
 ### Setup Netsuite ###
 ```
-import pathlib
 from netsuite import Netsuite
+import netsuite_client
+from netsuite_client.api.customer_api import CustomerApi
 
-#Include config file, config dict, or leave empty to use default setup
-
-# w/ config file 
-# netsuite = Netsuite(config_file=pathlib.Path('./netsuite-credentials.json'))
+netsuite = Netsuite(config_file=settings.NS_CREDENTIALS_PATH)
 
-# using default 
-netsuite = Netsuite()
+customer_api = CustomerApi(netsuite.REST_CLIENT)
 
-#initialize apis
-ns_contact_api = netsuite.REST_CLIENT.contact_api
-ns_customer_api = netsuite.REST_CLIENT.customer_api
+print(customer_api.customer_id_get(id=1617260))
 ```
 
 ## Example Usage ##
  ```
  print(ns_contact_api.contact_id_get(id=1413220))
  ```
```

### Comparing `netsuite_python-1.2.4/setup.py` & `netsuite_python-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.2.4',
+    version='1.3.0',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

