# Credit Card Tokenization

When attendees register for an event on Classy, the purchaser provides a credit card during checkout. Credit card tokenization is a process that can save the purchaser's card information, removing the hassle of re-entering it at the event.

![Example of tokenization](https://learn.classy.org/rs/673-DCU-558/images/tokenization-example.png?version=0)

!!! example "Sign up for this beta program is currently closed"

    This feature will soon be released for an open beta. Stay tuned and we'll update you when it is available to sign up again.

## Current checkout process

Currently, Classy does not sync this card information to the event, and the purchaser must re-enter their information to participate in the auction or make donations at the event.

## Benefits of tokenization

Credit card tokenization makes it easy for attendees to use the same credit card they provided during registration.

By matching the purchaser's name and email to an attendee during checkout and then securely storing the payment details for the integrated event, the attendee's card is saved to their record for use at the event.

## Rules for tokenization

The card will only sync when the ticket purchaser's first name, last name, and email match the information of an attendee provided during registration. The payment information will not sync to Classy Live if more than one attendee has the same information as the purchaser.

## Examples

For instance, Classy Live will store the card information if Stacy Rushing purchased two tickets and one of the attendees' names is Stacy Rushing with the same email address.

However, it will not store the card information if Peter Park purchases tickets on behalf of Luna and Alex or if Wendy Adams purchases tickets and skips all the attendees' information.

## Functionality in Classy Live

When a card syncs to Classy Live, admins can view the attendees' payment method, checkout an attendee with the card on file, remove or add a payment method.

Attendees can view and use the payment method at the Classy Live event and also have options to add or remove a payment method if they have two on file.

## Frequently asked questions

**Can a purchaser opt out of credit card tokenization at checkout?**

Not yet, but this feature will be available for general availability.

**If attendees register for a campaign and it's connected to a Classy Live event later, will the provided credit card information sync to Classy Live?**

No, payment information will not sync retroactively.

**Does offline ticket payment information sync to Classy Live?**

No, offline tickets added through Classy do not have credit card information, so there isn't any payment information to sync.

**Are attendees notified that their credit card information syncs to Classy Live?**

There's a tooltip on all payment methods synced from Classy campaigns in the attendee's cart.
