---
description: How to analyze cloud spend that pre-dates when you started using the CMP
---

# Upload Historical GCP Billing Data

### Overview

This feature enables you to upload all your historical Google Cloud billing data into DoiT Cloud Management Platform \(CMP\) to immediately analyze your cloud spend and promptly identify optimization opportunities through Cloud Analytics, BigQuery Lens, and other CMP features.

To get started, first, you need to ensure that you have a Service Account that connects your Google Cloud Organization to CMP. Then, you'll have to grant two additional required permissions.

### Step 1. Identify the service account linked to CMP

1. From CMP's left side navigation menu, click "**Settings**"
2. Select "**Google Cloud**" tab
3. Locate the "**Service Account**" listed in Configured Accounts

![](../.gitbook/assets/image%20%28103%29.png)

If you do not have this configured yet, you need to create a service account and connect CMP to your Google Cloud Organization. Follow the steps in this link: [Connect Google Cloud Service Account](https://help.doit-intl.com/google-cloud/connect-google-cloud-service-account)

Once you have identified the service account, copy the service account email and proceed to granting it with the the additional required permissions.

### Step 2. Grant Permissions

{% hint style="info" %}
You need to have the appropriate IAM role/permission in GCP to grant the required permissions to the service account
{% endhint %}

> ###  Grant access to the dataset

1. From GCP, navigate to the BigQuery Console and open the **dataset** where the billing data is stored, then click  "**Share dataset**"
2. In the Dataset Permissions tab, click "**Add Member**" and paste the **service account** **email** that was linked to CMP as identified in **Step 1**.
3. Click "**Select a Role**" highlight BigQuery then choose **BigQuery Data Viewer**
4. Click "**Add**" 
5. Click "**Done**"

![](../.gitbook/assets/image%20%2896%29.png)

![](../.gitbook/assets/image%20%2894%29.png)



> ### Grant access to the Project



### Step 3. Link your Google Cloud Direct Billing Account

{% hint style="info" %}
Required Permission: CMP Assets Manager or CMP Admin ?
{% endhint %}

1. From CMP's left side navigation menu, click "**Assets**"
2. Select "**Google Cloud**" tab
3. Click the dropdown button next to "New Billing Account" and select "**Link Direct Account**"

![](../.gitbook/assets/image%20%28107%29.png)

You can now import your historical billing data into CMP. You need the following information to complete the process:

* Billing Account ID: _example_ "**01CF51-9FDB87-7894FD"**
* Source Project: Enter the "**Project ID"**
* Source Dataset: Enter the "**Dataset ID"**

![](../.gitbook/assets/image%20%2899%29.png)

Once you click "**Import**" a new card will be added to your assets reflecting the details and status   


![](../.gitbook/assets/image%20%2893%29.png)



> &lt; add image for successful import &gt;
>
> &lt; add FAQ / steps to take if customer encounters issues / errors &gt;

