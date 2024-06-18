# Attack Protection

## Azure AD B2C

B2C has a slim version of the corporate side's Conditional Access which allows you to put rules in place to conditionally allow/deny access or force a step up before access is given. The CA can be a very specific rule like deny access from outside the US, or they also have risk based features that uses ML to evaluate the riskiness of the user and the sign in attempt before deciding what to do. There is no build in ddos or bot detection. To get these features you have to use another integration which Microsoft pitches Azure Front Door for ddos and firewall security, and Dynamics Fraud protection for bot and account protection.

## Clerk

The Account Protection features are some of the most exciting I saw on the platform because they are just baked in. Out of the box you get ddos and bot protection. If too many requests are coming in, the account get's locked out for an hour. Or you can lock them forever until you unlock them manually. You can also turn on the Cloudflare turnstile feature which is like a captch that helps block bots. These are things that my clients have begged for but the Microsoft offering fell short.