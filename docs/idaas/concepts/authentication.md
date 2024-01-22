# Authentication Methods

This chapter provides an overview of the fundamental concepts and best practices guiding authentication (authn) within our platform.

## User Authentication
Users have access to a range of convenient and secure authentication methods:

1. **Passwordless via SMS:** Users can opt for a passwordless authentication experience by receiving a one-time password (OTP) via SMS.
2. **Passwordless via Voice:** Users can enjoy a seamless passwordless authentication process by receiving a one-time password (OTP) via a voice call.
3. **Barcode:** Users have the option to authenticate using a barcode scanning method for quick and secure access.
4. **Single Sign-On (SSO):** Users can streamline their authentication process and access multiple applications securely with single sign-on (SSO) functionality.
5. **Username & Password:** Traditional but secure method allowing users to authenticate using their unique username and password combination.

## Client Authentication
Clients are authenticated through reliable and robust methods designed for security and authorization:

1. **Client Secret:** Clients can authenticate using a client secret to ensure secure and authorized interactions with the platform. For more details, refer to the relevant RFC. For more details, refer to [OAuth 2.0 RFC 6749 Section 2.3.1](https://datatracker.ietf.org/doc/html/rfc6749#section-2.3.1).


2. **Mutual TLS with x.509 Certificate:** OAuth client authentication and certificate-bound access and refresh tokens using mutual Transport Layer Security (TLS) authentication with X.509 certificates. This mechanism provides a secure method for client authentication and binding access tokens to a client's mutual-TLS certificate. For more details, refer to [OAuth 2.0 RFC 8705](https://datatracker.ietf.org/doc/html/rfc8705).


The inclusion of mutual TLS client authentication and certificate-bound access tokens based on X.509 certificates provides an additional layer of security and authentication for clients interacting with the platform.

This curated selection of authentication methods ensures a balanced approach to security, accessibility, and convenience for both users and clients within our platform.