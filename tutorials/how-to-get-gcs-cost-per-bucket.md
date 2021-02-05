---
description: extract cost insights about your Google Cloud Storage buckets
---

# How to get GCS cost per bucket

### Introduction

Google Cloud Storage \(GCS\) is object storage for companies of all sizes. You can use GCS to store any amount of data and retrieve it as often as you’d like.

Cloud Management Platform \(CMP\) is a software service that automatically identifies cloud cost issues, gives those insights to relevant teams, and delivers the context you need to get back on track.

{% hint style="success" %}
This tutorial is intended for people who are somewhat familiar with Google Cloud Console and want to learn about the Cloud Management Platform. There are explanations for all of the actions in Google Cloud Console, but they may not explain everything needed for someone completely new to Google Cloud. There is no assumed knowledge about CMP.
{% endhint %}

### Label Google Cloud Storage Buckets

Start with adding labels to your Google Cloud Storage buckets. 

1. Open the [Cloud Storage browser](https://console.cloud.google.com/storage/browser) in the Google Cloud Console
2. In the bucket list, find the bucket you want to apply a label to, and click its **overflow** menu![](https://cloud.google.com/images/overflow_menu_icon.png)
3. Click Edit labels
4. In the side panel that appears, click the + Add label button
5. Specify `bucket-name` as a 'key' and the name of the bucket as a 'value' for your label
6. Click Save

{% hint style="info" %}
In the Edit labels side panel, you can also edit the Value of existing labels.
{% endhint %}

### Create Cloud Analytics Report

Start with creating a new CMP Analytics Report

1. [ ] Open [CMP Analytics](https://app.doit-intl.com/analytics)
2. [ ] Click "Explore" to start a new report 

![](../.gitbook/assets/image%20%283%29.png)

* [ ] 






