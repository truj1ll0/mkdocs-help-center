<style type="text/css" rel="stylesheet">
img { width: 50%; margin:auto!important; }
</style>

# Multifactor authentication

Multi-factor authentication (MFA) is a user verification method that requires more than one type of user validation, such as a password and a one-time passcode (OTP). It helps prevent unauthorized account access even if someone has acquired the username and password.

During Early Access, you can use MFA for your organization’s Classy account. This will require admins to enter their password and OTP via the Okta Verify app on a mobile device to access your account.

!!! abstract "To use MFA on Classy, you need:"

    * A computer
    * A smartphone
    * Okta Verify downloaded on your <a href="https://itunes.apple.com/ca/app/okta-verify/id490179405">iPhone</a> or <a href="https://play.google.com/store/apps/details?id=com.okta.android.auth">Android</a> device

    **Want to participate?**

    [Sign up to join Classy's MFA beta program.](https://learn.classy.org/mfa-beta-program.html?utm_source=early-access&utm_medium=help-center&utm_campaign=beta-program)

## Why is MFA important?

MFA significantly reduces the risk of unauthorized access compared to passwords alone. It is an industry best practice and a critical component of a comprehensive security strategy against increasingly sophisticated cyber attacks.

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

3. Select your device type (iPhone or Android)
4. Download the Okta Verify app on your smartphone and select **Next**
5. Open the Okta Verify app on your device and select **Add an account or [+] button.**
6. Select **Organization**
7. Scan the QR code on the login screen with your smartphone
8. An OTP will display on your device
9. Enter the OTP on the Classy login screen and **Verify**

You’ll be successfully logged into Classy. At least once a day, you’ll need to enter the OTP via Okta Verify to log into your account.

## Log in with MFA

To log in with MFA:

1. Log in to Classy using your username and password
2. Enter the one-time passcode provided in the Okta Verify app on your smartphone
3. Select **Verify**

![Verify with a one-time passcode](https://learn.classy.org/rs/673-DCU-558/images/mfa-enter-otp.png)

And you’re in! We recommend marking the checkbox so we don't challenge you again on this device for 24 hours.

If you need help, check out Okta’s documentation for your device:

- [iPhone](https://help.okta.com/eu/en-us/content/topics/end-user/ov-new-install-qr-ios.htm)
- [Android](https://help.okta.com/eu/en-us/content/topics/end-user/ov-new-install-qr-android.htm)

!!! warning "Important"

    After five failed login attempts, you’ll be locked out of your account. Contact our [Care team](https://support.classy.org/s/contactcare) to restore access.

## Frequently asked questions

**Is MFA required?**

Yes. MFA will be required for all Classy users starting in February 2025. At that time, users must use MFA to log in.

**Why is MFA required?**

Classy is committed to top security standards. MFA helps prevent unauthorized access by adding an extra layer of protection to your account.

**Is there any additional cost associated with MFA?**

No. MFA is a security requirement, so there is no extra cost for customers.

**Will supporters need to use MFA to access their accounts?**

No, supporters will not be required to use MFA. They can continue to log in using their password or a one-time code sent to their email.

**How often will an organization need to use MFA?**

Organizations will need to log in with MFA once per day for each browser they use (e.g., once for Chrome, once for Safari).

**Can organizations configure the frequency of MFA?**

No. We’re using Okta’s out-of-the-box solution, so any changes must go through our product or support teams.

**What types of MFA options are available?**

Currently, the Okta Verify app with a one-time passcode (OTP) is available in our beta program. When MFA launches in February 2025, SMS will be an additional option.

**Is there a difference between two-factor and multi-factor authentication?**

Technically, yes—MFA allows for more than two factors. However, Classy will support two factors: a password and a one-time passcode.

**How is MFA different from SSO?**

SSO lets users access multiple applications with a single login. MFA requires an additional authentication step and can be used alongside SSO for extra security.

**If my organization already uses Classy’s SSO solution, will we also need to use MFA?**

Yes. Currently, there are no exceptions for organizations using SSO. All admins will need to use MFA.

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

**How does this work if my organization already has an identity provider (IDP)?**

Currently, Classy’s MFA only supports Okta Verify and, starting in February 2025, SMS. Other IDPs are not supported but may be considered in future updates.

**Is there any action required from the organization?**

Yes. Users will need to:

1. Download the Okta Verify mobile app.
2. Open the app and select “Add an account” or tap “[+]”.
3. Choose “Organization” and scan the QR code on the login screen.
4. Enter the one-time passcode on the Classy login screen.

**I don’t have a smartphone. How do I proceed?**

Once MFA is generally available, SMS will be an alternative option for users without smartphones.

**My organization doesn’t allow mobile devices at work. How do we proceed?**

If mobile devices are restricted, please contact us at multifactor@classy.org, and we’ll work with you to find a solution.
