---
description: Security and Data Access Policy for Cloud Management Platform
---

# Data Access Policy

This document outlines what customer data we access, why we do that, what data we store, and how we do that.

**TL;DR:** We only access data required for Cloud Management Platform \(CMP\) functionality. We store and handle your data in a secure way, encrypted in transit and at rest. We do not provide the data to any 3rd party, with the exceptions required for core CMP functionality and listed below.

* [What we access - GCP](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_7bc78dd6-eab0-4188-bf00-b0017561511f)
* [What we store](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_a0f898d0-5b4d-4976-94da-9babbed3ebc6)
* [How we handle and store your data](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_24ce7c2f-7dbb-482d-94a7-3a73a39adcb7)
* [Who can access your data](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_e71c7f53-d7e9-4273-a1cc-49e6714bbfa6)
* [3rd parties](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_2dd17fc8-13d8-4aad-b58c-3a9be9bc310e)
* [Compliance](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_cb4c8c24-7b2b-4458-b890-8c866b99aee6)
* [External references](https://help.doit-intl.com/hc/en-us/articles/360043006652-Security-and-Data-Access-Policy-for-Cloud-Management-Platform#h_923e9d39-0606-471f-bbb3-2f899c859d8c)

### What we access - Google Cloud <a id="h_7bc78dd6-eab0-4188-bf00-b0017561511f"></a>

The list below denotes all permissions we require to your Google Cloud Organization and why.

_Note: While this provides us permissions to read info about your resources, none of these allow us to access your data, such as GCS objects or BigQuery table's data._

* _resourcemanager.organizations.get, resourcemanager.organizations.getIamPolicy, resourcemanager.folders.get, resourcemanager.folders.list, resourcemanager.projects.get, resourcemanager.projects.list_  Used to get information about your GCP resource hierarchy and correlate with billing. 
* _resourcemanager.projects.create_  Required for [CMP Sandbox](https://help.doit-intl.com/hc/en-us/articles/360042612671-Create-Google-Cloud-Sandbox-Accounts) functionality.  
* _bigquery.datasets.create, bigquery.datasets.get, bigquery.tables.get, bigquery.tables.list, bigquery.jobs.get, bigquery.jobs.list, bigquery.jobs.listAll, bigquery.jobs.create_ Required for BigQuery info and optimization.  
* _compute.addresses.list, compute.disks.get, compute.disks.list, compute.images.get, compute.images.list, compute.instances.get, compute.instances.list, compute.projects.get, compute.regions.get. compute.regions.list, compute.snapshots.get, compute.snapshots.list, compute.zones.get, compute.zones.list, compute.commitments.get, compute.commitments.list, recommender.computeInstanceMachineTypeRecommendations.list_  Required for Compute instance optimization and commitments recommendation functionality.  
* compute.instances.setMachineType, compute.instances.stop, compute.instances.start   Required for [Right-sizing](https://help.doit-intl.com/hc/en-us/articles/360039630271-Rightsizing-for-Google-Cloud) functionality.  
* _serviceusage.services.enable_  Used to enable required APIs in projects \(such as the [Recommender API](https://cloud.google.com/recommender/docs/reference/rest)\)  
* _logging.sinks.get, logging.sinks.create_  Required for [superQuery Optimization Dashboard](https://help.doit-intl.com/hc/en-us/articles/360040580752-superQuery-Dashboard) functionality.

### What we store <a id="h_a0f898d0-5b4d-4976-94da-9babbed3ebc6"></a>

We only store data required for CMP functionality.

* **Cloud Billing exports** - required for core Billing functionality, stored in BigQuery
* **User information** - required for core CPM functionality, stored in Firestore
* **Assets created by using CMP** \(Invoices, Billing Profiles...\) - required for core CMP functionality, stored in Firestore
* **Contracts** - required for core CMP functionality, stored in Google Cloud Storage
* **Service Account Keys** - required for core CPM functionality, stored in Firestore, encrypted with KMS

### How we handle and store your data <a id="h_24ce7c2f-7dbb-482d-94a7-3a73a39adcb7"></a>

All data we handle are encrypted in transit using industry-standard protocols like HTTPS \(TLS\). 

All data we store are encrypted at rest:

* **BigQuery** - using Google-managed encryption keys and Advanced Encryption Standard \(AES\).
* **Firestore** - using Google-managed encryption keys and AES.
* **Cloud Storage** - using Google-managed encryption keys and AES
* **Service Account Keys** - encrypted using GCP KMS and keys we manage.

### Who can access your data <a id="h_e71c7f53-d7e9-4273-a1cc-49e6714bbfa6"></a>

DoiT employees in customer-facing roles, such as Account managers and Support engineers, can access your data using the CMP platform. Only a small team of core CMP developers is able to access your data directly in the underlying storage.

Service Account keys are only used by backend systems to retrieve relevant data from GCP. Only a small team of core CMP developers has access to the KMS keys used for encryption and would be able to decrypt the keys.

### 3rd parties <a id="h_2dd17fc8-13d8-4aad-b58c-3a9be9bc310e"></a>

We do not provide your data to any 3rd party, with the exceptions listed below required for core CMP functionality.

* **CMP Support** - We use Zendesk as a backend for support ticketing functionality. All ticket related data are stored in Zendedsk and retrieved using Zendesk APIs \[1\].
* **Payments** - We use Stripe for payments. All payment related data \(such as Credit card or bank account details\) are stored in the Stripe platform and used via Stripe APIs \[2\].

### Compliance <a id="h_cb4c8c24-7b2b-4458-b890-8c866b99aee6"></a>

EU and GDPR Compliance - we have many customers in the European Economic Area and we handle your data in compliance with the General Data Protection Regulation \(GDPR\) \[3\].

We're working towards completing our SOC 2 Type 2 audit. We anticipate the Type 2 report being available later in 2020.

### External references <a id="h_923e9d39-0606-471f-bbb3-2f899c859d8c"></a>

* \[1\]: Zendesk Privacy and Data Protection: [https://www.zendesk.co.uk/company/privacy-and-data-protection/](https://www.zendesk.co.uk/company/privacy-and-data-protection/)
* \[2\]: Stripe Global Privacy Policy: [https://stripe.com/gb/privacy](https://stripe.com/gb/privacy)
* \[3\]: EU Data Protection page: [https://ec.europa.eu/info/law/law-topic/data-protection\_en](https://ec.europa.eu/info/law/law-topic/data-protection_en)
