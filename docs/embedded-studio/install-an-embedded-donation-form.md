# Install an Embedded Donation Form

!!! example "Before you start"

    The steps to add an embedded form depend on your website builder. Check out our article for [WordPress](/embedded-studio/embed-a-donation-form-on-wordpress)

    **Note for Wix users:** Embedded Studio does not currently support Wix.

When installing an embedded form for the first time, you’ll complete two main steps:

1. Add the Install snippet to your website’s `<head>` section.
2. Add the form embed code to your pages.

You’ll find the Install snippet and embed code under **Settings** and **Install** in the campaign editor.

### Can I add embedded forms to my website?

Most website builders let you to add embedded forms. For specific steps, check your builder’s help center and search for topics like:

- Embed code
- Custom HTML
- Add external JavaScript

### Add the Install snippet to your website

The Install snippet is a script that lets embedded forms function on your site. You only need to add it once.

!!! warning "Important"

    Adding multiple Install snippets can slow down your site. Use only one Install snippet, even if you plan to embed multiple forms.

To add the Install snippet:

1. Go to the campaign’s **Settings** tab
2. Select **Installation**
3. Next to Install snippet, select **Copy**
4. Paste the snippet into your website’s `<head>` section

!!! tip

    If you can’t access the `<head>` section, try adding the snippet to the `<footer>` or using a custom code block on the page. We recommend the `<head>` for optimal performance.

### Add the form to your website

After adding the Install snippet, you’re ready to embed your campaigns.

#### Add a donate button

To create a donate button that opens the embedded form:

1. In the Studio builder, go to **Settings **and** Install**
2. Under **Donate button**, select **Copy campaign parameter**
3. In your website editor, paste the embed code in a custom HTML block

#### Place the form on the page

To embed the form directly on a webpage

1. In the Studio builder, select **Settings**
2. Select **Installation**
3. Under Inline donation grid, select **Copy inline embed code**
4. Go to your website’s editor
5. Paste the embed code inside a custom HTML block on your site

## Need help?

Check out our [troubleshooting article](/embedded-studio/troubleshooing-embedded-campaigns) for help when you run into any issues.
