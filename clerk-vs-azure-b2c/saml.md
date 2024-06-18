# SAML

## Azure AD B2C

Supports both SP and IdP initiated SAML. I noticed that Clerk calls out the security concerns with IdP initiated SAML, but Microsoft does not. You can also use SAML to connect to social providers that support it if you want, but it's a feature only available through custom policies, not in the UI driven user flows. It's just a generic SAML provider though, no pre-filled out information if you wanted to do a popular one like Azure or Salesforce.

## Clerk

Clerk supports both SP and IdP initiated SAML, and calls out the issues with IdP initiated SAML and the steps they are taking to help mitigate the risks if you choose to use it. Clerk also calls supports SAML for social providers and has some popular ones baked in like Azure, Google, and Okta. It also has a generic provider. It supports MFA, account linking, and just in time provisioning. It's $50 / month extra though which is interesting.