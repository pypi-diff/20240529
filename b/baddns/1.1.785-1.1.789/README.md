# Comparing `tmp/baddns-1.1.785.tar.gz` & `tmp/baddns-1.1.789.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baddns-1.1.785.tar", max compression
+gzip compressed data, was "baddns-1.1.789.tar", max compression
```

## Comparing `baddns-1.1.785.tar` & `baddns-1.1.789.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0    35149 2024-05-15 19:18:06.124731 baddns-1.1.785/LICENSE
--rw-r--r--   0        0        0     3720 2024-05-15 19:18:06.124731 baddns-1.1.785/README.md
--rw-r--r--   0        0        0      687 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/__init__.py
--rw-r--r--   0        0        0      918 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/base.py
--rw-r--r--   0        0        0     6304 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/cli.py
--rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/__init__.py
--rw-r--r--   0        0        0     5383 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/dnsmanager.py
--rw-r--r--   0        0        0     8060 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/dnswalk.py
--rw-r--r--   0        0        0      273 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/errors.py
--rw-r--r--   0        0        0     2481 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/findings.py
--rw-r--r--   0        0        0     1886 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/httpmanager.py
--rw-r--r--   0        0        0     1449 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/loader.py
--rw-r--r--   0        0        0     1117 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/logging.py
--rw-r--r--   0        0        0     3362 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/matcher.py
--rw-r--r--   0        0        0     3286 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/signature.py
--rw-r--r--   0        0        0     4100 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/whoismanager.py
--rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/__init__.py
--rw-r--r--   0        0        0     9404 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/cname.py
--rw-r--r--   0        0        0     2129 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/mx.py
--rw-r--r--   0        0        0     4545 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/ns.py
--rw-r--r--   0        0        0     3236 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/nsec.py
--rw-r--r--   0        0        0     6201 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/references.py
--rw-r--r--   0        0        0     4599 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/txt.py
--rw-r--r--   0        0        0     4121 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/zonetransfer.py
--rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/scripts/__init__.py
--rwxr-xr-x   0        0        0    12978 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/scripts/readsources.py
--rwxr-xr-x   0        0        0     4540 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/scripts/signaturetest.py
--rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/.gitignore
--rw-r--r--   0        0        0      341 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/baddns_aws-bucket-website.yml
--rw-r--r--   0        0        0      246 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_000domains.yml
--rw-r--r--   0        0        0      248 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_agilecrm.yml
--rw-r--r--   0        0        0      158 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_aws_ns.yml
--rw-r--r--   0        0        0      242 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_bizland.yml
--rw-r--r--   0        0        0      328 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_brandpad.yml
--rw-r--r--   0        0        0      382 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_brightcove.yml
--rw-r--r--   0        0        0      349 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_campaign_monitor.yml
--rw-r--r--   0        0        0      366 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_cargo_collective.yml
--rw-r--r--   0        0        0      327 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_convertkit.yml
--rw-r--r--   0        0        0      227 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_digitalocean.yml
--rw-r--r--   0        0        0      167 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_dnsmadeeasy.yml
--rw-r--r--   0        0        0      232 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_dnssimple.yml
--rw-r--r--   0        0        0      184 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_domain.yml
--rw-r--r--   0        0        0      239 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_dotster.yml
--rw-r--r--   0        0        0     1331 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_elastic_beanstalk.yml
--rw-r--r--   0        0        0      307 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_frontify.yml
--rw-r--r--   0        0        0      297 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_getresponse.yml
--rw-r--r--   0        0        0      475 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_github_pages.yml
--rw-r--r--   0        0        0      170 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_googlecloud.yml
--rw-r--r--   0        0        0      306 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_hatenablog.yml
--rw-r--r--   0        0        0      300 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_helpscout.yml
--rw-r--r--   0        0        0      193 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_hostinger.yml
--rw-r--r--   0        0        0      217 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_hurricane_electric.yml
--rw-r--r--   0        0        0      309 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_jetbrains.yml
--rw-r--r--   0        0        0      248 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_launchrock_cname.yml
--rw-r--r--   0        0        0      184 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_linode.yml
--rw-r--r--   0        0        0      298 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_mashery.yml
--rw-r--r--   0        0        0      199 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_mediatemplate.yml
--rw-r--r--   0        0        0      319 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_mysmartjobboard.yml
--rw-r--r--   0        0        0      158 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_name.yml
--rw-r--r--   0        0        0      300 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_netlify.yml
--rw-r--r--   0        0        0      401 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_ngrok.yml
--rw-r--r--   0        0        0      158 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_nsone.yml
--rw-r--r--   0        0        0      172 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_reg.yml
--rw-r--r--   0        0        0      303 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_shopify.yml
--rw-r--r--   0        0        0      352 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_simplebooklet.yml
--rw-r--r--   0        0        0      330 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_smartjobboard.yml
--rw-r--r--   0        0        0      290 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_surge.yml
--rw-r--r--   0        0        0      315 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_surveysparrow.yml
--rw-r--r--   0        0        0      323 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_teamwork.yml
--rw-r--r--   0        0        0      344 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_thinkific.yml
--rw-r--r--   0        0        0      200 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_tierranet.yml
--rw-r--r--   0        0        0      351 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_tribe.yml
--rw-r--r--   0        0        0      298 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_tumblr.yml
--rw-r--r--   0        0        0      338 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_vendhq.yml
--rw-r--r--   0        0        0      353 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_webflow.yml
--rw-r--r--   0        0        0      323 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_wishpond.yml
--rw-r--r--   0        0        0      306 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_wordpress_com_cname.yml
--rw-r--r--   0        0        0      215 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_wordpress_com_ns.yml
--rw-r--r--   0        0        0      359 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_zohoforms.yml
--rw-r--r--   0        0        0      324 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_zohoforms_in.yml
--rw-r--r--   0        0        0      411 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_aftership-takeover.yml
--rw-r--r--   0        0        0      347 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_agilecrm-takeover.yml
--rw-r--r--   0        0        0      366 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_aha-takeover.yml
--rw-r--r--   0        0        0      511 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_airee-takeover.yml
--rw-r--r--   0        0        0      382 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_anima-takeover.yml
--rw-r--r--   0        0        0      366 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_announcekit-takeover.yml
--rw-r--r--   0        0        0      479 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_aws-bucket-takeover.yml
--rw-r--r--   0        0        0     1022 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_azure-takeover-detection.yml
--rw-r--r--   0        0        0      456 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_bigcartel-takeover.yml
--rw-r--r--   0        0        0      407 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_bitbucket-takeover.yml
--rw-r--r--   0        0        0      406 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_campaignmonitor-takeover.yml
--rw-r--r--   0        0        0      382 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_canny-takeover.yml
--rw-r--r--   0        0        0      415 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_clever-takeover.yml
--rw-r--r--   0        0        0      374 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_flexbe-takeover.yml
--rw-r--r--   0        0        0      529 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_flywheel-takeover.yml
--rw-r--r--   0        0        0      343 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_gemfury-takeover.yml
--rw-r--r--   0        0        0      356 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_ghost-takeover.yml
--rw-r--r--   0        0        0      368 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_gitbook-takeover.yml
--rw-r--r--   0        0        0      430 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_gohire-takeover.yml
--rw-r--r--   0        0        0      365 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_helpdocs-takeover.yml
--rw-r--r--   0        0        0      387 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_helpjuice-takeover.yml
--rw-r--r--   0        0        0      394 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_helprace-takeover.yml
--rw-r--r--   0        0        0      487 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_heroku-takeover.yml
--rw-r--r--   0        0        0      357 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_hubspot-takeover.yml
--rw-r--r--   0        0        0      422 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_intercom-takeover.yml
--rw-r--r--   0        0        0      410 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_launchrock-takeover.yml
--rw-r--r--   0        0        0      482 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_leadpages-takeover.yml
--rw-r--r--   0        0        0      359 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_lemlist-takeover.yml
--rw-r--r--   0        0        0      320 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_meteor-takeover.yml
--rw-r--r--   0        0        0      379 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_pagewiz-takeover.yml
--rw-r--r--   0        0        0      346 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_pantheon-takeover.yml
--rw-r--r--   0        0        0      398 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_pingdom-takeover.yml
--rw-r--r--   0        0        0      394 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_proposify-takeover.yml
--rw-r--r--   0        0        0      336 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_readme-takeover.yml
--rw-r--r--   0        0        0      336 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_readthedocs-takeover.yml
--rw-r--r--   0        0        0      788 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_shopify-takeover.yml
--rw-r--r--   0        0        0      365 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_simplebooklet-takeover.yml
--rw-r--r--   0        0        0      332 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_smugmug-takeover.yml
--rw-r--r--   0        0        0      424 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_softr-takeover.yml
--rw-r--r--   0        0        0      623 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_sprintful-takeover.yml
--rw-r--r--   0        0        0      462 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_squadcast-takeover.yml
--rw-r--r--   0        0        0      394 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_strikingly-takeover.yml
--rw-r--r--   0        0        0      508 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_tilda-takeover.yml
--rw-r--r--   0        0        0      370 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_uberflip-takeover.yml
--rw-r--r--   0        0        0      434 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_uptime-takeover.yml
--rw-r--r--   0        0        0      356 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_uservoice-takeover.yml
--rw-r--r--   0        0        0      354 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_vend-takeover.yml
--rw-r--r--   0        0        0      348 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_vercel-takeover.yml
--rw-r--r--   0        0        0      423 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_wishpond-takeover.yml
--rw-r--r--   0        0        0      390 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_wix-takeover.yml
--rw-r--r--   0        0        0      359 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_wufoo-takeover.yml
--rw-r--r--   0        0        0      363 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_zendesk-takeover.yml
--rw-r--r--   0        0        0    10568 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/signature_history.txt
--rw-r--r--   0        0        0     1436 2024-05-15 19:18:21.532751 baddns-1.1.785/pyproject.toml
--rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 baddns-1.1.785/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-29 04:51:19.507277 baddns-1.1.789/LICENSE
+-rw-r--r--   0        0        0     3720 2024-05-29 04:51:19.507277 baddns-1.1.789/README.md
+-rw-r--r--   0        0        0      687 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/__init__.py
+-rw-r--r--   0        0        0      918 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/base.py
+-rw-r--r--   0        0        0     6304 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/cli.py
+-rw-r--r--   0        0        0        0 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/__init__.py
+-rw-r--r--   0        0        0     5383 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/dnsmanager.py
+-rw-r--r--   0        0        0     8060 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/dnswalk.py
+-rw-r--r--   0        0        0      273 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/errors.py
+-rw-r--r--   0        0        0     2481 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/findings.py
+-rw-r--r--   0        0        0     1886 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/httpmanager.py
+-rw-r--r--   0        0        0     1449 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/loader.py
+-rw-r--r--   0        0        0     1117 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/logging.py
+-rw-r--r--   0        0        0     3362 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/matcher.py
+-rw-r--r--   0        0        0     3286 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/signature.py
+-rw-r--r--   0        0        0     3919 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/lib/whoismanager.py
+-rw-r--r--   0        0        0        0 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/__init__.py
+-rw-r--r--   0        0        0     9404 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/cname.py
+-rw-r--r--   0        0        0     2129 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/mx.py
+-rw-r--r--   0        0        0     4545 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/ns.py
+-rw-r--r--   0        0        0     3236 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/nsec.py
+-rw-r--r--   0        0        0     6201 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/references.py
+-rw-r--r--   0        0        0     4599 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/txt.py
+-rw-r--r--   0        0        0     4121 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/modules/zonetransfer.py
+-rw-r--r--   0        0        0        0 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/scripts/__init__.py
+-rwxr-xr-x   0        0        0    12978 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/scripts/readsources.py
+-rwxr-xr-x   0        0        0     4540 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/scripts/signaturetest.py
+-rw-r--r--   0        0        0        0 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/.gitignore
+-rw-r--r--   0        0        0      341 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/baddns_aws-bucket-website.yml
+-rw-r--r--   0        0        0      246 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_000domains.yml
+-rw-r--r--   0        0        0      248 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_agilecrm.yml
+-rw-r--r--   0        0        0      158 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_aws_ns.yml
+-rw-r--r--   0        0        0      242 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_bizland.yml
+-rw-r--r--   0        0        0      328 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_brandpad.yml
+-rw-r--r--   0        0        0      382 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_brightcove.yml
+-rw-r--r--   0        0        0      349 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_campaign_monitor.yml
+-rw-r--r--   0        0        0      366 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_cargo_collective.yml
+-rw-r--r--   0        0        0      327 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_convertkit.yml
+-rw-r--r--   0        0        0      227 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_digitalocean.yml
+-rw-r--r--   0        0        0      167 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_dnsmadeeasy.yml
+-rw-r--r--   0        0        0      232 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_dnssimple.yml
+-rw-r--r--   0        0        0      184 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_domain.yml
+-rw-r--r--   0        0        0      239 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_dotster.yml
+-rw-r--r--   0        0        0     1331 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_elastic_beanstalk.yml
+-rw-r--r--   0        0        0      307 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_frontify.yml
+-rw-r--r--   0        0        0      297 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_getresponse.yml
+-rw-r--r--   0        0        0      475 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_github_pages.yml
+-rw-r--r--   0        0        0      170 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_googlecloud.yml
+-rw-r--r--   0        0        0      306 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_hatenablog.yml
+-rw-r--r--   0        0        0      300 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_helpscout.yml
+-rw-r--r--   0        0        0      193 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_hostinger.yml
+-rw-r--r--   0        0        0      217 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_hurricane_electric.yml
+-rw-r--r--   0        0        0      309 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_jetbrains.yml
+-rw-r--r--   0        0        0      248 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_launchrock_cname.yml
+-rw-r--r--   0        0        0      184 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_linode.yml
+-rw-r--r--   0        0        0      298 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_mashery.yml
+-rw-r--r--   0        0        0      199 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_mediatemplate.yml
+-rw-r--r--   0        0        0      319 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_mysmartjobboard.yml
+-rw-r--r--   0        0        0      158 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_name.yml
+-rw-r--r--   0        0        0      300 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_netlify.yml
+-rw-r--r--   0        0        0      401 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_ngrok.yml
+-rw-r--r--   0        0        0      158 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_nsone.yml
+-rw-r--r--   0        0        0      172 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_reg.yml
+-rw-r--r--   0        0        0      303 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_shopify.yml
+-rw-r--r--   0        0        0      352 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_simplebooklet.yml
+-rw-r--r--   0        0        0      330 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_smartjobboard.yml
+-rw-r--r--   0        0        0      290 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_surge.yml
+-rw-r--r--   0        0        0      315 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_surveysparrow.yml
+-rw-r--r--   0        0        0      323 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_teamwork.yml
+-rw-r--r--   0        0        0      344 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_thinkific.yml
+-rw-r--r--   0        0        0      200 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_tierranet.yml
+-rw-r--r--   0        0        0      351 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_tribe.yml
+-rw-r--r--   0        0        0      298 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_tumblr.yml
+-rw-r--r--   0        0        0      338 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_vendhq.yml
+-rw-r--r--   0        0        0      353 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_webflow.yml
+-rw-r--r--   0        0        0      323 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_wishpond.yml
+-rw-r--r--   0        0        0      306 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_wordpress_com_cname.yml
+-rw-r--r--   0        0        0      215 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_wordpress_com_ns.yml
+-rw-r--r--   0        0        0      359 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_zohoforms.yml
+-rw-r--r--   0        0        0      324 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/dnsreaper_zohoforms_in.yml
+-rw-r--r--   0        0        0      411 2024-05-29 04:51:19.507277 baddns-1.1.789/baddns/signatures/nucleitemplates_aftership-takeover.yml
+-rw-r--r--   0        0        0      347 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_agilecrm-takeover.yml
+-rw-r--r--   0        0        0      366 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_aha-takeover.yml
+-rw-r--r--   0        0        0      511 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_airee-takeover.yml
+-rw-r--r--   0        0        0      382 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_anima-takeover.yml
+-rw-r--r--   0        0        0      366 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_announcekit-takeover.yml
+-rw-r--r--   0        0        0      479 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_aws-bucket-takeover.yml
+-rw-r--r--   0        0        0     1022 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_azure-takeover-detection.yml
+-rw-r--r--   0        0        0      456 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_bigcartel-takeover.yml
+-rw-r--r--   0        0        0      407 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_bitbucket-takeover.yml
+-rw-r--r--   0        0        0      406 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_campaignmonitor-takeover.yml
+-rw-r--r--   0        0        0      382 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_canny-takeover.yml
+-rw-r--r--   0        0        0      415 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_clever-takeover.yml
+-rw-r--r--   0        0        0      374 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_flexbe-takeover.yml
+-rw-r--r--   0        0        0      529 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_flywheel-takeover.yml
+-rw-r--r--   0        0        0      343 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_gemfury-takeover.yml
+-rw-r--r--   0        0        0      356 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_ghost-takeover.yml
+-rw-r--r--   0        0        0      368 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_gitbook-takeover.yml
+-rw-r--r--   0        0        0      430 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_gohire-takeover.yml
+-rw-r--r--   0        0        0      365 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_helpdocs-takeover.yml
+-rw-r--r--   0        0        0      387 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_helpjuice-takeover.yml
+-rw-r--r--   0        0        0      394 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_helprace-takeover.yml
+-rw-r--r--   0        0        0      487 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_heroku-takeover.yml
+-rw-r--r--   0        0        0      357 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_hubspot-takeover.yml
+-rw-r--r--   0        0        0      422 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_intercom-takeover.yml
+-rw-r--r--   0        0        0      410 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_launchrock-takeover.yml
+-rw-r--r--   0        0        0      482 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_leadpages-takeover.yml
+-rw-r--r--   0        0        0      359 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_lemlist-takeover.yml
+-rw-r--r--   0        0        0      320 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_meteor-takeover.yml
+-rw-r--r--   0        0        0      379 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_pagewiz-takeover.yml
+-rw-r--r--   0        0        0      346 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_pantheon-takeover.yml
+-rw-r--r--   0        0        0      398 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_pingdom-takeover.yml
+-rw-r--r--   0        0        0      394 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_proposify-takeover.yml
+-rw-r--r--   0        0        0      336 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_readme-takeover.yml
+-rw-r--r--   0        0        0      336 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_readthedocs-takeover.yml
+-rw-r--r--   0        0        0      788 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_shopify-takeover.yml
+-rw-r--r--   0        0        0      365 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_simplebooklet-takeover.yml
+-rw-r--r--   0        0        0      332 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_smugmug-takeover.yml
+-rw-r--r--   0        0        0      424 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_softr-takeover.yml
+-rw-r--r--   0        0        0      623 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_sprintful-takeover.yml
+-rw-r--r--   0        0        0      462 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_squadcast-takeover.yml
+-rw-r--r--   0        0        0      394 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_strikingly-takeover.yml
+-rw-r--r--   0        0        0      508 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_tilda-takeover.yml
+-rw-r--r--   0        0        0      370 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_uberflip-takeover.yml
+-rw-r--r--   0        0        0      434 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_uptime-takeover.yml
+-rw-r--r--   0        0        0      356 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_uservoice-takeover.yml
+-rw-r--r--   0        0        0      354 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_vend-takeover.yml
+-rw-r--r--   0        0        0      348 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_vercel-takeover.yml
+-rw-r--r--   0        0        0      423 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_wishpond-takeover.yml
+-rw-r--r--   0        0        0      390 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_wix-takeover.yml
+-rw-r--r--   0        0        0      359 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_wufoo-takeover.yml
+-rw-r--r--   0        0        0      363 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/nucleitemplates_zendesk-takeover.yml
+-rw-r--r--   0        0        0    10568 2024-05-29 04:51:19.511277 baddns-1.1.789/baddns/signatures/signature_history.txt
+-rw-r--r--   0        0        0     1436 2024-05-29 04:51:36.135300 baddns-1.1.789/pyproject.toml
+-rw-r--r--   0        0        0     4866 1970-01-01 00:00:00.000000 baddns-1.1.789/PKG-INFO
```

### Comparing `baddns-1.1.785/LICENSE` & `baddns-1.1.789/LICENSE`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/README.md` & `baddns-1.1.789/README.md`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/__init__.py` & `baddns-1.1.789/baddns/__init__.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/base.py` & `baddns-1.1.789/baddns/base.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/cli.py` & `baddns-1.1.789/baddns/cli.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/dnsmanager.py` & `baddns-1.1.789/baddns/lib/dnsmanager.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/dnswalk.py` & `baddns-1.1.789/baddns/lib/dnswalk.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/findings.py` & `baddns-1.1.789/baddns/lib/findings.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/httpmanager.py` & `baddns-1.1.789/baddns/lib/httpmanager.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/loader.py` & `baddns-1.1.789/baddns/lib/loader.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/logging.py` & `baddns-1.1.789/baddns/lib/logging.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/matcher.py` & `baddns-1.1.789/baddns/lib/matcher.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/signature.py` & `baddns-1.1.789/baddns/lib/signature.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/lib/whoismanager.py` & `baddns-1.1.789/baddns/lib/whoismanager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,28 @@
-import sys
-
-
-# Temporary workaround for: https://github.com/blacklanternsecurity/baddns/issues/402
-class noop:
-    def __getattr__(self, item):
-        def method(*args, **kwargs):
-            pass  # Method does nothing
-
-        return method
-
-
-sys.modules["imp"] = noop()
-
-import os
-from contextlib import contextmanager
-
-
-# Another temporary workaround until https://github.com/richardpenman/whois gets updated version pushed to pypi :( :( :(
-@contextmanager
-def suppress_stdout():
-    original_stdout = sys.stdout
-    sys.stdout = open(os.devnull, "w")
-    try:
-        yield
-    finally:
-        sys.stdout = original_stdout
-
-
 import whois
 import logging
 import asyncio
 import tldextract
-from datetime import date, datetime, timedelta
+from datetime import datetime, timezone, timedelta, date
 from dateutil import parser as date_parser
 
-
 log = logging.getLogger(__name__)
 
 
 class WhoisManager:
     def __init__(self, target):
         self.target = target
         self.whois_result = None
 
     async def dispatchWHOIS(self):
         ext = tldextract.extract(self.target)
         log.debug(f"Extracted base domain [{ext.registered_domain}] from [{self.target}]")
         log.debug(f"Submitting WHOIS query for {ext.registered_domain}")
         try:
-            with suppress_stdout():
-                w = await asyncio.to_thread(whois.whois, ext.registered_domain)
+            w = await asyncio.to_thread(whois.whois, ext.registered_domain)
             log.debug(f"Got response to whois request for {ext.registered_domain}")
             self.whois_result = {"type": "response", "data": w}
         except whois.parser.PywhoisError as e:
             log.debug(f"Got PywhoisError for whois request for {ext.registered_domain}")
             self.whois_result = {"type": "error", "data": str(e)}
 
     def analyzeWHOIS(self):
@@ -68,19 +37,25 @@
                 log.debug("whois resulted in a response")
                 expiration_data = self.whois_result.get("data", {}).get("expiration_date", None)
 
                 if isinstance(expiration_data, list):
                     log.debug("Expiration data:")
                     log.debug(expiration_data)
                     log.debug("Got multiple expiration dates. Falling back to the latest...")
-                    expiration_date = max(expiration_data)
+
+                    normalized_dates = [
+                        self.normalize_date(self.date_parse(date)) for date in expiration_data if self.date_parse(date)
+                    ]
+                    expiration_date = max(normalized_dates) if normalized_dates else None
+
                 else:
-                    expiration_date = expiration_data
+                    expiration_date = self.date_parse(expiration_data)
+                    if expiration_date:
+                        expiration_date = self.normalize_date(expiration_date)
 
-                expiration_date = self.date_parse(expiration_date)
                 if expiration_date:
                     current_date = date.today()
                     expiration_plus_one = expiration_date.date() + timedelta(days=1)
                     if expiration_plus_one < current_date:
                         log.debug(
                             f"Current Date (minus one) ({current_date.strftime('%Y-%m-%d')}) is after Expiration Date ({expiration_date.date().strftime('%Y-%m-%d')})"
                         )
@@ -105,7 +80,14 @@
                 return date_parser.parse(unknown_date)
             except ValueError as e:
                 log.debug(f"Failed to parse date from string: {unknown_date}. Error: {e}")
                 return None
 
         log.debug(f"Unsupported date object type: {type(unknown_date)}. Value: {unknown_date}")
         return None
+
+    @staticmethod
+    def normalize_date(date):
+        if date.tzinfo is None:
+            return date.replace(tzinfo=timezone.utc)
+        else:
+            return date.astimezone(timezone.utc)
```

### Comparing `baddns-1.1.785/baddns/modules/cname.py` & `baddns-1.1.789/baddns/modules/cname.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/modules/mx.py` & `baddns-1.1.789/baddns/modules/mx.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/modules/ns.py` & `baddns-1.1.789/baddns/modules/ns.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/modules/nsec.py` & `baddns-1.1.789/baddns/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/modules/references.py` & `baddns-1.1.789/baddns/modules/references.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/modules/txt.py` & `baddns-1.1.789/baddns/modules/txt.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/modules/zonetransfer.py` & `baddns-1.1.789/baddns/modules/zonetransfer.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/scripts/readsources.py` & `baddns-1.1.789/baddns/scripts/readsources.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/scripts/signaturetest.py` & `baddns-1.1.789/baddns/scripts/signaturetest.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/signatures/dnsreaper_elastic_beanstalk.yml` & `baddns-1.1.789/baddns/signatures/dnsreaper_elastic_beanstalk.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/signatures/nucleitemplates_azure-takeover-detection.yml` & `baddns-1.1.789/baddns/signatures/nucleitemplates_azure-takeover-detection.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/signatures/nucleitemplates_flywheel-takeover.yml` & `baddns-1.1.789/baddns/signatures/nucleitemplates_flywheel-takeover.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/signatures/nucleitemplates_shopify-takeover.yml` & `baddns-1.1.789/baddns/signatures/nucleitemplates_shopify-takeover.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/signatures/nucleitemplates_sprintful-takeover.yml` & `baddns-1.1.789/baddns/signatures/nucleitemplates_sprintful-takeover.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/baddns/signatures/signature_history.txt` & `baddns-1.1.789/baddns/signatures/signature_history.txt`

 * *Files identical despite different names*

### Comparing `baddns-1.1.785/pyproject.toml` & `baddns-1.1.789/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baddns"
-version = "v1.1.785"
+version = "v1.1.789"
 description = "Check subdomains for subdomain takeovers and other DNS tomfoolery"
 authors = ["liquidsec <paul.mueller08@gmail.com>"]
 repository = "https://github.com/blacklanternsecurity/baddns"
 homepage = "https://github.com/blacklanternsecurity/baddns"
 documentation = "https://www.blacklanternsecurity.com/baddns/"
 license = "GPL-3.0"
 readme = "README.md"
@@ -12,15 +12,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 dnspython = "^2.4.1"
 colorama = "^0.4.6"
 httpx = "^0.26.0"
-python-whois = "^0.8.0"
+python-whois = "^0.9.4"
 tldextract = "^3.4.4"
 python-dateutil = "^2.8.2"
 setuptools = "^69.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-httpx = "^0.28.0"
```

### Comparing `baddns-1.1.785/PKG-INFO` & `baddns-1.1.789/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baddns
-Version: 1.1.785
+Version: 1.1.789
 Summary: Check subdomains for subdomain takeovers and other DNS tomfoolery
 Home-page: https://github.com/blacklanternsecurity/baddns
 License: GPL-3.0
 Author: liquidsec
 Author-email: paul.mueller08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dnspython (>=2.4.1,<3.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-whois (>=0.8.0,<0.9.0)
+Requires-Dist: python-whois (>=0.9.4,<0.10.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: tldextract (>=3.4.4,<4.0.0)
 Project-URL: Documentation, https://www.blacklanternsecurity.com/baddns/
 Project-URL: Repository, https://github.com/blacklanternsecurity/baddns
 Description-Content-Type: text/markdown
```

