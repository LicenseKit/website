---
id: proxying
title: Service Proxying
layout: page
permalink: /licenses/proxying

hero: /assets/heros/proxying.png

description: LicenseKit lets you combine multiple service types.
---

LicenseKit lets you create custom service proxies, which use many different service types to create more capable services. LicenseKit will then use all provided services when validating licenses. 

For instance, if you have many different license files, you can create one license service per file and combine them in a proxy. LicenseKit will then go through all files when validating a license key.

Another example of when service proxying can help, is if you prefer to use the more secure code-based licenses, but also want users to be able to use their license key right away without having to distribute a new binary right away, e.g. when purchasing a license over Gumroad. 

You can then use a code-based license service and a cloud-based one and provide full access when the license is defined by the code, and more limited access when it's validated over the cloud.