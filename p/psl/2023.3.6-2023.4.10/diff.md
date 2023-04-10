# Comparing `tmp/psl-2023.3.6.tar.gz` & `tmp/psl-2023.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.3.6.tar", last modified: Mon Mar  6 13:09:12 2023, max compression
+gzip compressed data, was "psl-2023.4.10.tar", last modified: Mon Apr 10 13:05:27 2023, max compression
```

## Comparing `psl-2023.3.6.tar` & `psl-2023.4.10.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:09:12.136438 psl-2023.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-03-06 13:08:34.000000 psl-2023.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-06 13:08:34.000000 psl-2023.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-06 13:09:12.136438 psl-2023.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-06 13:08:34.000000 psl-2023.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:09:12.132438 psl-2023.3.6/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-03-06 13:08:45.000000 psl-2023.3.6/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   117979 2023-03-06 13:08:45.000000 psl-2023.3.6/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 13:08:34.000000 psl-2023.3.6/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:09:12.136438 psl-2023.3.6/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-06 13:09:12.000000 psl-2023.3.6/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-06 13:09:12.000000 psl-2023.3.6/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 13:09:12.000000 psl-2023.3.6/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 13:08:59.000000 psl-2023.3.6/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 13:09:12.000000 psl-2023.3.6/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 13:09:12.136438 psl-2023.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-06 13:08:34.000000 psl-2023.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:05:27.813867 psl-2023.4.10/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-10 13:04:53.000000 psl-2023.4.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 13:04:53.000000 psl-2023.4.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-10 13:05:27.813867 psl-2023.4.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-10 13:04:53.000000 psl-2023.4.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:05:27.813867 psl-2023.4.10/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-10 13:05:01.000000 psl-2023.4.10/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   108947 2023-04-10 13:05:01.000000 psl-2023.4.10/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:04:53.000000 psl-2023.4.10/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:05:27.813867 psl-2023.4.10/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:05:15.000000 psl-2023.4.10/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 13:05:27.000000 psl-2023.4.10/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:05:27.813867 psl-2023.4.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-10 13:04:53.000000 psl-2023.4.10/setup.py
```

### Comparing `psl-2023.3.6/LICENSE` & `psl-2023.4.10/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.3.6/PKG-INFO` & `psl-2023.4.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.3.6
+Version: 2023.4.10
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.3.6/README.md` & `psl-2023.4.10/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.3.6/psl/__init__.py` & `psl-2023.4.10/psl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.3.6"
-__checksum__ = "b72f10dace8f91f397e8b0c7b7c4ea8ef1603a16"
+__version__ = "2023.4.10"
+__checksum__ = "39ac0fd18a8d6b9126a82fc3d5b5e96ea4d9808e"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.3.6/psl/psl.txt` & `psl-2023.4.10/psl/psl.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3603,560 +3603,14 @@
 net.mu
 org.mu
 gov.mu
 ac.mu
 co.mu
 or.mu
 museum
-academy.museum
-agriculture.museum
-air.museum
-airguard.museum
-alabama.museum
-alaska.museum
-amber.museum
-ambulance.museum
-american.museum
-americana.museum
-americanantiques.museum
-americanart.museum
-amsterdam.museum
-and.museum
-annefrank.museum
-anthro.museum
-anthropology.museum
-antiques.museum
-aquarium.museum
-arboretum.museum
-archaeological.museum
-archaeology.museum
-architecture.museum
-art.museum
-artanddesign.museum
-artcenter.museum
-artdeco.museum
-arteducation.museum
-artgallery.museum
-arts.museum
-artsandcrafts.museum
-asmatart.museum
-assassination.museum
-assisi.museum
-association.museum
-astronomy.museum
-atlanta.museum
-austin.museum
-australia.museum
-automotive.museum
-aviation.museum
-axis.museum
-badajoz.museum
-baghdad.museum
-bahn.museum
-bale.museum
-baltimore.museum
-barcelona.museum
-baseball.museum
-basel.museum
-baths.museum
-bauern.museum
-beauxarts.museum
-beeldengeluid.museum
-bellevue.museum
-bergbau.museum
-berkeley.museum
-berlin.museum
-bern.museum
-bible.museum
-bilbao.museum
-bill.museum
-birdart.museum
-birthplace.museum
-bonn.museum
-boston.museum
-botanical.museum
-botanicalgarden.museum
-botanicgarden.museum
-botany.museum
-brandywinevalley.museum
-brasil.museum
-bristol.museum
-british.museum
-britishcolumbia.museum
-broadcast.museum
-brunel.museum
-brussel.museum
-brussels.museum
-bruxelles.museum
-building.museum
-burghof.museum
-bus.museum
-bushey.museum
-cadaques.museum
-california.museum
-cambridge.museum
-can.museum
-canada.museum
-capebreton.museum
-carrier.museum
-cartoonart.museum
-casadelamoneda.museum
-castle.museum
-castres.museum
-celtic.museum
-center.museum
-chattanooga.museum
-cheltenham.museum
-chesapeakebay.museum
-chicago.museum
-children.museum
-childrens.museum
-childrensgarden.museum
-chiropractic.museum
-chocolate.museum
-christiansburg.museum
-cincinnati.museum
-cinema.museum
-circus.museum
-civilisation.museum
-civilization.museum
-civilwar.museum
-clinton.museum
-clock.museum
-coal.museum
-coastaldefence.museum
-cody.museum
-coldwar.museum
-collection.museum
-colonialwilliamsburg.museum
-coloradoplateau.museum
-columbia.museum
-columbus.museum
-communication.museum
-communications.museum
-community.museum
-computer.museum
-computerhistory.museum
-xn--comunicaes-v6a2o.museum
-contemporary.museum
-contemporaryart.museum
-convent.museum
-copenhagen.museum
-corporation.museum
-xn--correios-e-telecomunicaes-ghc29a.museum
-corvette.museum
-costume.museum
-countryestate.museum
-county.museum
-crafts.museum
-cranbrook.museum
-creation.museum
-cultural.museum
-culturalcenter.museum
-culture.museum
-cyber.museum
-cymru.museum
-dali.museum
-dallas.museum
-database.museum
-ddr.museum
-decorativearts.museum
-delaware.museum
-delmenhorst.museum
-denmark.museum
-depot.museum
-design.museum
-detroit.museum
-dinosaur.museum
-discovery.museum
-dolls.museum
-donostia.museum
-durham.museum
-eastafrica.museum
-eastcoast.museum
-education.museum
-educational.museum
-egyptian.museum
-eisenbahn.museum
-elburg.museum
-elvendrell.museum
-embroidery.museum
-encyclopedic.museum
-england.museum
-entomology.museum
-environment.museum
-environmentalconservation.museum
-epilepsy.museum
-essex.museum
-estate.museum
-ethnology.museum
-exeter.museum
-exhibition.museum
-family.museum
-farm.museum
-farmequipment.museum
-farmers.museum
-farmstead.museum
-field.museum
-figueres.museum
-filatelia.museum
-film.museum
-fineart.museum
-finearts.museum
-finland.museum
-flanders.museum
-florida.museum
-force.museum
-fortmissoula.museum
-fortworth.museum
-foundation.museum
-francaise.museum
-frankfurt.museum
-franziskaner.museum
-freemasonry.museum
-freiburg.museum
-fribourg.museum
-frog.museum
-fundacio.museum
-furniture.museum
-gallery.museum
-garden.museum
-gateway.museum
-geelvinck.museum
-gemological.museum
-geology.museum
-georgia.museum
-giessen.museum
-glas.museum
-glass.museum
-gorge.museum
-grandrapids.museum
-graz.museum
-guernsey.museum
-halloffame.museum
-hamburg.museum
-handson.museum
-harvestcelebration.museum
-hawaii.museum
-health.museum
-heimatunduhren.museum
-hellas.museum
-helsinki.museum
-hembygdsforbund.museum
-heritage.museum
-histoire.museum
-historical.museum
-historicalsociety.museum
-historichouses.museum
-historisch.museum
-historisches.museum
-history.museum
-historyofscience.museum
-horology.museum
-house.museum
-humanities.museum
-illustration.museum
-imageandsound.museum
-indian.museum
-indiana.museum
-indianapolis.museum
-indianmarket.museum
-intelligence.museum
-interactive.museum
-iraq.museum
-iron.museum
-isleofman.museum
-jamison.museum
-jefferson.museum
-jerusalem.museum
-jewelry.museum
-jewish.museum
-jewishart.museum
-jfk.museum
-journalism.museum
-judaica.museum
-judygarland.museum
-juedisches.museum
-juif.museum
-karate.museum
-karikatur.museum
-kids.museum
-koebenhavn.museum
-koeln.museum
-kunst.museum
-kunstsammlung.museum
-kunstunddesign.museum
-labor.museum
-labour.museum
-lajolla.museum
-lancashire.museum
-landes.museum
-lans.museum
-xn--lns-qla.museum
-larsson.museum
-lewismiller.museum
-lincoln.museum
-linz.museum
-living.museum
-livinghistory.museum
-localhistory.museum
-london.museum
-losangeles.museum
-louvre.museum
-loyalist.museum
-lucerne.museum
-luxembourg.museum
-luzern.museum
-mad.museum
-madrid.museum
-mallorca.museum
-manchester.museum
-mansion.museum
-mansions.museum
-manx.museum
-marburg.museum
-maritime.museum
-maritimo.museum
-maryland.museum
-marylhurst.museum
-media.museum
-medical.museum
-medizinhistorisches.museum
-meeres.museum
-memorial.museum
-mesaverde.museum
-michigan.museum
-midatlantic.museum
-military.museum
-mill.museum
-miners.museum
-mining.museum
-minnesota.museum
-missile.museum
-missoula.museum
-modern.museum
-moma.museum
-money.museum
-monmouth.museum
-monticello.museum
-montreal.museum
-moscow.museum
-motorcycle.museum
-muenchen.museum
-muenster.museum
-mulhouse.museum
-muncie.museum
-museet.museum
-museumcenter.museum
-museumvereniging.museum
-music.museum
-national.museum
-nationalfirearms.museum
-nationalheritage.museum
-nativeamerican.museum
-naturalhistory.museum
-naturalhistorymuseum.museum
-naturalsciences.museum
-nature.museum
-naturhistorisches.museum
-natuurwetenschappen.museum
-naumburg.museum
-naval.museum
-nebraska.museum
-neues.museum
-newhampshire.museum
-newjersey.museum
-newmexico.museum
-newport.museum
-newspaper.museum
-newyork.museum
-niepce.museum
-norfolk.museum
-north.museum
-nrw.museum
-nyc.museum
-nyny.museum
-oceanographic.museum
-oceanographique.museum
-omaha.museum
-online.museum
-ontario.museum
-openair.museum
-oregon.museum
-oregontrail.museum
-otago.museum
-oxford.museum
-pacific.museum
-paderborn.museum
-palace.museum
-paleo.museum
-palmsprings.museum
-panama.museum
-paris.museum
-pasadena.museum
-pharmacy.museum
-philadelphia.museum
-philadelphiaarea.museum
-philately.museum
-phoenix.museum
-photography.museum
-pilots.museum
-pittsburgh.museum
-planetarium.museum
-plantation.museum
-plants.museum
-plaza.museum
-portal.museum
-portland.museum
-portlligat.museum
-posts-and-telecommunications.museum
-preservation.museum
-presidio.museum
-press.museum
-project.museum
-public.museum
-pubol.museum
-quebec.museum
-railroad.museum
-railway.museum
-research.museum
-resistance.museum
-riodejaneiro.museum
-rochester.museum
-rockart.museum
-roma.museum
-russia.museum
-saintlouis.museum
-salem.museum
-salvadordali.museum
-salzburg.museum
-sandiego.museum
-sanfrancisco.museum
-santabarbara.museum
-santacruz.museum
-santafe.museum
-saskatchewan.museum
-satx.museum
-savannahga.museum
-schlesisches.museum
-schoenbrunn.museum
-schokoladen.museum
-school.museum
-schweiz.museum
-science.museum
-scienceandhistory.museum
-scienceandindustry.museum
-sciencecenter.museum
-sciencecenters.museum
-science-fiction.museum
-sciencehistory.museum
-sciences.museum
-sciencesnaturelles.museum
-scotland.museum
-seaport.museum
-settlement.museum
-settlers.museum
-shell.museum
-sherbrooke.museum
-sibenik.museum
-silk.museum
-ski.museum
-skole.museum
-society.museum
-sologne.museum
-soundandvision.museum
-southcarolina.museum
-southwest.museum
-space.museum
-spy.museum
-square.museum
-stadt.museum
-stalbans.museum
-starnberg.museum
-state.museum
-stateofdelaware.museum
-station.museum
-steam.museum
-steiermark.museum
-stjohn.museum
-stockholm.museum
-stpetersburg.museum
-stuttgart.museum
-suisse.museum
-surgeonshall.museum
-surrey.museum
-svizzera.museum
-sweden.museum
-sydney.museum
-tank.museum
-tcm.museum
-technology.museum
-telekommunikation.museum
-television.museum
-texas.museum
-textile.museum
-theater.museum
-time.museum
-timekeeping.museum
-topology.museum
-torino.museum
-touch.museum
-town.museum
-transport.museum
-tree.museum
-trolley.museum
-trust.museum
-trustee.museum
-uhren.museum
-ulm.museum
-undersea.museum
-university.museum
-usa.museum
-usantiques.museum
-usarts.museum
-uscountryestate.museum
-usculture.museum
-usdecorativearts.museum
-usgarden.museum
-ushistory.museum
-ushuaia.museum
-uslivinghistory.museum
-utah.museum
-uvic.museum
-valley.museum
-vantaa.museum
-versailles.museum
-viking.museum
-village.museum
-virginia.museum
-virtual.museum
-virtuel.museum
-vlaanderen.museum
-volkenkunde.museum
-wales.museum
-wallonie.museum
-war.museum
-washingtondc.museum
-watchandclock.museum
-watch-and-clock.museum
-western.museum
-westfalen.museum
-whaling.museum
-wildlife.museum
-williamsburg.museum
-windmill.museum
-workshop.museum
-york.museum
-yorkshire.museum
-yosemite.museum
-youth.museum
-zoological.museum
-zoology.museum
-xn--9dbhblg6di.museum
-xn--h1aegh.museum
 mv
 aero.mv
 biz.mv
 com.mv
 coop.mv
 edu.mv
 gov.mv
@@ -6795,15 +6249,14 @@
 lifestyle
 lighting
 like
 lilly
 limited
 limo
 lincoln
-linde
 link
 lipsy
 live
 living
 llc
 llp
 loan
@@ -6818,15 +6271,14 @@
 lpl
 lplfinancial
 ltd
 ltda
 lundbeck
 luxe
 luxury
-macys
 madrid
 maif
 maison
 makeup
 man
 management
 mango
@@ -9128,14 +8580,15 @@
 chirurgiens-dentistes-en-france.fr
 byen.site
 pubtls.org
 pythonanywhere.com
 eu.pythonanywhere.com
 qoto.io
 qualifioapp.com
+ladesk.com
 qbuser.com
 cloudsite.builders
 instances.spawn.cc
 instantcloud.cn
 ras.ru
 qa2.com
 qcx.io
```

### Comparing `psl-2023.3.6/psl.egg-info/PKG-INFO` & `psl-2023.4.10/psl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.3.6
+Version: 2023.4.10
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.3.6/setup.py` & `psl-2023.4.10/setup.py`

 * *Files identical despite different names*

