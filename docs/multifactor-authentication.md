<style type="text/css" rel="stylesheet">
img { width: 50%; margin:auto!important; }
</style>

# Multifactor authentication

Multifactor authentication (MFA) is a user verification method that requires more than one type of validation, such as a password and a one-time passcode (OTP). It helps prevent unauthorized account access even if someone has the username and password.

During Early Access, you can use MFA for your organization’s Classy account. This will require admins to enter their password and OTP via Google Authenticator on a mobile device to access your account.

!!! abstract "To use MFA on Classy, you need:"

    * A computer
    * A smartphone
    * Google Authenticator downloaded on your <a href="https://apps.apple.com/us/app/google-authenticator/id388497605">iPhone</a> or <a href="https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_US">Android</a> device

    **Want to participate?**

    [Sign up to join Classy's MFA beta program.](https://learn.classy.org/mfa-beta-program.html?utm_source=early-access&utm_medium=help-center&utm_campaign=beta-program)

## Why is MFA important?

MFA reduces the risk of unauthorized access compared to passwords alone. It's an industry best practice and a critical component in safeguarding user and supporter data.

MFA can also help you:

- Comply with regulatory requirements
- Protect sensitive data
- Prevent identity theft

## Set up MFA

!!! note

    If you’re a new Classy admin, select the button in the ‘Claim your account’ email sent to your address to set up your account for the first time.

To set up MFA:

1. Start on your computer and log in to [Classy](https://www.classy.org/sso) using your username and password
2. You’ll be prompted to set up multifactor authentication. Select **Setup.**

![Setup multifactor authentication](https://learn.classy.org/rs/673-DCU-558/images/mfa-setup-okta.png)

1. On your smartphone, download and open Google Authenticator
2. Tap the **+ icon**
3. Tap **Scan a QR code**
4. Use your camera to scan the QR code on your computer (Give Authenticator access to your smartphone's camera if you need to)
5. This adds your account to Authenticator and generates a one-time verification code
6. Enter the code on the Classy login screen and **Verify**
7. Select **Finish**

You've successfully set up multifactor authentication! From now on, you'll need to provide a verification code from the Authenticator app, at least once a day, to log into your account.

## Log in with MFA

To log in with MFA:

1. Log in to Classy using your username and password
2. Enter the verification code provided in the Google Authenticator app
3. Select **Verify**

![Verify with a one-time passcode](https://learn.classy.org/rs/673-DCU-558/images/mfa-enter-otp.png)

And you’re in! We recommend marking the checkbox so we don't challenge you again on this device for 24 hours.

If you need more help, check out [Google's documentation](https://support.google.com/accounts/answer/1066447?hl=en&co=GENIE.Platform%3DiOS&sjid=2573524651642187198-NC).

!!! warning "Important"

    After five failed login attempts, you’ll be locked out of your account. Contact our [Care team](https://support.classy.org/s/contactcare) to restore access.

## Frequently asked questions

**Is MFA required?**

Yes. MFA will be required for all Classy admins starting in February 2025. At that time, admins must use MFA to log in.

**Why is MFA required?**

Classy is committed to top security standards. MFA helps prevent unauthorized access by adding an extra layer of protection to your account.

**Is there any additional cost associated with MFA?**

No. MFA is a security requirement, so there is no extra cost for customers.

**Will supporters need to use MFA to access their accounts?**

No, supporters will not be required to use MFA. They can continue to log in using their password or a one-time code sent to their email.

**How often will an organization need to use MFA?**

Organizations will need to log in with MFA once per day for each browser they use (e.g., once for Chrome, once for Safari).

**Can organizations configure the frequency of MFA?**

No, not at this time.

**What types of MFA options are available?**

Organizations using MFA during our beta program need to set up Google Authenticator. After initial set up, users may optionally turn on text (SMS), call, or Okta Verify and use those instead.

**Is there a difference between two-factor and multi-factor authentication?**

Technically, yes—MFA allows for more than two factors. However, Classy will support two factors: a password and a one-time passcode.

**How is MFA different from SSO?**

SSO lets users access multiple applications with a single login. MFA requires an additional authentication step and can be used alongside SSO for extra security.

**How does this work if my organization already has an IDP (identity provider)?**

Classy’s multi-factor authentication solution is compatible through Google Authenticator, with the option to set up Okta Verify, and SMS/call. An IDP other than Google Authenticator or Okta Verify will not work for Classy’s MFA solution. We may consider verification through additional identity providers in future releases.

**How many failed attempts can be made, and what happens if that limit is reached?**

After five failed OTP attempts, the user’s account will be locked. To unlock it, contact our [Care team](https://support.classy.org/s/contactcare), who can unlock or reset authenticators via the Okta console.

**Can my organization configure which admins get prompted for MFA?**

No. Our out-of-the-box Okta solution applies MFA to all admins without customization options.

**Will MFA apply to Classy Live log-ins?**

Not at this time, but we may consider MFA for Classy Live in future updates.

**Will email be considered as an authentication factor?**

No. Due to phishing risks, email won’t be used as an authentication factor. We prioritize secure, industry-leading authentication options.

**What other factors will be considered for the future?**

We plan to expand our MFA options to include more authenticator app providers and potentially other secure factors.

**Is there any action required from the organization?**

Yes. Users will need to:

1. Download the Okta Verify mobile app.
2. Open the app and select “Add an account” or tap “[+]”.
3. Choose “Organization” and scan the QR code on the login screen.
4. Enter the one-time passcode on the Classy login screen.

**I don’t have a smartphone. How do I proceed?**

Contact our [Care team](https://support.classy.org/s/contactcare) who can help you set up text/call verification options.

**My organization doesn’t allow mobile devices at work. How do we proceed?**

If mobile devices are restricted, please contact us at multifactor@classy.org, and we’ll work with you to find a solution.

**Are there any known issues with the MFA solution?**

During testing, we found a bug with the SMS feature of MFA that causes two text messages to be sent to the user. The text messages will contain the same passcode, so it does not impact functionality and you will be able to use the passcode to login. A fix for this will be released before GA.
