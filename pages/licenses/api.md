---
id: cloud
title: API/Cloud-based Licenses
layout: page
permalink: /licenses/api

hero: /assets/heros/api.png

description: LicenseKit lets you validate licenses over the cloud.
---

API-based license validation is a great alternative when you want to validate customer licenses with an external license service, like Gumroad or LemonSqueezy.

## How does it work?

LicenseKit can integrate with any external license service provider and lets you easily map license provider-specific data to LicenseKit licenses.

## Offline mode

If your software needs to work offline, LicenseKit can cache the last successful validation and ignore any network-based errors. Any license-based error, like expiration, will reset the cache.

You can also define if a successful validation is needed before your customers can start using your software. This decision is up to you, and depends on your business model.

## License expiration

To stop a license from working when it expires, you need to get the expiration date from the API response and map it to the local license representation.