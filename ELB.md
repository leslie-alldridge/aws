Balances the load across web servers

Three types:

1. Application load balancers

Best suited for load balancing of HTTP and HTTPS traffic. Operate at layer 7 (can see all the way inside) and can detect where the traffic is coming from. Very intelligent load balancers with routing. 

2. Network load balancer

Best for TCP traffic where extreme performance is required. Works at layer 4 and capable of handling millions of requests with very minimal latency

3. Classic load balancer (elastic load balancer)

Balance HTTP/HTTPS, legacy elastic load balancers. Can use both layer 7 (X-Forwarded and Sticky sessions) and layer 4 load balancing. 

Load Balancer Errors

Error 504 - Load balancer exists but having problems communicating with EC2 instances behind it. Identify where it's failing (Web server or database) and scale up or down. 

The ELB has a X-Forwarded-For header and passes on the public IP address on to the EC2 instance. That way you can see the internal IP address of the classic load balancer and you can see where you users are coming from (IPv4 ip address).


Once an EC2 instance is out of service your load balancer will stop sending traffic to it. 

Amazon self manage the Public IP for load balancers and only provide you the DNS name.

ELBs are monitored as InService or OutofService and constantly ping the instance health.

