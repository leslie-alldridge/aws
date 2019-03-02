### Summary

S3 is object based storage and allows you to upload files
Unlimited Storage
Files can be 0-5tb in size
Files are stored in Buckets
Buckets have universal namespaces - must be unique globally and all lower case.
region - amazon aws - bucket name
https://s3-eu-west-1.amazonaws.com/leslie

---

Read after write consistency for PUTS of new Objects. Deleted or updated objects will take a bit of time to propagate (update).

---

S3 Standard 99.99% availability and 99.99999999 \*eleven nines durability
S3 - IA , lower fee but charged for retrieval. Less frequent access but top speed.
S3 One Zone - IA - lower cost, one zone, infrequently accessed
Glacier - very cheap, archival only. Epedidited, Standard or Bulk. 3-5 hour retrieval time.

---

Core fundamentals

Key (name) value (data) key value store
Version ID
Metadata
Object based only (files only)
Cannot run servers etc
Allows versioning and each version you pay for it
Great backup tool
Once versioning is enabled you can only suspend it, to delete it the bucket must be deleted.
Can use MFA on deletes using MFA app
Integrates with lifecycle rules
Cross region replication for versioning

--
Life cycle management

Can be used in conjunction with versioning.
Applied to current and previous versions

--
Cloud Front

Edge location - content will be cached, 50 in the world and separate to AWS region AZ.
Origin - origin of files the CDN will distrivute. Can be S3 bucket, EC2 instance, ELB or Route53.
Edge locations are both read and write. Auto replicates over to origin.
Objects are cached for the TTL life (24hrs by default)

--
Securing buckets

Private by default. Can edit bucket policies and access control lists. Can be configured to keep logs and save to same or different bucket

--
Encryption

In transit - SSL/TLS

At rest - server and client side versions with keys

--
Storage Gateways

File Gateway - flat files stored directly on S3
Volume Gateway - - stored volumes : entire dataset is stored on site and backed up to S3 - cached volumes - S3 main store with caches on site
Gateway Virtual Tape Library - used for backup applications like netbackup, backup exec, etc.

--
Snowball

Snowball - standard

Snowball Edge - storage plus compute (can run lambda functions)

Snowmobile - 100PB storage in a 45foot armoured protection truck

Snowball can import and export, the historic import / export was manually sending data to AWS

--
Transfer acceleration

You can transfer to edge location, costs extra and best results for far away people.

--
Static websites

serverless, very cheap and auto scales, static only.

--
Final tips

Write to S3 - HTTP 200 code for successful write
You can load files faster by enabling multipart upload
Read the S3 FAQ before the exam
