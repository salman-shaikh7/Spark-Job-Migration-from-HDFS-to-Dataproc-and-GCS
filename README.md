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