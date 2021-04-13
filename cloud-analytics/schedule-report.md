---
description: >-
  Send periodically Cloud Analytics Reports by setting up an email delivery
  schedule
---

# Schedule Report Email Delivery

You can send a copy of your Cloud Analytics report to yourself and your stakeholders on a regular basis by setting up an email delivery schedule.

{% hint style="info" %}
Required Permissions: **Cloud Analytics**
{% endhint %}

### Create a Scheduled Email Delivery

There are two ways to schedule emailed reports:

* Via a specific Report's page
* Via the main Cloud Analytics page 

#### Scheduling via a Report's Page

Begin by opening a report that you have "Owner" access to. Then, click on the mail icon at the far-right side of your screen.

![](../.gitbook/assets/schedulereport1.jpg)

 Then, configure the scheduled delivery:

* Set  other users, you'd like to be included on report's distribution
* Optionally, update email's subject and the message to provide more context for recipients
* Set up when you'd like to be delivered \(using [_cron expression_](https://crontab.guru/)\)

![](../.gitbook/assets/schedulereport2.jpg)

If you've included someone who doesn't have access to the report, you will be asked to add that user to the report. You can choose whether to grant the "Viewer" or "Editor" access.

![](../.gitbook/assets/image%20%2828%29.png)

### About Cron Expressions

The delivery time and recurrence of a Cloud Analytics Report can be configured by using a [cron expression](https://wikipedia.org/wiki/Cron#CRON_expression). Cron is a time-based job scheduler originally used in Unix-like computer operating systems. A cron expression is a string comprising of five or six fields separated by whitespace. The following table defines the fields of a cron expression and the possible values for each field.

| Minute | Hour | Day | Month | Day of the week |
| :--- | :--- | :--- | :--- | :--- |
| 0-59 | 0-23 | 1-31 | 1-12 \(Jan-Dec\)  `1`=`Jan`, `2`=`Feb`, ... `12`=`Dec` | 0-6 \(Sun-Sat\)  where `0`=`Sun`, `1`=`Mon`, ... `6`=`Sat` |

In addition to using these values, every field in a cron expression can also use special characters:

| Character | Meaning | Example |
| :--- | :--- | :--- |
| `*` | any | If the day of month field, day of the week field are each set to `*`, then the schedule starts every day. |
| `-` | range | If the day of week field is set to `1-5` or `Mon-Fri`, then the schedule starts every week Monday to Friday. |
| `,` | list | If the month field is set to `5,7,9` or `May,Jul,Sep`, then the schedule starts every May, July, and September. |
| `/` | step | If the month field is set to `*/3`, then the schedule starts during the first month and every 3 months after that: January, April, July, and October. |

{% hint style="warning" %}
Schedule intervals lower than daily are not permitted with Cloud Analytics, meaning the first 2 places must be numbers between \(0-59\) and \(0-23\)
{% endhint %}

To create a schedule that repeats, use special characters to describe when that schedule is to repeat. For example, the cron expression 30 8 \* \* Mon-Fri configures a schedule to start at 8:30 AM on every Monday, Tuesday, Wednesday, Thursday, and Friday.

Your scheduled report will look something like the image below. From the email, you'll be able to preview the report and open an interactive report in Cloud Analytics, by using the "Open Live Report" button.

Select the access level you'd like to give them, and click "Add" to give them access to the report and add them to the list of scheduled report recipients.

![](../.gitbook/assets/addpersonschedule.jpg)

Your scheduled report will look something like the image below. From the email, you'll be able to preview the report and open an interactive report in Cloud Analytics, by using the "Open Live Report" button.

Your scheduled report will look something like in the example below. From the email, you'll be able to preview the report and open an interactive report in Cloud Analytics, by using the "Open Live Report" button.

![](../.gitbook/assets/scheduledemail.jpg)

#### 

#### Scheduling via the Cloud Analytics page

You may also schedule emailed reports from the main Cloud Analytics page. 

First, find a report that you are the Owner of. Then, under the **Email Schedule** column, click on the envelope icon.

![](../.gitbook/assets/createschedule.jpg)

From there, configure your report as described above, modifying the message and interval as well as the recipients.

### Updating Scheduled Delivery

To update the scheduled email delivery configuration, open a report that already has a configured schedule. 

Then, click on the **blue** envelope icon on the far-right side of your report's page. 

Finally, make the changes then click on the Update button.

![](../.gitbook/assets/updateschedulereport.jpg)

You may also update a report's email delivery schedule from the Cloud Analytics page. 

First, identify a report that you've already set up an email schedule for, and click on the unix-cron interval ****syntax under the **Email Schedule** column for that report.

Then, as described above, make your changes and click on the Update button to implement your changes.

![](../.gitbook/assets/cleanshot-2020-12-14-at-11.36.08.jpg)

### Subscribing to a Scheduled Delivery

Add yourself as a recipient of someone else's scheduled report delivery to stay updated on reports other people on your team create.

Similar to creating a scheduled email delivery, you can subscribe to others' scheduled emails from both the main Cloud Analytics page and a specific report's page.

From the main Cloud Analytics page, identify a colleague's report that has a scheduled email set up already by looking for a **blue** envelope icon under the **Email Schedule** column.

![](../.gitbook/assets/subscribecloudschedule.jpg)

Conversely, you can subscribe to a colleague's scheduled email from a specific report's page itself.

![](../.gitbook/assets/subscribereportpage.jpg)

Confirm that you'd like to be added to the report's email distribution by clicking on **Subscribe**.

![](../.gitbook/assets/subscribeschedulereport.jpg)

### Deleting Scheduled Delivery

If you need to delete the scheduled report, please use the Delete button on the "Schedule Report Email Delivery" dialog.

![](../.gitbook/assets/updateschedule2.jpg)

### Limitations

A few limitations exist for scheduled reports:

* Each report can only have a single email delivery schedule
* Preset reports cannot be scheduled. You can [clone](cloning-and-or-customizing-cloud-reports.md#clone-reports) the report though and schedule it.
* The person who scheduled the report is always included in the email
* You can't schedule a report to be delivered more than once a day.
* Only chart-based reports can be scheduled \(i.e. no tables or heatmaps at this time\)

