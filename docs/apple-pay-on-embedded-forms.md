# Add Apple Pay to Embedded Donation Forms

You need to verify the domain where you plan to use Apple Pay to add it to your embedded donation forms. To verify the domain, add the [domain association file](https://stripe.com/files/apple-pay/apple-developer-merchantid-domain-association) to your website's file structure and contact our [Care team](https://support.classy.org/s/contactcare).

This is a security feature made by Apple to ensure that only authorized merchants process payments.

## General instructions

To verify your domain on most website providers:

1. Download the [domain association file](https://stripe.com/files/apple-pay/apple-developer-merchantid-domain-association)
2. On your website, host the file at `/.well-known/apple-developer-merchantid-domain-association`
3. Contact our [Care team](https://support.classy.org/s/contactcare) to complete verification and add Apple Pay to your forms

For example, if your website is `https://website.org`, make that file available at `https://website.org/.well-known/apple-developer-merchantid-domain-association`.

You should have your website admin create a new folder called `.well-known` and place the domain association file inside the folder.

We recommend contacting your website administrator or provider if you need help hosting the file on your website.

!!! note

    Apple Pay is available on Apple devices with Safari 17 or later and at least one valid card linked.

## WordPress

You can transfer files using [SFTP](https://wordpress.com/support/sftp/) and your preferred client program to host the domain association file on your WordPress site.

However, we recommend using the [File Manager plugin](https://wordpress.org/plugins/wp-file-manager/) to upload and host the file easily.

To add the File Manager plugin:

1. Go to your WordPress site’s Dashboard
2. In the menu, select **Plugins** and **Add New**
3. Search for and install **File Manager**

![Install file manager plugin](https://learn.classy.org/rs/673-DCU-558/images/edf-apple-pay-file-manager-plugin.png?version=1)

4. Once installed, select **Activate**

Now, you’ll have a new option for **WP File Manager** in your menu. This plugin lets you easily create folders and upload files to your site.

To upload the domain association file:

1. In the menu, select **WP File Manager**
2. Select the **Create New Folder** icon and name it `.well-known`
3. Within `.well-known`, create a new folder and name it `apple-developer-merchantid-domain-association`
4. Select the **Upload File** icon and upload the [domain association file](https://stripe.com/files/apple-pay/apple-developer-merchantid-domain-association)

![Using the file manager plugin](https://learn.classy.org/rs/673-DCU-558/images/edf-apple-pay-using-file-manager.png?version=0)

5. Contact our [Care team](https://support.classy.org/s/contactcare) to complete the verification

## Squarespace

Squarespace sites host the required domain association file by default.

Contact our [Care team](https://support.classy.org/s/contactcare), and they can activate Apple Pay for your embedded form.
