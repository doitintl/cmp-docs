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

### Step 2. Grant the required Permissions

{% hint style="info" %}
You need to have the appropriate IAM role/permission in GCP to grant the required permissions to the service account
{% endhint %}

> ###  Grant the **BigQuery Data Viewer role**

1. From GCP, navigate to the BigQuery Console and open the **dataset** where the billing data is stored, then click  "**Share dataset**"
2. In the Dataset Permissions tab, click "**Add Member**" and paste the **service account** **email** that was linked to CMP as identified in **Step 1**.
3. Click "**Select a Role**" highlight BigQuery then choose **BigQuery Data Viewer**
4. Click "**Add**" 
5. Click "**Done**"

![](../.gitbook/assets/image%20%2896%29.png)

![](../.gitbook/assets/image%20%2894%29.png)



> ### Grant the **bigquery.jobs.create permission**
>
> Depending on the features initially enabled from the process [Connect Google Cloud Service Account](https://help.doit-intl.com/google-cloud/connect-google-cloud-service-account), you may already have this permission granted to the role. Follow the steps below to verify / add the permission to the project.

1. Select your **organization** from the dropdown options
2. From the GCP Navigation Menu, navigate to "IAM & Admin" then select "**Roles**"
3. Click on the role "**DoiT CMP Service Account**"
4. Check if **bigquery.jobs.create** is included in the assigned permissions, if it is, then no further action is needed since these permissions will be inherited by the projects
5. If bigquery.jobs.create permission is not yet added, click on "**Edit Role**"
6. Click "**Add Permissions**"
7. Filter by **"Permission : bigquery.jobs.create**" and check the box for this permission
8. Click "**Add**"

![](../.gitbook/assets/image%20%28116%29.png)

![](../.gitbook/assets/image%20%28117%29.png)

![](../.gitbook/assets/image%20%28108%29.png)

![](../.gitbook/assets/image%20%28112%29.png)



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

![](../.gitbook/assets/image%20%28119%29.png)

Once you click "**Import**" a new card will be added to your assets reflecting the details and progress or completion status.  

![](../.gitbook/assets/image%20%28115%29.png)

![](../.gitbook/assets/image%20%28118%29.png)

