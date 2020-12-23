---
description: Cost allocation tags we natively support in Cloud Management Platform
---

# AWS Cost Allocation Tags

We have enabled the following user-defined tags \(case sensitive\) across our AWS consolidated billing accounts.

### User-defined cost allocation tags

```text
Alias
alias
Billing
billing
Env
env
Environment
environment
Name
Owner
owner
Product
product
Project
project
team
Team
unit
Unit
glue_job
service-name
kubernetes.io/service-name
```

### AWS-generated cost allocation tags

```text
aws:cloudformation:stack-name	
aws:createdBy	
aws:cloud9:owner	
aws:cloudformation:logical-id	
aws:cloud9:environment	
aws:cloudformation:stack-id	
aws:backup:source-resource	
aws:ec2launchtemplate:id	
aws:transfer:customHostname	
aws:elasticmapreduce:job-flow-id	
aws:servicecatalog:provisioningPrincipalArn	
aws:ecs:serviceName	
aws:elasticfilesystem:default-backup	
aws:ec2launchtemplate:version	
aws:elasticmapreduce:instance-group-role	
aws:servicecatalog:productArn	
aws:dlm:lifecycle-schedule-name	
aws:servicecatalog:portfolioArn	
aws:autoscaling:groupName	
aws:ec2spot:fleet-request-id	
aws:servicecatalog:source	
aws:zocalo:alias	
aws:ssmmessages:session-id	
aws:ec2:fleet-id	
aws:ecs:clusterName	
aws:dlm:lifecycle-policy-id	
aws:ssmmessages:target-id	
aws:eks:cluster-name	
aws:elasticmapreduce:editor-id	
aws:dlm:expirationTime	
aws:transfer:route53HostedZoneId
```

Ideally, you will be using one of these tags to track your AWS cost allocations. If you need a custom cost allocation tag, please open a support ticket using http://support.doit-intl.com

For more information about cost allocation tags, please read [this post](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-alloc-tags.html) about Cost Allocation Tags in AWS's documentation.

