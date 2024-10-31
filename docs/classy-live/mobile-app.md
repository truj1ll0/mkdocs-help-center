<style type="text/css" rel="stylesheet">
img { width: 50%; margin:auto!important; }

.md-typeset table:not([class]) td:not([align]), .md-typeset table:not([class]) th:not([align]) {
    text-align: left;
    vertical-align: text-bottom;
}

.md-typeset table:not([class]) {
    border: 0;
    border-radius: 19.8px;
}
</style>

# Classy Live Mobile App

Classy Live’s mobile app lets admins efficiently manage their events through easy-to-use check-in capabilities and integrations with Stripe’s M2 and WisePOS E card readers to add a payment method on file.

<div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><iframe src="https://fast.wistia.net/embed/iframe/kdrq775cv9?seo=true&videoFoam=true" title="Classy Live Mobile App + Reader M2 Video" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" msallowfullscreen width="100%" height="100%"></iframe></div></div>
<script src="https://fast.wistia.net/assets/external/E-v1.js" async></script>

!!! example "Want to participate?"

    <a href="https://learn.classy.org/classy-live-mobile-app-beta.html?utm_source=early_access_hub&utm_medium=microsite&utm_campaign=lighthouse_beta_programs">Sign up</a> to join the beta program for the Classy Live mobile app and M2 readers.

    To use the mobile app:
    - Your organization must not be using <a href="https://support.classy.org/s/article/federated-sso">Federated Single Sign-on (SSO)</a>.
    - You must have a compatible mobile device. View [compatibility requirements](#device-requirements).

## Download

The mobile app is available for download on smartphones and tablets. Visit your device’s app store to download:

- [iOS App Store](https://apps.apple.com/us/app/classy-live/id6457514197)
- [Android Apps on Google Play](https://play.google.com/store/search?q=classy%20live&c=apps&hl=en_US)

!!! warning "Important"

    You can only use the mobile app once accepted into the beta program. If you’ve already signed up, we’ll notify your organization when you can download the app.

## Log in

Once accepted into the program and downloaded the app, you can log in to begin managing your events.

To access your Classy Live account:

1. Enter your Classy email address and password
2. Tap **Sign in**

## M2 card reader

As part of the mobile app beta program, you can purchase Stripe's Reader M2 through Classy Live.

Here's how the M2 compares to the WisePOS E card readers:

|                     | ![WisePOS E](https://learn.classy.org/rs/673-DCU-558/images/wise-pos-e.png) </br>WisePOS E | ![Reader M2](https://learn.classy.org/rs/673-DCU-558/images/m2-reader.png) </br>Reader M2 |
| ------------------- | ------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------- |
| **Cost per device** | $282                                                                                       | $65                                                                                       |
| **Connectivity**    | WiFi                                                                                       | Bluetooth                                                                                 |
| **Feature**         | Add payment method                                                                         | Add payment method                                                                        |
| **Requirements**    | Password-protected WiFi network                                                            | Compatible smartphone or tablet with the Classy Live mobile app                           |

### Order a card reader

To purchase a reader:

1. Go to your Classy Live organization dashboard and select **Billing**
2. Under Card Reader Orders, select **Place Order**
3. Add the **Reader M2** to your cart
4. Enter shipping information and choose a shipping method
5. Enter your card info and process order

You'll receive updates about your order directly from Stripe.

## Add a card reader

You must add and connect card readers before using them to add attendees’ payment methods. The mobile app is compatible with Stripe’s M2 and WisePOS E card readers purchased through Classy Live.

[Learn more about card readers](/help-center/classy-live/reader-m2)

Before you start, ensure your card reader is fully charged, and you’ve turned on Bluetooth in your phone or tablet settings.

!!! note

    If you need to add a WisePOS card reader, make sure you’re connected to a password-protected WiFi network. Learn more about the [WisePOS E network requirements](https://support.classy.org/s/article/troubleshooting-card-readers#network).

To add a card reader to your event:

1. In the app, tap on the event
2. Tap the **Settings icon** in the top right corner
3. Tap **Add now**
4. Select a location and the device

!!! note

    Locations help ensure your reader has the correct regional settings. To [add device locations](https://support.classy.org/s/article/card-readers-on-classy-live#add-device-location), go to [Classy Live’s desktop site](live.classy.org).

5. Tap **Scan for available devices**.

Once recognized, the app will display a confirmation message.

!!! question "Need help connecting?"

    If your device and the M2 are not connecting, ensure Bluetooth and the Reader M2 are turned on. For more help, view [Stripe’s documentation on setting up the Stripe Reader M2](https://docs.stripe.com/terminal/payments/setup-reader/stripe-m2).

### Connect to the card reader

Once you’ve registered your device with the event, you can connect to it to start adding payment methods.

To connect your mobile device to the card reader:

1. On the Manage Card Readers screen, find your card reader
2. Tap the **three-dot menu** and select **Connect to device**

When the M2 is connected:

- The reader’s lights will flash four times.
- The first light will flash every 5 seconds.
- In the app, a star will appear next to the reader's name in the app.

Once connected, you can easily collect card information for attendees during check-in or after the event.

#### Device updates

When connecting to your M2 reader, you might be prompted to update. This is normal as Stripe regularly updates the reader's software. Wait for the update to complete, then connect to the card reader.

## Check-in with the mobile app

We recommend adding payment methods right at check-in, where you can also edit attendee details and send the attendee a link to the event’s auction page.

To check-in attendees:

1. In the app, select an event
2. Search for a specific attendee or filter attendees based on check-in status and ticket type

### QR code check-in

Tap **Scan Code** on the Attendees page to check in an attendee via QR code.

You’ll need to grant the app permission to use your device’s camera. Once allowed, you can scan the attendee’s QR code to check them in.

!!! note

    You can send QR codes to attendees via the event’s welcome message. Learn more about <a href="https://support.classy.org/s/article/sending-emails-and-SMS-to-your-attendees">messages on Classy Live</a>.

### Manual check-in

Tap **Check in** next to an attendee's name to check them in manually.

A success notification will appear with information about the attendees, such as their seating assignment, bidder number, and ticket type.

## Add payment method

To add a payment method when checking in an attendee:

1. Tap **Add Payment Method** or select **View Payment Methods** in the attendee's profile
2. Tap **Add from card reader** or **Manually add card**

### Add from card reader

To add a card via the card reader:

1. Scroll down and tap **Tap, swipe, or insert card**
2. Present the credit card using any of the three methods: tap, swipe, or insert.

When the card is accepted:

- You'll hear a beep.
- All the lights will turn on.
- For security reasons, the app will display asterisks in the Card Number field

Add a phone number, opt the attendee into auction notifications, and tap **Save**.

### Manually add card

If you don’t have a card reader or are having trouble connecting, tap **Manually add card** to enter the card details.

## Edit attendees

To edit attendee details in the mobile app:

1. Go to the event
2. Tap on the attendee's name or select **View Profile**

Then, you can edit their name, email, bidder number, phone number, notes, and custom question responses, plus you can opt them in to receive texts.

!!! note

    You cannot edit external bidders, or attendees added directly to Classy Live. We recommend adding [offline attendees](https://support.classy.org/s/article/manage-tickets-and-registrations#add-offline-tickets) to the Classy Campaign.

## Device requirements

To use the mobile app, your device must be either an:

- Apple device running iOS 14.0 or higher (released 2020)
- Android device running versions 8.0 or higher (released 2017)
  - Your Android device must also be NFC-compatible. [Find out if your device supports NFC](https://support.google.com/wallet/answer/12200245#checkNFC).

!!! question "Have feedback?"

    Let us know! [Fill out this form](https://classy.typeform.com/to/WD4msInJ) to report issues, make requests, or share positive notes.
