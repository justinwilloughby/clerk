# Allow / Block List

## Azure AD B2C

This is a simple enough feature, but in B2C this would need to be done in a custom policy. You could create a list directly in the policy but then need to update and deploy everytime you need a change, or you could make it dynamic by getting the list from a REST call and DB, but that just seems like too much to do for a simple feature. I didn't make much use of this during my implementations.

## Clerk

Built right into the UI. I added myself to the allow list so that only I could sign-up/in to my apps while it was on the public web but still in development. The block email subaddresses, and block disposable emails features seem very powerfull.