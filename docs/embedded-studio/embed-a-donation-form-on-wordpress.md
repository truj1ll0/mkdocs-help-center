# Embed a Donation Form on WordPress

To embed a donation form on your WordPress site:

1. Safelist your website
2. Install the code snippet
3. Add the donation form to a page

## Safelist your website

To make sure your embedded form appears, safelist your website. If you need to add multiple domains (such as a test site or sandbox), follow these steps:

1. Go to the **Settings** tab in the Studio designer
2. Select **Install**
3. Under **Safelisted domains**, add the URL of each website where you plan to embed the form
4. **Publish** or **Update** your campaign to push through the changes

## Install a code snippet

The Install snippet is a script that lets embedded campaigns appear on your site. You only need to add it once to your website’s `<head>` section, where it will work for all embedded campaigns.

!!! warning "Important"

    Only add one Install snippet. Multiple snippets may slow down your website.

**To copy the Install snippet**:

1. Go to the campaign’s **Settings** tab
2. Select **Install**
3. Next to **Install snippet**, select **Copy**

### Using WPCode to add the snippet

We recommend using the WPCode plugin to easily add the Install snippet to your WordPress site’s header.

**To install WPCode:**

1. Log in to WordPress
2. In the menu, go to **Plugins** and **Add New**
3. Search for **WPCode – Insert Headers and Footers + Custom Code Snippets**
4. Select **Install and activate**

![Add WPCode plugin](https://learn.classy.org/rs/673-DCU-558/images/wordpress-add-wpcode.gif)

!!! note

    If you don't have the **Plugins** option, your account doesn't have the necessary permissions to add plugins. Reach out to your team to get access.

**To add the snippet using WPCode**:

1. After installing WPCode, go to **Code Snippets **and** Header & Footer**
2. Under **Header**, paste the Install snippet
3. Select **Save changes**

Once the Install snippet is saved, you can add multiple embedded forms to your website without changing the snippet.

### Add the donation form to your website

With the Install snippet added, you’re ready to embed your donation form. You can place the form directly on the page or attach it to a button.

**Options for embedding the donation form**:

- **Donate button**: Add a button that opens the embedded form when selected.
- **Inline donation grid**: Embed the form directly on the page.

**To embed the form on a page**:

1. Go to your WordPress site’s editor
2. Add a **Custom HTML** block in the location where you want to place the form
3. In your campaign’s **Install** page, copy either:
   - The **Donate button** campaign parameter, or
   - The **Inline donation grid** embed code
4. Paste the code into the Custom HTML block, then **Save** and **Publish** the page

![WordPress HTML block](https://learn.classy.org/rs/673-DCU-558/images/wordpress-custom-html-block.png)

When viewing the page, supporters will have either a donate button or an inline donation grid. Selecting either option will open the embedded form in an overlay.

!!! tip

    Share a direct link to your form by attaching the campaign parameter to your URL (e.g., `https://yournonprofit.org/?campaign=12345`). This will open the form as soon as visitors land on the page.
