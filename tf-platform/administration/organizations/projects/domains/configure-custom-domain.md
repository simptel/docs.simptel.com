---
description: >-
  This article provides instructions for configuring a custom domain in the TF
  Platform.
---

# Configure custom domain

### Steps to Configure a Custom Domain

#### 1. Add Your Domain

* Navigate to **Add New Domain**.
* In the dialog, enter the domain name.
* Click **Save** to generate the required CNAME record for DNS setup.

#### 2. **Update DNS Settings**

* Log in to your DNS provider’s management console.
* Add the generated CNAME record to your DNS zone.
* Ensure the CNAME value points to the target **subdomain.tfplatform.com**.
* Save the updated DNS configuration.

#### 3. Domain Verification

* Return to the **Domains** page.
* Click **Verify** to confirm the DNS changes.
* When the domain is verified, a success message will indicate this. The status will update to “Verified” under the Domain tab.

{% hint style="info" %}
_The verification process can take up to 5 minutes, and DNS changes may take up to 24 hours to fully propagate._
{% endhint %}

***

### DNS Configuration Tips and Troubleshooting

**DNS Configuration Tips**

* Ensure the CNAME or A record is accurately entered in your DNS settings.
* Confirm that the domain points to the generated CNAME provided by the TF Platform.

**Verification Issues**

If verification fails, the platform will provide troubleshooting steps. Common issues include:

* **Propagation Delays**: DNS changes may take time to propagate. Wait up to 5 minutes for verification and 48 hours for full propagation before retrying.
* **Incorrect DNS Settings**: Double-check that the records were entered correctly.

For persistent issues, consult your DNS provider’s documentation or our support team for further assistance. Following these steps will help ensure the successful configuration of your custom domain.
