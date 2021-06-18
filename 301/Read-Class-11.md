# Authentication

## What is OAuth

- OAuth allows websites and services to share assets among users. It is widely accepted, but has vulnerabilities.

- Seamless SSO (single sign-on) has been a major challenge. Although not done, the progress we have made has been in a large part due to OAuth, thanks.

- It is widely adopted.

- It’s more helpful to understand it by thinking about it as open AUTHorization.

## How it works

- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

- The first site gives this token and secret to the initiating user’s client software.

- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

- The user approves (or their software silently approves) a particular transaction type at the first website.

- The user is given an approved access token (notice it’s no longer a request token).

- The user gives the approved access token to the first website.

- The first website gives the access token to the second website as proof of authentication on behalf of the user.

- The second website lets the first website access their site on behalf of the user.

- The user sees a successfully completed transaction occurring.

## OpenID vs. OAuth

OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

In 2014, OpenID Connect was released, which reinvented OpenID as an authentication layer for OAuth. In this space, OpenID has found a niche, and the two technologies now complement each other in many implementations.

## SAML vs. OAuth

The Security Assertion Markup Language, or SAML, is another technology. SAML describes a framework that allows one computer to perform both authentication and authorization on behalf of one or more other computers, unlike OAuth, which requires an additional layer like OpenID Connect to perform authentication. SAML can provide single sign-on functionality on its own.

## Authentication and Authorization Flows

Auth0 uses the OpenID Connect (OIDC) Protocol and OAuth 2.0 Authorization Framework to authenticate users and get their authorization to access protected resources. With Auth0, you can easily support different flows in your own applications and APIs without worrying about OIDC/OAuth 2.0 specifications or other technical aspects of authentication and authorization.

In simple terms, authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.

In short, access to a resource is protected by both authentication and authorization. If you can't prove your identity, you won't be allowed into a resource. And even if you can prove your identity, if you are not authorized for that resource, you will still be denied access.
