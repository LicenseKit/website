---
id: proxying
title: Service Proxying
layout: page
permalink: /licenses/proxying

hero: /assets/heros/proxying.png

description: LicenseKit lets you combine multiple service types.
---

LicenseKit lets you create custom service proxies, which wraps many services to create flexible license validations. LicenseKit will use all services when validating licenses with a proxy. 

## How does it work?

A service proxy is just another service, that takes a list of other services when you create it. It will then use all services when validating a license key.

For instance, say that you have several license files. You can then create one license service per file and combine them in a proxy. LicenseKit will then check all files until it finds a match, if any.

Another example of when service proxying can help, is if you prefer to use binary licenses, but also want users to be able to use their license key right away without having to distribute a new binary.

You can then use a binary license service first, and add a cloud-based service as a fallback for when the license is not yet available in the bundle.

By tagging licenses with their source, you can give different sources different capabilities. For instance, a cloud-based license may lack information and can therefore not be used in production.