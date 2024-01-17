# Set up Domain Masking

Domain mask your campaign’s URLs to replace `classy` with a domain of your choice.

A typical Classy campaign may appear as:

https://**www.classy**.org/give/123456/#!/donation/checkout

While a domain-masked campaign can appear as:

https://**give.santafepantry**.org/give/123456/#!/donation/checkout

Organizations often choose to replace the Classy domain with their website’s name. This helps create a consistent branded experience for supporters.

!!! example "To setup domain masking, you need:"

    * **Organization administrator** access in Classy
    * a Domain name
    * (Optional) a Favicon

You’ll start in your domain provider’s settings where you will choose a CNAME, point it towards `vanity.classy.org`, and then return to Classy to complete the setup.

## Choose a CNAME

A canonical name (CNAME) record maps an alias name to a canonical domain name. CNAME records usually map subdomains like _www_ to the domain that hosts the subdomain content.

For example, a CNAME record can map the address `www.classy.org` to the actual site for the domain, `classy.org`.

When you create a CNAME record for domain masking, you get to choose the subdomain that will replace ‘www’ in your campaign’s URL.

We recommend using a simple term that makes sense for all campaign pages such as, “give”.

![example of a domain masked url with a unique CNAME](https://learn.classy.org/rs/673-DCU-558/images/cname-url.png)

If you already have a CNAME and any existing page rules, redirects, or paths on your domain that you expect to be valid after the cutover, reach out to our [Care Team](https://support.classy.org/s/contactcare).

## Set up a CNAME

Next, you’ll need to create a corresponding CNAME record for your web address and associate it with `vanity.classy.org`.

1. Sign in to your domain provider’s site
2. Go to your domain’s DNS records
3. Create a CNAME record that points your domain to `vanity.classy.org`

Common fields you’ll encounter:

- **Alias** - Enter the subdomain you chose such as “give”
- **Type** - Enter `CNAME`
- **Points to**- Enter `vanity.classy.org`

CNAME record changes may take up to 48 hours to take effect.

!!! question "How do I set up a CNAME with my domain provider?"

    The process will depend on the domain provider you use. Here are guides for some of the popular providers:

    * [Domain.com](https://www.domain.com/help/article/dns-management-how-to-update-cname-aliases)
    * [GoDaddy](https://www.godaddy.com/help/add-a-cname-record-19236?)
    * [Google Domains](https://support.google.com/domains/answer/9211383?hl=en)
    * [Bluehost](https://my.bluehost.com/hosting/help/cname)
    * [Hover](https://help.hover.com/hc/en-us/articles/217282457-Managing-DNS-records-)
    * [Namecheap](https://www.namecheap.com/support/knowledgebase/article.aspx/9646/2237/how-to-create-a-cname-record-for-your-domain)

### Confirm CNAME setup

Once you create your CNAME record and point it to `vanity.classy.org`, you can confirm setup using MxToolbox.

1. Go to the [CNAME Lookup Tool](https://mxtoolbox.com/CNAMELookup.aspx)
2. In the search field, enter your domain with your new CNAME (E.g. give.santafepantry.org) and select **CNAME Lookup**
3. Under Canonical Name, confirm it shows `vanity.classy.org`

## Complete setup in Classy

To complete domain masking:

1. In your Classy account, select **Settings** and **Account**
2. Next to Domain Masking, select **Edit**
3. Enter your CNAME, CNAME redirect URL, a link to your Favicon, and **Save**

For example:

**CNAME:** give.santafepantry.org

**CNAME redirect URL:** https://give.santafepantry.org

![Domain masking settings](https://learn.classy.org/rs/673-DCU-558/images/example-domain-masking-settings.png?version=0)

Your campaign URLs are now domain-masked! Existing campaign URLs will redirect to the new domain.

!!! warning "Important"

    Short URLs set up before you set up domain masking will not redirect and will no longer work. Be sure to replace any Short URLs you currently have in use.

    [Learn more about Short URLs](https://support.classy.org/s/article/edit-your-campaign-details#short-url)

## Frequently asked questions

**Why can't I access my campaign?**

Some organizations have trouble accessing campaigns after setting up domain masking.

This is usually fixed by allowing `vanity.classy.org` within the network settings or confirming you are not pointing to a specific IP address.

**What are some other subdomain suggestions?**

We recommend subdomains that make sense across all your Classy campaigns year-round since this will appear on all campaign URLs.

Popular choices include:

- Give
- Fundraise
- Support
- Impact

**How do I find the URL for my website’s favicon?**

If you can’t find a URL to your website’s favicon, you can use [Favicon Finder](http://www.faviconfinder.com/) to help you.

1. Go to [faviconfinder.com](http://www.faviconfinder.com/)
2. Enter your organization’s website URL
3. Right-click on the image and select **Open Image in New Tab**
4. Copy the URL in the address bar

**Can I remove domain masking?**

Yes. To remove domain masking:

1. In Classy, Select **Settings** and **Account**
2. Scroll down to **Domain Masking**
3. Next to Remove domain mask, select **Remove**

When you remove domain masking, your campaign’s URL will revert to its original (E.g. https://www.classy.org/give/123456/#!/donation/checkout).

**Can I change the CNAME after I set up domain masking?**

Yes, you will first need to remove domain masking in your account and then go through the process to set it up again.

Campaign URLs using the original CNAME will no longer work.
