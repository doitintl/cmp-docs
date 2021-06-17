# Spot Scaling FAQ

### **What is a Spot instance?**

Spot instances are spare EC2 capacity that can save you up to 90% off On-Demand prices that Amazon Web Services can interrupt with a 2-minute notification. Spot uses the same underlying EC2 instances as On-Demand and Reserved Instances and is best suited for fault-tolerant, flexible workloads. In addition, spot instances provide an additional option for obtaining compute capacity and can be used along with On-Demand and Reserved Instances.

### **How is a Spot instance different from an On-Demand instance?**

While running, Spot instances are the essentially the same as On-Demand. The main differences are that Spot instances typically offer a significant discount over On-Demand prices. The tradeoff is that your spot instances can be interrupted by Amazon EC2 for capacity requirements with just two minutes' notice. Spot prices adjust gradually based on long-term supply and demand for spare EC2 capacity. See [here](https://www.amazonaws.cn/en/ec2/spot-instances) for details.

### **When to Use Spot Instances?**

Spot instances are most suitable for applications that have fault tolerance built in, are stateless, or perform data processing in large clusters \(for example, Hadoop\). 

Additional use cases include:

* **Batch processing** — you can use the AWS Batch service in combination with spot instances to run batch processing on spot instances that are currently available at a low cost. This can generate significant cost savings compared to running the same batch process using on-demand instances. 
* **Continuous integration** — development and testing are very common in a cloud environment. Dev/test tasks typically run on an irregular schedule, and because they are not production workloads, they can tolerate occasional interruptions. 
* **High performance computing \(HPC\)**—you can use spot instances to run massively parallel workloads like artificial intelligence analytics applications. These applications run on graphical processing units \(GPUs\), and since GPU instances are expensive, spot instances can be a big help.

### **What are the best practices to use Spot instances?**

We highly recommend using more than one Availability Zone and be flexible about the instance types to maximize the amount of Spot capacity available to you. A Spot capacity pool is a set of unused EC2 instances with the same instance type, operating system, Availability Zone, and network platform \(EC2-Classic or EC2-VPC\). 

### **What price will I pay for a Spot instance?**

With Spot Instances, you pay the Spot price that's in effect for the time period your instances are running. Spot Instance prices are set by Amazon EC2 and adjust gradually based on long-term trends in supply and demand for Spot Instance capacity. To learn more about please visit the AWS spot pricing [page](https://aws.amazon.com/ec2/spot/instance-advisor/).

### **What happens if there are no available spot instances?**

Spot Scaling supports Fallback to on-demand for scenarios where there are no available spot instances to ensure your workload availability, and it reverts back to spot instnaces as soon as they available again.

### **How do you calculate the Potential Savings?**

The potential saving calculation is based on the following inputs:  
 1. The number of the desired instances in the Auto Scaling Group  
 2. The diff between on-demand prices to spot prices per 1 hour  
 3. The number of hours in a given month \(approx 730 hours\)

### **What if I want to control the proportion of the spot and on-demand instances?**

By default Spot Scaling recommends 20% of desired capacity exists on-demand and 80% with spot instances.However, you can define the percentage split of On-Demand Instances and Spot Instances according to your use case.

