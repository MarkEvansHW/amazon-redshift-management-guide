# Viewing Cluster Metrics During Load Operations<a name="performance-metrics-loads"></a>

When you view cluster performance during load operations, you can identify queries that are consuming resources and take action to mitigate their effect\. You can terminate a load if you don't want it to run to completion\. 

**Note**  
The ability to terminate queries and loads in the Amazon Redshift console requires specific permission\. If you select the **Amazon Redshift Read Only** AWS managed policy or create a custom policy in IAM, and you want users to be able to terminate queries and loads, make sure to add the `redshift:CancelQuerySession` action to the policy\. Users who have the **Amazon Redshift Full Access** policy already have the necessary permission to terminate queries and loads\. For more information about actions in IAM policies for Amazon Redshift, see [Access Control](redshift-iam-authentication-access-control.md#redshift-iam-accesscontrol)\.

**To view cluster metrics during load operations**

1. Sign in to the AWS Management Console and open the Amazon Redshift console at [https://console\.aws\.amazon\.com/redshift/](https://console.aws.amazon.com/redshift/)\.

1. In the left navigation pane, click **Clusters**\.

1. In the **Cluster** list, select the cluster for which you want to view cluster performance during query execution\.  
![\[Image NOT FOUND\]](http://docs.aws.amazon.com/redshift/latest/mgmt/images/cm-metrics-10.png)

1. Click the **Loads** tab\.  
![\[Image NOT FOUND\]](http://docs.aws.amazon.com/redshift/latest/mgmt/images/cm-metrics-110.png)

1. In the load list, find the load operation you want to work with, and click the load ID in the **Load** column\.  
![\[Image NOT FOUND\]](http://docs.aws.amazon.com/redshift/latest/mgmt/images/cm-metrics-120.png)

1. In the new **Query** tab that is opened, you can view the details of the load operation\.

   At this point, you can work with the **Query** tab as shown in [Viewing Query Performance Data](performance-metrics-queries.md)\. You can review the details of the query and see the values of cluster metrics during the load operation\.

**To terminate a running load**

1. Sign in to the AWS Management Console and open the Amazon Redshift console at [https://console\.aws\.amazon\.com/redshift/](https://console.aws.amazon.com/redshift/)\.

1. In the left navigation pane, click **Clusters**\.

1. In the **Cluster** list, click the cluster you want to open\.

1. Click the **Loads** tab\.

1. Do one of the following:

   + In the list, select the load or loads that you want to terminate, and click **Terminate Load**\.

   + In the list, open a load if you want to review the load information first, and then click **Terminate Load**\.

1. In the **Terminate Loads** dialog box, click **Confirm**\.