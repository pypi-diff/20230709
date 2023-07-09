# Comparing `tmp/abuse_whois-0.6.0.tar.gz` & `tmp/abuse_whois-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuse_whois-0.6.0.tar", max compression
+gzip compressed data, was "abuse_whois-0.7.0.tar", max compression
```

## Comparing `abuse_whois-0.6.0.tar` & `abuse_whois-0.7.0.tar`

### file list

```diff
@@ -1,69 +1,66 @@
--rw-r--r--   0        0        0     1070 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/LICENSE
--rw-r--r--   0        0        0     3680 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/README.md
--rw-r--r--   0        0        0      130 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/abuse_whois/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/abuse_whois/api/__init__.py
--rw-r--r--   0        0        0      490 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/abuse_whois/api/app.py
--rw-r--r--   0        0        0        0 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/abuse_whois/api/endpoints/__init__.py
--rw-r--r--   0        0        0      194 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/abuse_whois/api/endpoints/index.py
--rw-r--r--   0        0        0      505 2023-02-26 06:28:35.235892 abuse_whois-0.6.0/abuse_whois/api/endpoints/whois.py
--rw-r--r--   0        0        0      582 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/cli.py
--rw-r--r--   0        0        0      146 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/errors.py
--rw-r--r--   0        0        0      954 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/ip.py
--rw-r--r--   0        0        0     2606 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/main.py
--rw-r--r--   0        0        0        0 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/__init__.py
--rw-r--r--   0        0        0      276 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/__init__.py
--rw-r--r--   0        0        0      193 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rule.py
--rw-r--r--   0        0        0      303 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/000webhost.yaml
--rw-r--r--   0        0        0      252 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/adobe.yaml
--rw-r--r--   0        0        0      263 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/backblaze.yaml
--rw-r--r--   0        0        0      298 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/bitly.yaml
--rw-r--r--   0        0        0      294 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/blogger.yaml
--rw-r--r--   0        0        0     3466 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/changeip.yaml
--rw-r--r--   0        0        0      271 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/cloudflare.yaml
--rw-r--r--   0        0        0      365 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/firebase.yaml
--rw-r--r--   0        0        0      258 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/glitch.yaml
--rw-r--r--   0        0        0      275 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/godaddy.yaml
--rw-r--r--   0        0        0      324 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/google_cloud.yaml
--rw-r--r--   0        0        0      347 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/google_site.yaml
--rw-r--r--   0        0        0      296 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/jimdo.yaml
--rw-r--r--   0        0        0      280 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/micorosoft.yaml
--rw-r--r--   0        0        0      242 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/netlify.yaml
--rw-r--r--   0        0        0      360 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/notion.yaml
--rw-r--r--   0        0        0      233 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/replit.yaml
--rw-r--r--   0        0        0      254 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/softlayer.yaml
--rw-r--r--   0        0        0      240 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/square.yaml
--rw-r--r--   0        0        0      266 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/telegram.yaml
--rw-r--r--   0        0        0      251 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/weebly.yaml
--rw-r--r--   0        0        0      262 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/wordpress.yaml
--rw-r--r--   0        0        0      399 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/yola.yaml
--rw-r--r--   0        0        0      543 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules.py
--rw-r--r--   0        0        0     1826 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/__init__.py
--rw-r--r--   0        0        0      462 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rule.py
--rw-r--r--   0        0        0      424 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/alibaba_cloud.yaml
--rw-r--r--   0        0        0      272 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/cloudflare.yaml
--rw-r--r--   0        0        0      340 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/digitalocean.yaml
--rw-r--r--   0        0        0      264 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/dynadot.yaml
--rw-r--r--   0        0        0      286 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/fran_tech.yaml
--rw-r--r--   0        0        0      268 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/godaddy.yaml
--rw-r--r--   0        0        0      303 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/hostinger.yaml
--rw-r--r--   0        0        0      249 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/name.yaml
--rw-r--r--   0        0        0      286 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/namecheap.yaml
--rw-r--r--   0        0        0      316 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/namesilo.yaml
--rw-r--r--   0        0        0     2451 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/noip.yaml
--rw-r--r--   0        0        0      254 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/orange.yaml
--rw-r--r--   0        0        0      343 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/publicdomainregistry.yaml
--rw-r--r--   0        0        0      265 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/registrareu.yaml
--rw-r--r--   0        0        0      289 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/tucows.yaml
--rw-r--r--   0        0        0      510 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/matchers/whois/rules.py
--rw-r--r--   0        0        0      193 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/schemas/__init__.py
--rw-r--r--   0        0        0      210 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/schemas/api_model.py
--rw-r--r--   0        0        0     1388 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/schemas/contact.py
--rw-r--r--   0        0        0      166 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/schemas/query.py
--rw-r--r--   0        0        0      136 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/schemas/rule.py
--rw-r--r--   0        0        0      775 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/schemas/whois.py
--rw-r--r--   0        0        0     1538 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/settings.py
--rw-r--r--   0        0        0     2526 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/utils.py
--rw-r--r--   0        0        0     1824 2023-02-26 06:28:35.239892 abuse_whois-0.6.0/abuse_whois/whois.py
--rw-r--r--   0        0        0     1398 2023-02-26 06:29:07.563912 abuse_whois-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 abuse_whois-0.6.0/setup.py
--rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 abuse_whois-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3827 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/README.md
+-rw-r--r--   0        0        0      130 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/api/endpoints/__init__.py
+-rw-r--r--   0        0        0      194 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/api/endpoints/index.py
+-rw-r--r--   0        0        0      609 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/api/endpoints/whois.py
+-rw-r--r--   0        0        0      490 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/api/main.py
+-rw-r--r--   0        0        0       98 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/errors.py
+-rw-r--r--   0        0        0     2105 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/main.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rule.py
+-rw-r--r--   0        0        0      303 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/000webhost.yaml
+-rw-r--r--   0        0        0      252 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/adobe.yaml
+-rw-r--r--   0        0        0      263 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/backblaze.yaml
+-rw-r--r--   0        0        0      298 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/bitly.yaml
+-rw-r--r--   0        0        0      294 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/blogger.yaml
+-rw-r--r--   0        0        0     3466 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/changeip.yaml
+-rw-r--r--   0        0        0      271 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/cloudflare.yaml
+-rw-r--r--   0        0        0      365 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/firebase.yaml
+-rw-r--r--   0        0        0      258 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/glitch.yaml
+-rw-r--r--   0        0        0      275 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/godaddy.yaml
+-rw-r--r--   0        0        0      324 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/google_cloud.yaml
+-rw-r--r--   0        0        0      347 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/google_site.yaml
+-rw-r--r--   0        0        0      296 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/jimdo.yaml
+-rw-r--r--   0        0        0      280 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/micorosoft.yaml
+-rw-r--r--   0        0        0      242 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/netlify.yaml
+-rw-r--r--   0        0        0      360 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/notion.yaml
+-rw-r--r--   0        0        0      233 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/replit.yaml
+-rw-r--r--   0        0        0      254 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/softlayer.yaml
+-rw-r--r--   0        0        0      240 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/square.yaml
+-rw-r--r--   0        0        0      266 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/telegram.yaml
+-rw-r--r--   0        0        0      251 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/weebly.yaml
+-rw-r--r--   0        0        0      262 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/wordpress.yaml
+-rw-r--r--   0        0        0      399 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/yola.yaml
+-rw-r--r--   0        0        0      548 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules.py
+-rw-r--r--   0        0        0     1938 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/whois/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rule.py
+-rw-r--r--   0        0        0      424 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/alibaba_cloud.yaml
+-rw-r--r--   0        0        0      272 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/cloudflare.yaml
+-rw-r--r--   0        0        0      340 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/digitalocean.yaml
+-rw-r--r--   0        0        0      264 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/dynadot.yaml
+-rw-r--r--   0        0        0      286 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/fran_tech.yaml
+-rw-r--r--   0        0        0      268 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/godaddy.yaml
+-rw-r--r--   0        0        0      303 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/hostinger.yaml
+-rw-r--r--   0        0        0      249 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/name.yaml
+-rw-r--r--   0        0        0      286 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/namecheap.yaml
+-rw-r--r--   0        0        0      316 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/namesilo.yaml
+-rw-r--r--   0        0        0     2451 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/noip.yaml
+-rw-r--r--   0        0        0      254 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/orange.yaml
+-rw-r--r--   0        0        0      343 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/publicdomainregistry.yaml
+-rw-r--r--   0        0        0      265 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/registrareu.yaml
+-rw-r--r--   0        0        0      289 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/tucows.yaml
+-rw-r--r--   0        0        0      497 2023-07-09 09:49:16.277200 abuse_whois-0.7.0/abuse_whois/matchers/whois/rules.py
+-rw-r--r--   0        0        0      193 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/schemas/__init__.py
+-rw-r--r--   0        0        0      214 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/schemas/api_model.py
+-rw-r--r--   0        0        0     1308 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/schemas/contact.py
+-rw-r--r--   0        0        0      166 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/schemas/query.py
+-rw-r--r--   0        0        0      136 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/schemas/rule.py
+-rw-r--r--   0        0        0      775 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/schemas/whois.py
+-rw-r--r--   0        0        0     1649 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/settings.py
+-rw-r--r--   0        0        0     3260 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/utils.py
+-rw-r--r--   0        0        0     1398 2023-07-09 09:49:16.281200 abuse_whois-0.7.0/abuse_whois/whois.py
+-rw-r--r--   0        0        0     1414 2023-07-09 09:49:37.649453 abuse_whois-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 abuse_whois-0.7.0/PKG-INFO
```

### Comparing `abuse_whois-0.6.0/LICENSE` & `abuse_whois-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.6.0/README.md` & `abuse_whois-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 - https://github.com/bradleyjkemp/abwhose
 - https://github.com/certsocietegenerale/abuse_finder
 
 ## Requirements
 
 - Python 3.10+
-- whois
 
 ## Installation
 
 ```bash
 pip install abuse_whois
 
 # or if you want to use built-in REST API
@@ -30,30 +29,30 @@
 ## Usage
 
 ### As a library
 
 ```python
 from abuse_whois import get_abuse_contacts
 
-get_abuse_contacts("1.1.1.1")
-get_abuse_contacts("github.com")
-get_abuse_contacts("https://github.com")
-get_abuse_contacts("foo@example.com")
+await get_abuse_contacts("1.1.1.1")
+await get_abuse_contacts("github.com")
+await get_abuse_contacts("https://github.com")
+await get_abuse_contacts("foo@example.com")
 ```
 
 ### As a CLI tool
 
 ```bash
 $ abuse_whois 1.1.1.1 | jq .
 ```
 
 ### As a REST API
 
 ```bash
-$ uvicorn abuse_whois.api.app:app
+$ uvicorn abuse_whois.api.main:app
 INFO:     Started server process [2283]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 
 $ http localhost:8000/api/whois/ address=https://github.com
 ```
@@ -67,25 +66,26 @@
 docker run -i -d -p 8000:8000 abuse-whois
 ```
 
 ## Settings
 
 All settings can be done via environment variables or `.env` file.
 
-| Name                                       | Type                   | Default  | Desc.                                                    |
-| ------------------------------------------ | ---------------------- | -------- | -------------------------------------------------------- |
-| WHOIS_LOOKUP_TIMEOUT                       | int                    | 10       | Timeout value for whois lookup (seconds)                 |
-| WHOIS_LOOKUP_CACHE_SIZE                    | int                    | 1024     | Cache size for whois lookup                              |
-| WHOIS_LOOKUP_CACHE_TTL                     | int                    | 3600     | Cache TTL value for whois lookup (seconds)               |
-| IP_ADDRESS_LOOKUP_TIMEOUT                  | int                    | 10       | Timeout value for IP address lookup (seconds)            |
-| IP_ADDRESS_LOOKUP_CACHE_SIZE               | int                    | 1024     | Cache size for IP address lookup                         |
-| IP_ADDRESS_LOOKUP_CACHE_TTL                | int                    | 3600     | Cache TTL value for IP address lookup (seconds)          |
-| RULE_EXTENSIONS                            | CommaSeparatedStrings  | yaml,yml | Rule file extensions                                     |
-| ADDITIONAL_WHOIS_RULE_DIRECTORIES          | CommaSeparatedStrings] |          | Additional directories contain whois rule files          |
-| ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES | CommaSeparatedStrings] |          | Additional directories contain shared hosting rule files |
+| Name                                       | Type                  | Default  | Desc.                                                    |
+| ------------------------------------------ | --------------------- | -------- | -------------------------------------------------------- |
+| WHOIS_LOOKUP_TIMEOUT                       | int                   | 10       | Timeout value for whois lookup (seconds)                 |
+| WHOIS_LOOKUP_CACHE_SIZE                    | int                   | 1024     | Cache size for whois lookup                              |
+| WHOIS_LOOKUP_CACHE_TTL                     | int                   | 3600     | Cache TTL value for whois lookup (seconds)               |
+| WHOIS_LOOKUP_MAX_RETRIES                   | int                   | 3        | Max retries on timeout error                             |
+| IP_ADDRESS_LOOKUP_TIMEOUT                  | int                   | 10       | Timeout value for IP address lookup (seconds)            |
+| IP_ADDRESS_LOOKUP_CACHE_SIZE               | int                   | 1024     | Cache size for IP address lookup                         |
+| IP_ADDRESS_LOOKUP_CACHE_TTL                | int                   | 3600     | Cache TTL value for IP address lookup (seconds)          |
+| RULE_EXTENSIONS                            | CommaSeparatedStrings | yaml,yml | Rule file extensions                                     |
+| ADDITIONAL_WHOIS_RULE_DIRECTORIES          | CommaSeparatedStrings |          | Additional directories contain whois rule files          |
+| ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES | CommaSeparatedStrings |          | Additional directories contain shared hosting rule files |
 
 ## Contributions
 
 `abuse_whois` works based on a combination of static rules and a parsing result of whois response.
 
 - Rules:
   - [Registrar and hosting provider](https://github.com/ninoseki/abuse_whois/wiki/Registrar-and-Hosting-Provider)
```

### Comparing `abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules/changeip.yaml` & `abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules/changeip.yaml`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.6.0/abuse_whois/matchers/shared_hosting/rules.py` & `abuse_whois-0.7.0/abuse_whois/matchers/shared_hosting/rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 @lru_cache(maxsize=1)
 def load_rules() -> list[SharedHostingRule]:
     paths = glob_rules(
         DEFAULT_RULE_DIRECTORY,
         additional_directories=settings.ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES,
     )
-    return [SharedHostingRule.parse_obj(load_yaml(path)) for path in paths]
+    return [SharedHostingRule.model_validate(load_yaml(path)) for path in paths]
```

### Comparing `abuse_whois-0.6.0/abuse_whois/matchers/whois/__init__.py` & `abuse_whois-0.7.0/abuse_whois/matchers/whois/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 import re
-from re import Pattern
 
 from abuse_whois.schemas import Contact, WhoisRecord
 from abuse_whois.utils import is_email
 from abuse_whois.whois import get_whois_record
 
 from .rules import load_rules
 
 
 def get_whois_abuse_contact_by_regexp(
-    record: WhoisRecord, *, abuse_email_pattern: Pattern = r"abuse@[a-z0-9\-.]+"
-) -> Contact | None:
-    provider = record.registrar or ""
-
-    matches = re.findall(abuse_email_pattern, record.raw_text)
+    record: WhoisRecord,
+    *,
+    email_pattern: str = r"[a-z0-9\.\-+_]+@[a-z0-9\.\-+_]+\.[a-z]+"
+) -> str | None:
+    matches = re.findall(email_pattern, record.raw_text)
     if len(matches) == 0:
         return None
 
-    # returns the email address in the bottom
-    matches.reverse()
-    for match in matches:
-        if is_email(str(match)):
-            return Contact(provider=provider, address=str(match))
+    # returns the email address which contains "abuse"
+    emails = [str(match) for match in matches if is_email(str(match))]
+    emails.reverse()
+
+    for email in emails:
+        if "abuse" in email:
+            return email
 
     return None
 
 
 def get_whois_abuse_contact(record: WhoisRecord) -> Contact | None:
     provider = record.registrar
     email: str | None = None
 
     # check email format for just in case
     if is_email(record.abuse.email or ""):
         email = record.abuse.email
 
     if email is None:
         # fallback to regexp based search
-        contact = get_whois_abuse_contact_by_regexp(record)
-        if contact is None:
+        email = get_whois_abuse_contact_by_regexp(record)
+        if email is None:
             return None
 
-        provider = contact.provider
-        email = contact.address
-
-    # use email's domain as a provider
-    if is_email(provider or ""):
+    # use email's domain as a provider if provider is None
+    if provider is None and is_email(email or ""):
         provider = email.split("@")[-1]
 
     if provider is None or email is None:
         return None
 
     return Contact(provider=provider, address=email)
 
 
-async def get_contact_from_whois(
+async def get_whois_contact(
     hostname: str,
 ) -> Contact | None:
     rules = load_rules()
     for rule in rules:
         if await rule.match(hostname):
             return rule.contact
 
     # Use whois registrar & abuse data
     try:
         whois_record = await get_whois_record(hostname)
     except Exception:
         return None
 
     return get_whois_abuse_contact(whois_record)
+
+
+async def get_optional_whois_contact(hostname: str | None) -> Contact | None:
+    if hostname is None:
+        return None
+
+    return await get_whois_contact(hostname)
```

### Comparing `abuse_whois-0.6.0/abuse_whois/matchers/whois/rules/noip.yaml` & `abuse_whois-0.7.0/abuse_whois/matchers/whois/rules/noip.yaml`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.6.0/abuse_whois/schemas/contact.py` & `abuse_whois-0.7.0/abuse_whois/schemas/contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-from typing import Any
-
-from abuse_whois.schemas.whois import WhoisRecord
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing import Literal
+from typing import Any, Literal
 
 from pydantic import Field
 
+from abuse_whois.schemas.whois import WhoisRecord
 from abuse_whois.utils import is_email, is_url
 
 from .api_model import APIModel
 
 
 class Contact(APIModel):
     provider: str = Field(..., description="Provider name")
```

### Comparing `abuse_whois-0.6.0/abuse_whois/schemas/whois.py` & `abuse_whois-0.7.0/abuse_whois/schemas/whois.py`

 * *Files identical despite different names*

### Comparing `abuse_whois-0.6.0/abuse_whois/settings.py` & `abuse_whois-0.7.0/abuse_whois/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 TESTING: bool = config("TESTING", cast=bool, default=False)
 
 LOG_FILE = config("LOG_FILE", default=sys.stderr)
 LOG_LEVEL: str = config("LOG_LEVEL", cast=str, default="DEBUG")
 LOG_BACKTRACE: bool = config("LOG_BACKTRACE", cast=bool, default=True)
 
 # Abuse Whois setting
+WHOIS_LOOKUP_MAX_RETRIES: int = config("WHOIS_LOOKUP_MAX_RETRIES", cast=int, default=3)
 WHOIS_LOOKUP_TIMEOUT: int = config("WHOIS_LOOKUP_TIMEOUT", cast=int, default=10)
 WHOIS_LOOKUP_CACHE_SIZE: int = config("WHOIS_LOOKUP_CACHE_SIZE", cast=int, default=1024)
 WHOIS_LOOKUP_CACHE_TTL: int = config(
     "WHOIS_LOOKUP_CACHE_TTL", cast=int, default=60 * 60
 )
 
 
@@ -34,14 +35,14 @@
     "IP_ADDRESS_LOOKUP_CACHE_TTL", cast=int, default=60 * 60
 )
 
 RULE_EXTENSIONS: CommaSeparatedStrings = config(
     "RULE_EXTENSIONS", cast=CommaSeparatedStrings, default="yaml,yml"
 )
 
-ADDITIONAL_WHOIS_RULE_DIRECTORIES = config(
+ADDITIONAL_WHOIS_RULE_DIRECTORIES: CommaSeparatedStrings = config(
     "ADDITIONAL_WHOIS_RULE_DIRECTORIES", cast=CommaSeparatedStrings, default=""
 )
 
 ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES: CommaSeparatedStrings = config(
     "ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES", cast=CommaSeparatedStrings, default=""
 )
```

### Comparing `abuse_whois-0.6.0/abuse_whois/utils.py` & `abuse_whois-0.7.0/abuse_whois/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,58 @@
+import asyncio
 import pathlib
+import socket
+from collections.abc import Callable
+from contextlib import contextmanager
 from functools import lru_cache
 from typing import cast
 from urllib.parse import urlparse
 
 import tldextract
+import validators
 import yaml
-from email_validator import EmailNotValidError, validate_email
-from pydantic import BaseModel, ValidationError
-from pydantic.networks import AnyHttpUrl
+from asyncer import asyncify
+from cachetools import TTLCache, cached
+from starlette.datastructures import CommaSeparatedStrings
 
-from abuse_whois import settings
+from . import settings
 
 
-class URLModel(BaseModel):
-    url: AnyHttpUrl
+def _is_x(v: str, *, validator: Callable[[str], bool]) -> bool:
+    res = validator(v)
+
+    if isinstance(res, validators.ValidationFailure):
+        return False
+
+    return res
 
 
 def is_ip_address(v: str) -> bool:
-    try:
-        model = URLModel(url=f"http://{v}")
-        return model.url.host_type in ["ipv4", "ipv6"]
-    except ValidationError:
-        return False
+    return _is_x(v, validator=validators.ipv4) or _is_x(v, validator=validators.ipv6)  # type: ignore
 
 
 def is_domain(v: str) -> bool:
     if len(v.split(".")) == 1:
         return False
 
     if "@" in v:
         return False
 
-    try:
-        model = URLModel(url=f"http://{v}")
-        return model.url.host_type in ["domain", "int_domain"]
-    except ValidationError:
-        return False
+    return _is_x(v, validator=validators.domain)  # type: ignore
 
 
 def is_url(v: str) -> bool:
     if not v.startswith(("http://", "https://")):
         return False
 
-    try:
-        URLModel(url=v)
-        return True
-    except ValidationError:
-        return False
+    return _is_x(v, validator=validators.url)  # type: ignore
 
 
 def is_email(v: str) -> bool:
-    try:
-        validate_email(v, check_deliverability=False)
-        return True
-    except EmailNotValidError:
-        return False
+    return _is_x(v, validator=validators.email)  # type: ignore
 
 
 def is_supported_address(v: str) -> bool:
     if is_domain(v) or is_ip_address(v) or is_email(v) or is_url(v):
         return True
 
     return False
@@ -81,23 +75,54 @@
     if is_email(value):
         value = f"http://{value}"
 
     parsed = urlparse(value)
     return parsed.hostname or value
 
 
+@contextmanager
+def with_socket_timeout(timeout: float):
+    old = socket.getdefaulttimeout()
+    try:
+        socket.setdefaulttimeout(timeout)
+        yield
+    except (socket.timeout, ValueError):
+        raise asyncio.TimeoutError(
+            f"{timeout} seconds have passed but there is no response"
+        )
+    finally:
+        socket.setdefaulttimeout(old)
+
+
+@cached(
+    cache=TTLCache(
+        maxsize=settings.IP_ADDRESS_LOOKUP_CACHE_SIZE,
+        ttl=settings.IP_ADDRESS_LOOKUP_CACHE_TTL,
+    )
+)
+def _resolve(
+    hostname: str, *, timeout: float = float(settings.IP_ADDRESS_LOOKUP_TIMEOUT)
+) -> str:
+    with with_socket_timeout(timeout):
+        ip = socket.gethostbyname(hostname)
+        return ip
+
+
+resolve = asyncify(_resolve)
+
+
 def load_yaml(path: str | pathlib.Path) -> dict:
     with open(path) as f:
         return cast(dict, yaml.safe_load(f))
 
 
 def glob_rules(
     base_directory: str | pathlib.Path,
     *,
-    additional_directories: list[str | pathlib.Path],
+    additional_directories: list[str] | list[pathlib.Path] | CommaSeparatedStrings,
     rule_extensions=settings.RULE_EXTENSIONS,
 ) -> list[pathlib.Path]:
     directories = [base_directory]
     directories.extend(additional_directories)
 
     directories = [pathlib.Path(d) for d in directories]
```

### Comparing `abuse_whois-0.6.0/abuse_whois/whois.py` & `abuse_whois-0.7.0/abuse_whois/whois.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,44 @@
 import asyncio
-import functools
-import shlex
-import warnings
+from dataclasses import asdict
 
+import stamina
 from asyncache import cached
+from asyncwhois.query import DomainQuery, NumberQuery
 from cachetools import TTLCache
 from whois_parser import WhoisParser
 
 from . import schemas, settings
-from .errors import TimeoutError
-from .utils import get_registered_domain, is_ip_address
-
-# Ignore dateparser warnings regarding pytz
-# ref. https://github.com/scrapinghub/dateparser/issues/1013
-warnings.filterwarnings(
-    "ignore",
-    message="The localize method is no longer necessary, as this time zone supports the fold attribute",
-)
+from .utils import get_registered_domain, is_domain, is_ip_address
 
+whois_parser = WhoisParser()
 
-@functools.lru_cache(maxsize=1)
-def get_whois_parser() -> WhoisParser:
-    return WhoisParser()
 
-
-def parse(raw_text: str, hostname: str) -> schemas.WhoisRecord:
-    parser = get_whois_parser()
+def parse(
+    raw_text: str, hostname: str, *, parser: WhoisParser = whois_parser
+) -> schemas.WhoisRecord:
     record = parser.parse(raw_text, hostname=hostname)
+    return schemas.WhoisRecord.model_validate(asdict(record))
 
-    return schemas.WhoisRecord.parse_obj(record.to_dict())
 
+async def query(address: str, *, timeout: int = settings.WHOIS_LOOKUP_TIMEOUT) -> str:
+    klass = DomainQuery if is_domain(address) else NumberQuery
+    query = await klass.new_aio(address, timeout=timeout)
+    return query.query_output
 
+
+@stamina.retry(on=asyncio.TimeoutError, attempts=settings.WHOIS_LOOKUP_MAX_RETRIES)
 @cached(
     cache=TTLCache(
         maxsize=settings.WHOIS_LOOKUP_CACHE_SIZE, ttl=settings.WHOIS_LOOKUP_CACHE_TTL
     )
 )
 async def get_whois_record(
     hostname: str, *, timeout: int = settings.WHOIS_LOOKUP_TIMEOUT
 ) -> schemas.WhoisRecord:
     if not is_ip_address(hostname):
         hostname = get_registered_domain(hostname) or hostname
 
-    # open a new process for "whois" command
-    cmd = f"whois {shlex.quote(hostname)}"
-    proc = await asyncio.create_subprocess_shell(
-        cmd,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
-
-    try:
-        # block for query_result
-        query_result_, _ = await asyncio.wait_for(proc.communicate(), timeout=timeout)
-        query_result = query_result_.decode(errors="ignore")
-        query_result = query_result.strip()
-    except asyncio.TimeoutError:
-        raise TimeoutError(f"{timeout} seconds have passed but there is no response")
+    query_result = await query(hostname, timeout=timeout)
+    query_result = "\n".join(query_result.splitlines())
 
     return parse(query_result, hostname)
```

### Comparing `abuse_whois-0.6.0/pyproject.toml` & `abuse_whois-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 [tool.poetry]
 name = "abuse_whois"
-version = "0.6.0"
+version = "0.7.0"
 description = "Find where to report a domain for abuse"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/ninoseki/abuse_whois"
 repository = "https://github.com/ninoseki/abuse_whois"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiometer = "^0.4.0"
-asyncache = "^0.3.1"
-asyncer = "^0.0.2"
-azuma = "0.1.0"
-cachetools = "^5.3.0"
-email-validator = "^1.3.1"
-fastapi = "^0.92.0"
-gunicorn = { version = "^20.1.0", optional = true }
-loguru = "^0.6.0"
-pydantic = "^1.10.4"
-pyhumps = "^3.8.0"
+asyncache = "^0.3"
+asyncer = "^0.0"
+asyncwhois = "^1.0"
+azuma = "^0.2"
+cachetools = "^5.3"
+fastapi = "^0.100.0"
+gunicorn = { version = "^20.1", optional = true }
+loguru = "^0.7"
+pydantic = "^2.0"
+pyhumps = "^3.8"
 PyYAML = "^6.0"
-tldextract = "^3.4.0"
-typer = "^0.7.0"
-uvicorn = { extras = ["standard"], version = "^0.20.0", optional = true }
-whois-parser = "^0.1.4"
+stamina = "^23.1"
+tldextract = "^3.4"
+typer = "^0.9"
+uvicorn = { extras = ["standard"], version = "^0.22", optional = true }
+validators = "^0.20"
+whois-parser = "^0.2"
 
-[tool.poetry.dev-dependencies]
-autoflake = "^2.0"
+[tool.poetry.group.dev.dependencies]
+autoflake = "^2.2"
 autopep8 = "^2.0"
-black = "^23.1"
+black = "^23.3"
 coveralls = "^3.3"
 isort = "^5.12"
-mypy = "^1.0"
-pre-commit = "^3.1"
-pytest = "^7.2"
-pytest-asyncio = "^0.20"
-pytest-cov = "^4.0"
-pytest-mock = "^3.10"
+mypy = "^1.4"
+pre-commit = "^3.3"
+pytest = "^7.4"
+pytest-asyncio = "^0.21"
+pytest-cov = "^4.1"
+pytest-mock = "^3.11"
 pytest-randomly = "^3.12"
 pytest-sugar = "^0.9"
-pyupgrade = "^3.3"
+pyupgrade = "^3.8"
+urllib3 = "1.26.16"
 
 [tool.poetry.extras]
 api = ["uvicorn", "gunicorn"]
 
 [tool.poetry.scripts]
-abuse_whois = "abuse_whois.cli:app"
+abuse_whois = "abuse_whois.main:app"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `abuse_whois-0.6.0/setup.py` & `abuse_whois-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,129 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: abuse-whois
+Version: 0.7.0
+Summary: Find where to report a domain for abuse
+Home-page: https://github.com/ninoseki/abuse_whois
+License: MIT
+Author: Manabu Niseki
+Author-email: manabu.niseki@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: api
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: asyncache (>=0.3,<0.4)
+Requires-Dist: asyncer (>=0.0,<0.1)
+Requires-Dist: asyncwhois (>=1.0,<2.0)
+Requires-Dist: azuma (>=0.2,<0.3)
+Requires-Dist: cachetools (>=5.3,<6.0)
+Requires-Dist: fastapi (>=0.100.0,<0.101.0)
+Requires-Dist: gunicorn (>=20.1,<21.0) ; extra == "api"
+Requires-Dist: loguru (>=0.7,<0.8)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pyhumps (>=3.8,<4.0)
+Requires-Dist: stamina (>=23.1,<24.0)
+Requires-Dist: tldextract (>=3.4,<4.0)
+Requires-Dist: typer (>=0.9,<0.10)
+Requires-Dist: uvicorn[standard] (>=0.22,<0.23) ; extra == "api"
+Requires-Dist: validators (>=0.20,<0.21)
+Requires-Dist: whois-parser (>=0.2,<0.3)
+Project-URL: Repository, https://github.com/ninoseki/abuse_whois
+Description-Content-Type: text/markdown
+
+# abuse_whois
+
+[![PyPI version](https://badge.fury.io/py/abuse-whois.svg)](https://badge.fury.io/py/abuse-whois)
+[![Python CI](https://github.com/ninoseki/abuse_whois/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/abuse_whois/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/ninoseki/abuse_whois/badge.svg?branch=main)](https://coveralls.io/github/ninoseki/abuse_whois?branch=main)
+
+Yet another way to find where to report an abuse.
+
+![img](./images/overview.jpg)
+
+This tool is highly inspired from the following libraries:
+
+- https://github.com/bradleyjkemp/abwhose
+- https://github.com/certsocietegenerale/abuse_finder
+
+## Requirements
+
+- Python 3.10+
+
+## Installation
+
+```bash
+pip install abuse_whois
+
+# or if you want to use built-in REST API
+pip install abuse_whois[api]
+```
+
+## Usage
+
+### As a library
+
+```python
+from abuse_whois import get_abuse_contacts
+
+await get_abuse_contacts("1.1.1.1")
+await get_abuse_contacts("github.com")
+await get_abuse_contacts("https://github.com")
+await get_abuse_contacts("foo@example.com")
+```
+
+### As a CLI tool
+
+```bash
+$ abuse_whois 1.1.1.1 | jq .
+```
+
+### As a REST API
+
+```bash
+$ uvicorn abuse_whois.api.main:app
+INFO:     Started server process [2283]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+
+$ http localhost:8000/api/whois/ address=https://github.com
+```
+
+### With Docker
+
+```bash
+git clone https://github.com/ninoseki/abuse_whois
+cd abuse_whois
+docker build . -t abuse-whois
+docker run -i -d -p 8000:8000 abuse-whois
+```
+
+## Settings
+
+All settings can be done via environment variables or `.env` file.
+
+| Name                                       | Type                  | Default  | Desc.                                                    |
+| ------------------------------------------ | --------------------- | -------- | -------------------------------------------------------- |
+| WHOIS_LOOKUP_TIMEOUT                       | int                   | 10       | Timeout value for whois lookup (seconds)                 |
+| WHOIS_LOOKUP_CACHE_SIZE                    | int                   | 1024     | Cache size for whois lookup                              |
+| WHOIS_LOOKUP_CACHE_TTL                     | int                   | 3600     | Cache TTL value for whois lookup (seconds)               |
+| WHOIS_LOOKUP_MAX_RETRIES                   | int                   | 3        | Max retries on timeout error                             |
+| IP_ADDRESS_LOOKUP_TIMEOUT                  | int                   | 10       | Timeout value for IP address lookup (seconds)            |
+| IP_ADDRESS_LOOKUP_CACHE_SIZE               | int                   | 1024     | Cache size for IP address lookup                         |
+| IP_ADDRESS_LOOKUP_CACHE_TTL                | int                   | 3600     | Cache TTL value for IP address lookup (seconds)          |
+| RULE_EXTENSIONS                            | CommaSeparatedStrings | yaml,yml | Rule file extensions                                     |
+| ADDITIONAL_WHOIS_RULE_DIRECTORIES          | CommaSeparatedStrings |          | Additional directories contain whois rule files          |
+| ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES | CommaSeparatedStrings |          | Additional directories contain shared hosting rule files |
+
+## Contributions
+
+`abuse_whois` works based on a combination of static rules and a parsing result of whois response.
+
+- Rules:
+  - [Registrar and hosting provider](https://github.com/ninoseki/abuse_whois/wiki/Registrar-and-Hosting-Provider)
+  - [Shared hosting provider](https://github.com/ninoseki/abuse_whois/wiki/Shared-Hosting)
 
-packages = \
-['abuse_whois',
- 'abuse_whois.api',
- 'abuse_whois.api.endpoints',
- 'abuse_whois.matchers',
- 'abuse_whois.matchers.shared_hosting',
- 'abuse_whois.matchers.whois',
- 'abuse_whois.schemas']
-
-package_data = \
-{'': ['*'],
- 'abuse_whois.matchers.shared_hosting': ['rules/*'],
- 'abuse_whois.matchers.whois': ['rules/*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'aiometer>=0.4.0,<0.5.0',
- 'asyncache>=0.3.1,<0.4.0',
- 'asyncer>=0.0.2,<0.0.3',
- 'azuma==0.1.0',
- 'cachetools>=5.3.0,<6.0.0',
- 'email-validator>=1.3.1,<2.0.0',
- 'fastapi>=0.92.0,<0.93.0',
- 'loguru>=0.6.0,<0.7.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'pyhumps>=3.8.0,<4.0.0',
- 'tldextract>=3.4.0,<4.0.0',
- 'typer>=0.7.0,<0.8.0',
- 'whois-parser>=0.1.4,<0.2.0']
-
-extras_require = \
-{'api': ['gunicorn>=20.1.0,<21.0.0', 'uvicorn[standard]>=0.20.0,<0.21.0']}
-
-entry_points = \
-{'console_scripts': ['abuse_whois = abuse_whois.cli:app']}
-
-setup_kwargs = {
-    'name': 'abuse-whois',
-    'version': '0.6.0',
-    'description': 'Find where to report a domain for abuse',
-    'long_description': '# abuse_whois\n\n[![PyPI version](https://badge.fury.io/py/abuse-whois.svg)](https://badge.fury.io/py/abuse-whois)\n[![Python CI](https://github.com/ninoseki/abuse_whois/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/abuse_whois/actions/workflows/test.yml)\n[![Coverage Status](https://coveralls.io/repos/github/ninoseki/abuse_whois/badge.svg?branch=main)](https://coveralls.io/github/ninoseki/abuse_whois?branch=main)\n\nYet another way to find where to report an abuse.\n\n![img](./images/overview.jpg)\n\nThis tool is highly inspired from the following libraries:\n\n- https://github.com/bradleyjkemp/abwhose\n- https://github.com/certsocietegenerale/abuse_finder\n\n## Requirements\n\n- Python 3.10+\n- whois\n\n## Installation\n\n```bash\npip install abuse_whois\n\n# or if you want to use built-in REST API\npip install abuse_whois[api]\n```\n\n## Usage\n\n### As a library\n\n```python\nfrom abuse_whois import get_abuse_contacts\n\nget_abuse_contacts("1.1.1.1")\nget_abuse_contacts("github.com")\nget_abuse_contacts("https://github.com")\nget_abuse_contacts("foo@example.com")\n```\n\n### As a CLI tool\n\n```bash\n$ abuse_whois 1.1.1.1 | jq .\n```\n\n### As a REST API\n\n```bash\n$ uvicorn abuse_whois.api.app:app\nINFO:     Started server process [2283]\nINFO:     Waiting for application startup.\nINFO:     Application startup complete.\nINFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)\n\n$ http localhost:8000/api/whois/ address=https://github.com\n```\n\n### With Docker\n\n```bash\ngit clone https://github.com/ninoseki/abuse_whois\ncd abuse_whois\ndocker build . -t abuse-whois\ndocker run -i -d -p 8000:8000 abuse-whois\n```\n\n## Settings\n\nAll settings can be done via environment variables or `.env` file.\n\n| Name                                       | Type                   | Default  | Desc.                                                    |\n| ------------------------------------------ | ---------------------- | -------- | -------------------------------------------------------- |\n| WHOIS_LOOKUP_TIMEOUT                       | int                    | 10       | Timeout value for whois lookup (seconds)                 |\n| WHOIS_LOOKUP_CACHE_SIZE                    | int                    | 1024     | Cache size for whois lookup                              |\n| WHOIS_LOOKUP_CACHE_TTL                     | int                    | 3600     | Cache TTL value for whois lookup (seconds)               |\n| IP_ADDRESS_LOOKUP_TIMEOUT                  | int                    | 10       | Timeout value for IP address lookup (seconds)            |\n| IP_ADDRESS_LOOKUP_CACHE_SIZE               | int                    | 1024     | Cache size for IP address lookup                         |\n| IP_ADDRESS_LOOKUP_CACHE_TTL                | int                    | 3600     | Cache TTL value for IP address lookup (seconds)          |\n| RULE_EXTENSIONS                            | CommaSeparatedStrings  | yaml,yml | Rule file extensions                                     |\n| ADDITIONAL_WHOIS_RULE_DIRECTORIES          | CommaSeparatedStrings] |          | Additional directories contain whois rule files          |\n| ADDITIONAL_SHARED_HOSTING_RULE_DIRECTORIES | CommaSeparatedStrings] |          | Additional directories contain shared hosting rule files |\n\n## Contributions\n\n`abuse_whois` works based on a combination of static rules and a parsing result of whois response.\n\n- Rules:\n  - [Registrar and hosting provider](https://github.com/ninoseki/abuse_whois/wiki/Registrar-and-Hosting-Provider)\n  - [Shared hosting provider](https://github.com/ninoseki/abuse_whois/wiki/Shared-Hosting)\n\nPlease submit a PR (or submit a feature request) if you find something missing.\n',
-    'author': 'Manabu Niseki',
-    'author_email': 'manabu.niseki@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ninoseki/abuse_whois',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+Please submit a PR (or submit a feature request) if you find something missing.
 
-
-setup(**setup_kwargs)
```

