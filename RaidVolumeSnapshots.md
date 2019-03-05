### Raid, Volumes and Snapshots

RAID = redundant array of independent disks 
- RAID 0 - striped, no redundancy, good performance
- RAID 1 - Mirrored, redundancy
- RAID 5 - discouraged on AWS (don't use it), good reads bad writes
- RAID 10 - striped, mirrored, redundancy, good performance

Can adjust striping in windows disk management 

To connect using RDP you will need to configure the access policy to allow RDP from your current IP address. 

Next, download and import the .pem key. And after it's booted up, go to Actions > Get Windows Password in AWS.

Q: How can I take a snapshot of a RAID array
A: Take an application consistent snapshot

To do this
- freeze the file system, unmount the raid array, shutting down EC2, either one works

AMI = Amazon Machine Image 

Snapshots for Amazon EBS volumes that serve as root devices, you should stop the instance before taking the snapshot. 

Encryped volumes = encrypted volumes

Can share unencrypted snapshots