---
description: >-
  This article provides an overview of the options for managing SSL Certificates
  for your domains.
---

# Certificates

When configuring a custom domain, **Automatic Certificate Management** is enabled by default. You can also opt for **Self-Managed Certificates.** If you disable the active self-managed certificate, the system will automatically revert to Automatic Certificate Management to maintain security.

***

### Automatic Certificate Management

By default, SSL/TLS certificates are automatically issued, renewed, and deployed. This guarantees that your domains remain secure without any manual effort.&#x20;

***

### Self-Managed Certificates

Self-managed certificates are suitable for:

* **Origin Servers**: Configuring SSL/TLS for secure communication between our service and your DNS provider.
* **Custom Certificates**: Providing your own certificates to meet specific requirements.

{% hint style="info" %}
You are responsible for obtaining and renewing certificates from your chosen Certificate Authority (CA) and configuring your DNS provider accordingly.
{% endhint %}







