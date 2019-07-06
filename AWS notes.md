AWS load balancers:
  Internet Facing 
  Internal only

ELB constantly do the health checks.
diff. AWS availabilty zones

DNS name will be given to ELB.
CNAME alias to resolve the DNS names.

Benefits of ELB
Highly available
Secure - SSL support, user auth
Elasticity - its managed service.
supports hybrid cloud.

Load balancing type:
1. Application Load Balancer - Layer 7 load balancing -  optimized for HTTP and HTTPS
  Server Name Indication (SNI) - single listener for multiple domain, -> handled diff. SSL for diff domains
  IP address as targets
  Lambda functions as targets
  Host/path-based routing
  Containerized application support
  Sticky sessions
  Security - user auth and WAF
  
2.Network Load Balancers
  Layer 4 load balancing - TCP traffic
  Supports millions req/sec
  Preserve source IP
  High throughput/low latency
  Static and Elastic support
  
3. Classic Load Balancers - legacy EC2 - classic network
   not recommended for VPC
   SSL offloading
   Sticky session
   High availability
   Layer 4 and Layer 7 of OSI model
   
ELB is regional service
   Working with multiple AZ in single regional/  for multiple region , use Route 53 load balancing
   Cross zone load balancing - required in application load balancers
   Load balancing nodes - amazon VPC - managed by AWS.
   
 Application Load Balancers
 
 ALB -> Listeners -> Target groups
 Listener -> Rules likes HTTP 8080 -> Target group 1
  Listener -> Rules likes HTTPS 443 -> Target group 3
  Target/Host conditions, Path conditions
  Host based routing -> supports for multiple domains using single load balancer
  Path based routing -> enables supports for microservices
  Integration with Amazon ECS supportd registering tasks with target groups

Network Load balancers  
  NLB ->   TCP based 
  Elastic IP 2 - > AZ1
  Elsatic IP 2 - > AZ 2
  in AZ- > choose Elastic IP address'
  ALB - > Cross zone is enabled by default. But not in NLB

Classic Load balancer
  Legacy model
  
Route 53 -> Records sets -> DNS ->  Routing Policy -> weighted,simple
Route 53 - > gives ability health checks
   
Amazon CI /CD
https://aws.amazon.com/products/developer-tools/
https://www.youtube.com/watch?v=77HvSGyBVdU
https://www.youtube.com/watch?v=Jnl29J3RJQ4
https://www.youtube.com/watch?v=01ewawuL-IY
https://www.youtube.com/watch?v=YDOrsVJiDxA
https://jenkins.io/blog/2016/06/10/save-costs-with-ec2-spot-fleet/
https://aws.amazon.com/blogs/devops/simplify-your-jenkins-builds-with-aws-codebuild/
https://aws.amazon.com/blogs/devops/use-aws-codedeploy-to-implement-blue-green-deployments-for-aws-fargate-and-amazon-ecs/
https://aws.amazon.com/blogs/devops/using-aws-codepipeline-to-perform-multi-region-deployments/
https://aws.amazon.com/blogs/devops/aws-building-a-secure-cross-account-continuous-delivery-pipeline/


Trafic Flow policy
- only way to get geo proximity routing policy.
policy records are not free.


Multi-value answer records vs simple records -> healthcheck, if health check is down for one Ip, then it won't get return in multi-value answer record set
but that is no the case with simple record sets.
what happens if all the servers are down -> route 53 will treat all the server as healthy
last TTL of multi-value record will be TTL of all the record

Transferring already registered domain
- min. 5 day required
- you need to unlock transfer
- you need auth code
- then go to route 53 regisred domain.

EC2 Fleet Strategies
---------------------
1. Spot 
  a. lowest price*N
  b. diversified 
2. On Demand
  a. lowest priced
  b. on-demand pririoty list
  
EC2 fleet uses launch Template



[VPC Design and New Capabilities for Amazon VPC](https://www.youtube.com/watch?v=rQvl-V3tLiQ)

[AWS Architecture Center](https://aws.amazon.com/architecture/?awsf.quickstart-architecture-page-filter=highlight%23new)

[Introducing AWS Fargate - AWS Online Tech Talks](https://www.youtube.com/watch?v=wrZvlJlcZio&list=PL5bUlblGfe0KczDeLstsaHl2aCBsodc_t&index=11)

[AWS Security State of the Union](https://www.youtube.com/watch?v=Wvyc-VEUOns&feature=youtu.be)

[Embracing Failure: Fault-Injection and Service Reliability](https://www.youtube.com/watch?v=wrY7XoOnysg)

[Choosing the Right EC2 Instance and Applicable Use Cases](https://www.youtube.com/watch?v=y-xicDOIiSQ)

[Optimizing Costs as You Scale on AWS](https://www.youtube.com/watch?v=iOWNZqG0RN4&list=PLQP5dDPLts650KRU0yhf8SHheMjsdreqj)

[RDS] (https://www.youtube.com/watch?v=TJxC-B9Q9tQ)
[when to use which DB] (https://www.youtube.com/watch?v=KWOSGVtHWqA)
