---
description: Adding existing AWS accounts to DoiT International consolidated billing
---

# Invite Existing AWS Account

You can add existing AWS accounts to DoiT International's consolidated billing using the Cloud Management Platform.

{% hint style="info" %}
Required Permission**: Licenses Manager**
{% endhint %}

{% hint style="warning" %}
Please note that you must be assigned access to the specific Billing Profile under which the domain is managed in order to invite an existing account.
{% endhint %}

Start with you logging into the [Cloud Management Platform](https://app.doit-intl.com), and select the 'Invite AWS Account' from the menu on the left-hand side of the page and clicking on Assets.

![](../.gitbook/assets/assets-icon-1-%20%284%29%20%285%29%20%281%29.png)

Once you're at the Assets page, go to the right-hand side of the page and click on '**Invite Account**'.

![](../.gitbook/assets/aws-invite-tab.png)

Choose the Billing Profile to which you'd like to have the existing AWS account now be a part of. Enter the 12-digit AWS Account ID and any optional notes before clicking 'Invite'.

![](../.gitbook/assets/aws-id.png)

An email will be sent on behalf of AWS.

![](../.gitbook/assets/invite-aws.png)

If within five minutes you haven't received the above email, please re-enter your AWS Account ID in the DoiT Cloud Management Platform and invite once again. 

To complete the process, sign in to the [AWS Organizations Console](https://console.aws.amazon.com/organizations/). On the Invitations page in the console, you can see your open invitations to join organizations. Finally, click the "Accept" button to accept the invitation.

![](../.gitbook/assets/cint_aws_invitation3.png)

Afterward, you will be redirected to the **Organization overview** page with details about the organization that your account is now a member of. You can view the organization's ID and the owner's email address.

### Multiple Accounts Under a Master Organization

In the event that you have multiple accounts under a Master account / organization, you will get an error trying to accept the invitation.

In order to successfully accept the invitation, you must remove each linked AWS account from your master account.

{% hint style="info" %}
Note: This will prompt you to input payment details for each linked account if you didn't do so while initially creating them.
{% endhint %}

For each account you must:

1. "Leave" the Organization \(no new invites will appear before you do this\)
2. Accept the invite from DoiT International in each linked account

### Completing IAM Access for CloudHealth

After signing in to the AWS Console and accepting the invitation, a final email will be sent instructing how to complete the IAM access for CloudHealth.

![](../.gitbook/assets/iam-last-steps.png)

## Frequently asked questions: 

> ### **I have followed all the steps, accepted the invite and created the IAM access for Cloudhealth but my account is not appearing, what is the reason?**

![Your account is not appearing in the &quot;Amazon Web Services&quot; section of the assets.](../.gitbook/assets/image%20%2875%29.png)

If you do not have spends on your billing account, the account  will stay under “invites”. It is based on the fact that an entry/file \(CUR's\) is created and populated by AWS for our system to be able to see and parse it.

If you have spends on your billing account, and after 48 hours you still see the account under "invites", please [open a support ticket.](https://help.doit-intl.com/tickets/open-a-new-support-request) 



> ### **I’ve performed all the requested steps, I have spends on my AWS billing account, but my information is not still there. What could be the reason ?**

Once successfully completed it takes 24-72 hours for the data to start flowing through from AWS, then our Cloud Management Platform will update. 



> ### **I have not received any invitation email. What could have gone wrong?**

1\) On your organization's page, check if you can see the invite: 

![Invite on your AWS Organizations page ](../.gitbook/assets/image%20%2872%29.png)

If you can't see that invite, check if you have left your organization as specified in the above "Multiple Accounts Under a Master Organization" steps. 

2\) If you can see the invite on the organization's page, consider the following:  
Is the invite on your spam folder? Did you enter the correct AWS account id when inviting the account?



> ### **My CloudHealth status shows as "critical" or "unknown", what does it mean?** 
>
> ### **My payer account is showing as N/A, what does that mean?**

![CloudHealth Status: Unknown.](../.gitbook/assets/image%20%2873%29.png)

  
It means that your Cloudhealth configuration was not done properly**.**

**Actions to take:** please [open a support ticket](https://help.doit-intl.com/tickets/open-a-new-support-request) if you see the  CloudHealth status as "critical" or "unknown", or if you see Payer Account: N/A.  
**The consequences are the following:** 

* Our Cloud Management Platform is not able to properly reflect your reservation data, and you cannot use the FlexRI and Spot0 services. 
* It also means you will not be able to run reports on this asset, the reason being that the data is not flowing to our platform. 

