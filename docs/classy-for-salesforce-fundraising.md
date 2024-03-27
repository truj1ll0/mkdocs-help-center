# Install Classy for Salesforce Fundraising

Learn how to install Classy for Salesforce Fundraising in your Nonprofit Cloud or Education Cloud instance.

## Requirements

To install the integration, you’ll need to:

- Be a System Administrator in Salesforce
- Have a Nonprofit Cloud or Education Cloud (with Advancement) instance \
  (sandbox is highly recommended first)
- Have access to the Salesforce Fundraising app in Classy
- Be an Organization Administrator or Settings Manager in Classy

### Dedicate an integration user

When setting up, we recommend completing the steps in Salesforce with a dedicated user for the integration. For example, you could create one and name it Classy Integration. That way, it’s easier to tell when Classy creates or updates a record.

As a reminder, you’ll need to be able to log in as this user, and it must have System Administrator access with Marketing User permissions. If you don’t use a System Admin user, your user must have the following Salesforce permission sets before completing the installation:

- Allows users to modify Named Credentials and External Credentials
- Download AppExchange Packages
- Manage Package Licenses
- Fundraising Access
- Assign Permission Sets
- Manage Profiles and Permission Sets

After successful installation, add the following permission sets to the user to avoid any syncing issues and to show the integration in a completed state in Classy:

- Classy API Access
- Classy Connector All Objects & Fields
- Classy for Salesforce Fundraising All Objects & Fields.
- Fundraising Access (Salesforce Permission Set)

## Give Classy access to your environment

!!! note

    We always recommend connecting to a Salesforce Full sandbox when setting up for the first time. Setting up and testing in a sandbox can help you identify any changes you need to make before you switch to production. If you do not have a Salesforce sandbox, you can create one using Salesforce's help article.

    If you don't have access to a Full sandbox through your SF account, you can use a Partial sandbox. However, using a Partial sandbox can lead to testing issues that Classy cannot provide support for or help troubleshoot. Developer sandboxes are not supported as they won’t let you successfully test the integration.

First, you’ll need to connect Classy to a Salesforce environment.

1. In your Classy account, go to **Apps & Extensions**
2. Select **Salesforce Fundraising**
3. Select your environment

![Connect Classy for Salesforce to a sandbox](https://learn.classy.org/rs/673-DCU-558/images/C4SFF-install-step1.png)

1. Select **Connect to Salesforce** to open a Salesforce dialog
2. Select **Allow** to give access to Salesforce \
   (you may be prompted to log in to Salesforce if you aren’t logged in already)

## Install base package

Next, you’ll need to install the Classy Connector base package.

1. Under Step 2, select **Install Package**

![Install package](https://learn.classy.org/rs/673-DCU-558/images/C4SFF-install-step2.png)

1. Select the Salesforce users who will use Classy data and custom objects
   - We recommend installing it for all users unless you have specific permission requirements. You can edit who can access Classy data and custom objects in Salesforce anytime.
2. Select **Install**
3. Mark the access checkbox and select **Continue**

You will receive an email when the installation is complete. Refresh the page to continue to the next step.

## Install the second package

In Step 3, select **Nonprofit Cloud** or **Education Cloud,** depending on which industry cloud you are using. The selection does not impact the integration, but Classy will use the information to better understand our customers.

After making your selection, select **Install Package **and follow the same steps as you did when installing the base package.

## Activate API Key

The last step for turning on the integration is to complete the connection. Under Step 4, either select **+ Create API key** or select an existing API key. If you create an API key, you must fill out the form and then select **Activate API key**.

![Activate API key](https://learn.classy.org/rs/673-DCU-558/images/C4SFF-install-step4.png)

### Application name

You can choose any application name. One name suggestion is **SF Fundraising**.

### Oauth2 Redirect URI

Enter the URL (web address) for your organization’s main website. The URL must include the full https protocol (E.g., https://www.classy.org/).

## Frequently asked questions

**Will Classy for Salesforce sync automatically?**

After you connect the integration, all incoming data will sync to Salesforce automatically. At this time, historical data will not sync.

**Can I use Salesforce’s Integration User when installing the integration?**

No, you cannot use the Integration User type when installing the packages. But, you can switch to an Integration User after the installation is complete. To do so, select **Disable Extension** in Classy. Then, select the Salesforce environment to connect Classy to and log in with the credentials for the new user.

Be sure to add the following permission sets to the user to avoid any syncing issues and to show the integration in a completed state in Classy:

- Classy API Access
- Classy Connector All Objects & Fields
- Salesforce Fundraising All Objects & Fields.
- Fundraising Access (Salesforce Permission Set)

**Can I connect multiple Classy accounts to the same cloud environment?**

Yes, up to 5 Classy accounts can be connected to the same cloud environment per Salesforce user. If you need to connect more than 5 accounts, use a different Salesforce System Administrator user.
