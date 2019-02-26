### What is a CDN

A content delivery network is a system of distributed servers that deliver webpages and other web content to a user based on the geographic locations of the user, the origin of the webpage and a content delivery server.

Edge Location: This is the location where content will be cached. This is separate to an AWS Region / AZ.

Origin: This is the origin of all the files that the CDN will distribute. This can be either an S3 Bucket, EC2 Instance, Elastic Load Balancer or Route53. You can have your own custom servers it doesn't have to be within AWS.

Distribution: This is the name given to the CDN which consists of a collection of Edge Locations. Web distribution is used for websites and RTMP is used for media streaming.

Edge Locations are not just Read only, you can write to them too. (Put an object to them).

Objects are cached for the life of the TTL (Time to live)

You can clear cached objects, but you will be charged.

Link will change to: https://d1cwtbnbaamlnn.cloudfront.net/bazzzzzzy.png
