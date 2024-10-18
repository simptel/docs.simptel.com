---
description: This article provides an overview about the concept of Tenants.
---

# Tenants

### **What is a Tenant?**

A **tenant** on TF Platform is a logically isolated environment where you can manage your own data, applications, resources, and configurations.

{% hint style="info" %}
Each project can have up to 10 tenants.
{% endhint %}

***

### How Are Tenants Identified?

Each tenant has its own domain. When end-users make requests to a configured domain, the platform routes them to the correct tenant environment. This setup ensures secure and independent operations for each tenant. For more information see [configure-custom-domain.md](../domains/configure-custom-domain.md "mention").

**Examples:**

* **Default Domain:** \[subdomain].tfplatform.com
* **Custom Domain:** yourdomain.com

