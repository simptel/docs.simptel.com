---
description: This article provides an overview of supported TLS/SSL certificates.
---

# TLS/SSL Support

When setting up a reverse proxy with self-managed certificates to connect to the TF Platform, it's crucial to ensure that you use a supported TLS version and cipher suite. The TLS handshake, which is the communication between the server and client, specifies the TLS version and cipher suite. Using an unsupported version could lead to failure.

### Supported TLS 1.3 Cipher Suites

* TLS\_AES\_128\_GCM\_SHA256
* TLS\_AES\_256\_GCM\_SHA384
* TLS\_CHACHA20\_POLY1305\_SHA256

{% hint style="info" %}
To learn more, read [Transport Layer Security (TLS) Parameters](https://www.iana.org/assignments/tls-parameters) for the Internet Assigned Numbers Authority (IANA) list of registered parameters, including ciphers.
{% endhint %}
