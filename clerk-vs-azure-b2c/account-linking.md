# Account Linking

## Azure AD B2C

I think built in user flows will auto link accounts, but in custom policies you have to specify the logic yourself. If you build it out of the gate it can be pretty simple, but adding it in later is challenging because you have to disect the existing custom policy and make sure you don't break the existing logic.

## Clerk

Clerk has built in account linking that takes into account the email verification status. If email matches in local directory and social directory and they are both verified then they link. If one is verified and not the other then they verify. If emails don't match then they can still manually link on Profile page. Very nice system.