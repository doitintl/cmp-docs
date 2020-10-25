# Edit Cloud Analytics Report

_**Note:** If you're new to Cloud Reports and/or haven't created a Cloud Report yet, we recommend reading our post on_ [_**Creating Cloud Reports**_](create-cloud-report.md) _before reading further._

There are several types of edits you can make to your Cloud Report:

* Adding additional dimensions
* Changing the metric by which your dimensions are being measured
* Reordering results
* Changing the visualization
* Modifying the time interval and/or range
* Filtering dimensions

Most of these are self-explanatory, as you would simply make your changes the same way you made your original selection. Let's briefly go over your metric options and how to filter your dimensions.

## **Metric Options**

**Cost:** Analyze your reports on a basis of how much your selected dimensions cost you.

**Usage**: Analyze your reports and selected dimensions on a usage basis. Make sure to pair this with the Unit chip as a Breakdown Dimension.

**Savings:** Analyze your reports and selected dimensions on a savings basis. These savings come as a result of your commercial agreement with Google Cloud and the agreed-upon discount between your company and DoiT International.

## **Filtering Dimension Values**

To view a subset of your dimension's values, click on the dimension chip you'd like to filter. Then check the boxes next to the subsets you'd like to view in the report.

You may also exclude a selection of values, or limit results to a specific number of values arranged in descending order according to the Metric \(Cost**,** Usage, or Savings\) selected.

Next, click "Save" in the lower-right corner of the popup modal.

![](../.gitbook/assets/cloudreports_filters.jpg)

Your filters are displayed along with any other visible configurations on the right-hand collapsable sidebar. To expand it, click on the **&gt;\|** icon in the lower-right corner of your screen.

![](../.gitbook/assets/cloudreports_filtervisibleconfig.jpg)

Finally, click the "Run" button to generate an updated report that reflects the filters you've selected.

## **Performing Edits**

Depending on the edits you're making to your Cloud Report, you may have to re-run your report for the changes to reflect while other edits will show up in real-time.

### **Real-time updates**

Any edits which don't alter the results themselves will update the report in real-time. This includes changes made to:

* Metric measurement
* Chart type
* Sorting of results
* [ML Features](understanding-your-ml-features.md)

Below, we can see the first three types of real-time edits being performed. 

![](../.gitbook/assets/cleanshot-2020-06-30-at-12.49.48.gif)

### **Edits requiring a refresh**

Updates made to reports which require you to refresh it include:

* Adding additional dimensions
* Modifying the time interval and/or range
* Filtering dimensions

Below, you'll see what it looks like to filter a dimension.

![](../.gitbook/assets/cleanshot-2020-06-30-at-13.19.17.gif)

