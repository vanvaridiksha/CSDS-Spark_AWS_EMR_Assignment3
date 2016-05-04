# CSDS-Spark_AWS_EMR_Assignment3

In this assignment, you will be running the same recommendation system that you built for AudioScrobbler Data but on a 3 node AWS-EMR cluster.


##Setup

We will first see how to set up a 3 node [AWS - ELastic Map Reduce cluster with Spark](http://docs.aws.amazon.com/ElasticMapReduce/latest/DeveloperGuide/emr-spark-launch.html) installed on it. To follow along, make sure you have a functioning AWS account and an IAM user created. You may want to refer to this [AWS Documentation](http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-set-up.html) for setting up AWS CLI.


Also, this service offered by AWS is chargeable. Do not keep you cluster running at all times and remember to keep checking your AWS bill under the Billing and Cost Management option.

AWS offers an easy to use dashboard for creating and launching a cluster and submitting a Spark job to it. Begin by clicking on EMR from the list of services offered on your AWS dashboard. Then click on Create Cluster and you will be directed to this page: 

![SetupImage](http://i.imgur.com/arhxIA9.png)


*Give the cluster a name, enable logging(this will be very useful to troubleshoot in case of failures) and select 'Cluster' in launch mode. 
*In software configuration, select Spark from the Applications list. 
*If you have not created a an EC2 key-pair yet, create one, download it and enter its name here. Select default permissions and then go ahead and click on 'Create Cluster'.

You will now be directed to this page.
![Cluster Details](http://i.imgur.com/kBcg4aO.png)

The cluster remains in the 'Starting' state for about 10 - 15 minutes. Once the cluster is ready for use, the status will change to 'Waiting'. 







