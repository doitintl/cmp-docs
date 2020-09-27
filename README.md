# What is the Cloud Management Platform?

Our Cloud Management Platform helps the developers and system administrators at digital-native companies improve cloud operations, maintain security, control cost, and ensure governance of its cloud estate. It has five strategic pillars: Analytics, Optimization, Enablement, Productivity, and Governance.

In this article, we'll briefly go over each of the main capabilities you have access to in the CMP, along with links to other articles for each feature if you're interested in doing a deeper dive.

## Cloud Analytics

### Reports

Cloud Reports give you instant visibility into your Google Cloud costs without having to spend agonizing hours scanning through GCP bills.

* Analyze cloud spend to identify optimization opportunities.
* [Build customized reports](https://help.doit-intl.com/hc/en-us/articles/360045644211-Creating-a-Cloud-Report) and [share](https://help.doit-intl.com/hc/en-us/articles/360045700631-Share-Cloud-Reports) them with others.
* Monitor costs on the go from your phone.
* Cross-check your SUD/CUD credits with by-the-hour reporting.

[Go here](https://help.doit-intl.com/hc/en-us/sections/360009379892-Cloud-Reports) for the full list of your capabilities with Cloud Reports.

### Cost Attributions

Attributions are a flexible way to group resources and their associated costs, helping you understand the cloud costs and relate them to the business in your Cloud Reports.

You may have various components of your application\(s\) spread across different projects, using different services. Attributions allow you to combine everything into something coherent.

 [![Attributions-team-prod.jpg](https://help.doit-intl.com/hc/article_attachments/360066691611/Attributions-team-prod.jpg)](https://help.doit-intl.com/hc/article_attachments/360066691611/Attributions-team-prod.jpg)

[How to use your Attributions in your Cloud Reports](https://www.loom.com/share/8d36dbd796c84d51a26b3f836226c883)

## Cloud Cost Optimization

### AWS-to-GCP TCO Analysis Report

As a DoiT International customer, you can [compare the Total Cost of Ownership \(TCO\)](amazon-web-services/aws-migration-tco-analysis.md) of your AWS assets vs. Google Cloud, directly from the Cloud Management Platform using your AWS invoice data in CSV format.

Within seconds of uploading your AWS invoice, you'll see what your potential GCP costs \(and savings\) would be if you ran the same compute workloads there.

Inside the report you'll find:

* Instances w/ break-down by region
* Usage in hours
* Estimated savings \(or extra spend\) per instance type 

### Instance Rightsizing for Google Cloud

When you create an instance in GCP and it is under-utilized, you are paying more than you should as a result of idle resources.

With Instance Rightsizing for Google Cloud, you will:

* Get notified of idle resources across **all** projects, and potential savings from rightsizing.
* [Identify and delete and/or modify idle VMs](https://help.doit-intl.com/hc/en-us/articles/360039630271-Rightsizing-for-Google-Cloud) in two clicks.
* Never pay for underutilized Google Compute instances again.

### Flexible Reserved Instances

AWS Reserved Instances \(RIs\) offer you between 30-70% savings on compute costs in exchange for a one or three-year commitment. Typically, you’d use RIs for predictable workloads, and pay on-demand pricing for the less predictable.

However getting RIs usage perfect is hard, because it relies on you being able to predict the future. Sometimes your predictions turn out wrong because usage needs suddenly change. As a result, 

[Flexible Reserved Instances](https://help.doit-intl.com/hc/en-us/articles/360043156112-Flexible-Reserved-Instances-RIs-) in the CMP allow customers to commit to RIs in one-month intervals while _still_ getting a 22% savings over on-demand prices.

This means you can reduce lock-in risk for your less-predictable workloads.

Placing an order for a Flex RI for the following month takes all but a few clicks, and you can easily monitor their performance from a central hub in the CMP.

### BigQuery FinOps Dashboard

As powerful as BQ is, it comes at a high cost depending on your analysts’ behavior and how your BigQuery architecture is set up. Adding on to this, trying to identify BigQuery resource inefficiencies without knowing _what_ you're looking for can be a huge timesuck.

As a result, we created the [BigQuery FinOps Dashboard](https://help.doit-intl.com/hc/en-us/articles/360040580752-BigQuery-FinOps-Dashboard), your Swiss Army knife for highlighting inefficiencies in your team's BigQuery usage.

It analyzes your team’s BigQuery behavior, aggregate information, and display the most important statistics for you. Unlike alternative solutions and methods, BigQuery FinOps Dashboard brings important information TO you, without you having to configure anything.

Below you will see the widgets of the dashboard that provide you with insights into your organization's BigQuery usage statistics. 

One important aspect of the BigQuery FinOps Dashboard is the Recommendations widget, which offers smart recommendations around the nature of how your datasets, tables, and queries are structured.

Each recommendation category comes with further details on how to act on each recommendation.

## Cloud Enablement

### Cloud Sandbox for Google Cloud

Cloud sandboxes offer engineering teams a safe and controlled environment to run experiments, test and build out new features without worrying about impacting production infrastructure. While easy, simply creating a new Google Cloud project cannot be considered a “complete” solution due to the lack of built-in budget management, self-service for developers, and governing policies.

Cloud Sandbox for Google Cloud gives admins and developers the governance and autonomy they both need, respectively, all while connecting to their Google Cloud Organization.

First, [create a sandbox policy](https://help.doit-intl.com/hc/en-us/articles/360042369611-Configure-A-Policy-For-Sandbox-Accounts) to automate sandbox management. With a policy set up, you can:

* Connect to your GCP billing account, organization, and IAM folder.
* Set sandbox budgets.
* Get alerts when a budget is hit, or automatically disable the billing.
* Limit the number of sandboxes per user.
* Give your sandbox names a stable naming convention.

Once a policy is created, developers are free to [create cloud sandbox environments](https://help.doit-intl.com/hc/en-us/articles/360042612671-Create-Google-Cloud-Sandbox-Accounts) themselves. No more submitting tickets just to get a new environment provisioned by an SRE. Finally, when sandboxes are up and running, you can monitor them all from a central hub.

### Quota Monitoring for Google Cloud and AWS

Every cloud provider has resource quotas for things like VPCs, CPU cores, and more. If you'd like to change that quota, you can request more, and typically cloud vendors will approve it. However, this takes hours to days.

However, sometimes your quota limits can, without warning, be hit by a surge of demand that causes you to hit those quotas. When this happens, you're forced to wait for your ticket to be addressed.

With Quota Monitoring for [Google Cloud](google-cloud/google-cloud-quotas.md) and [AWS](https://help.doit-intl.com/hc/en-us/articles/360038791071-AWS-Service-Limits-Quotas-Alerts) you can stay on top of your cloud quotas with proactive monitoring. You'll get notified when you're approaching quotas.

This way, you'll keep services always running by adjusting limits ahead of time.

### Anomaly Detection for Google Cloud

With so many moving parts in the cloud, it’s critical to keep a finger on the pulse of your costs. However, unless IT regularly monitors cloud spend, sudden spikes in resource costs can remain undetected for weeks — until the monthly bill arrives.

As a result, critical staff resources are wasted manually monitoring for and identifying the scope & source of problems.

[Cloud cost anomaly detection](https://help.doit-intl.com/hc/en-us/articles/360035689731-Cost-Anomalies-for-Google-Cloud) offers end-to-end **autonomous monitoring** of spikes in your Google Cloud billing, seamlessly, across all your projects and services right.

Available to DoiT customers right from the CMP, it also offers:

* Context-aware detection that treats each Google Cloud service uniquely.
* Advanced alerting that goes beyond static budgets & thresholds
* Fine-tune alerts by training them with your direct feedback.
* Real-time analysis of workload activity 

### Perks

[Perks](general/perks.md) are service-based benefits available to DoiT International customers at no extra cost, including workshops, training, cost optimization sessions, case studies, and co-produced webinars. They can easily be browsed and requested on-demand from within the CMP.

 [![Perks.jpg](https://help.doit-intl.com/hc/article_attachments/360062960052/Perks.jpg)](https://help.doit-intl.com/hc/article_attachments/360062960052/Perks.jpg)

## Cloud Productivity

### superQuery

[superQuery](http://web.superquery.io/) is a web-based IDE that enables you to leverage BigQuery, AWS Athena, and DynamoDB at peak efficiency. With superQuery, you get top-notch capabilities for:

* Query Management with [Tabs](https://support.superquery.io/en/articles/2988041-query-tabs) and [Boards](https://support.superquery.io/en/articles/3077544-boards)
* Collaboration
* [Ad-hoc Visualization](https://support.superquery.io/en/articles/2988069-chart)
* [Enhanced Caching](https://support.superquery.io/en/articles/3543297-setting-up-enhanced-caching)
* [Git functionality support](https://support.superquery.io/en/collections/1746442-superquery-key-features-explained#git-functionality-and-github)

DoiT customers get unlimited seats and access to superQuery at no additional cost, and can quickly access it from the CMP.

## Cloud Governance

### Asset Management

CMP gives you complete self-service management of assets across Google Cloud, AWS, G Suite, Azure, and Office 365.

From your Asset Management screen, you can:

* View all cloud subscriptions in one place.
* [Create a new Google Cloud Billing Account](google-cloud/create-google-cloud-billing-account.md) and/or an [AWS account](amazon-web-services/create-an-aws-account.md).
* [Invite an existing AWS account](amazon-web-services/invite-existing-aws-account.md)
* [Purchase additional seats for G Suite](https://help.doit-intl.com/hc/en-us/articles/360032598271-Purchase-G-Suite-Licenses) and/or [Office 365](https://help.doit-intl.com/hc/en-us/articles/360032598391-Purchase-Office-365-Licenses) yourself.
* Automate subscription management with [auto-provisioning](https://help.doit-intl.com/hc/en-us/articles/360038041751-Configure-Auto-Increase-for-G-Suite-Subscriptions) for G Suite, guaranteeing there is an open seat at all times.
* [Tag Assets](general/tag-assets.md) for classification and invoicing purposes \(e.g. team name, cost center, location, etc.\).

Additionally, you can view your order history of all licenses and subscriptions across all of your cloud products.

[~~Go here~~]() ~~~~for the full list of your asset management capabilities in CMP.

### Billing Profiles, Invoices, and Invoice Buckets

CMP gives you capabilities unavailable in GCP or AWS to customize _precisely_ how you'd like to billed via Billing Profiles, Invoices, and Invoice Buckets. 

[**Billing Profiles**](https://help.doit-intl.com/hc/en-us/articles/360032254792-Set-Up-New-Billing-Profile) are for when your company has different entities requiring separate invoices. For instance, you may use a different payment method or currency depending on the entity.

In the CMP, customers can create as many Billing Profiles as required, per their company's needs.

Additionally, whereas with GCP or AWS you can only pay with a credit card, DoiT International customers have more options for customizing the payment method for their Billing Profile\(s\) including Credit Card, Wire, Bill.com, and ACH. 

[**Invoices**](https://help.doit-intl.com/hc/en-us/articles/360032254812-Manage-Invoices) across all cloud platforms and their current statuses can be easily accessed using the CMP.

From the Invoices page, you can:

* Click on an invoice to view a detailed breakdown.
* Download invoices.
* Sort invoices by billing profile, cloud service, date, etc.
* Get an at-a-glance look of the invoice status, the product its referencing, and the total/balance.

Any tags placed on assets will also appear in invoices so you can more easily identify invoice items.

[**Invoice Bucketing**](https://help.doit-intl.com/hc/en-us/articles/360033254111--Change-Invoice-Settings) ****lets you create custom "buckets" and assign specific assets to those buckets.

This is especially useful when you have different cost centers such as R&D or Operations using different assets and want to bill them separately.

With invoice buckets, you will receive separate invoices for each invoice bucket, billed to the billing profile it is associated with. 

[Go here](https://help.doit-intl.com/hc/en-us/sections/360006391152-Invoices-Payments) for the full list of your billing and payment related capabilities.

### Contract Management

Via the Contracts page, you get [self-service access to all cloud contracts](https://help.doit-intl.com/hc/en-us/articles/360032255892-Accessing-Contracts) you are being billed for through DoiT International.

### User Management

Use User Management to:

* [Add colleagues](https://help.doit-intl.com/hc/en-us/articles/360032246952-Create-Users) to your CMP team.
* Management Billing Profile assignments.
* Configure notifications for alerts like payment reminders, new invoices, and more.
* [Grant permissions](https://help.doit-intl.com/hc/en-us/articles/360033254031-User-Permissions) to access various CMP features.

### Managed Google Cloud and Amazon Web Services Support

Within the CMP you can resolve your cloud issues quickly with hyper-responsive and unlimited support from DoiT International— **at no extra cost**.

* [Open tickets](tickets/open-a-new-support-request.md) with experienced Cloud Architects and Engineers.
* View open or historical tickets and their statuses.
* [Share tickets](tickets/ticket-sharing.md) with other team members.
* Stay up to date on any [known issues](tickets/cloud-infrastructure-known-issues.md) across all clouds you use.



