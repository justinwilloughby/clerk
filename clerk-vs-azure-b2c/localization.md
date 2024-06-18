# Localization

## Azure AD B2C

Build in attributes and components are automatically localized to 36 languages and render based on the browser context. If you have any custom attributes, or components though, which we always do, those need to be manually translated and explicitly added to the custom policy files.

## Clerk

Looks like localization is an exerimental feature right now. They have 25 supported languages, and the language is passed as a prop to the ClerkProvider. In the example, the prop is imported from the clerk package. I suspect if you wanted to dynamically supply the language you would have to import all the languages, do some preprocessing to find the browser language and pick the right one to pass as a prop, but if you only wanted to support one language it's easy enough. You are able to overwrite any of the elements that are populated from the Clerk package so if you didn't like the translation for one, you could overwrite it directly in the code and pass it to the ClerkProvider. This is import for not just localizing the text, but also if you wanted to change any of the built in element text you could do it this way too. Don't like that the button says "Continue"? You can change it to "Next" through this method as well.