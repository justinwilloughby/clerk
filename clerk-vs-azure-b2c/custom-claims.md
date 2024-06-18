# Custom Claims

## Azure AD B2C

In Azure AD B2C, you have the ability to add extension attributes, have the user populate them or have them programatically popuated, and then you can add them to the JWT returned to the app. In custom policies you can also use a REST API at the end of the flow to go grab external data and put it into the token too if the app needs special data that the IdP does not have.

## Clerk

Clerk has the ability to augment the session token, and it's way easier to do so, it's just done through the UI, but it doesn't seem to have custom attributes, and you can't augment the JWT with arbitrary data from a REST API call either. It could be argued that if the app needs data it should just go get it though after the user logs in and that shouldn't be on the IdP. Often times the app teams were unable to make changes fast when migrating off the old IdP so it was easier for us to augment the JWT with the data they needed.