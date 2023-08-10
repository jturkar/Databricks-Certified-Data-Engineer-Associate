# Databricks-Certified-Data-Engineer-Associate
Data Engineer Associate Certification Preparation guide

## Types of Cluster

 All-purpose clusters | Job clusters
 ------------- | -------------
 Can be shared by multiple users | used for operationalizing your code
 Best for performing ad-hoc analysis, data exploration, or development | Job clusters terminate when your job ends, reducing resource usage and cost

 ## Cluster mode 

 Multi-Node | Single Node
 -------- | -------
 Are intended for jobs that use small amounts of data | Are for larger jobs with distributed workloads
 used for non-distributed workloads such as single-node ML libraries | 

## Autoscaling
### Note 
Compute auto-scaling has limitations scaling down cluster size for Structured Streaming workloads. Databricks recommends using Delta Live Tables with Enhanced Autoscaling for streaming workloads.
Autoscaling allows clusters to resize automatically based on workloads.

## Pools

Create a pool reduce cluster start and scale-up times by maintaining a set of available, ready-to-use instances. **Databricks recommends taking advantage of pools to improve processing time while minimizing cost.**

## Databricks Runtime versions
Databricks recommends using the latest Databricks Runtime version for all-purpose clusters.  


