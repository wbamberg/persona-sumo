# First-time sign-in with Persona #

One thing that's different about Persona is that if your email provider supports Persona, you don't have to create a new account - you just use your existing email address. That is, you don't have to "sign up" before "signing in".

So even if you've never used Persona before, you'll get started by clicking a "Sign In" button on a website that supports Persona. The site might use the [Persona branding](https://developer.mozilla.org/en-US/docs/persona/branding), and say something like "Sign in with your email" or "Sign in with Persona". But sites can use different branding or wording if they choose. Here's https://developer.mozilla.org/en-US/:

**[-- screenshot --]**

Here's https://www.voo.st/:

**[-- screenshot --]**

When you click the button you'll see a popup dialog with the Persona branding, that asks you for an email address to use. You can use any email address that you own. The address you choose will be used as your identity on this particular website.

What happens next depends on whether your email provider supports Persona or not. Most email providers don't support it yet, but we're working on adding support for Yahoo! Mail, Gmail and Outlook/Hotmail in the next few months. Note that you don't have to figure out whether your email provider supports Persona or not: your browser will work it out based on the email address you choose.

## If your email provider doesn't support Persona ##

If your email provider does not support Persona (and most don't, yet), and you've never used Persona before, then you'll now be asked to think of a new password. Once you've chosen a password, you'll be asked to check for an email from Mozilla Persona, and click a link in it to confirm that you own the email address you used. You'll then be returned to the original website and signed in. If you're signing into the website for the first time, the website will now ask you to enter anything else it needs to complete your registration, such as your address or age.

Now you have an account with the Mozilla Persona service. Mozilla runs this service specifically for people whose email providers don't yet support Persona. You can add as many email addresses to it as you want, from any email provider - so this is the only password you'll ever need. You can manage your account by visiting https://login.persona.org/.

Your password is only ever shared with the Mozilla Persona service. Because you proved to Mozilla Persona that you owned the email addresses attached to the account, Mozilla can vouch for you whenever you try to sign into a website with using one of those addresses, and issue your browser a credential that it can use to sign in.

Your browser caches this credential for a limited time, so you don't have to re-enter the password every time you sign into a website.

## If your email provider does support Persona ##

If your email provider does support Persona, it's even simpler. Your browser will ask the email provider to confirm that you own the email address:

* If you're already signed into your email (for instance, if you stay signed into Gmail most of the time, then you probably are) then your browser signs you into the website without asking for any password at all.
* If you're not signed into your email, then your browser will ask you to sign in, then sign you into the original website.

Again, if you're signing into the website for the first time, the website will now ask you to enter anything else it needs to complete your registration, such as your address or age.

## Remembering your Persona login ##

When you sign in using Persona, you may be presented with a dialog like this:

**[-- screenshot --]**

If you click "One month", then your browser will store your Persona credentials for a month, enabling you to sign into any Persona-enabled site without having to enter a password. Of course, that means anyone else sitting at your computer can sign in as you, so only choose this option if you're the only person using the computer, or you trust anyone else who might use it.

Otherwise, select "This session only". If you do this, your browser will store your Persona credentials for about an hour.

If you want to make sure the website asks for a password the next time someone logs in from this browser, see the guide to [signing out with Persona].