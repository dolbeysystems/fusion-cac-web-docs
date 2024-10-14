+++
title = "Getting Connected"
weight = 20
+++

Fusion CAC is a **browser-based** program. To launch the CAC browser application,
open your web browser and enter your site’s Fusion CAC server address into the
{{%button%}}browser address bar{{%/button%}}.  You will need to get the Fusion
CAC server address from your {{%icon icon="user-tie"%}} site administrator or
manager.

> [!info] Fusion CAC URL Example
> **https://fusion-cac-production/cac2**
>
>*This address is just an example. The address for your server will be different.*

> [!note] Shortcut
Your facility may have created an shortcut icon on your desktop to make it easier
for you to quickly connect to the Fusion CAC application.

## {{%icon icon="globe"%}} Web Browser Support

Fusion CAC works on *recent versions* of the following web browsers:

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
Microsoft Internet Explorer is no longer supported by Microsoft and is also not compatible with
the Fusion CAC software.

## {{% icon icon="user" %}} Logging in to the Fusion CAC Coding Application

Once the Fusion CAC application has loaded in your browser, enter the username and password
provided to you by your facility, and then press the {{%button%}}Login{{%/button%}} button.

{{%video "/logging-in.webm"%}}

> [!warning] Account Lock-Out
Five consecutive failed logins will cause your account to be locked out of the
application.  If you are locked out, contact your {{% icon icon="user-tie" %}} supervisor.

## {{% icon icon="lock" %}} Two-Factor Authentication (Optional)

> [!important] Your organization may not have Two-Factor Authentication configured
Two-factor authentication must be configured for your site by the Dolbey Support team.
If your site is not using two-factor authentication, this section will not apply to your login
process.

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

> [!warning] Account Lock-Out In Two-Factor Flow
Five consecutive failed logins at either stage will cause your account to be locked out of the
application.  If you are locked out, contact your {{% icon icon="user-tie" %}} supervisor.

If your site is configured for **two-factor authentication**, after your first login, you will be
taken to a screen showing a QR code to scan or a key to enter into
an authenticator app on your {{% icon icon="phone" %}} smartphone.  

Once you have scanned or saved the code to your authenticator app, the TOTP (time-based one-time
password) entry for Fusion CAC will appear in your authenticator  app with a title similar to this:

```
Fusion CAC Dolbey Health Production: heminger
```

At this point, your {{% icon icon="phone" %}} authenticator app has been configured and will now
give you time-based codes to log in to the Fusion CAC coding application.

To view the time-based code when logging into the app, select the entry in your authenticator app.
You should see a long sequence of characters that will change every minute.  When you login to the
Fusion CAC application, you will need to view and enter this key from your {{%icon icon="phone"%}}
authenticator app into the field beneath the password field.

> [!note] What if I get a new phone?
Your {{%icon icon="user-tie"%}} site administrator or supervisor can reset your two-factor
authentication setup if you have replaced or reset your phone and no longer have access
to the "Fusion CAC" entry in your authenticator application.

