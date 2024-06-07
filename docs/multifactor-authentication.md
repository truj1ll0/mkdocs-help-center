# Multifactor authentication

Multi-factor authentication (MFA) is a user verification method that requires more than one type of user validation, such as a password and a one-time passcode (OTP). It helps prevent unauthorized account access even if someone has acquired the username and password.

During Early Access, you can use MFA for your organization’s Classy account. This will require admins to enter their password and OTP via the Okta Verify app on a mobile device to access your account.

!!! example "To use MFA on Classy, you need:"

    * A computer
    * A smartphone
    * Okta Verify downloaded on your device
      * <a href="https://itunes.apple.com/ca/app/okta-verify/id490179405">iPhone</a>
      * <a href="https://play.google.com/store/apps/details?id=com.okta.android.auth">Android</a>

    <strong>Want to participate?</strong>

    <a href="https://learn.classy.org/mfa-beta-program.html">Sign up</a> to join the waitlist for Bulk Close of Balances on Classy Live.

## Why is MFA important?

MFA significantly reduces the risk of unauthorized access compared to passwords alone. It is an industry best practice and a critical component of a comprehensive security strategy against increasingly sophisticated cyber attacks.

MFA can also help you:

- Comply with regulatory requirements
- Protect sensitive data
- Prevent identity theft

## Set up MFA

!!! note

    If you’re a new Classy admin, select the button in the ‘Claim your account’ email sent to your address to set up your account for the first time.

You need a smartphone to set up MFA for your account.

To set up MFA:

1. Start setup on your computer and log in to [Classy](https://www.classy.org/sso) using your username and password
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

# Frequently asked questions

**Is MFA required?**

MFA will be required for all organizations and admins using Classy when the feature reaches general availability (GA).

**Does MFA also apply to Classy Live?**

Not at this time.

**Can I use another authentication app or method?**

OTP via the Okta Verify app is the only authentication we currently support.

**Where can I download the Okta Verify app?**

This depends on your device type. For iPhones, visit the [Apple App Store](https://itunes.apple.com/ca/app/okta-verify/id490179405). For Android, visit the [Google Play Store](https://play.google.com/store/apps/details?id=com.okta.android.auth).

**Will it prompt me for a passcode every time I log in?**

Okta Verify will prompt you to enter an OTP at least once daily and again if you log in with a different device or browser.

**What if I don’t have a smartphone?**

We plan to release support for SMS/text messaging via Twilio soon. In any case, you must have a cell phone to access Classy as an admin.

**Will supporters need to use MFA to access their accounts?**

No, supporters will not have MFA support for their accounts. They can continue to use their password or a one-time code sent to their email address to sign in.

**How is MFA different from SSO?**

Single Sign-On (SSO) lets users access multiple applications or websites with one set of credentials. MFA requires users to input more than one type of authentication credential.

**Is there a difference between two-factor authentication and multifactor authentication?**

Not really. Multifactor authentication allows for the possibility of more than two factors. However, Classy only supports two factors (password and one-time passcode).
