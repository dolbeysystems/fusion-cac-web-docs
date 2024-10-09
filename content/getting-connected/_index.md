+++
title = "Getting Connected"
weight = 20
+++

Fusion CAC is a **browser-based** program. To launch the CAC browser application, open your web browser and enter
your site’s Fusion CAC server address into the browser address bar.  You will need to get the Fusion CAC server
address from your site administrator or manager.

The address will usually look something like this: 

```bash
https://fusion-cac-production/cac2
```

> [!important] Example Only
This address is just an example. The address for your server will be different. Be sure to type the
server address into the URL box, not the Search box.

> [!note] Shortcut
Your facility may have created an icon on your desktop or in another location based on how you connect to the
hospital network, but either way, you can load the Fusion CAC software by typing the Fusion CAC server
address into your browser's URL box manually.


Dolbey currently supports recent versions of the following web browsers:

<div style="display: flex; justify-content: center;">
  <figure>
    <img src="https://upload.wikimedia.org/wikipedia/commons/e/e1/Google_Chrome_icon_%28February_2022%29.svg" style="width: 120px">
    <figcaption>Google Chrome</figcaption>
  </figure>
  <figure>
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/Microsoft_Edge_logo_%282019%29.png" style="width: 120px">
    <figcaption>Microsoft Edge</figcaption>
  </figure>
  <figure>
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/76/Mozilla_Firefox_logo_2013.svg" style="width: 120px">
    <figcaption>Mozilla Firefox</figcaption>
  </figure>
</div>

> [!caution] Internet Explorer Support
Microsoft Internet Explorer is no longer supported by Microsoft and is also not compatible with the
Fusion CAC software.

## {{% icon icon="user" %}} Logging in to the Fusion CAC Coding Application

Log in to Fusion CAC using the username and password provided to you by your facility.

![login page](/images/image-004.jpg)

## {{% icon icon="lock" %}} Two-Factor Authentication (Optional)

> [!important] Two-Factor Configuration Required
Two-factor authentication must be configured for your site by the Dolbey Support team.  If your site
is not using two-factor authentication, this section will not apply to your login process.

{{< mermaid >}}
flowchart LR;
  qr --> login

  subgraph First Time Login Process
  ft{First Time Login} --> |Successful| qr(QR Code Setup)
  ft --> |Failure| ft-fail(Login Failed)
  ft-fail --> ft
  end

  subgraph Normal Login Process
  login{Login} --> |Successful| Application
  login --> |Failure| fail(Login Failed)
  fail --> login
  end
{{< /mermaid >}}

> [!caution]
Five consecutive failed logins at either stage will cause your account to be locked out of the
application.

Your site may be configured for two-factor authentication.  If this is the case, the first time that
you login, you will be presented with a screen showing a QR code or setup key to scan or enter into
an authenticator app on your phone.  Once you have scanned or saved the code to your authenticator
app, the TOTP (time-based one-time password) entry for Fusion CAC will appear in your authenticator 
app with the following title.

```bash
"Fusion CAC " + environmentName appSetting + ": " + user's login ID
```
To view the TOTP key for the app, select this entry in your authenticator app.  You should see a 
long sequence of characters that will change every minute.  From now on, when you login to the Fusion
CAC application, you will need to view and enter this key from your phone into the field beneath the
password field.

An administrator or user with privileges to User Management will be able to reset any user's two factor
authenticator for situations in which the user lost the phone or purchased a new phone that requires a
new QR code to scan. A new "Two Factor" line will appear in the User Detail page indicating whether the
user has successfully logged in with a TOTP previously. If the user did, a link will appear for the
administrator to reset the user's TOTP (which will cause a new QR code to appear for that user).

> [!caution] Save Required
The user's profile must be saved after clinking the link in case the reset was accidental. 

> [!caution] Reset Creates a New QR Code
The QR Code and Setup Key newly provided to the user after a reset is NOT the same as the prior QR Code
and Setup Key intentionally, which should cause the prior TOTP to no longer work.

