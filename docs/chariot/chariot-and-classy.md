# Chariot and Classy

!!! example "To participate in the Chariot and Classy pilot program, you need to:"

    * Be a **current **Classy customer
    * Create a Chariot account
    * Add Donor Advised Fund as a checkout option on a **currently transacting Classy campaign**
    * Must be willing to test for 2-3 months with periodic check-ins

Classy’s comprehensive fundraising platform gives organizations the scalability and flexibility to create giving experiences that unlock generosity. Chariot’s Donor Advised Fund (DAF) solutions allow nonprofits to seamlessly accept DAF donations online and capture more of the $234 Billion sitting in these charitable giving accounts.

Through the Classy x Chariot integration, supporters have the ability to check out online with their DAF account. With this new payment option and simple, user-friendly flow, we hypothesize that nonprofits will:

- Increase donation volume
- Identify more high-value DAF donors
- Increase the size and frequency of their DAF gifts
- Capture more DAF donor information (email address and phone number)
- Increase their average gift size thanks to diversified giving options

## Set up Chariot

To set up the Chariot and Classy integration, you need to first register with Chariot, and then you’ll work with one of our partners, Cro Metrics, to add Chariot to your Classy account.

### Register with Chariot

To register with Chariot:

1. Visit their [signup page](http://app.givechariot.com/signup)
2. Create a username and password for your organization’s account
3. Provide some basic information such as your name and your nonprofit’s EIN
4. Select the **Integrations** tab and search for **Classy**
5. Select **Activate** to get started

### Add Chariot as a Payment Option

Classy is working with our long-time partner, Cro Metrics, to embed the DAF giving widget for pilot customers.

#### Setup within Classy

1. [Login to Classy](https://www.classy.org/)
2. Identify the transacting campaign you would like to embed the Chariot DAF widget
3. Share the campaign’s link with the Classy partners team ([partners@classy.org](mailto:partners@classy.org))

Classy and Cro Metrics will activate the widget for your identified campaign. Once activated, your campaign will display the DAF option to donors.

## Getting transaction data to flow into Classy

Chariot needs API keys from your Classy account to send donor data to Classy from each transaction. To do so:

### Create a Chariot application on Classy

To activate API Access for Chariot, you need to create a new Application on Classy:

1. In Classy’s menu, select **Apps & Extensions**
2. Select **Classy API**
3. Enter the name of your application: **Chariot**
4. Enter an Oauth2 Redirect URI: [https://www.givechariot.com/](https://www.givechariot.com/)
5. Check the terms of service checkbox
6. Select **Create App**

### Send the auth credentials to Chariot

Next, locate and send over the auth credentials to Chariot:

1. Locate the Chariot application you created in the **Your Applications** list and select **Edit**
2. Find the **Client ID** and **Client Secret**
3. Securely send them to Chariot using a secret-sharing service like [Doppler](https://share.doppler.com)
4. Set the credentials to expire in **three days**
5. Send to <developers@givechariot.com>

#### API Request URL

Chariot will use the following API to add offline donations to your Classy account.

```
https://api.classy.org/2.0/campaigns/:campaignId/trans
```

## Pilot Timeframe

_3 Months: November 1, 2023 - January 31, 2024_

Given that:

- DAF gift sizes are 24x larger than credit card gifts on average
- DAF gifts are[ resilient during economic downturns](https://www.givechariot.com/post/why-donor-advised-funds-matter-more-than-ever-during-a-recession)
- 20% of donors reconsider making a donation if they don’t see their preferred payment option

And,

- 30% of annual giving happens in December

The giving season is the optimal time to surface a DAF giving option to donors who are already inclined to give more.

## Customer Expectations

- Embed Chariot’s DAF experience on a transacting Classy donation page
- Participate in one kick-off call and 2-3 check-ins over the course of the pilot
- Provide honest feedback about the value of the integration
- Share metrics around:
  - Click rates
  - Giving mechanism success (venmo vs. DAF, for example)
  - Conversion rates
  - DAF average gift size
- Consenting to sharing anonymized transaction data
  - Total donation volume
  - Number of donations
  - Donations by payment method: # of donations & sizes
- Ability to add DAF language to marketing materials
- 1 DAF specific outbound marketing message/solicitation

## Pricing

All fees and costs associated with the Classy x Chariot integration will be waived for pilot participants. Post-pilot, Chariot charges a 2.9% donation processing fee.

## Frequently asked questions

**How long do DAF donations take to be distributed to my organization?**

Depending on the account and DAF provider, funds can take a few days to a few weeks.

[Learn more about the wait times for different providers](https://www.givechariot.com/donor-advised-fund-donation-wait-times)

**What DAF donor data will I receive?**

Your organization will receive all information the form collects, including name, email, and mailing address. You'll also receive a Chariot ID, a unique, 5-digit identifier accompanying the DAF gift, helping you reconcile the transaction.

**Do donors receive acknowledgment of their DAF donation post-giving?**

Chariot and Classy do not send the DAF acknowledgment. Instead, each DAF provider sends varying information. Some may send acknowledgment to the donor when the money is received, while others may communicate when the grant is initiated.

**How many DAFs are currently integrated?**

Chariot is integrated with 70% of the DAF market (by assets under management). Regarding numbers, Chariot has about 20 integrations, which account for the largest providers in the market.

**For DAFs that are not integrated, what is the process for making the gift? Does a supporter go directly to their site to log in?**

For DAFs that are not integrated, Chariot redirects donors back to the Classy form to choose an alternative method. However, there is also an option for a donor to be redirected to their DAF portal to donate. In this scenario, Chariot collects the name, email, and donation amount suggested by the donor. However, because these grants are manual, we cannot guarantee that the donor submitted them.

**Can you confirm that these donors will only receive a confirmation email from Classy, not a tax-deductible receipt?**

The donor **will not** receive an email or receipt from Classy when they complete a DAF donation via Chariot. Once the DAF donation is processed, the donor will be redirected to a standard Thank You page. The donor would receive an email notification from their DAF brokerage (e.g., Fidelity Charitable), which would be consistent with the donor experience if they made the grant request directly from their DAF account.

**For the Classy reporting, would we receive the donor-advised fund name (i.e., Kohl Fund at Fidelity)?**

Currently, Classy will only receive the name of the Donor Advised Fund (i.e., Fidelity, Schwab) and the donor's information on the Classy form (First, Last, Email). The check or EFT will come with the Fund Name on the DAF side.
