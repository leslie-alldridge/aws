### IAM

Users - end users

Groups - A collection of users under one set of permissions

Roles - You create roles and can then assign them to AWS resources

Policies - A document that defines on (or more) permissions. Stored in JSON format with key value pairs.

IAM is universal. It doesn't apply to specific regions.

The Root account is the first account created when the AWS account is set up. By default it has overall admin access.

New users have NO permissions when first created. They are assigned an Access Key ID and Secret Access Key when first created.

These are not the same as a password, and cannot login to the console with these keys.

If the keys are lost they need to be generated so it's best to store the .csv safely.

Always set up MFA on your root account.

You can create and customise your own password rotation policies.
