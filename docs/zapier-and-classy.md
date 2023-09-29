# Zapier and Classy

Classy’s native integration with Zapier allows organizations to integrate with 5,000+ web applications and automate workflows. Classy customers leveraging Zapier will benefit from fluid data that is not isolated, helping organizations save time by avoiding manual work and opening up new opportunities for integrations without building from scratch using the public API.

Customers will also benefit from data visibility across their organization, keeping staff aligned on how donors interact with them and ensuring everyone on the team is on the same page and communicates effectively with their supporter base.

!!! abstract "Requirements"

    - Admin access to your organization’s Zapier account to set up new Zaps
    - **Once accepted into the lighthouse program:** Classy will give access to the Zapier integration in your Classy account.
    - Included in the Professional and Advanced subscription plans
        - $17/month fee for Essentials plans

!!! example "Want to participate?"

    <a href="https://learn.classy.org/beta-zapier-integration-sign-up.html?utm_source=early_access_hub&utm_medium=microsite&utm_campaign=lighthouse_beta_programs">Sign up</a> to join the waitlist for the Zapier integration in Classy.

## **Activate Zapier in Classy**

To activate Zapier in your Classy account, you will need administrator permissions.

1. In Classy, select **Apps & Extensions**
2. Select **Zapier**
3. Select **Generate credentials**

![Zapier app in Classy](https://learn.classy.org/rs/673-DCU-558/images/zapier-classy-overview.png)

4. Under **Integration details**, you’ll have an organization ID, client ID, and API key.

You’ll need to copy and paste these details into Zapier in a moment, so keep this window open.

![Zapier credentials in Classy](https://learn.classy.org/rs/673-DCU-558/images/zapier-classy-credentials.png)

## **Connect Classy to your Zapier account**

There are two ways to connect Classy to your Zapier account:

- Through **My apps** in Zapier
- Or, in the **Zap editor**

Then, you can **add a new connection** or **update an existing connection.**

[Learn more about connecting app accounts in Zapier](https://help.zapier.com/hc/en-us/articles/8496258785421)

### **From My apps**

To connect Classy through My apps:

1. In the Zapier account menu, select **Apps**
2. Select **Add connection**

![Add connection button in Apps](https://learn.classy.org/rs/673-DCU-558/images/zapier-apps-add-connection.png)

3. Under **App name**, enter **Classy** and select version 1.6.0. _For lighthouse customers, Classy will share a link to a private app for you to test_.
4. A pop-up window will appear asking if you want to Allow Zapier to access your Classy app account

![Allow access modal in Zapier](https://learn.classy.org/rs/673-DCU-558/images/zapier-allow-access.png)

5. Copy and paste the **Client ID**, **Client Secret (API Key in Classy)**, and **Organization ID** generated in Classy into these fields
6. Select **Yes, Continue**

Now that you’ve entered your credentials and added Classy as a connection, you can create Zaps with the Classy app.

### **From the Zap editor**

To add Classy via the Zap editor:

1. In the Zapier account menu, select **Create Zap**

![Create Zap button in Zapier](https://learn.classy.org/rs/673-DCU-558/images/zapier-create-zap.png)

2. Select **Trigger**
3. In the Trigger search field, enter **Classy** and select** version 1.6.0**. _For lighthouse customers, Classy will share a link to a private app for you to test_.

![Create new trigger modal in Zapier](https://learn.classy.org/rs/673-DCU-558/images/zapier-create-trigger.png)

4. Select the **event** you want to use for the trigger
   - You can choose from New Transaction, Updated Transaction, New Supporter, Updated Supporter, New Campaign, or Updated Campaign.

![Choose trigger event in Zapier](https://learn.classy.org/rs/673-DCU-558/images/zapier-trigger.png)

5. If you already have an active connection with Classy, you can select **Change** to update it. Otherwise, select **New connection**.
6. A pop-up window will appear asking if you want to Allow Zapier to access your Classy app account

![Allow access modal in Zapier](https://learn.classy.org/rs/673-DCU-558/images/zapier-allow-access.png)

7. Copy and paste the **Client ID**, **Client Secret**, and **Organization ID** generated on Classy into these fields
8. Select **Yes, Continue**

Now that you’ve entered your credentials and added Classy as a connection, you can create Zaps with the Classy app.

Learn more about [Zap triggers](https://help.zapier.com/hc/en-us/articles/8496288188429#trigger-types-0-0) and [Zap actions](https://help.zapier.com/hc/en-us/articles/8496257774221-Set-up-your-Zap-action#1-choose-your-app-and-event-0-0).

## **Manage Zapier in Classy**

You can remove your Classy credentials to disconnect the Zapier integration or generate new credentials to update the connection in Zapier.

To disconnect the integration or generate new credentials:

1. In your Classy account, select **Apps & Integrations**
2. Select **Zapier**
3. Select **Disconnect integration**.

![Disconnect integration in Classy](https://learn.classy.org/rs/673-DCU-558/images/zapier-classy-disconnect.png)

4. To confirm, select **Disconnect**.
   - This will invalidate the previously generated credentials, and any Zaps using the invalidated credentials will not sync Classy data.
   - If you do not plan to generate new credentials, we recommend deactivating any Zaps using this connection, as any callouts from Zapier to Classy will fail.

![Confirm disconnect Zapier](https://learn.classy.org/rs/673-DCU-558/images/zapier-disconnect.png)

5. **Optional**: To generate new credentials, follow the steps in **Activate Zapier in Classy**
   - You must update your Classy connection in Zapier with the newly generated credentials to resume syncing Classy data in your Zaps.

## **Sync data to Zapier**

Classy’s Zapier integration allows your organization to do what you want with the data in the systems of your choice. You define the actions and triggers you want for your Zaps and where your Classy data will go once synced to Zapier.

The integration supports polling for new or updated Transaction, Supporter, and Campaign data. View our [API documentation](https://developers.classy.org/overview/welcome) to learn more about all available fields and parameters. The frequency in which Zapier will poll the API is based on the Zapier subscription you have. For example, Zapier’s Starter plan will poll every 2 minutes, whereas Zapier’s Enterprise plan polls every minute.

Zapier will automatically deduplicate data sent from Classy based on record ID and timestamp.

In Zapier, you can filter based on the data in the object or sort the data by dates. In addition, organizations can push supporter data back into Classy. For example, if an offline gift is recorded in your organization’s CRM, you can configure a Zap to update the existing supporter record in Classy.

!!! note

    You will need at least a Zapier Starter plan to use filters.

### Sample Zaps

With over 5000+ apps to choose from on the Zapier Marketplace, there are endless possibilities for what you can do to connect your Classy data with other tools you use to manage your mission.

Here are some examples of ways you can automate your processes using the Zapier integration:

<table>
  <tr style="background-color: #425cc3; color: #fff">
   <td>When this happens… (Trigger)
   </td>
   <td>automatically do this (Action)
   </td>
  </tr>
  <tr>
   <td>A new Supporter is created in Classy
   </td>
   <td>Find and Add/Update a subscriber in Mailchimp
   </td>
  </tr>
  <tr>
   <td>A Supporter is updated in Classy
   </td>
   <td>Add/Update a subscriber in Mailchimp
   </td>
  </tr>
  <tr>
   <td>A new recurring transaction is created in Classy
   </td>
   <td>Add/Update a subscriber in Mailchimp
   </td>
  </tr>
  <tr>
   <td>A contact record is updated in Salesforce
   </td>
   <td>Update a Supporter record in Classy
   </td>
  </tr>
</table>

## **Frequently asked questions**

**What type of data can I sync from Classy to Zapier? What type of data can I sync from Zapier to Classy?**

The Zapier integration will use Classy's Public API to send available Transaction, Supporter, or Campaign data to Zapier, including any available parameters associated with each object. You can choose to sync data from any of these objects to Zapier.

Also, you can sync updates to an existing Supporter record for the following Supporter fields from Zapier to Classy: Address Line 1, Address Line 2, City, Country, State, Postal Code, Email Address, First Name, Last Name, Gender, Nickname, Phone.

A full list of the available Transaction, Supporter, and Campaign parameters can be found in Classy’s [API documentation](https://developers.classy.org/overview/welcome).

**Do I need a specific Zapier Plan to use the Classy Integration?**

The Classy integration will work with any Zapier plan. However, you need a minimum of a starter plan to use Zapier’s filter feature.

Your Zapier plan will also determine how frequently new or updated Classy data can be polled.

**What events can I use in Classy as a trigger in Zapier?**

Classy’s Zapier integration supports polling triggers. With a polling trigger, Zapier will request data from your trigger every 1 to 15 minutes to start your Zap, depending on your Zapier plan.

Available Classy events are New Transaction, Updated Transaction, New Supporter, Updated Supporter, New Campaign, or Updated Campaign.

**What actions are available in Zapier for Classy when creating a Zap? **

Classy’s Zapier integration supports syncing updates from Zapier to an existing Classy Supporter record.

**How do I update or remove the integration?**

Follow the steps in **Manage Classy credentials for Zapier** to deactivate the integration on Classy.

To manage or remove an app connection in Zapier, read [Manage your app connections](https://help.zapier.com/hc/en-us/articles/8496290788109-Manage-your-app-connections). To manage or delete a Zap in Zapier, read [Manage your Zaps](https://help.zapier.com/hc/en-us/articles/8496326119565-Manage-your-Zaps).

**What happens if I deactivate and then reactivate the Zapier integration on Classy without deactivating my Classy Zaps?**

When the Zapier integration is deactivated on Classy, the Classy client ID and API key you used to authenticate the connection in Zapier will be invalidated. A new client ID and API key will be generated upon reactivating the integration.

Any Zaps using the previous Classy client ID and API key for the connection should be updated with the new credentials, otherwise, the Zaps will fail.
