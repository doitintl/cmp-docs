# Setting Up Spot Scaling

## Connect your AWS Accounts

To use Spot Scaling, you must provide access to your AWS account\(s\) to the CMP. [**Read this article**](https://help.doit-intl.com/amazon-web-services/add-your-amazon-web-services-iam-role) to see how to link your AWS account\(s\).

{% hint style="info" %}
If you’ve already linked your AWS account\(s\) to the CMP, go to this step instead.
{% endhint %}

As part of linking your account, you will need to create an AWS IAM Role and attach an IAM Policy to it containing a requisite set of permissions. These permissions allow Spot Scaling to function — monitor your ASG behavior, make spot instance recommendations, and allow you to implement them from the CMP

In the same article linked above, read the section on [**how to create a policy for Spot Scaling**](https://help.doit-intl.com/amazon-web-services/add-your-amazon-web-services-iam-role#spot0) with the requisite permissions.

## Setup Spot Scaling

If your account was already linked prior to enabling Spot Scaling functionality, you need to update the role attached to the account with the additional requisite permissions for Spot Scaling**.**

**Follow** [**these instructions**](https://help.doit-intl.com/amazon-web-services/add-your-amazon-web-services-iam-role#adding-a-feature) **on adding a feature to an already-linked AWS account.** Be sure to check the box next to "Spot Scaling", as shown below.

![](../.gitbook/assets/image%20%2869%29.png)



