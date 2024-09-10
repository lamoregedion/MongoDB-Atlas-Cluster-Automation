# Atlas Cluster Automation Using Scheduled Triggers

Every action you can take in the Atlas user interface is backed by a corresponding [Administration API](https://www.mongodb.com/docs/atlas/reference/api-resources-spec/), which allows you to easily bring automation to your Atlas deployments. Some of the more common forms of Atlas automation occur on a schedule, such as pausing a cluster that’s only used for testing in the evening and resuming the cluster again in the morning.

Having an API to automate Atlas actions is great, but you’re still on the hook for writing the script that calls the API, finding a place to host the script, and setting up the job to call the script on your desired schedule. This is where Atlas [Scheduled Triggers](https://www.mongodb.com/docs/atlas/triggers/#scheduled-triggers) come to the rescue.

In this [Atlas Cluster Automation Using Scheduled Triggers](https://www.mongodb.com/developer/products/atlas/atlas-cluster-automation-using-scheduled-triggers) article I will show you how a Scheduled Trigger can be used to easily incorporate automation into your environment. In addition to pausing and unpausing a cluster, I’ll similarly show how cluster scale up and down events could also be placed on a schedule. Both of these activities allow you to save on costs for when you either don’t need the cluster (paused), or don’t need it to support peak workloads (scale down).

