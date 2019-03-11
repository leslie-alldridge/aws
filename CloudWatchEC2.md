### Cloud Watch EC2

Default metric types available for your EC2 instance:
- CPU
- Disk (read/write)
- Network
- Status

Custom metrics need to be created if you want to monitor RAM (or anything else..e.g. storage space)

Alarm won't send any emails until the recipient email address has confirmed their address within 72 hours.

CloudWatch Events
- Help you respond to state changes within your AWS resources
- Connects different AWS service blocks with rules and actions so that when you deploy a lamba it can set itself up correctly (DNS, routing, etc)
- Logs : you can do down into the application layer and log events there. Whereas the dashboard (disk, cpu, etc) are host level logs. 

Tips:

Standard monitoring = 5 minutes

Detailed monitoring = 1 minute

Can create dashboards, alarms and events, as well as view logs.

CloudWatch vs CloudTrail 
- CloudWatch is for performance monitoring and logging
- CloudTrail is for auditing (new user / new roles / buckets/ etc)