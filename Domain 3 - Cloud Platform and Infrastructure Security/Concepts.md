# Domain 3 Cloud Platform and Infrastructure Security Concepts

# SAML

## What is SAML?
- **SAML** (Security Assertion Markup Language) is an **open** standard for exchanging authentication and authorization data between identity providers (IdPs) and
  service providers (SPs). It’s XML-based and widely used in Single Sign-On (SSO) systems.

## What is an Assertion?
- An assertion is a **package of information** that the **IdP sends to the SP**. It tells the SP:
	✅ Who the user is (Authentication)
	✅ What the user can do (Authorization)
	✅ Other attributes about the user (Attributes)
- So, an identity assertion token is essentially the **SAML message** **carrying user’s identity and claims**.

## Types of SAML Assertions
- **SAML** defines **three** types of assertions (tokens):
1. Authentication Assertion
	- Proves the user’s identity (e.g., Ravi successfully logged in at 10:00AM using password).
2. Attribute Assertion
	- Provides additional details (e.g., Ravi’s role = Admin, Department = Security).
3. Authorization Decision Assertion
	- Specifies access rights (e.g., Ravi is permitted to access financial records).

## SAML Identity Assertion Token Flow (SSO Example)
1. User tries to access a cloud service (SP).
2. SP redirects to IdP.
3. IdP authenticates the user.
4. **IdP creates a SAML assertion token → digitally signed XML**.
5. Token is sent back to SP.
6. SP validates the token → grants access.

## Why It Matters?
- Enables SSO across multiple services without multiple logins.
- Provides secure, signed proof of identity.
- Avoids storing passwords in multiple places.

👉 In short: A SAML identity assertion token is the **signed XML message issued by the Identity Provider**, which carries the authenticated identity (and possibly roles/permissions) of a user to the Service Provider for secure access.


# SAML identity assertions vs. OAuth access tokens vs. OpenID Connect ID tokens

## Quick Way to Remember:
- SAML → Old school, XML-based, enterprise SSO.
- OAuth → Delegated authorization (what you can do).
- OIDC → Authentication built on OAuth (who you are).

## ⚡Example in real life:
- SAML → Employee logs in once to use multiple internal apps (HR portal, payroll, CRM).
- OAuth → Mobile app wants access to your Google Drive files (without knowing your password).
- OIDC → Website uses Google/Facebook login button to know who you are.

## 🔐 SAML vs. OAuth vs. OIDC – Token Comparison
________________________________________________________________________________________________________________________
Features			|	 SAML Identity 					|
					|	Assertion (Token)				|
____________________|___________________________________|______________________________________________________________________
Purpose				| Provides identity & attributes	|
					| to a Service Provider (SP)		|
Used in				| Enterprise SSO, WebApps, XML based|
Format				| XML (digitally signed)			|
Issuer				| Idnetity Provider (IdP)			|
Consumer			| Service Provider (SP)				|
Contains			| - Authentication statement 		|
					| - Attribue Statement				|
	 				| - Authorization decision			|
Focus				| Authentication + Attributes		|
Transport			| Browser Redirects (POST binding)	|
Token Lifetime		| Short (minutes)					|
Security Mechanism	| XML Signature & Encryption		|
Best for			| Federated SSO between orgs 		|

____________________________________________________________________________________________________________________________________
- OAuth 2.0 Access Token
- OpenID Connect (OIDC) ID Token
