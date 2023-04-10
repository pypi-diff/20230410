# Comparing `tmp/eea.volto.policy-1.7.zip` & `tmp/eea.volto.policy-2.0.zip`

## zipinfo {}

```diff
@@ -1,277 +1,256 @@
-Zip file size: 85167 bytes, number of entries: 275
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/buildouts/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/docs/
--rw-r--r--  2.0 unx     2286 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/CONTRIBUTING.md
--rw-r--r--  2.0 unx     2989 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/README.rst
--rw-r--r--  2.0 unx     4981 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/PKG-INFO
--rw-r--r--  2.0 unx     9225 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/Jenkinsfile
--rw-r--r--  2.0 unx       38 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/setup.cfg
--rw-r--r--  2.0 unx      245 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/.editorconfig
--rw-r--r--  2.0 unx     3987 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/tox.ini
--rw-r--r--  2.0 unx     1693 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/.travis.yml
--rw-r--r--  2.0 unx       29 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/.gitattributes
--rw-r--r--  2.0 unx     1758 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/setup.py
--rw-r--r--  2.0 unx      426 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/.gitignore
--rw-r--r--  2.0 unx      126 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/MANIFEST.in
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/
--rw-r--r--  2.0 unx       93 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/
--rw-r--r--  2.0 unx       93 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/behaviors/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/profiles/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/vocabularies/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/tests/
--rw-r--r--  2.0 unx      707 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/interfaces.py
--rw-r--r--  2.0 unx     1307 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/patches.py
--rw-r--r--  2.0 unx      115 b- defN 22-Dec-09 11:42 eea.volto.policy-1.7/eea/volto/policy/overrides.zcml
--rw-r--r--  2.0 unx      346 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/README.txt
--rw-r--r--  2.0 unx      594 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/patches.zcml
--rw-r--r--  2.0 unx        4 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/version.txt
--rw-r--r--  2.0 unx      456 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/configure.zcml
--rw-r--r--  2.0 unx      221 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/__init__.py
--rw-r--r--  2.0 unx    14755 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/setuphandlers.py
--rw-r--r--  2.0 unx     1410 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles.zcml
--rw-r--r--  2.0 unx      139 b- defN 22-Dec-09 11:42 eea.volto.policy-1.7/eea/volto/policy/behaviors/configure.zcml
--rw-r--r--  2.0 unx       18 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/behaviors/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/profiles/default/
--rw-r--r--  2.0 unx      126 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/uninstall/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types/
--rw-r--r--  2.0 unx       94 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/catalog.xml
--rw-r--r--  2.0 unx      173 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/browserlayer.xml
--rw-r--r--  2.0 unx      253 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/metadata.xml
--rw-r--r--  2.0 unx      619 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/controlpanel.xml
--rw-r--r--  2.0 unx      241 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types.xml
--rw-r--r--  2.0 unx      573 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/registry.xml
--rw-r--r--  2.0 unx      584 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types/Document.xml
--rw-r--r--  2.0 unx     1699 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types/Plone_Site.xml
--rw-r--r--  2.0 unx       94 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/default/catalog.xml
--rw-r--r--  2.0 unx      173 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/default/browserlayer.xml
--rw-r--r--  2.0 unx      179 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/profiles/default/metadata.xml
--rw-r--r--  2.0 unx      510 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/default/controlpanel.xml
--rw-r--r--  2.0 unx      589 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/profiles/default/registry.xml
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/de/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/pt/
--rwxr-xr-x  2.0 unx      218 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/eea.pot
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx       28 b- defN 22-Aug-01 11:41 eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx       88 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/vocabularies/configure.zcml
--rw-r--r--  2.0 unx       21 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/vocabularies/__init__.py
--rw-r--r--  2.0 unx      452 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/upgrades/configure.zcml
--rw-r--r--  2.0 unx       17 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/upgrades/__init__.py
--rw-r--r--  2.0 unx      672 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/tests/__init__.py
--rw-r--r--  2.0 unx     1984 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/eea/volto/policy/tests/base.py
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/buildouts/plone5/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Dec-09 11:43 eea.volto.policy-1.7/buildouts/plone4/
--rw-r--r--  2.0 unx      232 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone5/docker-compose.yml
--rw-r--r--  2.0 unx      231 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone5/buildout.cfg
--rwxr-xr-x  2.0 unx      153 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone5/install.sh
--rw-r--r--  2.0 unx      121 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone5/.gitignore
--rw-r--r--  2.0 unx      232 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone4/docker-compose.yml
--rw-r--r--  2.0 unx      231 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone4/buildout.cfg
--rwxr-xr-x  2.0 unx      153 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone4/install.sh
--rw-r--r--  2.0 unx       83 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/buildouts/plone4/.gitignore
--rw-r--r--  2.0 unx        1 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       40 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/entry_points.txt
--rw-r--r--  2.0 unx     4981 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       14 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        4 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/top_level.txt
--rw-r--r--  2.0 unx     8243 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/eea.volto.policy.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Aug-01 11:37 eea.volto.policy-1.7/eea.volto.policy.egg-info/not-zip-safe
--rw-r--r--  2.0 unx     1041 b- defN 22-Dec-09 11:43 eea.volto.policy-1.7/docs/HISTORY.txt
--rw-r--r--  2.0 unx      915 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 22-Aug-01 11:35 eea.volto.policy-1.7/docs/LICENSE.GPL
-275 files, 93980 bytes uncompressed, 31507 bytes compressed:  66.5%
+Zip file size: 72216 bytes, number of entries: 254
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/setup.cfg
+-rw-r--r--  2.0 unx     2286 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     5138 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/PKG-INFO
+-rw-r--r--  2.0 unx     2989 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/README.rst
+-rw-r--r--  2.0 unx     1672 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/MANIFEST.in
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      915 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/docs/LICENSE.GPL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5138 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     7716 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea.volto.policy.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/
+-rw-r--r--  2.0 unx       93 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/
+-rw-r--r--  2.0 unx       93 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/behaviors/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/vocabularies/
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/version.txt
+-rw-r--r--  2.0 unx      454 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/configure.zcml
+-rw-r--r--  2.0 unx      759 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/setuphandlers.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/interfaces.py
+-rw-r--r--  2.0 unx      346 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/README.txt
+-rw-r--r--  2.0 unx      115 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/overrides.zcml
+-rw-r--r--  2.0 unx     1039 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles.zcml
+-rw-r--r--  2.0 unx      221 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/configure.zcml
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/__init__.py
+-rw-r--r--  2.0 unx      168 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/configure.zcml
+-rw-r--r--  2.0 unx     2335 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/dxfields.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/__init__.py
+-rw-r--r--  2.0 unx      166 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/configure.zcml
+-rw-r--r--  2.0 unx     1163 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/dxfields.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/__init__.py
+-rw-r--r--  2.0 unx      759 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/upgrades/configure.zcml
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/upgrades/__init__.py
+-rw-r--r--  2.0 unx     1428 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/tests/base.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/tests/__init__.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/behaviors/configure.zcml
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/behaviors/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles/default/
+-rw-r--r--  2.0 unx      126 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--  2.0 unx      179 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx      173 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/profiles/default/browserlayer.xml
+-rw-r--r--  2.0 unx       88 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/vocabularies/configure.zcml
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-10 16:56 eea.volto.policy-2.0/eea/volto/policy/vocabularies/__init__.py
+254 files, 58567 bytes uncompressed, 22084 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,826 +1,763 @@
-Filename: eea.volto.policy-1.7/
+Filename: eea.volto.policy-2.0/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/
+Filename: eea.volto.policy-2.0/docs/
 Comment: 
 
-Filename: eea.volto.policy-1.7/buildouts/
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/
+Filename: eea.volto.policy-2.0/eea/
 Comment: 
 
-Filename: eea.volto.policy-1.7/docs/
+Filename: eea.volto.policy-2.0/setup.cfg
 Comment: 
 
-Filename: eea.volto.policy-1.7/CONTRIBUTING.md
+Filename: eea.volto.policy-2.0/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.volto.policy-1.7/README.rst
+Filename: eea.volto.policy-2.0/PKG-INFO
 Comment: 
 
-Filename: eea.volto.policy-1.7/PKG-INFO
+Filename: eea.volto.policy-2.0/README.rst
 Comment: 
 
-Filename: eea.volto.policy-1.7/Jenkinsfile
+Filename: eea.volto.policy-2.0/setup.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/setup.cfg
+Filename: eea.volto.policy-2.0/MANIFEST.in
 Comment: 
 
-Filename: eea.volto.policy-1.7/.editorconfig
+Filename: eea.volto.policy-2.0/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/tox.ini
+Filename: eea.volto.policy-2.0/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/.travis.yml
+Filename: eea.volto.policy-2.0/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.volto.policy-1.7/.gitattributes
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/setup.py
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/.gitignore
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.volto.policy-1.7/MANIFEST.in
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/__init__.py
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/requires.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/__init__.py
+Filename: eea.volto.policy-2.0/eea.volto.policy.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/behaviors/
+Filename: eea.volto.policy-2.0/eea/volto/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/
+Filename: eea.volto.policy-2.0/eea/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/
+Filename: eea.volto.policy-2.0/eea/volto/policy/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/vocabularies/
+Filename: eea.volto.policy-2.0/eea/volto/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/upgrades/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/tests/
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/interfaces.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/upgrades/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/patches.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/tests/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/overrides.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/behaviors/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/README.txt
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/patches.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/vocabularies/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/version.txt
+Filename: eea.volto.policy-2.0/eea/volto/policy/version.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/configure.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/__init__.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/setuphandlers.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/setuphandlers.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/interfaces.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/README.txt
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/behaviors/configure.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/overrides.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/behaviors/__init__.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/uninstall/
+Filename: eea.volto.policy-2.0/eea/volto/policy/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/default/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/en/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/uninstall/browserlayer.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hr/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/es/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/catalog.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/browserlayer.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ro/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/metadata.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eu/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/controlpanel.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/el/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/it/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/registry.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ru/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types/Document.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/is/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/plone4/types/Plone_Site.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lt/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/default/catalog.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hu/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/default/browserlayer.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/nl/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/default/metadata.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/default/controlpanel.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fi/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/profiles/default/registry.xml
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lv/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sl/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sl/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/en/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/mt/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/da/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/tr/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/is/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/no/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/cs/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sv/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hr/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/bg/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lt/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/kl/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/nl/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/et/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/no/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sk/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/el/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pl/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/cs/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fi/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/da/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/tr/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fr/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/et/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/de/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hu/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eea.pot
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/update.sh
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ru/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/mt/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/es/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fr/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pl/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/kl/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sk/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/it/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lv/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eu/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ro/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/de/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/bg/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sv/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/update.sh
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/plone-manual.pot
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/__init__.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eea.pot
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/dxfields.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/deserializer/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/dxfields.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/restapi/serializer/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/upgrades/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/
+Filename: eea.volto.policy-2.0/eea/volto/policy/tests/base.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/tests/test_doctests.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/tests/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-2.0/eea/volto/policy/behaviors/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-2.0/eea/volto/policy/behaviors/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/vocabularies/configure.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles/uninstall/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/vocabularies/__init__.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles/default/
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/upgrades/configure.zcml
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/upgrades/__init__.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/tests/test_doctests.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/tests/__init__.py
+Filename: eea.volto.policy-2.0/eea/volto/policy/vocabularies/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-1.7/eea/volto/policy/tests/base.py
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone5/
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone4/
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone5/docker-compose.yml
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone5/buildout.cfg
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone5/install.sh
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone5/.gitignore
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone4/docker-compose.yml
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone4/buildout.cfg
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone4/install.sh
-Comment: 
-
-Filename: eea.volto.policy-1.7/buildouts/plone4/.gitignore
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/dependency_links.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/entry_points.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/PKG-INFO
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/namespace_packages.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/top_level.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/SOURCES.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/requires.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/eea.volto.policy.egg-info/not-zip-safe
-Comment: 
-
-Filename: eea.volto.policy-1.7/docs/HISTORY.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/docs/LICENSE.txt
-Comment: 
-
-Filename: eea.volto.policy-1.7/docs/LICENSE.GPL
+Filename: eea.volto.policy-2.0/eea/volto/policy/vocabularies/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.volto.policy-1.7/CONTRIBUTING.md` & `eea.volto.policy-2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-1.7/README.rst` & `eea.volto.policy-2.0/README.rst`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-1.7/PKG-INFO` & `eea.volto.policy-2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: eea.volto.policy
-Version: 1.7
+Version: 2.0
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.volto.policy
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/x-rst
 Provides-Extra: test
@@ -126,14 +125,21 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+2.0 - (2023-04-10)
+---------------------------
+* Bug fix: RestAPI fix DateTime timezone for publication fields serializer/deserializer
+  [avoinea refs #250368]
+* Cleanup: Drop Python2/Plone4 support
+  [avoinea refs #250368]
+
 1.7 - (2021-11-23)
 ---------------------------
 * Change: Removed types already present in plone.volto
   [iulianpetchesi refs #139888]
 
 1.6 - (2021-11-22)
 ---------------------------
@@ -165,7 +171,9 @@
 * Change: fixed history.txt
   [Petchesi-Iulian refs #121942]
 
 1.0 - (2020-12-08)
 -----------------------
 * Initial release: Added behaviors/controlpanel/patches/vocabulary from kitconcept.volto
   [Petchesi-Iulian refs #121942]
+
+
```

## Comparing `eea.volto.policy-1.7/setup.py` & `eea.volto.policy-2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,17 @@
         open("README.rst").read() + "\n" +
         open(os.path.join("docs", "HISTORY.txt")).read()
     ),
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
-        "Framework :: Plone :: 4.3",
         "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='EEA Add-ons Plone Zope',
```

## Comparing `eea.volto.policy-1.7/eea/volto/policy/profiles.zcml` & `eea.volto.policy-2.0/eea/volto/policy/profiles.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,23 @@
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="eea">
 
   <five:registerPackage package="." initialize=".initialize" />
 
   <genericsetup:registerProfile
-      zcml:condition="have plone-5"
       name="default"
       title="eea.volto.policy"
       directory="profiles/default"
       description="Installs the eea.volto.policy add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
       post_handler=".setuphandlers.post_install"
       />
 
   <genericsetup:registerProfile
-      zcml:condition="not-have plone-5"
-      name="default"
-      title="eea.volto.policy"
-      directory="profiles/plone4"
-      description="Installs the eea.volto.policy add-on."
-      provides="Products.GenericSetup.interfaces.EXTENSION"
-      post_handler=".setuphandlers.post_install"
-      />
-
-  <genericsetup:registerProfile
       name="uninstall"
       title="eea.volto.policy (uninstall)"
       directory="profiles/uninstall"
       description="Uninstalls the eea.volto.policy add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
       post_handler=".setuphandlers.uninstall"
       />
```

## Comparing `eea.volto.policy-1.7/eea/volto/policy/tests/test_doctests.py` & `eea.volto.policy-2.0/eea/volto/policy/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-1.7/eea/volto/policy/tests/base.py` & `eea.volto.policy-2.0/eea/volto/policy/tests/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,50 @@
 # pylint: disable = C0412
 """ Base test cases
 """
-from Products.CMFPlone import setuphandlers
 from plone.testing import z2
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import setRoles
 
 
-try:
-    # Plone 4
-    from Products.CMFPlone.interfaces import IFactoryTool
-    assert IFactoryTool
-    IS_PLONE_4 = True
-except ImportError:
-    IS_PLONE_4 = False
-
-
-
 class EEAFixture(PloneSandboxLayer):
     """ EEA Testing Policy
     """
     def setUpZope(self, app, configurationContext):
         """ Setup Zope
         """
         import eea.volto.policy
         self.loadZCML(package=eea.volto.policy)
         z2.installProduct(app, 'eea.volto.policy')
 
-        # Plone 4
-        if IS_PLONE_4:
-            z2.installProduct(app, 'Products.DateRecurringIndex')
-
 
     def setUpPloneSite(self, portal):
         """ Setup Plone
         """
         applyProfile(portal, 'eea.volto.policy:default')
 
         # Default workflow
         wftool = portal['portal_workflow']
         wftool.setDefaultChain('simple_publication_workflow')
 
         # Login as manager
         setRoles(portal, TEST_USER_ID, ['Manager'])
 
         # Add default Plone content
-        try:
-            applyProfile(portal, 'plone.app.contenttypes:plone-content')
-        except KeyError:
-            # BBB Plone 4
-            setuphandlers.setupPortalContent(portal)
+        applyProfile(portal, 'plone.app.contenttypes:default')
 
         # Create testing environment
-        portal.invokeFactory("Folder", "sandbox", title="Sandbox")
+        portal.invokeFactory("Document", "sandbox", title="Sandbox")
 
 
     def tearDownZope(self, app):
         """ Uninstall Zope
         """
         z2.uninstallProduct(app, 'eea.volto.policy')
 
-        # Plone 4
-        if IS_PLONE_4:
-            z2.uninstallProduct(app, 'Products.DateRecurringIndex')
-
 
 EEAFIXTURE = EEAFixture()
 FUNCTIONAL_TESTING = FunctionalTesting(bases=(EEAFIXTURE,),
                                        name='EEApolicy:Functional')
```

## Comparing `eea.volto.policy-1.7/eea.volto.policy.egg-info/PKG-INFO` & `eea.volto.policy-2.0/eea.volto.policy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: eea.volto.policy
-Version: 1.7
+Version: 2.0
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.volto.policy
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/x-rst
 Provides-Extra: test
@@ -126,14 +125,21 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+2.0 - (2023-04-10)
+---------------------------
+* Bug fix: RestAPI fix DateTime timezone for publication fields serializer/deserializer
+  [avoinea refs #250368]
+* Cleanup: Drop Python2/Plone4 support
+  [avoinea refs #250368]
+
 1.7 - (2021-11-23)
 ---------------------------
 * Change: Removed types already present in plone.volto
   [iulianpetchesi refs #139888]
 
 1.6 - (2021-11-22)
 ---------------------------
@@ -165,7 +171,9 @@
 * Change: fixed history.txt
   [Petchesi-Iulian refs #121942]
 
 1.0 - (2020-12-08)
 -----------------------
 * Initial release: Added behaviors/controlpanel/patches/vocabulary from kitconcept.volto
   [Petchesi-Iulian refs #121942]
+
+
```

## Comparing `eea.volto.policy-1.7/eea.volto.policy.egg-info/SOURCES.txt` & `eea.volto.policy-2.0/eea.volto.policy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-.editorconfig
-.gitattributes
-.gitignore
-.travis.yml
 CONTRIBUTING.md
-Jenkinsfile
 MANIFEST.in
 README.rst
 setup.py
-tox.ini
-buildouts/plone4/.gitignore
-buildouts/plone4/buildout.cfg
-buildouts/plone4/docker-compose.yml
-buildouts/plone4/install.sh
-buildouts/plone5/.gitignore
-buildouts/plone5/buildout.cfg
-buildouts/plone5/docker-compose.yml
-buildouts/plone5/install.sh
 docs/HISTORY.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 eea/__init__.py
 eea.volto.policy.egg-info/PKG-INFO
 eea.volto.policy.egg-info/SOURCES.txt
 eea.volto.policy.egg-info/dependency_links.txt
@@ -30,16 +16,14 @@
 eea.volto.policy.egg-info/top_level.txt
 eea/volto/__init__.py
 eea/volto/policy/README.txt
 eea/volto/policy/__init__.py
 eea/volto/policy/configure.zcml
 eea/volto/policy/interfaces.py
 eea/volto/policy/overrides.zcml
-eea/volto/policy/patches.py
-eea/volto/policy/patches.zcml
 eea/volto/policy/profiles.zcml
 eea/volto/policy/setuphandlers.py
 eea/volto/policy/version.txt
 eea/volto/policy/behaviors/__init__.py
 eea/volto/policy/behaviors/configure.zcml
 eea/volto/policy/locales/__init__.py
 eea/volto/policy/locales/eea.pot
@@ -166,27 +150,24 @@
 eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
 eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
 eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
 eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
 eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
 eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
 eea/volto/policy/profiles/default/browserlayer.xml
-eea/volto/policy/profiles/default/catalog.xml
-eea/volto/policy/profiles/default/controlpanel.xml
 eea/volto/policy/profiles/default/metadata.xml
-eea/volto/policy/profiles/default/registry.xml
-eea/volto/policy/profiles/plone4/browserlayer.xml
-eea/volto/policy/profiles/plone4/catalog.xml
-eea/volto/policy/profiles/plone4/controlpanel.xml
-eea/volto/policy/profiles/plone4/metadata.xml
-eea/volto/policy/profiles/plone4/registry.xml
-eea/volto/policy/profiles/plone4/types.xml
-eea/volto/policy/profiles/plone4/types/Document.xml
-eea/volto/policy/profiles/plone4/types/Plone_Site.xml
 eea/volto/policy/profiles/uninstall/browserlayer.xml
+eea/volto/policy/restapi/__init__.py
+eea/volto/policy/restapi/configure.zcml
+eea/volto/policy/restapi/deserializer/__init__.py
+eea/volto/policy/restapi/deserializer/configure.zcml
+eea/volto/policy/restapi/deserializer/dxfields.py
+eea/volto/policy/restapi/serializer/__init__.py
+eea/volto/policy/restapi/serializer/configure.zcml
+eea/volto/policy/restapi/serializer/dxfields.py
 eea/volto/policy/tests/__init__.py
 eea/volto/policy/tests/base.py
 eea/volto/policy/tests/test_doctests.py
 eea/volto/policy/upgrades/__init__.py
 eea/volto/policy/upgrades/configure.zcml
 eea/volto/policy/vocabularies/__init__.py
 eea/volto/policy/vocabularies/configure.zcml
```

## Comparing `eea.volto.policy-1.7/docs/HISTORY.txt` & `eea.volto.policy-2.0/docs/HISTORY.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0 - (2023-04-10)
+---------------------------
+* Bug fix: RestAPI fix DateTime timezone for publication fields serializer/deserializer
+  [avoinea refs #250368]
+* Cleanup: Drop Python2/Plone4 support
+  [avoinea refs #250368]
+
 1.7 - (2021-11-23)
 ---------------------------
 * Change: Removed types already present in plone.volto
   [iulianpetchesi refs #139888]
 
 1.6 - (2021-11-22)
 ---------------------------
```

## Comparing `eea.volto.policy-1.7/docs/LICENSE.txt` & `eea.volto.policy-2.0/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-1.7/docs/LICENSE.GPL` & `eea.volto.policy-2.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

