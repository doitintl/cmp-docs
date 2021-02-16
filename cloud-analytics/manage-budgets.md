---
description: Track your cloud spend against your planned spend.
---

# Manage Budgets

{% hint style="success" %}
_**Note:** If you're new to Budgets and/or aren't familiar with Attributions we recommend reading our post on_ [_Creating Attributions_](attributing-cloud-spend.md) _before reading further._
{% endhint %}

Setting budgets and forecasting IT spend is a well-established FinOps practice, ensuring that you won’t get surprised by your cloud bill.

Within the Cloud Management Platform, you can set Budgets using [Attributions](attributing-cloud-spend.md), custom-defined groupings of cloud resources \(accounts, services, etc.\) that map to your organizational and financial reporting structure.

{% hint style="info" %}
Required Permissions: **Cloud Analytics**
{% endhint %}

### Creating budgets

Go to the main Budgets page by clicking on the \[1\] Cloud Analytics icon in the left-hand navigation panel, and then clicking on the \[2\] Budgets tab.

You will see a list of your team’s Budgets that you’ve created, been shared on, or have been made public if there are any.

To create a new Budget, click the \[3\] “**+ NEW BUDGET**”  button. 

![](../.gitbook/assets/budgets1.jpg)

### Configure your Budget

After giving your Budget a suitable name, set the Budget’s scope by selecting the Attribution\(s\) your Budget will be allocated to. As mentioned earlier, [Attributions](attributing-cloud-spend.md) let you group any combination of cloud resources \(and their associated costs\) so you can better relate cloud costs to your financial reporting structure.

Next, select the Budget type, time interval, and start date. If you’re configuring a Fixed Budget, you’ll need to set the end date as well. After defining the above, it’s time to set your Budget’s amount or upper limit. Before entering a number, it might be helpful to see what the last period’s cost was for reference. 

Click on the “**Refresh**” icon to view your last period’s cost, given the Budget scope, time interval, and date\(s\) you’ve selected.

![](../.gitbook/assets/refreshbudget.gif)

After refreshing and setting a Budget amount, two visual bars will appear below:

* **Current Spend:** Your current spend relative to alert thresholds \(next section\) you've set.
* **Forecasted Spend:** How much you are forecasted to spend by the end of the Budget period.

Lastly, if you’re configuring a recurring Budget, you have the option to factor in growth in spending for subsequent periods. This will adjust your Budget amount in future periods, increasing it by a growth percentage rate set by you.

Enable this by checking the “Allow growth in recurring budget periods” box, and then enter in a % growth rate for each subsequent period.

![](../.gitbook/assets/growthbudget.jpg)

### Set Budget Thresholds

After configuring your Budget, you can set up to three Budget thresholds. By default, thresholds are set at 50%, 85%, and 95% of your Budget amount, but you can modify any of the percentages as you wish.

You will see the corresponding amount for each threshold, and the forecasted date that you will reach each threshold.

Setting thresholds is useful especially when setting up Budget alerts.

{% hint style="info" %}
Note: In order to see forecasted dates for Budget thresholds, you need to click the "Refresh" button after setting a Budget amount.
{% endhint %}

![](../.gitbook/assets/budgets3.jpg)

### Sharing Budgets

By default, Budgets are only viewable by the creator. Sharing your Budget makes it visible to others.

To share your Budget, click the “Share” icon in the top right of the “Sharing & Alerting” widget. 

This will open a pop-up that will give you two options when sharing:

* Give everyone on your team Viewer access.
* Explicitly give someone from your team Viewer or Editor Access.

Having View access means the Budget will appear on the main Budgets page, and that you can view the Budget itself — but you can’t make any edits to the Budget.

Edit access allows you to edit a Budget, but not delete it. Only those with Owner access can delete Budgets.

Once you've entered the email\(s\) of who you're sharing your Budget with, click "Add" and then hit "Save" to apply your changes.

{% hint style="info" %}
Sharing someone on your Budget does not mean they will be alerted when usage thresholds are exceeded. 
{% endhint %}

![](../.gitbook/assets/budgets4.gif)

#### Changing a user’s Budget permission

To change a user's permission, make them the owner of the report, or remove them from the report, click on the dropdown next to their email in the Share Budget pop-up.

Then make a selection and click "Save" to apply the changes.

### Receive Alerts for Budgets

Alerts help notify yourself and others when you exceed a Budget threshold.

To add someone as a recipient of an email alert notification, enter their email in the “Send to” text box in the “Sharing & Alerting” widget. If they haven't been shared on the Budget already, you will be asked to share it with them first before being able to subscribe them to the Budget's alert.

You will see a confirmation in the lower-left corner of your screen when someone has been successfully subscribed to your Budget’s email alerts.

![](../.gitbook/assets/budgets5.jpg)

When you exceed a Budget threshold, you’ll receive an email detailing:

1. Which budget threshold you exceeded
2. Your current spend
3. The forecasted date when you will reach 100% of your budget

Here is what a typical alert looks like:

![](../.gitbook/assets/budgetalert.jpg)





