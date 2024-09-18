# Spark Job Migration from HDFS-to-Dataproc and GCS.

Overview
In project we will migrate Apache Spark code to Cloud Dataproc. 

We will follow a sequence of steps progressively moving more of the job components over to Google Cloud services:

1.  Run original Spark code on Cloud Dataproc (Lift and Shift)
2.  Replace HDFS with Cloud Storage (cloud-native)
3.  Automate everything so it runs on job-specific clusters (cloud-optimized)

## Objective 

* Migrate existing Spark jobs to Cloud Dataproc.
* Modify Spark jobs to use Cloud Storage instead of HDFS.
* Optimize Spark jobs to run on Job specific clusters.

## Scenario

You are migrating an existing Spark workload to Cloud Dataproc and then progressively modifying the Spark code to make use of Google Cloud native features and services.

## Task 1. Migrate existing Spark jobs to Cloud Dataproc : Lift and shift

You will create a new Cloud Dataproc cluster and then run an imported Jupyter notebook that uses the cluster's default local Hadoop Distributed File system (HDFS) to store source data and then process that data just as you would on any Hadoop cluster using Spark. 

This demonstrates how many existing analytics workloads such as Jupyter notebooks containing Spark code require no changes when they are migrated to a Cloud Dataproc environment.

### STEP 1 : Configure and start a Cloud Dataproc cluster