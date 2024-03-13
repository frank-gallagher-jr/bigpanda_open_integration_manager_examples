# BigPanda OIM (Open Integration Manager) Example Configuration for Statuspage from OpenAI

_________________________________
**Utilize the API docs page at BigPanda.io if you're interested in applying this configuration change via the API**

BigPanda API Documentation here - https://docs.bigpanda.io/reference/open-integration-manager-v2

BigPanda Community here - https://community.bigpanda.io/  

BigPanda Official Support here -  https://www.bigpanda.io/customer-support/

_________________________________

The exported configuration is an example of how to define an OIM integration for a Statuspage webhook. This allows you to avoid using Email Parser integrations for 3rd Party Service Provider integrations that utilize Statuspage thanks to BigPanda's power OIM preprocessing features. 

This example is not intended to serve as official guidance from BigPanda (although I do work at BigPanda at the time of the commit) and it's provided with the caveat that I will provide no warranty and that you use it at your own risk.  I'd recommend testing this in a lower environment before applying to your BigPanda production environment.

OpenAI's Statuspage alerts are received in two different formats.  One that is component driven, one that is incident driven.  I've tried to encompass both possible formats and some test payloads which I tried in my configuration.  You might have a better approach, but again, this is provided for example / reference purposes only.  Use your best judgement.

**Step 1:**  Create a new OIM Integration inside of BigPanda on the Integrations Tab

**Step 2:**  Browse to the Statuspage URL for the 3rd Party Service (in this case OpenAI's is https://status.openai.com/)

Click "Subscribe To Updates Button"

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/0a6898c0-6e5a-4b77-a8d4-9ae2a55456c6)

**Step 3:** Select the <> tab on the configuration widget (This is the same across every Statuspage I've come across, you're looking for "Webhook"):  

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/8a6689ef-cd31-4a23-87a3-ca2b6794f9a9)

AND THEN -> 

In the webhook URL on the Statuspage, enter your OIM Integration URL provided on the BigPanda OIM "Setup Instructions" tab.  **USE THE EXAMPLE URL WHICH HAS BOTH THE APP_KEY AND THE ORG TOKEN IN IT!**

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/45f349f5-9b9f-4b6d-92f0-69f8347f9352)

Enter your email address so that you can manage your subscriptions and make changes as necessary.  Save the configuration and take the necessary steps to confirm your Webhook subscription.

**Step 4** - Configure BigPanda via the Integration Page tab labeled "Integration Manager"

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/a029452e-81d8-4105-b598-2deb7b7e1310)

Here's what this looks like inside of BigPanda's OIM Integration UI (refer to the exported OIM Config file in the folder): 

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/1f0b45ab-11ad-44d7-86ac-28801030a6d8)

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/cf1f215a-71b1-4a4f-866b-498a3a899f22)

Again... MAKE NOTE OF THE DIFFERENT FORMATS OF STATUS ALERTS YOU MIGHT RECEIVE.  YOU NEED TO ACCOUNT FOR THOSE FORMATS IN YOUR CONFIGURATION!


Example BigPanda Incident View (demo account):

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/5019fbb7-3255-4a01-9860-93ade6bac6bf)


You can apply this same approach across other Statuspage companies.  

Statuspage webhook documentation here:  [https://support.atlassian.com/statuspage/](https://support.atlassian.com/statuspage/docs/enable-webhook-notifications/)https://support.atlassian.com/statuspage/docs/enable-webhook-notifications/
