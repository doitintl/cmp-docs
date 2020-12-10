---
description: Share your reports via automatic email delivery
---

# Schedule Report Email Delivery

You can send a copy of your Cloud Analytics Reports to yourself and your stakeholders on a regular basis by setting up an email delivery schedule.

## Create a Scheduled Email Delivery

Begin by opening a report that you have "Owner" access to. Then, click on the mail icon at the far-right side of your screen.

![](../.gitbook/assets/schedulereport1.jpg)

 Next, configure your scheduled report by:

* CC'ing anyone who you'd like to be included
* Editing the scheduled email's subject if you'd like it to differ from the report's name
* Add an additional message to provide more context for recipients.
* Set up the scheduled report's interval using [unix-cron format](https://crontab.guru/) and specify the timezone.

![](../.gitbook/assets/schedulereport2.jpg)

If you've cc'd a user\(s\) who was not previously shared on the report, a modal will appear asking you to add that user to the report. You can choose whether to give the user\(s\) "Viewer" or "Editor" access rights.

![](../.gitbook/assets/scheduledreportinvite.jpg)

Once the day & time you set under "Frequency" arrives, your scheduled report will look something like the image below.

From the email, you'll be able to open the report in CMP to investigate further.

![](../.gitbook/assets/scheduledemail.jpg)

## Updating Scheduled Delivery

To update a report's scheduled email delivery configuration — or delete it — open a report that already has a configured schedule. Then, click on the blue envelope icon in the far-right side of your report's page.

![](../.gitbook/assets/updateschedulereport.jpg)

In the "Schedule Report Email Delivery" modal, make your changes then click on the Update button.

## Deleting Scheduled Delivery

If you're deleting the scheduled report, simply click on the Delete button.

![](../.gitbook/assets/updateschedule2.jpg)

## Limitations

A few limitations exist for scheduled reports:

* Each report can only have one email schedule
* The person who scheduled the report is always included in the email
* The minimum interval for a scheduled report is 24 hours
* Only chart-based reports can be scheduled \(i.e. no tables or heatmaps\)

