---
description: >-
  Connect CMP to your Slack workspace to help share reports, budgets, anomalies
  or almost anything else with your colleagues faster.
---

# Slack Integration

The DoiT CMP Slack application will automatically unfurl a preview of any CMP link, including chart images for certain reports, making it easy for anyone in your Slack workspace to learn from your CMP analyses.

### Enable the Integration

To enable the integration, log in to both CMP and Slack, then click "Add to Slack" below:

[link](https://slack.com/oauth/v2/authorize?client_id=95544667184.517333928260&scope=commands,links:read,links:write,users.profile:read,users:read,users:read.email&user_scope=links:read,links:write,users.profile:read)

![](../.gitbook/assets/add_to_slack.png)

At this point, DoiT CMP is a part of your Slack workspace, and any CMP links you send in Slack will unfurl with metadata, and if applicable a chart preview.

Once at least one member of your CMP organization has set up the Slack integration for their account, any other members of the Slack workspace will see a prompt the next time they paste a CMP link. The prompt will ask them to connect their own CMP account to Slack as well. If they choose to do so, Slack will guide them through the authentication flow. Once they have successfully connected CMP to Slack, any further links they paste in Slack will unfurl.

### Using the Integration

Once you've set up the integration, CMP links pasted in Slack will unfurl. Most links will provide some basic link metadata, and links to Reports, Budgets, Anomalies, or Dashboards and will also include a chart preview, for example:

![](../.gitbook/assets/image%20%2876%29.png)

### Permissions

CMP does not restrict who can enable the CMP Slack integration. However, your Slack workspace may limit who can perform the connection.

After CMP is connected to Slack, any Slack user who posts a CMP link will be prompted to connect their own account, in order to unfurl report previews. By performing this integration at the user level, it ensures that only reports the user has access to will unfurl in Slack.

### Privacy

The CMP Slack app adheres to DoiT International overall privacy policy, available in full here: https://www.doit-intl.com/privacy

