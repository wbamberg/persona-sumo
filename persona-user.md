
## What is Persona? ##

Persona is a new way to sign into websites. With Persona, you:

* sign into websites using your email address and a password
* use a single password to sign into any website that supports Persona
* can use multiple email addresses, and choose which address you want to use with each website

Persona's been designed from the ground up to protect your privacy and put you in control of how your data is shared. It works on all major desktop, smartphone, and tablet browsers.

### Sign in with your email address ###

With Persona your username is your email address.

You can use any email address, as long as it's one you own (you have to prove you own it). You can use more than one email address: so you could use your work email address to sign into work-related accounts and your personal address to sign into personal accounts.

### No new passwords ###

Most of us have several websites we sign into, and many of us have dozens of them. It's very difficult to remember a separate strong password for each site. Using the same password for every site is easier, but it means that if one site is hacked, the attacker could get access to all your other accounts.

Persona is different:

* If your email provider supports Persona, you can sign into any Persona-enabled website without needing any new passwords at all.
* If your email provider doesn't support Persona, you'll need one new password for all sites.

Either way, you never send a password to the websites you're signing into. You sign into your email provider, or the Persona service, which then sends your browser a message that it can use to prove to the website that you logged into Persona successfully.

So with Persona you get the best of both worlds: a single password for all websites, but the password is never actually sent to any of the websites. (Of course, you still have to trust that the Persona server itself won't get hacked.)

### Persona takes privacy seriously ###

Many of our interactions on the web involve sharing and exchanging personal data. As we do so, we enable the companies that provide web services to collect, correlate, and sell information about us in ways we can't control.

Mozilla wants to give the user control over the data they share, and an identity system - Persona - is the first building block. There are other identity systems, such as Facebook Connect, in which you can sign into multiple sites with a single password. But with these systems the website has to "phone home" to the provider - Facebook, for example - which is then able to compile information about your browsing habits for its own purposes.

We've designed Persona from the start so that's not needed. At the moment, Mozilla's Persona service does get to see which websites you sign into, but we're working on removing this requirement, and in future versions of Persona nobody will be able to track which websites you visit.

### Use Persona with any modern browser ###

Persona's not just for Firefox users. You can use Persona on the desktop with any modern version of Internet Explorer, Firefox, Chrome, Safari, and Opera. You can use it with the Mobile Safari browser on the iPhone and iPad. You can use it on Android phones with the built-in Android browser, Firefox and Chrome.

## How Persona works ##

To begin with, you'll click a "Sign In" button on a website that supports Persona. The site might use the Persona branding (see https://developer.mozilla.org/en-US/docs/persona/branding), and say something like "Sign in with your email" or "Sign in with Persona". But sites can use different branding or wording if they choose. Here's https://developer.mozilla.org/en-US/:

<!-- screenshot -->

Here's https://www.voo.st/:

<!-- screenshot -->

You'll see a popup dialog with the Persona branding, that asks you for an email address to use. You can use any email address that you own. This email address will be used as your identity on this particular website.

What happens next depends on whether your email provider supports Persona or not. Most email providers don't support it yet, but we're working on adding support for Yahoo! Mail, Gmail and Outlook/Hotmail in the next few months.

### If your email provider doesn't support Persona ###

If your email provider does not support Persona (and most don't, yet), then you'll now be asked to think of a new password. Once you've chosen a password, you'll be asked to check for an email from Mozilla Persona, and click a link in it to confirm that you own the email address you used. You'll then be returned to the original website and logged in.

Now you have an account with the Mozilla Persona service. Mozilla runs this service specifically for people whose email providers don't yet support Persona. You can add as many email addresses to it as you want, from any email provider - so this is the only password you'll ever need. You can manage your account by visiting https://login.persona.org/.

This password is only ever shared with the Mozilla Persona service. Because you proved to Mozilla Persona that you owned the email addresses attached to the account, Mozilla can vouch for you whenever you try to log into a website with using one of those addresses, and issue your browser a credential that it can use to log in.

Your browser caches this credential for a limited time, so you don't have to re-enter the password every time you log into a website.

### If your email provider does support Persona ###

If your email provider does support Persona, it's even simpler. Your browser will ask the email provider to confirm that you own the email address:

* If you're already logged in to your email (for instance, if you stay logged into Gmail most of the time, then you probably are) then your browser signs you right into the website, without asking for any password at all.
* If you're not logged into your email, then your browser will ask you to log in, then log you into the original website.
