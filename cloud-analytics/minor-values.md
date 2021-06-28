---
description: 'by default, reports hide very small values to make reports more "readable"'
---

# Understanding "Minor Values"

To make reports more human-readable, very small values are removed by default from CMP Cloud Analytics reports, for the Cost metric.

{% hint style="info" %}
By default, CMP will remove report result cells that are &lt; $1. For example, a report that groups by “project” and by "day", will not show data for days that have less than $1
{% endhint %}

While this is very useful for performing cloud cost analytics, it may cause reports not to match the invoices, though by a very small amount \(usually far less than US$1\).

To make Cloud Analytics reports show "minor values", please enable the "Minor Values" filter and run the report again.

![Cloud Analytics Report with Minor Values filter disabled](../.gitbook/assets/show-minor-values.png)

{% hint style="info" %}
The "Filtering minor values" option is not available for "Usage" and "Savings" metrics.
{% endhint %}



