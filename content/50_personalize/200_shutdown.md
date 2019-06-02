+++
title = "Shutting Down"
chapter = false
weight = 200
+++

### Shutting Down the SageMaker Notebook Instance

1. Open the Amazon SageMaker console and click on **Notebook instances**
2. Find the notebook instance listed as _[Name]-lab-notebook_, select its radio button and then click the **Actions** dropdown.

    ![Terminate instance](/images/terminateNotebook.png)

3. Click **Stop** to stop the Notebook Instance.  This does not delete the underlying data and resources.  After a few minutes the instance status will change to _Stopped_, and you can now click on the **Actions** dropdown again, but this time select **Delete**.

Note that by selecting the name of the Notebook instance on this dialog you are taken to a more detailed information page regarding that instance, which also has **Stop** and **Delete** buttons present – notebooks can also be deleted using this method.

### Shutting Down the CloudFormation Stack

The CloudFormation stack we deployed in [this step]({{<ref "20_deploytemplate.md" >}}) contains multiple resources that we'll to terminate:

* EC2 Instance
* Application Load Balancer
* Networking: Internet Gateway, VPC, Subnets, NAT Gateways, Route Table
