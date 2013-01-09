# First-time sign-in with Persona #

One thing that's different about Persona is that if your email provider supports Persona, you don't have to create a new account - you just use your existing email address. That is, you don't have to "sign up" before "signing in".

Even if you've never used Persona before, you'll get started by clicking a "Sign In" button on a website that supports Persona. The site might use the [Persona branding](https://developer.mozilla.org/en-US/docs/persona/branding) and say something like "Sign in with your email" or "Sign in with Persona," but sites can use different branding or wording if they choose. For example, here's the [Mozilla Developer Network](https://developer.mozilla.org/en-US/):

**[-- screenshot --]**

Here's [Voost](https://www.voo.st/):

**[-- screenshot --]**

When you click the button you'll see a popup from Persona that asks you for an email address to use. You can use any email address that you own. The address you choose will be used as your identity on this particular website.

What happens next depends on your email provider. Some email providers offer enhanced support for Persona, while others let the Persona service itself handle their users. Note that you don't have to figure out whether your email provider has enhanced support for Persona or not: your browser will work it out based on the email address you choose.

## If your email provider doesn't have enhanced support for Persona ##

If your email provider does not have enhanced support for Persona, and you've never used Persona before, then you'll be asked to think of a new password to use with Persona. Once you've chosen a password, you'll be asked to check for an email from Persona and click a link in it. Clicking the link confirms that you own the email address you entered, since only you have access to your inbox.

After confirming your address, you'll then be returned to the original website and signed in. If you're signing into the website for the first time, the website may ask you for additional information to complete your registration, such as your address or age.

Now you have an account with the Mozilla Persona service. Mozilla runs this service specifically for people whose email providers don't yet have enhanced support for Persona. You can add as many email addresses to it as you want, from any email provider. This is the only password you'll ever need when visiting Persona-enabled sites. You can manage your account by visiting https://login.persona.org/.

This password is only ever shared with the Mozilla Persona service. Because you proved to Mozilla Persona that you owned the email addresses attached to the account, Mozilla can vouch for you whenever you try to sign into a website with using one of those addresses. Mozilla does this by issuing your browser a credential that is shown to sites when you try to sign in.

Your browser automatically stores this credential for a limited time, so you don't have to re-enter the password every time you sign into a website.

## If your email provider has enhanced support for Persona ##

If your email provider has enhanced support Persona, it's even simpler. Your browser will ask the email provider to confirm that you own the email address:

* If you're already signed into your email (for instance, if you stay signed into Gmail most of the time, then you probably are) then your browser signs you into the website without asking for any password at all.
* Otherwise, your browser will ask you to sign into your email. Afterwards, you'll automatically be signed into the original website.

Again, if you're signing into the website for the first time, the website may ask you to enter additional information to complete your registration, such as your address or age.

## Remembering your Persona login ##

When you sign in using Persona, you may be presented with a dialog like this:

**[-- screenshot --]**

If you click "One month", then your browser will store your Persona credentials for a month, enabling you to sign into any Persona-enabled site without having to enter a password for a whole month. Of course, that means anyone else sitting at your computer can sign in as you, so only choose this option if you're the only person using the computer, or you trust anyone else who might use it.

Otherwise, select "This session only". If you do this, your browser will only store your Persona credentials for about an hour before asking you to re-enter your password.

If you want to make sure the website asks for a password the next time someone logs in from this browser, see the guide to [signing out with Persona](sign-out-with-persona.md).
