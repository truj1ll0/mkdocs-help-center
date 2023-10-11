---
search:
  exclude: true
---

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
3. Securely send them to Chariot (you can use a secret-sharing service like [Doppler](https://share.doppler.com)).

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
