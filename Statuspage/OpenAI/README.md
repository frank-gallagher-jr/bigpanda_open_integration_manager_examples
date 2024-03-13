#BigPanda OIM (Open Integration Manager) Example Configuration for Statuspage from OpenAI

**Utilize the API docs page at BigPanda.io if you're interested in applying this configuration change via the API**
_________________________________

BigPanda API Documentation here - https://docs.bigpanda.io/reference/open-integration-manager-v2
BigPanda Community here - https://community.bigpanda.io/  
BigPanda Official Support here -  https://www.bigpanda.io/customer-support/

_________________________________

The exported configuration is an example of how to define an OIM integration for a Statuspage webhook. This allows you to avoid using Email Parser integrations for 3rd Party Service Provider integrations that utilize Statuspage thanks to BigPanda's power OIM preprocessing features. 

This example is not intended to serve as official guidance from BigPanda (although I do work at BigPanda at the time of the commit) and it's provided with the caveat that I will provide no warranty and that you use it at your own risk.  I'd recommend testing this in a lower environment before applying to your BigPanda production environment.

OpenAI's Statuspage alerts are received in two different formats.  One that is component driven, one that is incident driven.  I've tried to encompass both possible formats and some test payloads which I tried in my configuration.  You might have a better approach, but again, this is provided for example / reference purposes only.  Use your best judgement.

Here's what this looks like inside of BigPanda's OIM Integration UI: 

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/1f0b45ab-11ad-44d7-86ac-28801030a6d8)

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/cf1f215a-71b1-4a4f-866b-498a3a899f22)


Example BigPanda Incident View (demo account):

![image](https://github.com/frank-gallagher-jr/bigpanda_open_integration_manager_examples/assets/99338731/5019fbb7-3255-4a01-9860-93ade6bac6bf)
