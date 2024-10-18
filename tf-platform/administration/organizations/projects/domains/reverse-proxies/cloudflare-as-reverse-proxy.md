---
description: >-
  This article provides a steps to configure Cloudflare as a reverse proxy for
  your application.
---

# Cloudflare as Reverse Proxy

#### Steps to Configure Cloudflare

1. **Sign Up for Cloudflare**
   * **Create a Cloudflare Account**: If you don’t already have an account, sign up on Cloudflare's website.
   * **Add Your Domain**: Follow the prompts to add your domain to your account.
2. **Update DNS Settings**
   * **Verify Domain Ownership**: Follow the instructions to verify ownership, typically by adding a TXT record at your domain registrar.
   * **Change DNS Records**:
     * Go to the **DNS** tab in your Cloudflare dashboard.
     * Add or modify DNS records to point to your origin server using the following settings:
       * **Type**: A or CNAME
       * **Name**: Your subdomain (e.g., platform or www)
       * **Value**: Your origin server’s IP address or hostname
       * **Proxy Status**: Set to **Proxied** (indicated by the orange cloud icon).
3. **Configure SSL/TLS Settings**
   * **Set SSL/TLS Mode**: Navigate to the **SSL/TLS** tab and choose an appropriate mode (e.g., Full or Full (strict)). If you have added the origin server certificate as a custom certificate in the platform, use **Full (strict)**.
   * **Enable Always Use HTTPS**: Turn on the **Always Use HTTPS** option to ensure secure connections.
4. **Test Your Setup**
   * **Access Your Tenant**: Ensure your tenant is accessible through the Cloudflare proxy. Verify that SSL/TLS functionality works and that requests are routing correctly to your origin server.
