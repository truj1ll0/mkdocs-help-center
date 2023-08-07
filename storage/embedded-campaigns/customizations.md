# Embedded Form Customizations

Learn about additional customizations you can make to your embedded forms.

## Donation settings

You can add more donation options to your form such as the ability to give with company credit cards and dedicate gifts to others. To access these settings:

1. Open the campaign editor
2. Select the Details tab
3. In the menu, select Donation Page to turn on or off settings such as comments and simple billing address. Also, select Theme to adjust the form’s logo and primary color.

## Nudges

Nudges give you two additional revenue-driving features to convert more visitors into lasting donors.

### Abandoned cart nudges

You can encourage supporters to complete their donation with friendly abandoned cart notifications that appear when supporters exit the popup checkout flow.

Note: Abandoned cart nudges are only available with popup donation forms.

To add an abandoned cart nudge to your form, copy the following code and add it to your code embed where it says // ADD ABANDON CART NUDGE CODE HERE TO ENABLE.

Then add the code to your website's footer.

        nudgeTrays: [
        // CUSTOMIZE YOUR MESSAGE
        {
          title: 'Make a difference 💜',
          content: 'Complete your gift to help make our mission possible.',
          ctaLabel: 'Give Now',
          ctaColor: '#1a73e8',
          triggerEvent: 'eg:donation:incomplete',
        },
      ],

### Recurring nudges

Use recurring nudges to help turn one-time gifts into sustainable, monthly donors. This nudge works by suggesting a smaller monthly donation when someone chooses a one-time gift amount between your highest and lowest options. The suggested amount will be one-fourth of the one-time amount.

### Recurring nudges for popup and inline donation forms

To add a recurring nudge, add egrn: true between the urlParams brackets in your code embed.

     urlParams: { egrn: true }

If you plan to use recurring nudges and source codes or pass-through parameters, replace urlParams: { egrn: true } with

     urlParams: { ...readURLParams(), ...{ egrn: true } },

**Can I use both nudges with popup embeds?**

Yes! Just add both the abandoned cart tray and the recurring giving nudge to their respective locations in the code embed.

## Source codes and pass-through parameters

To use source codes and pass-through parameters with your embedded donation page, you'll first need to edit your code embed.

In your code embed, find `urlParams: { },` and replace it with `urlParams: readURLParams(),`

Now, URL parameters you add will pass through to the embedded donation form.

### Source codes

To use source codes with your embedded donation form, add the source code to the URL you share with supporters. This URL should take supporters to the page where they are most likely to interact with the embed, like your homepage.

If the supporter navigates to another page before interacting with the embed, the source code will not pass on to Classy.

For example, if you think supporters are most likely to interact with your embed on your homepage, https://npo.org, you should share that URL with the source code attached. Such as, https://npo.org/?c_src=newsletter. If the supporter moves to https://npo.org/our-impact before they interact with the embed, the source code will not pass on.

Learn more about source codes

### Pass-through parameters

You can use pass-through parameters with your embedded donation forms, but you'll need to add the ones you want to use to your code embed.

In your code embed, find `const validUrlParams = ['c_src', 'c_src2']`

On this line, add the pass-through parameters you plan to use, such as:

     const validUrlParams = ['c_src', 'c_src2', 'amount', 'recurring', 'designation'];

Then, add the pass-through parameter to the URL you share with supporters. For example, https://npo.org/?amount=50

Learn more about pass-through parameters

## Collect billing address

You can collect billing addresses on embedded forms in two ways, simple billing address or full billing address. We recommend simple billing address because it uses a single auto-complete field for a streamlined donation experience.

### Simple billing address

To use simple billing address, go to Details and Donation Page in your campaign editor. Then turn on the option for simple billing address.

Note: if you use simple billing address, it will override full billing address. So if you'd rather use full billing address, be sure to leave simple billing address turned off.

### Collect full billing address

To require a supporter's full billing address, enter egfa: true between the urlParams brackets.

     urlParams: { egfa: true }

This will prompt supporters to enter their billing address after they have entered their payment details. Note that the billing address will not be captured for supporters who use digital wallets and do not have a billing address saved in their wallet.

If you have already included the recurring nudge parameter, separate each with a comma.

     urlParams: { egrn: true, egfa: true }

If you plan to use source codes or pass-through parameters, replace urlParams: { egrn: true, egfa: true }, with

     urlParams: { ...readURLParams(), ...{ egfa: true, egrn: true } },

## Use more than one campaign

If you'd like to add more than one campaign to your website, for example, if you want to include both a pop-up and an inline embed, you can edit your code embed to include multiple campaigns.

To add another campaign to your embed code snippet, find campaigns:, and then duplicate the segment within the square brackets [ ] and separate the two segments with a comma. Finally, replace the Campaign ID and the element selector with the ones you want to use for the other campaign.

```js
campaigns: [
  {
    campaignId: "YOUR CAMPAIGN ID",
    donation: {
      modal: {
        urlParams: {},
        elementSelector: "SELECTOR FROM YOUR WEBSITE" /* (1) */,
      },
      // Add ABANDON cart NUDGE Code Here to enable
    },
  },
  {
    campaignId: "YOUR OTHER CAMPAIGN ID",
    donation: {
      modal: {
        urlParams: {},
        elementSelector: "ANOTHER SELECTOR FROM YOUR WEBSITE",
      },
      // Add ABANDON cart NUDGE Code Here to enable
    },
  },
];
```

1. Does this work?

When you need additional help, view this complete example. Copy and paste this code snippet directly into your website's footer. Remember to replace the campaign IDs and element selectors.

Important: Add only one code embed to your website's footer. If you add more than one code embed, your website will only read the last one entered, and the earlier embeds will not work.

###Lazy load

By default, embedded forms load in background on page load. This allows popup forms to open instantly when a supporter selects Donate.

If you plan to use multiple embedded campaigns on one page, this will slow down your page load. To fix this, you can adjust your campaigns to lazy load. This means the embedded form will only load when selected instead.

To set your embedded campaign to lazy load, add lazyLoad: true, to the campaign snippet in your embed code.

              {
                campaignId: "123456",
                donation: {
                  modal: {
                    lazyLoad: true,
                    urlParams: { },
                    elementSelector: '.donate-btn'
                  },

## Use more than one button

If you used your donation page URL as your button selector, you can link any button on your website to that same donation page and the popup donation form will open.

However, if you added another selector, you can use multiple buttons by separating each selector with a comma in the code embed. For example:

    elementSelector: '.donate-btn, .donate-btn2'

**Have a customization in mind that’s not listed?**

Let us know via our feedback forum.
