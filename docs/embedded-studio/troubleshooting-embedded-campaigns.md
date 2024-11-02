# Troubleshooting embedded campaigns

In this article, you’ll find common issues you may encounter with Embedded Studio campaigns and steps to resolve them.

## Error: We can’t seem to find that page

This error message likely means your campaign isn’t published.

**To publish your campaign**:

1. Go to the campaign’s designer
2. Select **Publish** in the header to make the form live

## Error: Classy refused to connect

This error usually indicates that your website’s domain is not safelisted. To display the donation form, you need to safelist each domain where the form will appear, including test sites, preview pages, and sandbox environments.

**To safelist your site**:

1. Go to your campaign’s designer
2. Select the **Settings** tab
3. Choose **Install**
4. Under **Safelisted domains**, add the URL of each site where you plan to display the form
5. Select **Update** in the header to push through the changes
