# Overview
This guide outlines how applications interact with our services.

## Client Categories

### Client
Represents an application that interacts with other applications or services, regardless of whether the application runs on a server, PC, or other device.

For more details, refer to the [OAuth 2.0 RFC 6749 Section 1.1](https://datatracker.ietf.org/doc/html/rfc6749#section-1.1).


### 


## Types of Clients within OAuth

OAuth classifies clients into two types based on their capability to securely authenticate with the authorization server, principally, their ability to maintain the confidentiality of their client credentials:

### Confidential Clients
Confidential clients are able to securely authenticate with the authorization server and are capable of keeping their client credential (client secret) confidential. These could be applications running on a server where the source code isn't exposed to the public and they support the following flows:

- Authorization Code Flow with PKCE
- Client Credentials Flow


### Public Clients
On the other hand, public clients are unable to maintain the confidentiality of their client credentials. These are typically client-side applications like Single Page Applications (SPA), mobile apps, or other browser-based apps where the source code (and thus any included credentials) could be exposed to the end user and they support the following flows:

- Authorization Code Flow with PKCE

