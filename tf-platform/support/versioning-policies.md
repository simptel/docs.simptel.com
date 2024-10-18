---
description: This article describes how we incorporate versioning of the services.
---

# Versioning Policies

#### Header-Based Versioning

For our APIs, versioning is handled through **header-based versioning**. This approach lets you specify the API version you want to use without altering the URL structure.

To use a specific version, include the following header in your requests:

```http
API-Version: 1.0.0
```

If you omit the version header, the latest stable version of the API will be used by default.

#### Semantic Versioning

We use **semantic versioning** (semver), which follows the format `{major}.{minor}.{patch}`. Each component of the version number indicates the nature of changes:

* **Major (X.0.0)**: Introduces breaking changes that are not backward-compatible. You may need to update your implementation when the major version changes.
* **Minor (X.Y.0)**: Adds new, backward-compatible features. Updating to a new minor version should not break existing functionality but testing is advised.
* **Patch (X.Y.Z)**: Applies bug fixes or minor improvements that do not alter the API's core behavior. These are typically safe to apply without concern for compatibility issues.

Examples: `1.2.0`, `2.0.3`, `3.1.1`.

#### API Request Example

To specify a version when making API requests, you use the `TF-API-Version` header:

```http
GET https://your-domain.com/api/resource
Host: your-domain.com
API-Version: 1.2.3
```

#### Best Practices for Production

For production environments, we recommend specifying the **full version** (major.minor.patch) in the `API-Version` header. This ensures that unexpected updates do not affect your system and performs consistently with the version you have tested.

#### Version Tags

All TF Platform open-source components follow semantic versioning, and releases are tagged accordingly in repositories. Versions are prefixed with "v" (e.g., `v2.3.1`).

