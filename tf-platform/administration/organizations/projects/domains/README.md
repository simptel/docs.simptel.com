---
description: >-
  This article provides instructions for supported custom domains in the TF
  Platform.
---

# Domains

By default, your tenant will be assigned a platform subdomain (`[subdomain].tfplatform.com`).

However, we recommend setting up your own domain for an improved user experience. A custom domain can enhance your brand identity, build trust, and provide a more personalized experience for your end users.\
\


### Choose a subdomain

Here are some examples of domains you can set in the Platform.

| Domain type      | Example                                                                                                          | Supported?                                     |
| ---------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Apex domain      | `example.com`                                                                                                    | Only if DNS provider supports CNAME flattening |
| `www` subdomain  | `www.example.com`                                                                                                | ✅                                              |
| Custom subdomain | <p><code>platform.example.com</code></p><p><code>portal.example.com</code> <code>anything.example.com</code></p> | ✅                                              |



