+++
title = "Getting Connected"
weight = 20
+++

Fusion CAC is a web-based program. To get connected, open your web browser, and go to your site’s
Fusion CAC server address.

Some facilities will put an icon on your desktop or in another location based on how you connect to the
hospital network, but if all else fails you should be able to connect by typing the Fusion CAC server
address into your browser's URL box manually.

It will usually look something like this: https://dolbeyfusion.test.com/cac2

> [!info] 
> This address is just an example. The address for your server will be different. Be sure to type the
> server address into the URL box, not the Search box.

Dolbey currently supports the following web browsers:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox

## How to Log onto Fusion CAC Coding Application

Log in to Fusion CAC using the username and password provided to you by your facility.

![login page](/images/image-004.jpg)

## Two-Factor Authentication

A configuration change can be made by the Dolbey Support team to allow an organization to use two-
factor authentication using time-based one-time passwords (TOTP) provided from an authenticator app.
When enabled, the first time the user logs into Fusion CAC with a correct password, a new panel will
appear in the login screen with a QR code or setup key to scan/enter into an authenticator app. When
the authenticator app is updated, the TOTP will appear in the app with the following title:

`"Fusion CAC " + environmentName appSetting + ": " + user's login ID`

A new field will appear below the password field to enter the TOTP. If the TOTP matches the app, the
user is logged in. Like with the password field, five consecutive failed attempts will lock the user.

After the first successful use of the TOTP, the QR code will not be presented again for that user. After
entering the password, an additional field for the TOTP will appear. The TOTP must come from the
authenticator app at that time. Entering the correct TOTP will log the user in.

An administrator or user with privileges to User Management will be able to reset any user's two factor
authenticator for situations in which the user lost the phone or purchased a new phone that requires a
new QR code to scan. A new "Two Factor" line will appear in the User Detail page indicating whether the
user has successfully logged in with a TOTP previously. If the user did, a link will appear for the
administrator to reset the user's TOTP (which will cause a new QR code to appear for that user).

> [!info]
> Note that the user's profile must be saved after clinking the link in case the reset was accidental. The
> QR Code and Setup Key newly provided to the user after a reset is NOT the same as the prior QR Code
> and Setup Key intentionally, which should cause the prior TOTP to no longer work.
