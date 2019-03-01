### Storage Gateway

Service that connects an on-premises software appliance with cloud-based storage to provide seamless and secure integration between an organizations on-premises IT environment and AWS's storage infrastructure. The service enables you to securely store data to the AWS cloud for scalable and cost-effective storage.

Four Types of Storage Gateways

- File Gateway (NFS) - Flat files stored directly on S3
- Volumes Gateway (iSCSI) - think of it as a virutal hard disk
  - stored volumes (complete copy of site - backed up incrementally to S3)
  - cached volumes (only most recently read data is stored locally, the rest is stored in S3)
- Tape Gateway (VTL) Virtual Tape Library - used for backup and uses popular backup apps like NetBackup, Veeam, etc

EBS = elastic block store
