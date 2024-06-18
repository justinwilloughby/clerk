# Social Login

## Azure AD B2C

Both services hit the core social providers. The main differences here are in the docs. The Azure Docs give pretty detailed steps for doing the integration, but it's just words. No screenshots. Also the Apple integration with custom policies is not finshed. Instead of using the details for your app and service with the private key, it makes you use an Azure Function to use those values and generates a token to use for Apple Login that needs regenerated every 6 months. Not a great operational experience.

## Clerk

The Clerk docs shine here with the use of screenshots. I think it really helps when you're not familar with these other developer portals to know where to go. Also the Apple integration is fully fleshed out and easy to configure in the UI. Clerk also seems to provide more startup friendly social integrations like Coinbase, Discord, Notion, Slack, Spotify, etc. They have both versions of the Twitter login, and the Twitter V2 docs call out that the email is not returned. That's a nice thing to know up front. I did that integration before and had to debug and figure that out myself.