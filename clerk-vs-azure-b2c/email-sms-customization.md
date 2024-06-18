# Email and SMS Customization

## Azure AD B2C

The templates are only fully customizable if you use custom policies. If you use the GUI user flows you only get the OOTB wording, but you can customize the logo and app name and stuff like that. For a fully customized template, you need to use the MS Graph to send mail, or you need to integrate with a third party provider like SendGrid. It's the same for SMS. The integration with third party in the custom policies is done via REST.

## Clerk

Clerk has this awesome handlebars GUI editor for customized templates and I love it. This is how easy it should be. I also like that they have the ability to integrate with a third party provider too which gives you more flexibility on where the email or SMS is coming from. The integration is a little different though, it uses hooks instead of direct REST call. So pull instead of push. I don't mind that, you just need to have something listening for the event, and then trigger your email or sms code.