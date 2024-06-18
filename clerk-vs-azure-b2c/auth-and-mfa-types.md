# Auth and MFA Types

## Azure AD B2C

Supports any number of local account email, username, and passwords. Phone login. Social/federated login. MFA can be email, SMS, security questions, authenticator app (no push, just TOTP). SMS is an up charge of $0.03 per SMS. Other MFA methods may be supported but require a third party API, like Okta Push or something like that.

## Clerk

Supports local accounts email, username, and passwords. Phone login. Social/federated login. Those are pretty standard, but something I love is that passkeys are included out of the box (even if it's in beta). I am increasingly using passkeys stored in my password manager to get into sights, and I think it's the way of the future. The less we have to rely on passwords the better. The MFA options are the pretty standard SMS and Authenticator app and then they also include backup codes, and are marketing that security keys like Yubikey are coming soon. Very exciting stuff. I really appreciate that they don't even allow security questions. They are too phisable. They also include a metamask login option, which is nice if you're into the web3 world.