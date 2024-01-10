# Add Apple Pay to Embedded Donation Forms

Apple requires all merchants to host a verification file on their domain(s) to ensure that Apple Pay payments are only processed by authorized merchants.

Domain verification helps to prevent fraudulent use of Apple Pay and protects donors from unauthorized transactions.

To add Apple Pay as a payment option on your embedded donation forms, you must verify the domain where it will be used.

To verify your domain:

1. Download the [domain association file](https://stripe.com/files/apple-pay/apple-developer-merchantid-domain-association)
2. On your website, host the file at `/.well-known/apple-developer-merchantid-domain-association`
3. Contact our [Care team](https://support.classy.org/s/contactcare) to verify your domain

For example, if your website is `https://website.org`, make that file available at `https://website.org/.well-known/apple-developer-merchantid-domain-association`.

You should have your website admin create a new folder called `.well-known` and place the domain association file inside the folder.

We recommend contacting your website administrator or provider if you need help hosting the file on your website.

!!! note

    Apple Pay is available on Apple devices with Safari 17 or later and at least one valid card linked.

## WordPress

You can transfer files using [SFTP](https://wordpress.com/support/sftp/) and your preferred client program to host the domain association file on your WordPress site.

However, we recommend using the [File Manager plugin](https://wordpress.org/plugins/wp-file-manager/) to upload and host the file easily.

## Squarespace

Squarespace sites host the required domain association file by default.

Contact our [Care team](https://support.classy.org/s/contactcare), and they can activate Apple Pay for your embedded form.
