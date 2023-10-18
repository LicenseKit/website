---
id: caching
title: License Caching
layout: page
permalink: /licenses/caching

hero: /assets/heros/caching.png

description: LicenseKit lets you combine multiple service types.
---

LicenseKit lets you wrap any license service in a cached service, which will cause it to cache successful license validations and use the last successful validation if a network error occurs.


## How does it work?

A cached license service is just another service, that takes another service as input parameter when you create it. It will then use that services to fetch licenses based on license key.

It will then save the last fetched license for a key, and return that license if the license validation fails due to a network error. Any other errors will clear the cache and cause the validation to fail.