---
description: Connect your Google Cloud Organization IAM to unlock additional CMP features.
---

# Connect Your Google Cloud IAM

In order to use many of the functionalities available to you within the **Cloud Management Platform**, we request an extra set of permissions, depending on the features you'd like to use. These permissions allow us to access the Google API and obtain information for monitoring or alerts, and/or help you take action on recommendations.

To grant these permissions, you will need to create a Google Cloud Service Account, set up a Google Cloud IAM Role at the organization level, and upload the key to the Cloud Management Platform. In this article, we'll go over how to do all of the above.

{% hint style="info" %}
Required Permissions**: Manage Settings**
{% endhint %}

## Create Google Service Account 

To create a Google Cloud Service account, please execute the following steps:

1. Open [Cloud Management Platform](https://app.doit-intl.com/) 
2. Navigate to the Settings icon in your lefthand navigation panel
3. Check the features you'd like to enable within the CMP
4. Review the permissions each service request \(by expanding the card\)
5. Click on "Create Service Account"

![](../.gitbook/assets/cmp_featuresconfig_serviceaccount.jpg)

Next, a slide-out will appear on the right side of your screen, containing all of the Google SDK \([gcloud\)](https://cloud.google.com/sdk) commands you need to run in order to create the service account and set it up with the correct role. Copy the commands and run them sequentially in your terminal or Google Cloud Shell.

{% hint style="info" %}
The `gcloud` commands vary according to the boxes of the features you checked
{% endhint %}

![](../.gitbook/assets/cmp_gcp_createserviceaccount2.jpg)

Once finished, you have the key JSON file for your new service account.

## Upload the Service Account Key

Whether you've generated your service account key, your next step is to upload the JSON file to the CMP by clicking on "Upload File".

If configured successfully, you should see a "**Healthy**" or "**Partial**" value appear under the "Status" column in the "Configured Accounts" widget.

"**Partial**" will only appear next to your configured service account if you didn't grant permissions for _all_ of the available features. What's important in this case is to examine the "Features" widget and verify that all of the features you selected have a "**Healthy**" status.

If there is something wrong with the JSON file you uploaded, you will see an "**Unhealthy**" value under the "Status" column. 

![](../.gitbook/assets/cmp_gcp_serviceaccount3.jpg)

## Updating your Service Account

If, after initially connecting your Google Cloud Organization, you decide that you want to grant permissions for an additional feature — or remove permissions — you can do that easily from the same page. 

First, check or uncheck the feature\(s\) you'd like to add or remove. Then click on "Update Role".

![](../.gitbook/assets/cmp_updaterole.jpg)

A slide-out will appear containing the `gcloud` commands you need to run to update your service account's role so that permissions corresponding to the feature you checked or unchecked are added or removed, respectively.

![](../.gitbook/assets/cmp_updaterole2.jpg)

## Adding Multiple Service Accounts

In the very rare event that you have multiple Google Cloud Organizations, you can upload multiple service account keys to regulate which Organizations get access to which features.

To add a new service account, click on the **"+"** icon in the top-right corner of the Configured Accounts widget. 

![](../.gitbook/assets/cmp_addmulitpleserviceaccount.jpg)

Once clicked, notice that all of the Features will revert back to "Not Configured" since you are setting up a new service account.

As you did with your initial service account, select the features you'd like to grant permissions for this service account, and run the `gcloud` commands provided.

Check out the bite-sized video below for a closer look at connecting your Google Cloud Organization to CMP.

{% embed url="https://www.loom.com/share/55c2fd9dbde74ac6bd2d3ac7e8c8bd45?sharedAppSource=team\_library" %}



