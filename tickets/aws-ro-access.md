---
description: how to securely grant DoiT International access to your AWS account
---

# Read-Only Access to AWS

DoiT International is committed to access transparency and access approval. When you open a technical support request with DoiT International, we may need to access your AWS account so we could help you in the most effective way, including to involve the AWS support team.

### Important to Know

* Your AWS account is not accessed for any reason other than to fulfill contractual obligations
* Valid business justification required for any access by our engineering personnel
* Approve or dismiss requests for DoiT employees access, working to support your service

### How does it work?

When you request technical support and create a new service request with DoiT International, you will be offered to grant DoiT International access to the AWS account set in your request.

![](../.gitbook/assets/image-43-.png)

To make it easier for you, we have prepared an AWS CloudFormation stack you can run from here [https://l.doit-intl.com/aws-ops-cfn](https://l.doit-intl.com/aws-ops-cfn)

Before deploying the AWS CloudFormation stack, you can download and review it at [https://doit-aws-ops-prod-templates.s3.amazonaws.com/doitmanagement.yaml](https://doit-aws-ops-prod-templates.s3.amazonaws.com/doitmanagement.yaml)

The CloudFormation will create an IAM Policy and IAM Role the DoiT International engineers can use to access your AWS account. 

The CloudFormation will use a small AWS Lambda function to notify our system of the created role so that we can add it to our system automatically, this saves you copying and pasting. You can see in the CloudFormation that the Lambda runs with very restricted permissions to just serve this purpose.



