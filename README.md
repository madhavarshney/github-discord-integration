# github-discord-integration
This repo provides information for setting up Discord to receive notifications about GitHub events.

Source: [Discord Support - Intro to Webhooks](https://support.discordapp.com/hc/en-us/articles/228383668-Intro-to-Webhooks)

## Setup

### Discord:

#### Step 1: Create a text channel
Create a Discord channel to receive bot messages in, such as `#gitupdates`.

#### Step 2: Create a Discord webhook
1) Go to Server Settings > Webhooks and click "Create Webhook"
2) Set any name and icon you like
3) Select the channel that you created in Step 1
4) Copy the Webhook URL

### Github:

#### Step 1: Configure the repo to use the webhook
1) Go to the repo that you want to receive notifications from.
2) Go to Settings > Webhooks and click "Add Webhook".
3) Enter the URL of the Discord Webhook that was copied above into the "Payload URL" field.
4) IMPORTANT: Add `/github` at the end of the URL! This is really really important.
5) In "Content type", choose `application/json`.
6) Optional: Customize which events you want to receive.

#### Step 2: Enjoy!
Commit and push some changes to your repo and test that you receive a message in the Discord channel that you configured.

## Conclusion
This is a nifty feature of Discord and GitHub if you're using them together. Please star this repo if this helped you in any way! Thank you.
