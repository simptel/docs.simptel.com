---
description: >-
  This article provides instructions for removing a custom domain in the TF
  Platform.
---

# Remove custom domain

#### Removing a Custom Domain

**Step 1: Remove the Domain**

* Select the custom domain you wish to remove.
* Click **Delete**. A confirmation dialog will appear.

**Step 2: Confirm Deletion**

* Review the warning, fill in the confirmation prompt, then click **Delete** again to confirm and finalize the removal.

**Step 3: Update DNS Records**

* Access your DNS provider's console after the domain is removed from the platform.
* Remove or unpoint the CNAME record linked to the deleted domain.

{% hint style="warning" %}
Removing a custom domain will disrupt all associated services and features, rendering them inaccessible. Ensure you are prepared for this impact before proceeding with deletion.
{% endhint %}
