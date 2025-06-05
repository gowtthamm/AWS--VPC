# AWS--VPC-PROJECT

![image alt](https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/c6e17508080f4e32fa4cc5fb3b910591ff4366fe/VPC_Architecture.jpg)

COMPONENT AND CONFIGURTION :

01 . VPC (CIDR: 10.0.0.0/16): Acts as a logically isolated network in AWS to host all resources.

02. Public Subnet (10.0.1.0/24): Contains an EC2 instance with direct internet access via an Internet Gateway. This is ideal for web servers and publicly accessible applications.

03. Private Subnet (10.0.2.0/24): Hosts EC2 instances that cannot be accessed directly from the internet, used for backend or internal processes.

04. NAT Gateway: Deployed in the public subnet, it allows instances in the private subnet to securely access the internet for updates or external requests without exposing them.

05. Public route table directs internet-bound traffic to the Internet Gateway.

06. Private route table sends internet-bound traffic from the private subnet to the NAT Gateway.

PURPOSE AND OUTCOME 

Allow selective internet access from private networks.
Secure internal resources Like databases and application servers.

