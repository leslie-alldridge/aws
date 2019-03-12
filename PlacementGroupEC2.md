### Placement Groups

1. Clustered Placement Groups
- Grouping of instances within a single Availability Zone. Placement groups are recommended for applications that need low network latency, high network throughput, or both.
- Only certain instances can be launched in to a Clustered Placement Group.

2. Spread Placement Groups
- Group of instances that are each placed on distinct underlying hardware. Good for apps that have a small number of critical instances that should be kept separate from each other.
- Can span multiple Availability Zones

Placement group name must be unique across your AWS account. 

Only certain types of instances can be launched in a placement group (Compute Optimized, GPU, Memory Optimized, Storage Optimized)

AWS recommends homogenous instances within placement groups

You can't merge placement groups

You can't move an existing instance into a placement group. But, you can create an AMI from your existing instance, and then launch a new instance from the AMI into a placement group. 

If the exam only mentions 'placement group' assume they're talking about Clustered as Placements were only recently released.