### Securing Buckets

By default all buckets are private

You can set up access control policies using

- bucket policies
- access control lists

S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done into another bucket.

### Encryption

Two Types

- In transit, secured using SSL and TLS (https)
- At rest
  - server side encryption
    - S3 managed keys (SSE-S3)
    - AWS KMS Managed Keys (SSE KMS)
    - Server side with Customer Provided Keys (SSE-C)
  - client side encryption
