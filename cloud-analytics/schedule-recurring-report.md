---
description: >-
  You can send a copy of your Cloud Analytics Reports to yourself and your
  stakeholders on a regular basis by setting up an email delivery schedule.
---

# Schedule Report Email Delivery

### Create a Scheduled Email Delivery

Begin by opening a report that you have "Owner" access to. Then, click on the mail icon at the far-right side of your screen.

![](../.gitbook/assets/schedulereport1.jpg)

 Next, configure your scheduled report by:

* Other stakeholders, you'd like to be included
* Update email's subject if you'd like it to differ from the report's name
* Add an optional message to provide more context for recipients
* Set up the scheduled report's interval using [unix-cron format](https://crontab.guru/) and select the timezone

{% hint style="info" %}
You can't schedule a report to be delivered more than once a day.
{% endhint %}

![](../.gitbook/assets/schedulereport2.jpg)

If you've included someone who doesn't have access to the report, you will be asked to add that user to the report. You can choose whether to grant the "Viewer" or "Editor" access.

![](../.gitbook/assets/scheduledreportinvite.jpg)

Your scheduled report will look something like the image below. From the email, you'll be able to preview the report and open an interactive report in Cloud Analytics, by using the "Open Live Report" button.

![](../.gitbook/assets/scheduledemail.jpg)

### Updating Scheduled Delivery

To update the scheduled email delivery configuration, open a report that already has a configured schedule. Then, click on the blue envelope icon on the far-right side of your report's page. Then, make the changes then click on the Update button.

![](../.gitbook/assets/updateschedulereport.jpg)

### Deleting Scheduled Delivery

If you need to delete the scheduled report, please use the Delete button on the "Schedule Report Email Delivery" dialog.

![](../.gitbook/assets/updateschedule2.jpg)

### Limitations

A few limitations exist for scheduled reports:

* Each report can only have a single email delivery schedule
* The person who scheduled the report is always included in the email
* The minimum interval for a scheduled report is 24 hours. In other words, you can't schedule a report to be delivered more than once a day.
* Only chart-based reports can be scheduled \(i.e. no tables or heatmaps\)

