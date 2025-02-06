<style type="text/css" rel="stylesheet">
img { width: 50%; margin:auto!important; }
</style>

# Multifactor authentication

Multifactor authentication (MFA) is a user verification method that requires more than one type of validation, such as a password and a one-time passcode (OTP). It helps prevent unauthorized account access even if someone has the username and password.

During Early Access, you can use MFA for your organization’s Classy account. This will require admins to enter their password and OTP via Google Authenticator on a mobile device to access your account.

Want to preview the set up experience? [View this Storylane walkthrough](https://app.storylane.io/share/eqzllyenh5tm)

!!! abstract "To set up and use MFA, you'll need a:"

    * Computer
    * Phone

    **Want to participate?**

    [Sign up to join Classy's MFA beta program.](https://learn.classy.org/mfa-beta-program.html?utm_source=early-access&utm_medium=help-center&utm_campaign=beta-program)

## Why is it important?

MFA reduces the risk of unauthorized access compared to passwords alone. It's an industry best practice and a critical component in safeguarding user and supporter data.

MFA can also help you:

- Comply with regulatory requirements
- Protect sensitive data
- Prevent identity theft

## MFA options

When first setting up MFA, you can choose your preferred authentication option. Classy supports:

- Google Authenticator ([iPhone](https://apps.apple.com/us/app/google-authenticator/id388497605) or [Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_US))
- Okta Verify ([iPhone](https://apps.apple.com/us/app/okta-verify/id490179405) or [Android](https://play.google.com/store/apps/details?id=com.okta.android.auth&hl=en_US))
- Call or text verification (Recommended if you do not have a smartphone)

## Set up MFA

!!! note

    If you’re a new Classy admin, select the button in the ‘Claim your account’ email sent to your address to set up your account for the first time.

To set up MFA:

1. Start on your computer and log in to [Classy](https://www.classy.org/sso) using your username and password
2. You’ll be prompted to set up multifactor authentication. Select **Setup** under your preferred option.

![Setup multifactor authentication](https://learn.classy.org/rs/673-DCU-558/images/set-up-security-methods.png)

3. Follow the prompts to verify
4. Select **Finish**

You've successfully set up multifactor authentication! From now on, you'll need to provide a verification code from your chosen app or phone, at least once a day, to log into your account.

!!! note

    Before you finish, you'll be prompted to set up an additional security method. **This step is optional** and you only need one authenticator to access your account.

    However, you will not be able to set up additional security options after you select **Finish**.

## Log in with MFA

To log in with MFA:

1. Log in to Classy using your username and password
2. Enter the verification code provided in your chosen authenticator app or phone
3. Select **Verify**

## Frequently asked questions

**Is MFA required?**

Yes. MFA will be required for all Classy admins starting in the first half of 2025. Your organization will be notified before MFA is required for your account.

**Is there any additional cost associated with MFA?**

No, there is no extra cost.

**Will supporters need to use MFA to access their accounts?**

No, supporters will not be required to use MFA. They can continue to log in using their password or a one-time code sent to their email.

**How often will an organization need to use MFA?**

Organizations will need to log in with MFA once per day for each browser they use (e.g., once for Chrome, once for Safari).

**Can organizations configure the frequency of MFA?**

No, not at this time.

**Is there a difference between two-factor and multi-factor authentication?**

Technically, yes—MFA allows for more than two factors. However, Classy will support two factors: a password and a one-time passcode.

**How is MFA different from SSO?**

SSO lets users access multiple applications with a single login. MFA requires an additional authentication step and can be used alongside SSO for extra security.

**How does this work if my organization already has an IDP (identity provider)?**

Classy’s multi-factor authentication solution is compatible through Google Authenticator, Okta Verify, and SMS/call.

An IDP other than Google Authenticator or Okta Verify will not work for Classy’s MFA solution. We may consider verification through additional identity providers in future releases.

**How many failed attempts can be made, and what happens if that limit is reached?**

After five failed OTP attempts, the user’s account will be locked. To unlock it, contact our [Care team](https://support.classy.org/s/contactcare), who can unlock or reset authenticators via the Okta console.

**Can my organization configure which admins get prompted for MFA?**

No. Our out-of-the-box Okta solution applies MFA to all admins without customization options.

**Will MFA apply to Classy Live log-ins?**

Not at this time, but we may consider MFA for Classy Live in future updates.

**Will email be considered as an authentication factor?**

No. Due to phishing risks, email won’t be used as an authentication factor. We prioritize secure, industry-leading authentication options.

**My organization doesn’t allow mobile devices at work. How do we proceed?**

If mobile devices are restricted, please contact us at multifactor@classy.org, and we’ll work with you to find a solution.
