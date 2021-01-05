---
description: How to purchase AWS EC2 Flexible Reservations and monitor their utilization
---

# Purchase Flexible Reservations

### Overview

Flexible Reserved Instances let you commit to EC2 Reserved Instances in one-month intervals while still sharing in the AWS-listed RI commitment discount. With Flex RIs, you'll eliminate RI lock-in risk for your less predictable workloads.

In order to use Flexible Reservations, your AWS account/s should be consolidated with DoiT International billing organization. DoiT International is a global [AWS Advanced Channel Reseller](https://partners.amazonaws.com/partners/001E000001HPlIAIA1/).

{% hint style="info" %}
Required Permissions: **Flexible RI Admin**
{% endhint %}

### How-To Purchase FlexRIs

To begin, click the 'Flexible RIs' icon on the left-hand side of the page. Once you're at the Flexible Reserved Instances page, click on 'New Order', located on the right-hand side of the page.

![](../.gitbook/assets/cleanshot-2020-11-26-at-10.42.36.jpg)

Complete your Flexible Reserved Instances order by providing the following information: 

| Field | Description |
| :--- | :--- |
| Account | AWS account for this order |
| Region | AWS region for this order |
| Instance | note, only instances not associated with existing reservations or saving plans are shown |
| Qty | how many instances of the selected "Instance Type" the order should include |
| Recurring | For orders with a recurring basis, select the last month you want this order to go  |
| Notes | Use notes to give more context to your order such as PO numbers, workload names, etc. |

Click "Submit" and your order will be created and become visible in the list:

![](../.gitbook/assets/flexriordersuccess.jpg)

{% hint style="info" %}
Please note that new orders and editing previous orders can only be submitted up to the 25th day of the month. After that date, orders will become **Pending** while we conduct an internal review before activating your Flexible Reservations.
{% endhint %}

### Monitoring FlexRIs

At the top of the FlexRI page, you'll see four FlexRI Reporting metrics that give you a high-level overview of your past and existing FlexRI purchases:

* **Total Expected Savings** - the maximum amount you could have saved, given 100% utilization
* **Actual Savings** - the amount you actually saved
* **Flexible Reservation Utilization** - how well you are utilizing your Flexible Reserved Instances.
* **YTD Savings** - the total saving across all your reservations, from the beginning of the current year.

{% hint style="info" %}
Note: The first three metrics are based on what is shown in the table, meaning taking into account any filters you've set on your orders. The last metric takes _every_ FlexRI order into account when calculating the number.
{% endhint %}

To view information on a specific order, click on the arrow next to an active or retired order to expand your order and view details further. 

You can see the difference between the on-demand price per hour vs. the FlexRI, and further inspecting the utilization graph for additional details of your flexible reservation.

![](../.gitbook/assets/viewflexriorder.jpg)

### FlexRIs Invoices

For each order of Flexible Reservations, you'll see one or both of the following lines on your monthly invoice:

* Flexible RI \#ID Savings
* Flexible RI \#ID Underutilization

The "Flexible RI Savings" will state the amount you have saved due to the purchase of Flexible Reservation/s for a given month.

The optional "Flexible RI Underutilization" will state the amount deducted from the cost of the reservation if the underlying instance wasn't utilized 100% of the time during the month.

View the bite-sized video below for a closer look at purchasing and viewing your Flex RIs.

{% embed url="https://www.loom.com/share/7385b68facec49569fcbc3d377f05fbf" %}



