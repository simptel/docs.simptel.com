---
description: >-
  This article provides an overview of how to manage, upload, and renew SSL/TLS
  self-managed certificates.
---

# Configure Self-Managed Certificates

#### Steps to Add a Self-Managed Certificate

1. **Access the Certificates Section**
   * Navigate to the **Domains** page.
   * Locate and select the **Certificates** section.
2. **Upload the Certificate**
   * Click on the **Upload Certificate** option.
3. **Input Certificate and Key**
   * **Enter SSL Certificate and Private Key**:
     * Ensure your SSL certificate file is in PEM format (typically a `.crt` or `.pem` file).
     * Ensure your private key file is in PEM format (usually a `.key` file).
   * **Copy and Paste Contents**:
     * Copy the contents of your SSL certificate and paste them into the **Certificate** field.
     * Copy the contents of your private key and paste them into the **Private Key** field.
4. **Save the Certificate**
   * Click the **Save** button to upload the certificate
5. **Review Certificate details**
   * **Common Name**: A name for easy identification.
   * **Issuer**: The organization that issued the certificate.
   * **Valid From**: The start date of the certificate's validity.
   * **Valid to**: The certificate's expiration date.
   * **Covered Domains**: Domains secured by the certificate.
   * **Thumbprint**: A unique identifier for quick reference.
6. **Activate the Certificate**
   * After saving, ensure the certificate is activated by clicking the **Activate** button (if applicable) in the Certificates section. This step is essential for enabling secure connections using the newly uploaded certificate.

{% hint style="info" %}
Each tenant is limited to **5 certificates**.
{% endhint %}
