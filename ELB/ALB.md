Application Load Balancer 


HTTP, HTTPS, Websocket (L7)
Load balancing to multiple [[EC2]] instances or within an instance
Redirecting is possible from https to http
Routing based on 
1. path
2. host name
3. query string 

is possible

used in microservice environment - Docker and Amazon ECS

Fixed host name - xxx.region.elb.amazonaws.com
Application servers don't see the ip of the client. Ip will be included within http header X-Forwarded-For
Port will be available in X-Forwarded-Port
Protocol will be in X-Forwarded-Proto

Target group refers to destination of Load Balancer
it can be
1. Instances
2. Ip Address
3. [[Lambda]] Functions
4. Another application load balancer
5. 

One can't attach [[Elastic Ip]] to ALB
