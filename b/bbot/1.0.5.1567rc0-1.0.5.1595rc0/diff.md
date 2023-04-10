# Comparing `tmp/bbot-1.0.5.1567rc0.tar.gz` & `tmp/bbot-1.0.5.1595rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1567rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1595rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1567rc0.tar` & `bbot-1.0.5.1595rc0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0    32473 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/LICENSE
--rw-r--r--   0        0        0    51011 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/README.md
--rw-r--r--   0        0        0      211 2023-04-10 15:24:42.389136 bbot-1.0.5.1567rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6478 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13323 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3137 2023-04-10 15:24:19.924126 bbot-1.0.5.1567rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8919 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    29858 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     7432 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29297 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4261 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5364 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    28093 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9514 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8092 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3102 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10695 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3637 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25405 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-04-10 15:24:19.928126 bbot-1.0.5.1567rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     4526 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1165 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10060 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5491 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9336 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      311 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    14125 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4481 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10777 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    12554 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4012 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0     3561 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     1737 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1787 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1007 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-04-10 15:24:19.932127 bbot-1.0.5.1567rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3609 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1606 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8304 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2080 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     5752 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11271 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    25262 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3251 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4057 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0     2591 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/helpers.py
--rw-r--r--   0        0        0    71497 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5669 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4012 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-04-10 15:24:19.936127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34925 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11466 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      479 2023-04-10 15:24:19.940127 bbot-1.0.5.1567rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-04-10 15:24:19.944127 bbot-1.0.5.1567rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-04-10 15:24:19.944127 bbot-1.0.5.1567rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-04-10 15:24:19.944127 bbot-1.0.5.1567rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-04-10 15:24:19.948127 bbot-1.0.5.1567rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1338 2023-04-10 15:24:42.389136 bbot-1.0.5.1567rc0/pyproject.toml
--rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1567rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/LICENSE
+-rw-r--r--   0        0        0    51011 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/README.md
+-rw-r--r--   0        0        0      211 2023-04-10 18:25:13.425493 bbot-1.0.5.1595rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     6478 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      376 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    13323 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3137 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8912 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     4261 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      632 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    29954 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1498 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3644 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1256 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     2875 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     7432 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    13841 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     8540 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    29187 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     4261 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5435 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1414 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    28177 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14848 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9514 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-04-10 18:24:52.145482 bbot-1.0.5.1595rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     2919 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/queueing.py
+-rw-r--r--   0        0        0     1890 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     8474 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/threadpool.py
+-rw-r--r--   0        0        0     3987 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3193 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0     9324 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    10967 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     7859 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3731 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3461 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2350 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25265 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2197 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1225 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5502 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1065 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      847 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1167 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2169 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4550 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5107 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1116 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     5432 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      732 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     4614 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1160 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13578 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15617 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5763 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2516 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2954 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2862 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      866 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11117 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2164 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1093 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7290 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     2723 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10060 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      658 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7395 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5491 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7748 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     1944 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9438 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      311 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    15650 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     4481 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1274 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2037 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0      707 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10777 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    13311 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4012 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     4867 2023-04-10 18:24:52.149482 bbot-1.0.5.1595rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0     3844 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1379 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     1737 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1809 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1787 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1007 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1255 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      204 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3609 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     1747 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1532 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1620 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5360 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1533 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1310 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      746 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1606 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8304 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      742 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2080 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2578 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1071 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1198 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1432 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1607 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1527 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     8014 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6077 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11235 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      566 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3819 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2759 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2458 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1158 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1569 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1169 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2190 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2095 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    26114 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    22025 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3251 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4057 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    18609 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0      559 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0     2591 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/helpers.py
+-rw-r--r--   0        0        0    71538 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/modules_test_classes.py
+-rw-r--r--   0        0        0       15 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/pytest.ini
+-rwxr-xr-x   0        0        0      578 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0      904 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1397 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_1/test_before_patching.py
+-rw-r--r--   0        0        0     5669 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_1/test_modules_full.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_agent.py
+-rw-r--r--   0        0        0     4012 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_cli.py
+-rw-r--r--   0        0        0      932 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_cloud_helpers.py
+-rw-r--r--   0        0        0      462 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_config.py
+-rw-r--r--   0        0        0      722 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_depsinstaller.py
+-rw-r--r--   0        0        0    15064 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_events.py
+-rw-r--r--   0        0        0    34798 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_helpers.py
+-rw-r--r--   0        0        0     7171 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_manager.py
+-rw-r--r--   0        0        0    11466 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_modules_basic.py
+-rw-r--r--   0        0        0      789 2023-04-10 18:24:52.153482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_python_api.py
+-rw-r--r--   0        0        0     3215 2023-04-10 18:24:52.157482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_scan.py
+-rw-r--r--   0        0        0     1395 2023-04-10 18:24:52.157482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_scope.py
+-rw-r--r--   0        0        0     2163 2023-04-10 18:24:52.157482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_target.py
+-rw-r--r--   0        0        0      707 2023-04-10 18:24:52.157482 bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_threadpool.py
+-rw-r--r--   0        0        0      479 2023-04-10 18:24:52.157482 bbot-1.0.5.1595rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-04-10 18:24:52.161482 bbot-1.0.5.1595rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-04-10 18:24:52.161482 bbot-1.0.5.1595rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-04-10 18:24:52.161482 bbot-1.0.5.1595rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-04-10 18:24:52.165482 bbot-1.0.5.1595rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1338 2023-04-10 18:25:13.425493 bbot-1.0.5.1595rc0/pyproject.toml
+-rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1595rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1567rc0/LICENSE` & `bbot-1.0.5.1595rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/README.md` & `bbot-1.0.5.1595rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/agent/agent.py` & `bbot-1.0.5.1595rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/cli.py` & `bbot-1.0.5.1595rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1595rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1595rc0/bbot/core/configurator/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         metavar="FLAG",
     )
     p.add_argument(
         "-rf",
         "--require-flags",
         nargs="+",
         default=[],
-        help=f"Disable modules that don't have these flags (e.g. -rf passive)",
+        help=f"Only enable modules with these flags (e.g. -rf passive)",
         metavar="FLAG",
     )
     p.add_argument(
         "-ef",
         "--exclude-flags",
         nargs="+",
         default=[],
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1595rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1595rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/errors.py` & `bbot-1.0.5.1595rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/event/base.py` & `bbot-1.0.5.1595rc0/bbot/core/event/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,19 +294,19 @@
         if not self._made_internal:
             self._internal = True
             self.add_tag("internal")
             self._made_internal = True
 
     def unmake_internal(self, set_scope_distance=None, force_output=False):
         source_trail = []
+        self.remove_tag("internal")
         if self._made_internal:
             if set_scope_distance is not None:
                 self.scope_distance = set_scope_distance
             self._internal = False
-            self.remove_tag("internal")
             self._made_internal = False
         if force_output is True:
             self._force_output = True
         if force_output == "trail_only":
             force_output = True
 
         if getattr(self.source, "_internal", False):
@@ -525,16 +525,17 @@
 
     def __hash__(self):
         if self._hash is None:
             self._hash = hash(self.id)
         return self._hash
 
     def __str__(self):
+        max_event_len = 80
         d = str(self.data)
-        return f'{self.type}("{d[:50]}{("..." if len(d) > 50 else "")}", module={self.module}, tags={self.tags})'
+        return f'{self.type}("{d[:max_event_len]}{("..." if len(d) > max_event_len else "")}", module={self.module}, tags={self.tags})'
 
     def __repr__(self):
         return str(self)
 
 
 class FINISHED(BaseEvent):
     """
@@ -646,25 +647,23 @@
     def sanitize_data(self, data):
         return validators.validate_host(data)
 
     def _host(self):
         return self.data
 
     def _words(self):
-        # only operate on resolved DNS_NAMEs
-        if self.type == "DNS_NAME":
-            stem = self.host_stem
-            if not is_ptr(stem):
-                split_stem = stem.split(".")
-                if split_stem:
-                    leftmost_segment = split_stem[0]
-                    if leftmost_segment == "_wildcard":
-                        stem = ".".join(split_stem[1:])
-                if stem:
-                    return extract_words(stem)
+        stem = self.host_stem
+        if not is_ptr(stem):
+            split_stem = stem.split(".")
+            if split_stem:
+                leftmost_segment = split_stem[0]
+                if leftmost_segment == "_wildcard":
+                    stem = ".".join(split_stem[1:])
+            if stem:
+                return extract_words(stem)
         return set()
 
 
 class OPEN_TCP_PORT(BaseEvent):
     def sanitize_data(self, data):
         return validators.validate_open_port(data)
 
@@ -738,15 +737,15 @@
             raise ValidationError(
                 'Must specify HTTP status tag for URL event, e.g. "status-200". Use URL_UNVERIFIED if the URL is unvisited.'
             )
         return super().sanitize_data(data)
 
     @property
     def resolved_hosts(self):
-        return [i.split("-")[1] for i in self.tags if i.startswith("ip-")]
+        return [".".join(i.split("-")[1:]) for i in self.tags if i.startswith("ip-")]
 
     @property
     def pretty_string(self):
         return self.data
 
 
 class STORAGE_BUCKET(DictEvent, URL_UNVERIFIED):
@@ -797,14 +796,20 @@
                 k, v = i.split(":", 1)
                 k = k.strip().lower()
                 v = v.lstrip()
                 header_dict[k] = v
         data["header-dict"] = header_dict
         return data
 
+    def _data_human(self):
+        data = dict(self.data)
+        new_data = {"url": data.pop("url")}
+        new_data.update(data)
+        return new_data
+
     def _words(self):
         return set()
 
     def _pretty_string(self):
         return f'{self.data["hash"]["header_mmh3"]}:{self.data["hash"]["body_mmh3"]}'
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1595rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/dns.py`

 * *Files 6% similar despite different names*

```diff
@@ -214,25 +214,14 @@
                     tries_left -= 1
                     if tries_left > 0:
                         retry_num = (retries + 2) - tries_left
                         self.debug(f"Retrying (#{retry_num}) {query} with kwargs={kwargs}")
         self.debug(f"Results for {query} with kwargs={kwargs}: {results}")
         return results, errors
 
-    def resolve_event(self, event, minimal=False):
-        log.debug(f"Resolving {event}")
-        result = self._resolve_event(event, minimal=minimal)
-        # if it's a wildcard, go again with _wildcard.{domain}
-        if len(result) == 2:
-            event, wildcard_rdtypes = result
-            return self._resolve_event(event, minimal=minimal, _wildcard_rdtypes=wildcard_rdtypes)
-        # else we're good
-        else:
-            return result
-
     def handle_wildcard_event(self, event, children):
         event_host = str(event.host)
         # wildcard checks
         if not is_ip(event.host):
             # check if this domain is using wildcard dns
             event_target = "target" in event.tags
             for hostname, wildcard_domain_rdtypes in self.is_wildcard_domain(
@@ -250,15 +239,15 @@
                     event.add_tag("wildcard")
                     wildcard_tag = "wildcard"
                 event.add_tag(f"{rdtype.lower()}-{wildcard_tag}")
 
         # wildcard event modification (www.evilcorp.com --> _wildcard.evilcorp.com)
         if not is_ip(event.host) and children and wildcard_rdtypes:
             # these are the rdtypes that successfully resolve
-            resolved_rdtypes = set([c[0].upper() for c in children])
+            resolved_rdtypes = set([c.upper() for c in children])
             # these are the rdtypes that have wildcards
             wildcard_rdtypes_set = set(wildcard_rdtypes)
             # consider the event a full wildcard if all its records are wildcards
             event_is_wildcard = False
             if resolved_rdtypes:
                 event_is_wildcard = all(r in wildcard_rdtypes_set for r in resolved_rdtypes)
             if event_is_wildcard and event.type in ("DNS_NAME",) and not "_wildcard" in event.data.split("."):
@@ -268,38 +257,37 @@
                         wildcard_parent = _parent_domain
                         break
                 wildcard_data = f"_wildcard.{wildcard_parent}"
                 if wildcard_data != event.data:
                     log.debug(f'Wildcard detected, changing event.data "{event.data}" --> "{wildcard_data}"')
                     event.data = wildcard_data
 
-    def _resolve_event(self, event, minimal=False):
+    def resolve_event(self, event, minimal=False):
         """
         Tag event with appropriate dns record types
         Optionally create child events from dns resolutions
         """
-        event_tags = set()
-        if not event.host or event.type in ("IP_RANGE",):
-            return [], set(), False, False, set()
-        children = []
+        log.debug(f"Resolving {event}")
         event_host = str(event.host)
-
+        event_tags = set()
+        dns_children = dict()
         event_whitelisted = False
         event_blacklisted = False
 
-        resolved_hosts = set()
+        if not event.host or event.type in ("IP_RANGE",):
+            return event_tags, event_whitelisted, event_blacklisted, dns_children
 
         # lock to ensure resolution of the same host doesn't start while we're working here
         with self._event_cache_locks.get_lock(event_host):
             # try to get data from cache
-            _event_tags, _event_whitelisted, _event_blacklisted, _resolved_hosts = self.event_cache_get(event_host)
+            _event_tags, _event_whitelisted, _event_blacklisted, _dns_children = self.event_cache_get(event_host)
             event_tags.update(_event_tags)
             # if we found it, return it
             if _event_whitelisted is not None:
-                return children, event_tags, _event_whitelisted, _event_blacklisted, _resolved_hosts
+                return event_tags, _event_whitelisted, _event_blacklisted, _dns_children
 
             # then resolve
             types = ()
             if self.parent_helper.is_ip(event.host):
                 if not minimal:
                     types = ("PTR",)
             else:
@@ -327,56 +315,63 @@
                         rdtype = str(rdtype).upper()
                         event_tags.add(f"{rdtype.lower()}-record")
 
                         # whitelisting and blacklisting of IPs
                         for r in records:
                             for _, t in self.extract_targets(r):
                                 if t:
-                                    if rdtype in ("A", "AAAA", "CNAME"):
-                                        ip = self.parent_helper.make_ip_type(t)
+                                    ip = self.parent_helper.make_ip_type(t)
 
+                                    if rdtype in ("A", "AAAA", "CNAME"):
                                         with suppress(ValidationError):
                                             if self.parent_helper.is_ip(ip):
                                                 if self.parent_helper.scan.whitelisted(ip):
                                                     event_whitelisted = True
                                         with suppress(ValidationError):
                                             if self.parent_helper.scan.blacklisted(ip):
                                                 event_blacklisted = True
-                                        resolved_hosts.add(ip)
 
                                     if self.filter_bad_ptrs and rdtype in ("PTR") and self.parent_helper.is_ptr(t):
                                         self.debug(f"Filtering out bad PTR: {t}")
                                         continue
-                                    children.append((rdtype, t))
 
+                                    try:
+                                        dns_children[rdtype].add(ip)
+                                    except KeyError:
+                                        dns_children[rdtype] = {ip}
+
+                # tag with cloud providers
                 if not self.parent_helper.in_tests:
-                    ips = set()
+                    to_check = set()
                     if event.type == "IP_ADDRESS":
-                        ips.add(event.data)
-                    for rdtype, target in children:
+                        to_check.add(event.data)
+                    for rdtype, ips in dns_children.items():
                         if rdtype in ("A", "AAAA"):
-                            ips.add(target)
-                    for ip in ips:
+                            for ip in ips:
+                                to_check.add(ip)
+                    for ip in to_check:
                         provider, provider_type, subnet = cloudcheck.check(ip)
                         if provider:
                             event_tags.add(f"{provider_type}-{provider}")
 
+                # check for private IPs
                 if "resolved" not in event_tags:
                     event_tags.add("unresolved")
-                for ip in resolved_hosts:
-                    try:
-                        ip = ipaddress.ip_address(ip)
-                        if ip.is_private:
-                            event_tags.add("private-ip")
-                    except ValueError:
-                        continue
+                for rdtype, ips in dns_children.items():
+                    for ip in ips:
+                        try:
+                            ip = ipaddress.ip_address(ip)
+                            if ip.is_private:
+                                event_tags.add("private-ip")
+                        except ValueError:
+                            continue
 
-                self._event_cache[event_host] = (event_tags, event_whitelisted, event_blacklisted, resolved_hosts)
+                self._event_cache[event_host] = (event_tags, event_whitelisted, event_blacklisted, dns_children)
 
-        return children, event_tags, event_whitelisted, event_blacklisted, resolved_hosts
+        return event_tags, event_whitelisted, event_blacklisted, dns_children
 
     def event_cache_get(self, host):
         try:
             return self._event_cache[host]
         except KeyError:
             return set(), None, None, set()
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/interactsh.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             if not self.token:
                 log.verbose("Interact.sh token is not set")
             headers["Authorization"] = self.token
             self.server_list = [self.custom_server]
         else:
             self.server_list = random.sample(server_list, k=len(server_list))
         for server in self.server_list:
+            log.info(f"Registering with interact.sh server: {server}")
             data = {
                 "public-key": encoded_public_key,
                 "secret-key": self.secret,
                 "correlation-id": self.correlation_id,
             }
             r = self.parent_helper.request(f"https://{server}/register", headers=headers, json=data, method="POST")
             if r is None:
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,22 +348,24 @@
     """
     pool = rand_pool
     if digits:
         pool = rand_pool_digits
     return "".join([random.choice(pool) for _ in range(int(length))])
 
 
-def extract_words(data, acronyms=True, wordninja=True, model=None, max_length=100):
+def extract_words(data, acronyms=True, wordninja=True, model=None, max_length=100, word_regexes=None):
     """
     Intelligently extract words from given data
     Returns set() of extracted words
     """
+    if word_regexes is None:
+        word_regexes = regexes.word_regexes
     words = set()
     data = smart_decode(data)
-    for r in regexes.word_regexes:
+    for r in word_regexes:
         for word in set(r.findall(data)):
             # blacklanternsecurity
             if len(word) <= max_length:
                 words.add(word)
 
     # blacklanternsecurity --> ['black', 'lantern', 'security']
     # max_slice_length = 3
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/queueing.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/queueing.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/threadpool.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/threadpool.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,25 +104,26 @@
     """
 
     def __init__(self, executor, max_workers=None, qsize=None):
         self.executor = executor
         self.max_workers = max_workers
         self.max_qsize = qsize
         self.futures = set()
-        try:
-            self.executor._thread_pool_wrappers.append(self)
-        except AttributeError:
-            self.executor._thread_pool_wrappers = [self]
 
         self._num_tasks = 0
         self._task_count_lock = threading.Lock()
 
         self._lock = threading.RLock()
         self.not_full = threading.Condition(self._lock)
 
+        try:
+            self.executor._thread_pool_wrappers.append(self)
+        except AttributeError:
+            self.executor._thread_pool_wrappers = [self]
+
     def submit_task(self, callback, *args, **kwargs):
         """
         A wrapper around threadpool.submit()
         """
         block = kwargs.pop("_block", True)
         force = kwargs.pop("_force_submit", False)
         success = False
@@ -240,7 +241,26 @@
     def get_lock(self, name):
         try:
             return self._cache.get(name)
         except KeyError:
             new_lock = _Lock(name)
             self._cache.put(name, new_lock)
             return new_lock
+
+
+class TaskCounter:
+    def __init__(self):
+        self._value = 0
+        self.lock = threading.Lock()
+
+    def __enter__(self):
+        with self.lock:
+            self._value += 1
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        with self.lock:
+            self._value -= 1
+
+    @property
+    def value(self):
+        with self.lock:
+            return self._value
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
         # if IPv6 fails, strip ports and root zone
         host = host.split(":")[0].rstrip(".")
         try:
             ip = ipaddress.IPv4Address(host)
             return str(ip)
         except Exception:
             # finally, try DNS_NAME
-            host = smart_decode_punycode(host.lstrip("*."))
+            host = smart_decode_punycode(host)
+            # clean asterisks and clinging dashes
+            host = host.strip("*.-").replace("*", "")
             for r in regexes.event_type_regexes["DNS_NAME"]:
                 if r.match(host):
                     return host
             if regexes._hostname_regex.match(host):
                 return host
     assert False, f'Invalid hostname: "{host}"'
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1595rc0/bbot/core/helpers/wordcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if numbers > 0:
             modifiers.update(self.parent_helper.gen_numbers(numbers, number_padding))
         return modifiers
 
     def absorb_event(self, event):
         for word in event.words:
             self.add_word(word)
-        if event.scope_distance == 0 and event.type == "DNS_NAME":
+        if event.scope_distance == 0 and event.type.startswith("DNS_NAME"):
             subdomain = tldextract(event.data).subdomain
             if subdomain and not self.parent_helper.is_ptr(subdomain):
                 for s in subdomain.split("."):
                     self.dns_mutator.add_word(s)
 
     def absorb_word(self, word, ninja=True):
         """
@@ -246,27 +246,37 @@
 
     def add_word(self, word):
         pass
 
 
 class DNSMutator(Mutator):
     word_regex = re.compile(r"[^_\W]+")
+    extract_word_regexes = [
+        re.compile(r, re.I)
+        for r in [
+            r"[a-z]+",
+            r"[a-z0-9]+",
+            r"[a-z0-9-]+",
+            r"[a-z0-9_]+",
+            r"[a-z0-9_-]+",
+        ]
+    ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         wordlist_dir = Path(__file__).parent.parent.parent / "wordlists"
         wordninja_dns_wordlist = wordlist_dir / "wordninja_dns.txt.gz"
         self.model = wordninja.LanguageModel(wordninja_dns_wordlist)
 
     def mutations(self, words, max_mutations=None):
         if isinstance(words, str):
             words = [words]
         new_words = set()
         for word in words:
-            for e in extract_words(word, acronyms=False, model=self.model):
+            for e in extract_words(word, acronyms=False, model=self.model, word_regexes=self.extract_word_regexes):
                 new_words.add(e)
         return super().mutations(new_words, max_mutations=max_mutations)
 
     def add_word(self, word):
         for match in self.word_regex.finditer(word):
             start, end = match.span()
             match_str = word[start:end]
```

### Comparing `bbot-1.0.5.1567rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1595rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1595rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/defaults.yml` & `bbot-1.0.5.1595rc0/bbot/defaults.yml`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 http_debug: false
 # Maximum number of HTTP redirects to follow
 http_max_redirects: 5
 # Set the maximum number of HTTP links that can be followed in a row (0 == no spidering allowed)
 web_spider_distance: 0
 # Set the maximum directory depth for the web spider
 web_spider_depth: 1
+# Set the maximum number of links that can be followed per page
+web_spider_links_per_page: 25
 # DNS query timeout
 dns_timeout: 5
 # How many times to retry DNS queries
 dns_retries: 1
 # Disable BBOT's smart DNS wildcard handling for select domains
 dns_wildcard_ignore: []
 # How many sanity checks to make when verifying wildcard DNS
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1595rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1595rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1595rc0/bbot/modules/badsecrets.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class badsecrets(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
     meta = {"description": "Library for detecting known or weak secrets across many web frameworks"}
     max_event_handlers = 2
-    deps_pip = ["badsecrets~=0.1.279"]
+    deps_pip = ["badsecrets~=0.1.287"]
 
     def handle_event(self, event):
         resp_body = event.data.get("body", None)
         resp_headers = event.data.get("header", None)
         resp_cookies = {}
         if resp_headers:
             resp_cookies_raw = resp_headers.get("set_cookie", None)
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/base.py` & `bbot-1.0.5.1595rc0/bbot/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import threading
 import traceback
 from sys import exc_info
 from contextlib import suppress
 
 from ..core.helpers.misc import get_size
-from ..core.helpers.threadpool import ThreadPoolWrapper
+from ..core.helpers.threadpool import ThreadPoolWrapper, TaskCounter
 from ..core.errors import ScanCancelledError, ValidationError, WordlistError
 
 
 class BaseModule:
     # Event types to watch
     watched_events = []
     # Event types to produce
@@ -51,16 +51,14 @@
 
     # Options, e.g. {"api_key": ""}
     options = {}
     # Options description, e.g. {"api_key": "API Key"}
     options_desc = {}
     # Maximum concurrent instances of handle_event() or handle_batch()
     max_event_handlers = 1
-    # Max number of concurrent calls to submit_task()
-    max_threads = 10
     # Batch size
     # If batch size > 1, override handle_batch() instead of handle_event()
     batch_size = 1
     # Seconds to wait before force-submitting batch
     batch_wait = 10
     # Use in conjunction with .request_with_fail_count() to set_error_state() after this many failed HTTP requests
     failed_request_abort_threshold = 5
@@ -82,26 +80,25 @@
         self.scan = scan
         self.errored = False
         self._log = None
         self._incoming_event_queue = None
         # seconds since we've submitted a batch
         self._last_submitted_batch = None
         # wrapper around shared thread pool to ensure that a single module doesn't hog more than its share
-        max_workers = self.config.get("max_threads", self.max_threads)
-        self.thread_pool = ThreadPoolWrapper(self.scan._thread_pool, max_workers=max_workers)
+        self.thread_pool = ThreadPoolWrapper(self.scan._thread_pool)
         self._internal_thread_pool = ThreadPoolWrapper(
             self.scan._internal_thread_pool.executor, max_workers=self.max_event_handlers
         )
         # additional callbacks to be executed alongside self.cleanup()
         self.cleanup_callbacks = []
         self._cleanedup = False
         self._watched_events = None
 
         self._lock = threading.RLock()
-        self._running_semaphore = threading.Semaphore()
+        self._running_counter = TaskCounter()
         self.event_received = threading.Condition(self._lock)
 
         # string constant
         self._custom_filter_criteria_msg = "it did not meet custom filter criteria"
 
         # track number of failures (for .request_with_fail_count())
         self._request_failures = 0
@@ -205,29 +202,30 @@
         Override if you need your watched_events to be dynamic
         """
         if self._watched_events is None:
             self._watched_events = set(self.watched_events)
         return self._watched_events
 
     def submit_task(self, *args, **kwargs):
+        kwargs["_block"] = False
         return self.thread_pool.submit_task(self.catch, *args, **kwargs)
 
     def catch(self, *args, **kwargs):
         return self.scan.manager.catch(*args, **kwargs)
 
     def _postcheck_and_run(self, callback, event):
         acceptable, reason = self._event_postcheck(event)
         if not acceptable:
             if reason:
                 self.debug(f"Not accepting {event} because {reason}")
             return
         return callback(event)
 
     def _register_running(self, callback, *args, **kwargs):
-        with self._running_semaphore:
+        with self._running_counter:
             return callback(*args, **kwargs)
 
     def _handle_batch(self, force=False):
         if self.batch_size <= 1:
             return
         if self.num_queued_events > 0 and (force or self.num_queued_events >= self.batch_size):
             on_finish_callback = None
@@ -562,15 +560,15 @@
         return self._foo
 
     @property
     def running(self):
         """
         Indicates whether the module is currently processing data.
         """
-        return self._running_semaphore._value < 1
+        return self._running_counter.value > 0
 
     def request_with_fail_count(self, *args, **kwargs):
         r = self.helpers.request(*args, **kwargs)
         if r is None:
             self._request_failures += 1
         else:
             self._request_failures = 0
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1595rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1595rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1595rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1595rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1595rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1595rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1595rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1595rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1595rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/c99.py` & `bbot-1.0.5.1595rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/censys.py` & `bbot-1.0.5.1595rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1595rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1595rc0/bbot/modules/crobat.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,30 @@
 
     def setup(self):
         self.processed = set()
         self.http_timeout = self.scan.config.get("http_timeout", 10)
         self._failures = 0
         return True
 
+    def _is_wildcard(self, query):
+        for domain, wildcard_rdtypes in self.helpers.is_wildcard_domain(query).items():
+            if any(t in wildcard_rdtypes for t in ("A", "AAAA", "CNAME")):
+                return True
+        return False
+
     def filter_event(self, event):
         """
         This filter_event is used across many modules
         """
         query = self.make_query(event)
         # reject if already processed
         if self.already_processed(query):
             return False, "Event was already processed"
         # check if wildcard
-        is_wildcard = False
-        for domain, wildcard_rdtypes in self.helpers.is_wildcard_domain(query).items():
-            if any(t in wildcard_rdtypes for t in ("A", "AAAA", "CNAME")):
-                is_wildcard = True
+        is_wildcard = self._is_wildcard(query)
         # check if cloud
         is_cloud = False
         if any(t.startswith("cloud-") for t in event.tags):
             is_cloud = True
         # reject if it's a cloud resource and not in our target
         if is_cloud and event not in self.scan.target:
             return False, "Event is a cloud resource and not a direct target"
@@ -67,26 +70,26 @@
                 return True
         return False
 
     def abort_if(self, event):
         # this helps weed out unwanted results when scanning IP_RANGES and wildcard domains
         if "in-scope" not in event.tags:
             return True
-        if any(t in event.tags for t in ("wildcard", "wildcard-domain")):
+        if self._is_wildcard(event.data):
             return True
         return False
 
     def handle_event(self, event):
         query = self.make_query(event)
         results = self.query(query)
         if results:
             for hostname in set(results):
                 if hostname:
-                    hostname = hostname.lower()
-                    if hostname.endswith(f".{query}") and not hostname == event.data:
+                    hostname = self.helpers.validators.validate_host(hostname)
+                    if hostname and hostname.endswith(f".{query}") and not hostname == event.data:
                         self.emit_event(hostname, "DNS_NAME", event, abort_if=self.abort_if)
 
     def request_url(self, query):
         url = f"{self.base_url}/subdomains/{self.helpers.quote(query)}"
         return self.request_with_fail_count(url)
 
     def make_query(self, event):
@@ -108,10 +111,10 @@
         if request_fn is None:
             request_fn = self.request_url
         try:
             results = list(parse_fn(request_fn(query), query))
             if results:
                 return results
             self.debug(f'No results for "{query}"')
-        except Exception:
-            self.verbose(f"Error retrieving results for {query}")
+        except Exception as e:
+            self.info(f"Error retrieving results for {query}: {e}")
             self.trace()
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/crt.py` & `bbot-1.0.5.1595rc0/bbot/modules/crt.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     reject_wildcards = False
 
     def setup(self):
         self.cert_ids = set()
         return super().setup()
 
     def request_url(self, query):
-        params = {"q": query, "output": "json"}
+        params = {"q": f"%.{query}", "output": "json"}
         url = self.helpers.add_get_params(self.base_url, params).geturl()
         return self.request_with_fail_count(url, timeout=self.http_timeout + 10)
 
     def parse_results(self, r, query):
         j = r.json()
         for cert_info in j:
             if not type(cert_info) == dict:
@@ -27,8 +27,8 @@
             cert_id = cert_info.get("id")
             if cert_id:
                 if hash(cert_id) not in self.cert_ids:
                     self.cert_ids.add(hash(cert_id))
                     domain = cert_info.get("name_value")
                     if domain:
                         for d in domain.splitlines():
-                            yield d.lower().strip("*.")
+                            yield d.lower()
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1595rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1595rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1595rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1595rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1595rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1595rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1595rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1595rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1595rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1595rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1595rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/github.py` & `bbot-1.0.5.1595rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1595rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1595rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1595rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1595rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1595rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1595rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1595rc0/bbot/modules/iis_shortnames.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         technique = None
         detections = []
         random_string = self.helpers.rand_string(8)
         control_url = f"{target}{random_string}*~1*/a.aspx"
         test_url = f"{target}*~1*/a.aspx"
 
         for method in ["GET", "POST", "OPTIONS", "DEBUG", "HEAD", "TRACE"]:
-            control = self.helpers.request(method=method, url=control_url, allow_redirects=False, retries=2)
-            test = self.helpers.request(method=method, url=test_url, allow_redirects=False, retries=2)
+            control = self.helpers.request(method=method, url=control_url, allow_redirects=False, timeout=10)
+            test = self.helpers.request(method=method, url=test_url, allow_redirects=False, timeout=10)
             if (control != None) and (test != None):
                 if control.status_code != test.status_code:
                     technique = f"{str(control.status_code)}/{str(test.status_code)} HTTP Code"
                     detections.append((method, test.status_code, technique))
 
                 elif ("Error Code</th><td>0x80070002" in control.text) and (
                     "Error Code</th><td>0x00000000" in test.text
@@ -54,15 +54,17 @@
     @staticmethod
     def normalize_url(url):
         return str(url.rstrip("/") + "/").lower()
 
     def directory_confirm(self, target, method, url_hint, affirmative_status_code):
         payload = encode_all(f"{url_hint}")
         url = f"{target}{payload}"
-        directory_confirm_result = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2)
+        directory_confirm_result = self.helpers.request(
+            method=method, url=url, allow_redirects=False, retries=2, timeout=10
+        )
 
         if directory_confirm_result.status_code == affirmative_status_code:
             return True
         else:
             return False
 
     def duplicate_check(self, target, method, url_hint, affirmative_status_code):
@@ -71,29 +73,31 @@
         base_hint = re.sub(r"~\d", "", url_hint)
         suffix = "\\a.aspx"
 
         while 1:
             payload = encode_all(f"{base_hint}~{str(count)}*")
             url = f"{target}{payload}{suffix}"
 
-            duplicate_check_results = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2)
+            duplicate_check_results = self.helpers.request(
+                method=method, url=url, allow_redirects=False, retries=2, timeout=10
+            )
             if duplicate_check_results.status_code != affirmative_status_code:
                 break
             else:
                 duplicates.append(f"{base_hint}~{str(count)}")
                 count += 1
 
             if count > 5:
                 self.warning("Found more than 5 files with the same shortname. Will stop further duplicate checking.")
                 break
 
         return duplicates
 
     def threaded_request(self, method, url, affirmative_status_code):
-        r = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2)
+        r = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2, timeout=10)
         if r is not None:
             if r.status_code == affirmative_status_code:
                 return True
 
     def solve_shortname_recursive(
         self, method, target, prefix, affirmative_status_code, extension_mode=False, node_count=0
     ):
@@ -122,15 +126,15 @@
                     )
                     return url_hint_list
 
                 # check to make sure the file isn't shorter than 6 characters
                 wildcard = "~1*"
                 payload = encode_all(f"{prefix}{c}{wildcard}")
                 url = f"{target}{payload}{suffix}"
-                r = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2)
+                r = self.helpers.request(method=method, url=url, allow_redirects=False, retries=2, timeout=10)
                 if r is not None:
                     if r.status_code == affirmative_status_code:
                         url_hint_list.append(f"{prefix}{c}")
 
                 url_hint_list += self.solve_shortname_recursive(
                     method, target, f"{prefix}{c}", affirmative_status_code, extension_mode, node_count=node_count
                 )
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1595rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1595rc0/bbot/modules/internal/excavate.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,24 @@
     def __init__(self, excavate):
         self.excavate = excavate
         self.compiled_regexes = {}
         for rname, r in self.regexes.items():
             self.compiled_regexes[rname] = re.compile(r)
 
     def search(self, content, event, **kwargs):
+        results = set()
+        for result, name in self._search(content, event, **kwargs):
+            results.add(result)
+        for result in results:
+            self.report(result, name, event, **kwargs)
+
+    def _search(self, content, event, **kwargs):
         for name, regex in self.compiled_regexes.items():
-            results = regex.findall(content)
-            for result in results:
-                self.report(result, name, event, **kwargs)
+            for result in regex.findall(content):
+                yield result, name
 
     def report(self, result, name, event):
         pass
 
 
 class HostnameExtractor(BaseExtractor):
     regexes = {}
@@ -52,39 +58,65 @@
         "fullurl": r"(?i)" + r"(\w{2,15})://((?:\w|\d)(?:[\d\w-]+\.?)+(?::\d{1,5})?(?:/[-\w\.\(\)]+)*/?)",
         "a-tag": r"<a\s+(?:[^>]*?\s+)?href=([\"'])(.*?)\1",
         "script-tag": r"<script\s+(?:[^>]*?\s+)?src=([\"'])(.*?)\1",
     }
 
     prefix_blacklist = ["javascript:", "mailto:", "tel:", "data:", "vbscript:", "about:", "file:"]
 
-    def report(self, result, name, event, **kwargs):
-        spider_danger = kwargs.get("spider_danger", True)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.web_spider_links_per_page = self.excavate.scan.config.get("web_spider_links_per_page", 20)
 
-        tags = []
+    def search(self, content, event, **kwargs):
+        result_hashes = set()
+        results = []
+        for result in self._search(content, event, **kwargs):
+            result_hash = hash(result)
+            if result_hash not in result_hashes:
+                result_hashes.add(result_hash)
+                results.append(result)
+        for i, (result, name) in enumerate(results):
+            new_kwargs = dict(kwargs)
+            if i > self.web_spider_links_per_page:
+                # self.excavate.critical(f"SPIDER DANGER: {result}")
+                new_kwargs["exceeded_max_links"] = True
+            self.report(result, name, event, **new_kwargs)
+
+    def _search(self, content, event, **kwargs):
         parsed = getattr(event, "parsed", None)
+        for name, regex in self.compiled_regexes.items():
+            for result in regex.findall(content):
+                if name == "fullurl":
+                    protocol, other = result
+                    result = f"{protocol}://{other}"
+
+                elif name in ("a-tag", "script-tag") and parsed:
+                    path = html.unescape(result[1]).lstrip("/")
+
+                    for p in self.prefix_blacklist:
+                        if path.lower().startswith(p.lower()):
+                            self.excavate.debug(
+                                f"omitted result from a-tag parser because of blacklisted prefix [{p}]"
+                            )
+                            continue
+
+                    if not self.compiled_regexes["fullurl"].match(path):
+                        path = f"{'/'.join(event.parsed.path.split('/')[0:-1])}/{path}"
+                        full_url = f"{event.parsed.scheme}://{event.parsed.netloc}{path}"
+                        result = urljoin(full_url, urlparse(full_url).path)
+                    else:
+                        result = path
 
-        if name == "fullurl":
-            protocol, other = result
-            result = f"{protocol}://{other}"
-
-        elif name in ("a-tag", "script-tag") and parsed:
-            path = html.unescape(result[1]).lstrip("/")
-
-            for p in self.prefix_blacklist:
-                if path.lower().startswith(p.lower()):
-                    self.excavate.debug(f"omitted result from a-tag parser because of blacklisted prefix [{p}]")
-                    return
-
-            if not self.compiled_regexes["fullurl"].match(path):
-                path = f"{'/'.join(event.parsed.path.split('/')[0:-1])}/{path}"
-                full_url = f"{event.parsed.scheme}://{event.parsed.netloc}{path}"
-                result = urljoin(full_url, urlparse(full_url).path)
+                yield result, name
 
-            else:
-                result = path
+    def report(self, result, name, event, **kwargs):
+        spider_danger = kwargs.get("spider_danger", True)
+        exceeded_max_links = kwargs.get("exceeded_max_links", False)
+
+        tags = []
 
         parsed_uri = self.excavate.helpers.urlparse(result)
         host, port = self.excavate.helpers.split_host_port(parsed_uri.netloc)
         # Handle non-HTTP URIs (ftp, s3, etc.)
         if not "http" in parsed_uri.scheme.lower():
             event_data = {"host": str(host), "description": f"Non-HTTP URI: {result}"}
             parsed_url = getattr(event, "parsed", None)
@@ -98,15 +130,15 @@
             self.excavate.emit_event(
                 {"protocol": parsed_uri.scheme, "host": str(host)},
                 "PROTOCOL",
                 source=event,
             )
             return
 
-        if spider_danger and self.excavate.is_spider_danger(event, result):
+        if exceeded_max_links or (spider_danger and self.excavate.is_spider_danger(event, result)):
             tags.append("spider-danger")
 
         self.excavate.debug(f"Found URL [{result}] from parsing [{event.data.get('url')}] with regex [{name}]")
         self.excavate.emit_event(result, "URL_UNVERIFIED", source=event, tags=tags)
 
 
 class EmailExtractor(BaseExtractor):
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1595rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1595rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1595rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1595rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1595rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1595rc0/bbot/modules/massdns.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,39 +75,37 @@
         self.resolver_file = self.helpers.wordlist(
             nameservers_url,
             cache_hrs=24 * 7,
         )
         self.devops_mutations = list(self.helpers.word_cloud.devops_mutations)
         return super().setup()
 
+    def filter_event(self, event):
+        self.add_found(event)
+        return super().filter_event(event)
+
     def handle_event(self, event):
         query = self.make_query(event)
         h = hash(query)
         if not h in self.source_events:
             self.source_events[h] = event
 
         self.info(f"Brute-forcing subdomains for {query}")
         for hostname in self.massdns(query, self.helpers.read_file(self.subdomain_file)):
             self.emit_result(hostname, event, query)
 
     def abort_if(self, event):
         if not event.scope_distance == 0:
             return True, "event is not in scope"
-        if "unresolved" in event.tags:
-            return True, "event is unresolved"
         if "wildcard" in event.tags:
             return True, "event is a wildcard"
-        if not any(x in event.tags for x in ("a-record", "aaaa-record", "cname-record")):
-            return True, "event is not a valid record type"
 
     def emit_result(self, result, source_event, query):
         if not result == source_event:
             kwargs = {"abort_if": self.abort_if}
-            if result.endswith(f".{query}"):
-                kwargs["on_success_callback"] = self.add_found
             self.emit_event(result, "DNS_NAME", source_event, **kwargs)
 
     def already_processed(self, hostname):
         if hash(hostname) in self.processed:
             return True
         return False
 
@@ -117,15 +115,20 @@
             self.info(abort_msg)
             return []
         results = list(self._massdns(domain, subdomains))
         if len(results) > 50:
             if self._canary_check(domain):
                 self.info(abort_msg)
                 return []
-        return results
+        self.verbose(f"Resolving batch of {len(results):,} results")
+        resolved = dict(self.helpers.resolve_batch(results, type=("A", "AAAA", "CNAME"), cache_result=True))
+        resolved = {k: v for k, v in resolved.items() if v}
+        for hostname in resolved:
+            self.add_found(hostname)
+        return list(resolved)
 
     def _canary_check(self, domain, num_checks=50):
         random_subdomains = list(self.gen_random_subdomains(num_checks))
         self.verbose(f"Testing {len(random_subdomains):,} canaries against {domain}")
         canary_results = list(self._massdns(domain, random_subdomains))
         for result in canary_results:
             if self.helpers.resolve(result):
@@ -221,78 +224,91 @@
                             yield hostname
 
     def finish(self):
         found = sorted(self.found.items(), key=lambda x: len(x[-1]), reverse=True)
 
         base_mutations = set()
         for i, (domain, subdomains) in enumerate(found):
-            max_mem_percent = 90
-            mem_status = self.helpers.memory_status()
-            # abort if we don't have the memory
-            mem_percent = mem_status.percent
-            if mem_percent > max_mem_percent:
-                free_memory = mem_status.available
-                free_memory_human = self.helpers.bytes_to_human(free_memory)
-                self.hugewarning(
-                    f"Cannot proceed with DNS mutations because system memory is at {mem_percent:.1f}% ({free_memory_human} remaining)"
-                )
-                break
-
-            query = domain
-            domain_hash = hash(domain)
-            if self.scan.stopping:
-                return
-
-            mutations = set(base_mutations)
-
-            def add_mutation(_domain_hash, m):
-                h = hash((_domain_hash, m))
-                if h not in self.mutations_tried:
-                    self.mutations_tried.add(h)
-                    mutations.add(m)
-
-            # try every subdomain everywhere else
-            for _i, (_domain, _subdomains) in enumerate(found):
-                if _domain == domain:
-                    continue
-                for s in _subdomains:
-                    first_segment = s.split(".")[0]
-                    # skip stuff with lots of numbers (e.g. PTRs)
-                    digits = self.digit_regex.findall(first_segment)
-                    excessive_digits = len(digits) > 1
-                    long_digits = any(len(d) > 3 for d in digits)
-                    if excessive_digits or long_digits:
+            # keep looping as long as we're finding things
+            while 1:
+                max_mem_percent = 90
+                mem_status = self.helpers.memory_status()
+                # abort if we don't have the memory
+                mem_percent = mem_status.percent
+                if mem_percent > max_mem_percent:
+                    free_memory = mem_status.available
+                    free_memory_human = self.helpers.bytes_to_human(free_memory)
+                    self.hugewarning(
+                        f"Cannot proceed with DNS mutations because system memory is at {mem_percent:.1f}% ({free_memory_human} remaining)"
+                    )
+                    break
+
+                query = domain
+                domain_hash = hash(domain)
+                if self.scan.stopping:
+                    return
+
+                mutations = set(base_mutations)
+
+                def add_mutation(_domain_hash, m):
+                    h = hash((_domain_hash, m))
+                    if h not in self.mutations_tried:
+                        self.mutations_tried.add(h)
+                        mutations.add(m)
+
+                # try every subdomain everywhere else
+                for _domain, _subdomains in found:
+                    if _domain == domain:
                         continue
-                    add_mutation(domain_hash, first_segment)
+                    for s in _subdomains:
+                        first_segment = s.split(".")[0]
+                        # skip stuff with lots of numbers (e.g. PTRs)
+                        digits = self.digit_regex.findall(first_segment)
+                        excessive_digits = len(digits) > 2
+                        long_digits = any(len(d) > 3 for d in digits)
+                        if excessive_digits or long_digits:
+                            continue
+                        add_mutation(domain_hash, first_segment)
+                        for word in self.helpers.extract_words(
+                            first_segment, word_regexes=self.helpers.word_cloud.dns_mutator.extract_word_regexes
+                        ):
+                            add_mutation(domain_hash, word)
+
+                # word cloud
+                for mutation in self.helpers.word_cloud.mutations(
+                    subdomains, cloud=False, numbers=3, number_padding=1
+                ):
+                    for delimiter in ("", ".", "-"):
+                        m = delimiter.join(mutation).lower()
+                        add_mutation(domain_hash, m)
+
+                # special dns mutator
+                for subdomain in self.helpers.word_cloud.dns_mutator.mutations(
+                    subdomains, max_mutations=self.max_mutations
+                ):
+                    add_mutation(domain_hash, subdomain)
+
+                if mutations:
+                    self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
+                    results = list(self.massdns(query, mutations))
+                    for hostname in results:
+                        source_event = self.get_source_event(hostname)
+                        if source_event is None:
+                            self.verbose(f"Could not correlate source event from: {hostname}")
+                            source_event = self.scan.root_event
+                        self.emit_result(hostname, source_event, query)
+                    if results:
+                        continue
+                break
 
-            # word cloud
-            for mutation in self.helpers.word_cloud.mutations(subdomains, cloud=False, numbers=3, number_padding=1):
-                for delimiter in ("", ".", "-"):
-                    m = delimiter.join(mutation).lower()
-                    add_mutation(domain_hash, m)
-
-            # special dns mutator
-            to_mutate = subdomains.union(self.helpers.word_cloud.devops_mutations)
-            for subdomain in self.helpers.word_cloud.dns_mutator.mutations(
-                to_mutate, max_mutations=self.max_mutations
-            ):
-                add_mutation(domain_hash, subdomain)
-
-            if mutations:
-                self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
-                for hostname in self.massdns(query, mutations):
-                    source_event = self.get_source_event(hostname)
-                    if source_event is None:
-                        self.verbose(f"Could not correlate source event from: {hostname}")
-                        source_event = self.scan.root_event
-                    self.emit_result(hostname, source_event, query)
-
-    def add_found(self, event):
-        if self.helpers.is_subdomain(event.data):
-            subdomain, domain = event.data.split(".", 1)
+    def add_found(self, host):
+        if not isinstance(host, str):
+            host = host.data
+        if self.helpers.is_subdomain(host):
+            subdomain, domain = host.split(".", 1)
             if not self.helpers.is_ptr(subdomain):
                 try:
                     self.found[domain].add(subdomain)
                 except KeyError:
                     self.found[domain] = set((subdomain,))
 
     def gen_subdomains(self, prefixes, domain):
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1595rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1595rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/otx.py` & `bbot-1.0.5.1595rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/asset_inventory.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class asset_inventory(CSV):
     watched_events = ["OPEN_TCP_PORT", "DNS_NAME", "URL", "FINDING", "VULNERABILITY", "TECHNOLOGY"]
     meta = {"description": "Output to an asset inventory style flattened CSV file"}
     options = {"output_file": ""}
     options_desc = {"output_file": "Set a custom output file"}
 
-    header_row = ["Host", "IP(s)", "Status", "Open Ports", "Risk Rating", "Findings", "Description"]
+    header_row = ["Host", "Provider", "IP(s)", "Status", "Open Ports", "Risk Rating", "Findings", "Description"]
     filename = "asset-inventory.csv"
 
     def setup(self):
         self.assets = {}
         self.open_port_producers = "httpx" in self.scan.modules or any(
             ["portscan" in m.flags for m in self.scan.modules.values()]
         )
@@ -61,20 +61,26 @@
                 severity_int = severity_map.get(event.data.get("severity", "N/A"), 0)
                 if severity_int > self.assets[event.host].risk_rating:
                     self.assets[event.host].risk_rating = severity_int
 
             if event.type == "TECHNOLOGY":
                 self.assets[event.host].technologies.add(event.data["technology"])
 
+            for tag in event.tags:
+                if tag.startswith("cdn-") or tag.startswith("cloud-"):
+                    self.assets[event.host].provider = tag
+                    break
+
     def report(self):
         for asset in sorted(self.assets.values(), key=lambda a: str(a.host)):
             findings_and_vulns = asset.findings.union(asset.vulnerabilities)
             self.writerow(
                 [
                     getattr(asset, "host", ""),
+                    getattr(asset, "provider", ""),
                     ",".join(str(x) for x in getattr(asset, "ip_addresses", set())),
                     "Active" if (asset.ports) else ("Inactive" if self.open_port_producers else "N/A"),
                     ",".join(str(x) for x in getattr(asset, "ports", set())),
                     severity_map[getattr(asset, "risk_rating", "")],
                     ",".join(findings_and_vulns),
                     ",".join(str(x) for x in getattr(asset, "technologies", set())),
                 ]
@@ -89,8 +95,9 @@
         self.host = host
         self.ip_addresses = set()
         self.ports = set()
         self.findings = set()
         self.vulnerabilities = set()
         self.status = "UNKNOWN"
         self.risk_rating = 0
+        self.provider = ""
         self.technologies = set()
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1595rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1595rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1595rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1595rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1595rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1595rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1595rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1595rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1595rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1595rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/robots.py` & `bbot-1.0.5.1595rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1595rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1595rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1595rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1595rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1595rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/social.py` & `bbot-1.0.5.1595rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1595rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1595rc0/bbot/modules/subdomain_hijack.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,33 +67,39 @@
             self.debug(reason)
 
     def check_subdomain(self, event):
         for f in self.fingerprints:
             for domain in f.domains:
                 self_matches = self.helpers.host_in_host(event.data, domain)
                 child_matches = any(self.helpers.host_in_host(domain, h) for h in event.resolved_hosts)
-                if self_matches or child_matches:
-                    for scheme in ("https", "http"):
-                        if self.scan.stopping:
-                            return False, "Scan cancelled"
-                        # first, try base request
-                        url = f"{scheme}://{event.data}"
-                        match, reason = self._verify_fingerprint(f, url)
-                        if match:
-                            return match, reason
-                        # next, try {random_domain} -[DNS]-> domain
-                        url = f"{scheme}://{domain}"
-                        headers = {"Host": event.data}
-                        match, reason = self._verify_fingerprint(f, url, headers=headers)
-                        if match:
-                            return match, reason
+                if event.type == "DNS_NAME_UNRESOLVED":
+                    if self_matches and f.nxdomain:
+                        return True, "NXDOMAIN"
+                else:
+                    if self_matches or child_matches:
+                        for scheme in ("https", "http"):
+                            if self.scan.stopping:
+                                return False, "Scan cancelled"
+                            # first, try base request
+                            url = f"{scheme}://{event.data}"
+                            match, reason = self._verify_fingerprint(f, url, cache_for=60 * 60 * 24)
+                            if match:
+                                return match, reason
+                            # next, try subdomain -[CNAME]-> other_domain
+                            url = f"{scheme}://{domain}"
+                            headers = {"Host": event.data}
+                            match, reason = self._verify_fingerprint(f, url, headers=headers)
+                            if match:
+                                return match, reason
         return False, f'Subdomain "{event.data}" not hijackable'
 
     def _verify_fingerprint(self, fingerprint, *args, **kwargs):
         kwargs["raise_error"] = True
+        kwargs["timeout"] = 10
+        kwargs["retries"] = 0
         if fingerprint.http_status is not None:
             kwargs["allow_redirects"] = False
         try:
             r = self.helpers.request(*args, **kwargs)
             if fingerprint.http_status is not None and r.status_code == fingerprint.http_status:
                 return True, f"HTTP status == {fingerprint.http_status}"
             text = getattr(r, "text", "")
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1595rc0/bbot/modules/telerik.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,14 @@
             return
         else:
             self.scanned_hosts.add(host_hash)
 
         webresource = "Telerik.Web.UI.WebResource.axd?type=rau"
         result = self.test_detector(event.data, webresource)
         if result:
-            self.debug(result.text)
             if "RadAsyncUpload handler is registered succesfully" in result.text:
                 self.debug(f"Detected Telerik instance (Telerik.Web.UI.WebResource.axd?type=rau)")
                 description = f"Telerik RAU AXD Handler detected"
                 self.emit_event(
                     {"host": str(event.host), "url": f"{event.data}{webresource}", "description": description},
                     "FINDING",
                     event,
```

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1595rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1595rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1595rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1595rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1595rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1595rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1595rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1595rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1595rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1595rc0/bbot/scanner/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """
         if event._dummy:
             log.warning(f"Cannot emit dummy event: {event}")
             return False
         if event == event.get_source():
             log.debug(f"Skipping event with self as source: {event}")
             return False
-        if self.is_duplicate_event(event):
+        if not event._force_output and self.is_duplicate_event(event):
             log.debug(f"Skipping {event} because it is a duplicate")
             return False
         return True
 
     def _emit_event(self, event, *args, **kwargs):
         log.debug(f"Emitting {event}")
         distribute_event = True
@@ -116,36 +116,40 @@
             on_success_callback = kwargs.pop("on_success_callback", None)
             abort_if = kwargs.pop("abort_if", None)
 
             # skip DNS resolution if it's disabled in the config and the event is a target and we don't have a blacklist
             skip_dns_resolution = (not self.dns_resolution) and "target" in event.tags and not self.scan.blacklist
             if skip_dns_resolution:
                 event._resolved.set()
-                dns_children = []
+                dns_children = {}
                 dns_tags = {"resolved"}
                 event_whitelisted_dns = True
                 event_blacklisted_dns = False
                 resolved_hosts = []
             else:
                 # DNS resolution
                 (
-                    dns_children,
                     dns_tags,
                     event_whitelisted_dns,
                     event_blacklisted_dns,
-                    resolved_hosts,
+                    dns_children,
                 ) = self.scan.helpers.dns.resolve_event(event, minimal=not self.dns_resolution)
+                resolved_hosts = set()
+                for rdtype, ips in dns_children.items():
+                    if rdtype in ("A", "AAAA", "CNAME"):
+                        for ip in ips:
+                            resolved_hosts.add(ip)
 
             # kill runaway DNS chains
             dns_resolve_distance = getattr(event, "dns_resolve_distance", 0)
             if dns_resolve_distance >= self.scan.helpers.dns.max_dns_resolve_distance:
                 log.debug(
                     f"Skipping DNS children for {event} because their DNS resolve distances would be greater than the configured value for this scan ({self.scan.helpers.dns.max_dns_resolve_distance})"
                 )
-                dns_children = []
+                dns_children = {}
 
             # We do this again in case event.data changed during resolve_event()
             if event.type == "DNS_NAME" and not self._event_precheck(event, exclude=()):
                 log.debug(f"Omitting due to failed precheck: {event}")
                 distribute_event = False
 
             if event.type in ("DNS_NAME", "IP_ADDRESS"):
@@ -178,15 +182,15 @@
             # Scope shepherding
             event_is_duplicate = self.is_duplicate_event(event)
             event_in_report_distance = event.scope_distance <= self.scan.scope_report_distance
             set_scope_distance = event.scope_distance
             if event_whitelisted:
                 set_scope_distance = 0
             if event.host:
-                if (event_whitelisted or event_in_report_distance) and not event_is_duplicate:
+                if (event_whitelisted or event_in_report_distance) and (event._force_output or not event_is_duplicate):
                     if set_scope_distance == 0:
                         log.debug(f"Making {event} in-scope")
                     source_trail = event.make_in_scope(set_scope_distance)
                     for s in source_trail:
                         self.emit_event(s, _block=False, _force_submit=True)
                 else:
                     if event.scope_distance > self.scan.scope_report_distance:
@@ -228,16 +232,14 @@
                 for s in source_trail:
                     self.emit_event(s, _block=False, _force_submit=True)
 
             if distribute_event:
                 self.distribute_event(event)
                 event_distributed = True
 
-            ### Emit DNS children ###
-            emit_children = -1 < event.scope_distance < self.scan.dns_search_distance
             # speculate DNS_NAMES and IP_ADDRESSes from other event types
             source_event = event
             if (
                 event.host
                 and event.type not in ("DNS_NAME", "DNS_NAME_UNRESOLVED", "IP_ADDRESS", "IP_RANGE")
                 and not str(event.module) == "speculate"
             ):
@@ -246,29 +248,43 @@
                 source_event = self.scan.make_event(event.host, "DNS_NAME", module=source_module, source=event)
                 # only emit the event if it's not already in the parent chain
                 if source_event is not None and source_event not in source_event.get_sources():
                     source_event.scope_distance = event.scope_distance
                     if "target" in event.tags:
                         source_event.add_tag("target")
                     self.emit_event(source_event, _block=False, _force_submit=True)
-            if self.dns_resolution and emit_children:
-                dns_child_events = []
-                if dns_children:
-                    for rdtype, record in dns_children:
-                        module = self.scan.helpers.dns._get_dummy_module(rdtype)
-                        module._priority = 4
-                        try:
-                            child_event = self.scan.make_event(record, "DNS_NAME", module=module, source=source_event)
-                            dns_child_events.append(child_event)
-                        except ValidationError as e:
-                            log.warning(
-                                f'Event validation failed for DNS child of {source_event}: "{record}" ({rdtype}): {e}'
-                            )
-                for child_event in dns_child_events:
-                    self.emit_event(child_event, _block=False, _force_submit=True)
+
+            ### Emit DNS children ###
+            if self.dns_resolution:
+                emit_children = -1 < event.scope_distance < self.scan.dns_search_distance
+                if emit_children:
+                    host_hash = hash(str(event.host))
+                    with self.events_accepted_lock:
+                        if host_hash in self.events_accepted:
+                            emit_children = False
+                        self.events_accepted.add(host_hash)
+
+                if emit_children:
+                    dns_child_events = []
+                    if dns_children:
+                        for rdtype, records in dns_children.items():
+                            module = self.scan.helpers.dns._get_dummy_module(rdtype)
+                            module._priority = 4
+                            for record in records:
+                                try:
+                                    child_event = self.scan.make_event(
+                                        record, "DNS_NAME", module=module, source=source_event
+                                    )
+                                    dns_child_events.append(child_event)
+                                except ValidationError as e:
+                                    log.warning(
+                                        f'Event validation failed for DNS child of {source_event}: "{record}" ({rdtype}): {e}'
+                                    )
+                    for child_event in dns_child_events:
+                        self.emit_event(child_event, _block=False, _force_submit=True)
 
         except ValidationError as e:
             log.warning(f"Event validation failed with args={args}, kwargs={kwargs}: {e}")
             log.trace(traceback.format_exc())
 
         finally:
             event._resolved.set()
@@ -298,18 +314,19 @@
         """
         event_hash = self.hash_event(event)
         suppress_dupes = getattr(event.module, "suppress_dupes", True)
         with self.events_accepted_lock:
             duplicate_event = suppress_dupes and event_hash in self.events_accepted
             if add:
                 self.events_accepted.add(event_hash)
-        return duplicate_event and not event._force_output
+        return duplicate_event
 
     def accept_event(self, event):
-        if self.is_duplicate_event(event, add=True):
+        is_duplicate = self.is_duplicate_event(event, add=True)
+        if is_duplicate and not event._force_output:
             log.debug(f"{event.module}: not raising duplicate event {event}")
             return False
         return True
 
     def catch(self, callback, *args, **kwargs):
         """
         Wrapper to ensure error messages get surfaced to the user
```

### Comparing `bbot-1.0.5.1567rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1595rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1595rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/scanner/target.py` & `bbot-1.0.5.1595rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1595rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/conftest.py` & `bbot-1.0.5.1595rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/helpers.py` & `bbot-1.0.5.1595rc0/bbot/test/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/modules_test_classes.py` & `bbot-1.0.5.1595rc0/bbot/test/modules_test_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             if (
                 event.type == "FINDING"
                 and event.data["description"].startswith("Hijackable Subdomain")
                 and self.rand_subdomain in event.data["description"]
                 and event.data["host"] == self.rand_subdomain
             ):
                 return True
-        return False
+        return False, f"No hijackable subdomains in {events}"
 
 
 class Fingerprintx(HttpxMockHelper):
     targets = ["127.0.0.1:8888"]
 
     def mock_args(self):
         pass
```

### Comparing `bbot-1.0.5.1567rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1595rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test.conf` & `bbot-1.0.5.1595rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_1/test_before_patching.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_1/test_before_patching.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_1/test_modules_full.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_1/test_modules_full.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_agent.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_cloud_helpers.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_helpers.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -531,23 +531,17 @@
     assert "SRV" not in wildcard_rdtypes
     assert wildcard_rdtypes["A"] == (True, "github.io")
     assert hash("github.io") in helpers.dns._wildcard_cache
     assert len(helpers.dns._wildcard_cache[hash("github.io")]) > 0
     wildcard_event1 = scan.make_event("wat.asdf.fdsa.github.io", "DNS_NAME", dummy=True)
     wildcard_event2 = scan.make_event("wats.asd.fdsa.github.io", "DNS_NAME", dummy=True)
     wildcard_event3 = scan.make_event("github.io", "DNS_NAME", dummy=True)
-    children1, event_tags1, event_whitelisted1, event_blacklisted1, resolved_hosts1 = scan.helpers.resolve_event(
-        wildcard_event1
-    )
-    children2, event_tags2, event_whitelisted2, event_blacklisted2, resolved_hosts2 = scan.helpers.resolve_event(
-        wildcard_event2
-    )
-    children3, event_tags3, event_whitelisted3, event_blacklisted3, resolved_hosts3 = scan.helpers.resolve_event(
-        wildcard_event3
-    )
+    event_tags1, event_whitelisted1, event_blacklisted1, children1 = scan.helpers.resolve_event(wildcard_event1)
+    event_tags2, event_whitelisted2, event_blacklisted2, children2 = scan.helpers.resolve_event(wildcard_event2)
+    event_tags3, event_whitelisted3, event_blacklisted3, children3 = scan.helpers.resolve_event(wildcard_event3)
     helpers.handle_wildcard_event(wildcard_event1, children1)
     helpers.handle_wildcard_event(wildcard_event2, children2)
     helpers.handle_wildcard_event(wildcard_event3, children3)
     assert "wildcard" in wildcard_event1.tags
     assert "a-wildcard" in wildcard_event1.tags
     assert "srv-wildcard" not in wildcard_event1.tags
     assert "wildcard" in wildcard_event2.tags
@@ -564,23 +558,20 @@
     assert helpers.is_ptr("wsc-11-22-33-wat.evilcorp.com") == False
     assert helpers.is_ptr("11wat.evilcorp.com") == False
 
     # Ensure events with hosts have resolved_hosts attribute populated
 
     resolved_hosts_event1 = scan.make_event("dns.google", "DNS_NAME", dummy=True)
     resolved_hosts_event2 = scan.make_event("http://dns.google/", "URL_UNVERIFIED", dummy=True)
-    children, event_tags1, event_whitelisted1, event_blacklisted1, resolved_hosts1 = scan.helpers.resolve_event(
-        resolved_hosts_event1
-    )
-    children, event_tags2, event_whitelisted2, event_blacklisted2, resolved_hosts2 = scan.helpers.resolve_event(
-        resolved_hosts_event2
-    )
+    event_tags1, event_whitelisted1, event_blacklisted1, children1 = scan.helpers.resolve_event(resolved_hosts_event1)
+    event_tags2, event_whitelisted2, event_blacklisted2, children2 = scan.helpers.resolve_event(resolved_hosts_event2)
 
-    assert "8.8.8.8" in [str(x) for x in resolved_hosts1]
-    assert resolved_hosts_event1.resolved_hosts == resolved_hosts_event2.resolved_hosts
+    assert "8.8.8.8" in [str(x) for x in children1["A"]]
+    assert "8.8.8.8" in [str(x) for x in children2["A"]]
+    assert set(children1.keys()) == set(children2.keys())
 
     msg = "Ignore this error, it belongs here"
 
     def raise_e():
         raise Exception(msg)
 
     def raise_k():
```

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_scope.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/test/test_step_2/test_threadpool.py` & `bbot-1.0.5.1595rc0/bbot/test/test_step_2/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1595rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1595rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1595rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1595rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1567rc0/pyproject.toml` & `bbot-1.0.5.1595rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1567rc"
+version = "v1.0.5.1595rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1567rc0/PKG-INFO` & `bbot-1.0.5.1595rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1567rc0
+Version: 1.0.5.1595rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

