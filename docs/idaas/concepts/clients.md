# Clients and Identity Hub Overview

Clients are at the core of any OAuth infrastructure. In the context of web applications, a "client" is an entity that interacts with the server, by sending requests which the server processes and then returns a response. This interaction can happen through various interfaces and methodologies such as web browsers, mobile applications, and APIs.

In our platform, these clients interact with the "Identity Hub", a service that is responsible for managing these software applications. The Identity Hub registers new clients, issues and renews client credentials, and orchestrates OAuth workflows, all while ensuring the security and integrity of client interactions.

When a client application is registered with our Identity Hub, it's assigned a unique identifier - the client ID. This ID is used to authenticate the client application to the server, ensuring only authenticated clients can access user resources.

## Types of Clients within OAuth

OAuth classifies clients into two types based on their capability to securely authenticate with the authorization server, principally, their ability to maintain the confidentiality of their client credentials:

### Confidential Clients
Confidential clients are able to securely authenticate with the authorization server and are capable of keeping their client credential (client secret) confidential. These could be applications running on a server where the source code isn't exposed to the public.

### Public Clients
On the other hand, public clients are unable to maintain the confidentiality of their client credentials. These are typically client-side applications like Single Page Applications (SPA), mobile apps, or other browser-based apps where the source code (and thus any included credentials) could be exposed to the end user.

## OAuth Flows Supported by the Identity Hub

Our Identity Hub supports two common OAuth workflows, each tailored for different types of client app scenarios:

### Client Credentials Flow
This flow is most suitable for confidential clients and for scenarios where the client is requesting access to the resources it owns. 

In this flow, the client application uses its client ID and secret to authenticate itself and get an access token. This flow is most commonly used for server-to-server interactions.

### Authorization Code Flow with Proof Key for Code Exchange (PKCE)
This flow is most suitable for public clients and acts on behalf of the user to access the user's resources.

In this flow, the client starts the authorization process by directing the user to the authorization server for authentication. After successful authentication, the client receives an authorization code that can be exchanged for an access token. PKCE adds an additional layer of security that protects this exchange from authorization code interception attacks.

## Adherence to OAuth 2.1
Our Identity Hub is designed in adherence with the principles of OAuth 2.0 and is future-ready for OAuth 2.1.

For both confidential and public clients, we follow the two primary flows outlined in OAuth 2.1 (and commonly used in OAuth 2.0), namely the Client Credentials flow and the Authorization Code flow with PKCE.

By avoiding the Implicit Flow and the Resource Owner Password Credentials Flow, which are not advised due to known security vulnerabilities, we ensure that our Identity Hub remains in compliance with the most secure versions of the OAuth specifications.

## Common Concerns:

1. **Securing Client Credentials:**  
    Client credentials include the client ID and any other key credential and these need to be kept securely to mitigate unauthorized access.
	
2. **Action Steps for Compromised Credentials:**  
    In the event of compromised credentials, immediate action towards revocation and incident response, followed by adherence to the set incident management procedures is recommended.
	
3. **Protection of Client Application and User Information:** 
    The inclusion of both the Client Credentials flow and the Authorization Code flow with PKCE in the Identity Hub offers a protective layer for client-side authentication and interaction with the user's resources. This layer of security is beneficial for client applications and their users. 