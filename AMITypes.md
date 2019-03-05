### AMI

You can select your AMI based on
- Region, operating system, architecture (32 or 62bit), launch permissions, storage for root
- Root device storage can be EBS backed volumes or Instance Store (ephemeral storage)

EBS vs Instance Store 

All AMI's (amazon machine image) are categorized as either backed by Amazon EBS or backed by instance store. 

For EBS Volumes: The root device for an instance launched from the AMI is an Amazon EBS volume created from an Amazon EBS snapshot. 

For Instance Store Volumes: The root device for an instance launched from the AMI is an instance store volume created from a template stored in Amazon S3. 

Exam Notes: 
1. Instance store volumes are sometimes called ephemeral storage
2. Instance store volumes cannot be stopped. If the underlying host fails, you will lose your data. 
3. EBS backed instances can be stopped. You will not lose the data on this instance if it is stopped. 
4. You can reboot both, you will not lose your data.
5. By default both Root volumes will be deleted on termination however with EBS volumes, you can tell AWS to keep the root device volume. 