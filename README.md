---
description: Overview of DoiT International Cloud Management Platform
---

# What is CMP?

**Welcome to DoiT International's Help Center for all things Cloud Management Platform!**

{% hint style="info" %}
You can request changes to articles or report issues via our [public GitHub repository](https://github.com/doitintl/cmp-docs) by submitting a pull request or creating an issue.
{% endhint %}

But for now, let's go over what exactly the CMP is and how _you_ can benefit from using it.

The Cloud Management Platform helps the developers and system administrators at digital-native companies improve cloud operations, maintain security, control cost, and ensure governance of its cloud estate. It has five strategic pillars: Analytics, Optimization, Enablement, Productivity, and Governance.

In this brief, we'll briefly go over each of the main capabilities you have access to in the CMP, along with links to other articles for each feature if you're interested in doing a deeper dive.

## Cloud Analytics

### Reports

Cloud Reports give you instant visibility into your Google Cloud and AWS costs without having to spend agonizing hours manually scanning through cloud bills.

* Analyze cloud spend to identify optimization opportunities.
* [Build customized reports](cloud-analytics/create-cloud-report.md) and [share](cloud-analytics/sharing-cloud-reports.md) them with others.
* Monitor costs on the go from your phone.
* [Detect trends](cloud-analytics/trend-analysis.md) in your cloud usage
* [Forecast your cloud spend](cloud-analytics/forecasting.md) across all time ranges and any cloud services
* Cross-check your SUD/CUD credits with by-the-hour reporting.

{% embed url="https://www.loom.com/share/3bb89b9c624a4a52a2ecfbb61a56b4b8" caption="" %}

### Cost Attributions

Attributions are a flexible way to group resources and their associated costs, helping you understand the cloud costs and relate them to the business in your Cloud Reports.

You may have various components of your application\(s\) spread across different projects, using different services. Attributions allow you to combine everything into something coherent.

{% embed url="https://www.loom.com/share/8d36dbd796c84d51a26b3f836226c883?sharedAppSource=team\_library" caption="" %}

## Cloud Cost Optimization

### Rightsizing for Google Cloud

When you create an instance in Google Cloud and it is under-utilized, you are paying more than you should as a result of idle resources.

With Instance Rightsizing for Google Cloud, you will:

* Get notified of idle resources across **all** projects, and potential savings from rightsizing.
* [Identify and delete and/or modify idle VMs](dashboards/rightsizing-for-google-cloud.md) in two clicks.
* Never pay for underutilized Google Compute instances again.

{% embed url="https://www.loom.com/share/cecfc1a7f3d84240a5be922e27c0ac56?sharedAppSource=team\_library" caption="" %}

### Flexible Reserved Instances

AWS Reserved Instances \(RIs\) offer you between 30-70% savings on compute costs in exchange for a one or three-year commitment. Typically, you’d use RIs for predictable workloads, and pay on-demand pricing for the less predictable.

However getting RIs usage perfect is hard, because it relies on you being able to predict the future. Sometimes your predictions turn out wrong because usage needs suddenly change. As a result, you're stuck overpaying for instances you need no more, or forced to re-sell it at a huge discount.

[Flexible Reserved Instances](flexsave/overview.md) in the CMP let you commit to EC2 Reserved Instances in one-month intervals while still sharing in the AWS-listed RI commitment discount. With Flex RIs, you'll eliminate RI lock-in risk for your less predictable workloads.

Placing an order for a Flex RI for the following month takes all but a few clicks, and you can easily monitor their performance from a central hub in the CMP.

{% embed url="https://youtu.be/Si6mZvn-z7I" %}



### BigQuery FinOps

As powerful as BQ is, it comes at a high cost depending on your analysts’ behavior and how your BigQuery architecture is set up. Adding on to this, trying to identify BigQuery resource inefficiencies without knowing _what_ you're looking for can be a huge time-suck.

As a result, we created the [BigQuery FinOps Dashboard](dashboards/bigquery-finops-dashboard.md), your Swiss Army knife for highlighting inefficiencies in your team's BigQuery usage.

It analyzes your team’s BigQuery behavior, aggregate information, and display the most important statistics for you. Unlike alternative solutions and methods, BigQuery FinOps Dashboard brings important information TO you, without you having to configure anything.

Below you will see the widgets of the dashboard that provide you with insights into your organization's BigQuery usage statistics.

One important aspect of the BigQuery FinOps Dashboard is the Recommendations widget, which offers smart recommendations around the nature of how your datasets, tables, and queries are structured.

Each recommendation category comes with further details on how to act on each recommendation.

{% embed url="https://youtu.be/7r1WfwnBAA4" %}



## Cloud Enablement

### Cloud Sandboxes

Cloud sandboxes \(or DCEs, - disposable cloud environments\) offer engineering teams a safe and controlled environment to run experiments, test, and build out new features without worrying about impacting production infrastructure. While easy, simply creating a new Google Cloud project cannot be considered a “complete” solution due to the lack of built-in budget management, self-service for developers, and governing policies.

Cloud Sandbox for Google Cloud gives admins and developers the governance and autonomy they both need, respectively, all while connecting to their Google Cloud Organization.

First, [create a sandbox policy](cloud-sandbox-management/configuring-a-policy-for-sandbox-accounts.md) to automate sandbox management. With a policy set up, you can:

* Connect to your Google Cloud billing account, organization, and IAM folder.
* Set sandbox budgets.
* Get alerts when a budget is hit, or automatically disable the billing.
* Limit the number of sandboxes per user.
* Give your sandbox names a stable naming convention.

Once a policy is created, developers are free to [create cloud sandbox environments](cloud-sandbox-management/create-gcp-sandbox-accounts.md) themselves. No more submitting tickets just to get a new environment provisioned by an SRE. Finally, when sandboxes are up and running, you can monitor them all from a central hub.

{% embed url="https://www.loom.com/share/2e2adffc48464c0189b87e4750e7b7d3?sharedAppSource=team\_library" caption="" %}

### Cloud Quota Monitoring

Every cloud provider has resource quotas for things like VPCs, CPU cores, and more. If you'd like to change that quota, you can request more, and typically cloud vendors will approve it. However, this takes hours to days.

However, sometimes your quota limits can, without warning, be hit by a surge of demand that causes you to hit those quotas. When this happens, you're forced to wait for your ticket to be addressed.

With Quota Monitoring for [Google Cloud](google-cloud/google-cloud-quotas.md), and [AWS](amazon-web-services/aws-quotas.md) you can stay on top of your cloud quotas with proactive monitoring. You'll get notified when you're approaching quotas.

This way, you'll keep services always running by adjusting limits ahead of time.

### Cost Anomalies 

With so many moving parts in the cloud, it’s critical to keep a finger on the pulse of your costs. However, unless IT regularly monitors cloud spend, sudden spikes in resource costs can remain undetected for weeks — until the monthly bill arrives.

As a result, critical staff resources are wasted manually monitoring for and identifying the scope & source of problems.

[Cloud cost anomaly detection](anomaly-detection/cloud-anomalies.md) offers end-to-end **autonomous monitoring** of spikes in your AWS & Google Cloud usage & billing, seamlessly, across all your projects and services.

Available to DoiT customers right from the CMP, it also offers:

* Context-aware detection that treats each Google Cloud service uniquely.
* Advanced alerting that goes beyond static budgets & thresholds
* Fine-tune alerts by training them with your direct feedback.
* Real-time analysis of workload activity 

{% embed url="https://www.youtube.com/watch?v=h6V7XfhsdmY&list=PLEBxNMZ7Mu3\_hmB2I2LXcDSYt1SXcjwMz&index=1" %}



### Cloud Support and Advisory

As a DoiT International customer, you have access to 80+ battle-tested senior cloud engineers around the globe with over 200 certifications between them.

Within the CMP you can:

* Create [support or advisory requests](tickets/open-a-new-support-request.md)
* [Escalate](tickets/escalating-support-requests.md) support requests
* [Share](tickets/ticket-sharing.md) support requests with others

{% embed url="https://www.loom.com/share/ec2e0bca53fc46ef80061dd96be2f1a0?sharedAppSource=team\_library" caption="" %}

### Perks

[Perks](perks/perks.md) are service-based benefits available to DoiT International customers at no extra cost, including workshops, training, cost optimization sessions, case studies, and co-produced webinars. They can easily be browsed and requested on-demand from within the CMP.

{% embed url="https://www.loom.com/share/9ff183270cb84e32817818589a80d37e?sharedAppSource=team\_library" caption="" %}

## Cloud Productivity

### superQuery

[superQuery](http://web.superquery.io/) is a web-based IDE that enables you to leverage BigQuery, AWS Athena, and DynamoDB at peak efficiency. With superQuery, you get top-notch capabilities for:

* Query Management with [Tabs](https://support.superquery.io/en/articles/2988041-query-tabs) and [Boards](https://support.superquery.io/en/articles/3077544-boards)
* Collaboration
* [Ad-hoc Visualization](https://support.superquery.io/en/articles/2988069-chart)
* [Enhanced Caching](https://support.superquery.io/en/articles/3543297-setting-up-enhanced-caching)
* [Git functionality support](https://support.superquery.io/en/collections/1746442-superquery-key-features-explained#git-functionality-and-github)

As a customer, you get unlimited superQuery seats and access to superQuery at no additional cost, and can quickly access it from the CMP.

## Cloud Governance

### Asset Management

CMP gives you complete self-service management of assets across Google Cloud, AWS, G Suite, Azure, and Office 365.

From your Asset Management screen, you can:

* View all cloud subscriptions in one place.
* [Create a new Google Cloud Billing Account](google-cloud/create-google-cloud-billing-account.md) and/or an [AWS account](amazon-web-services/create-an-aws-account.md).
* [Invite an existing AWS account](amazon-web-services/invite-existing-aws-account.md)
* [Purchase additional seats for G Suite](g-suite-and-workspace/purchasing-g-suite-licenses.md) and/or [Office 365](microsoft-office-365/purchasing-office-365-licenses.md) yourself.
* Automate subscription management with [auto-provisioning](https://help.doit-intl.com/hc/en-us/articles/360038041751-Configure-Auto-Increase-for-G-Suite-Subscriptions) for G Suite, guaranteeing there is an open seat at all times.
* [Tag Assets](assets-and-contracts/tag-assets.md) for classification and invoicing purposes \(e.g. team name, cost center, location, etc.\).

Additionally, you can view your order history of all licenses and subscriptions across all of your cloud products.

### Advanced Billing

CMP gives you capabilities unavailable in Google Cloud or AWS to customize _precisely_ how you'd like to billed via Billing Profiles, Invoices, and Invoice Buckets.

[**Billing Profiles**](invoices-and-payments/setting-up-a-new-billing-profile.md) are for when your company has different entities requiring separate invoices. For instance, you may use a different payment method or currency depending on the entity.

In the CMP, customers can create as many Billing Profiles as required, per their company's needs.

Additionally, whereas with Google Cloud or AWS you can only pay with a credit card, DoiT International customers have more options for customizing the payment method for their Billing Profile\(s\) including Credit Card, Wire, Bill.com, and ACH.

[**Invoices**](invoices-and-payments/managing-invoices.md) across all cloud platforms and their current statuses can be easily accessed using the CMP.

From the Invoices page, you can:

* Click on an invoice to view a detailed breakdown.
* Download invoices.
* Sort invoices by billing profile, cloud service, date, etc.
* Get an at-a-glance look of the invoice status, the product its referencing, and the total/balance.

Any tags placed on assets will also appear in invoices so you can more easily identify invoice items.

[**Invoice Bucketing**](invoices-and-payments/changing-invoice-settings.md) _\*\*_lets you create custom "buckets" and assign specific assets to those buckets.

This is especially useful when you have different cost centers such as R&D or Operations using different assets and want to bill them separately.

With invoice buckets, you will receive separate invoices for each invoice bucket, billed to the billing profile it is associated with.

[Go here](invoices-and-payments/managing-invoices.md) for the full list of your billing and payment related capabilities.

### Contract Management

Via the Contracts page, you get self-service access to all cloud contracts you are being billed for through DoiT International.

### User and Role Management

Use User Management to:

* [Add colleagues](user-management/creating-a-new-user.md) to your CMP team.
* Management Billing Profile assignments.
* Configure notifications for alerts like payment reminders, new invoices, and more.
* [Set up and grant roles ](user-management/manage-roles.md)that give access to various CMP features.

### Managed Cloud Support

Within the CMP you can resolve your cloud issues quickly with hyper-responsive and unlimited support from DoiT International— **at no extra cost**.

* [Open tickets](tickets/open-a-new-support-request.md) with experienced Cloud Architects and Engineers.
* View open or historical tickets and their statuses.
* [Share tickets](tickets/ticket-sharing.md) with other team members.
* Stay up to date on any [known issues](tickets/cloud-infrastructure-known-issues.md) across all clouds you use.

