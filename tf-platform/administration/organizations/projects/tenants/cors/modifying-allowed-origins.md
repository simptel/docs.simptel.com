---
description: This article provides an overview of modifying cors
---

# Modifying Allowed Origins

**Configuring CORS**

1. **Go to Projects**: Access the "Projects" section within the platform.
2. **Select the Tenant**: Choose the tenant you wish to configure.
3. **Access CORS Settings**: Navigate to the CORS settings in the tenant's "Domains" section.
4. **Allowed Origins**: Specify up to 10 origins allowed to make cross-origin requests.

**Configuration Examples:**

* **Subdomain Wildcard**: `https://*.example.com`
* **Environments**:
  * Production: `https://myapp.com`
  * Local Development: `http://localhost:4200`

{% hint style="info" %}
_Using `*` as a wildcard is not recommended in production environments for security reasons._
{% endhint %}
