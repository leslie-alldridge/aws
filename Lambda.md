### Lambda 

IAAS - Infrastructure as a service 

Lambda encapsulates 
- Data centres and hardware
- Assembly code / protocols
- High level languages
- Operating systems
- Application layer / AWS APIs
- AWS Lambda

It is a compute service where you can upload your code and create a Lambda function. It takes care of provisioning and managing the servers that you use to run the code. 

It can be used to: 
- Event driven compute service where AWS Lambda runs your code in response to events. These events could be changes to data in an Amazon S3 bucket or an Amazon DynamoDB table.
- As a compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs. 

Lambda automatically scales so you don't need to worry about ELBs. 

Triggers: 
- Api gateway, AWS IoT, Alexa Skills kit, Alexa smart home, CloudFront, CloudWatch events and logs, Codecommit, S3, SNS, Dynamo DB, Kineses

If two users send requests to the lamba, two lamba functions are invoked. 

One set of code that can respond to multiple requests.

1,000,000 free invokations per month

Lambda is price on requests per month (20 cents per million after the first million). Very low cost. Also billed on duration rounded to the nearest 100ms and also depends on the amount of memory allocated. 

Lambda functions cannot execute for more than 5 minutes (otherwise you'll need to split out the functions if it exceeds 5 minutes)

No servers required. Continuos scaling. 

Lambda 
- Scales out (not up) automatically
- 1 event = 1 function
- serverless
- lambda functions can trigger other lambda functions
- AWS X-ray allows you to debug what is happening in complex landscapes
- lambda can do things globally like backing up s3 buckets to other buckets
