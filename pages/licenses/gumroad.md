---
id: gumroad
title: Gumroad Licenses
layout: page
permalink: /licenses/gumroad

hero: /assets/heros/gumroad.png

description: LicenseKit lets you validate Gumroad licenses.

gumroad: https://gumroad.com
---

Using a Gumroad license service is a great way to validate licenses you've sold at Gumroad.

## How does it work?

LicenseKit has a Gumroad license service that can fetch licenses from the Gumroad validation API. All you have to do to use the service is to provide your product ID and a response mapper.

The response mapper will provide you with a strongly typed response object. You can then map this information in any way you want, to return a LicenseKit-specific license.

The license will then be validated as normal, using the mapped information that you return. 



## Offline mode

If your software needs to work offline, LicenseKit can cache the last successful validation and ignore any network-based errors. Any license-based error, like expiration, will reset the cache.

You can also define if a successful validation is needed before your customers can start using your software. This decision is up to you, and depends on your business model.


## License expiration

To stop a license from working when it expires, you need to get the expiration date from the API response and map it to the local license representation.