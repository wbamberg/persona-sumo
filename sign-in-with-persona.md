# Signing in with Persona #

To begin with, you'll click a "Sign In" button on a website that supports Persona. The site might use the Persona branding (see https://developer.mozilla.org/en-US/docs/persona/branding), and say something like "Sign in with your email" or "Sign in with Persona". But sites can use different branding or wording if they choose. Here's https://developer.mozilla.org/en-US/:

<!-- screenshot -->

Here's https://www.voo.st/:

<!-- screenshot -->

You'll see a popup dialog with the Persona branding, that asks you for an email address to use. You can use any email address that you own. The address you choose will be used as your identity on this particular website.

What happens next depends on whether your email provider supports Persona or not. Most email providers don't support it yet, but we're working on adding support for Yahoo! Mail, Gmail and Outlook/Hotmail in the next few months.

## If your email provider doesn't support Persona ##

If your email provider does not support Persona (and most don't, yet), and you've never used Persona before, then you'll now be asked to think of a new password. Once you've chosen a password, you'll be asked to check for an email from Mozilla Persona, and click a link in it to confirm that you own the email address you used. You'll then be returned to the original website and signed in.

Now you have an account with the Mozilla Persona service. Mozilla runs this service specifically for people whose email providers don't yet support Persona. You can add as many email addresses to it as you want, from any email provider - so this is the only password you'll ever need. You can manage your account by visiting https://login.persona.org/.

This password is only ever shared with the Mozilla Persona service. Because you proved to Mozilla Persona that you owned the email addresses attached to the account, Mozilla can vouch for you whenever you try to sign into a website with using one of those addresses, and issue your browser a credential that it can use to sign in.

Your browser caches this credential for a limited time, so you don't have to re-enter the password every time you sign into a website.

## If your email provider does support Persona ##

If your email provider does support Persona, it's even simpler. Your browser will ask the email provider to confirm that you own the email address:

* If you're already signed into your email (for instance, if you stay signed into Gmail most of the time, then you probably are) then your browser signs you right into the website, without asking for any password at all.
* If you're not signed into your email, then your browser will ask you to sign in, then sign you into the original website.
