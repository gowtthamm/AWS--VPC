# AWS--VPC-PROJECT

"Developed a cloud environment with public and private subnets, connected via a NAT Gateway, enabling safe internet access for internal EC2 instances" 

![image alt](https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/c6e17508080f4e32fa4cc5fb3b910591ff4366fe/VPC_Architecture.jpg)

🧑🏻‍💻 COMPONENT AND CONFIGURTION :

01. VPC (CIDR: 10.0.0.0/16): Acts as a logically isolated network in AWS to host all resources.

02. Public Subnet (10.0.1.0/24): Contains an EC2 instance with direct internet access via an Internet Gateway. This is ideal for web servers and publicly accessible applications.

03. Private Subnet (10.0.2.0/24): Hosts EC2 instances that cannot be accessed directly from the internet, used for backend or internal processes.

04. NAT Gateway: Deployed in the public subnet, it allows instances in the private subnet to securely access the internet for updates or external requests without exposing them.

05. Public route table directs internet-bound traffic to the Internet Gateway.

06. Private route table sends internet-bound traffic from the private subnet to the NAT Gateway.

🚀 PURPOSE AND OUTCOME 

• Allow selective internet access from private networks.

• Secure internal resources Like databases and application servers.


LINUX COMMAND TO ACCESS THE PRIVATE SERVER 

-->  ssh -i "password filename " ec2-user@ip-address



<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/e4e70af8e63191fdcec7ea5ba870f866af71c8cf/Subnet.png" width="700" height="300" />


<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/e4e70af8e63191fdcec7ea5ba870f866af71c8cf/Subnet.png" width="700" height="300" />



<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/1f67c791fc27f7949d6bceb253e0c0a403c882e6/NAT.png" width="700" height="300" />


<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/2029f7aad26316fdf1aa5f099ca870c6ae5cb7a9/Route%20Table.png" width="700" height="300" />



<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/ac4af26a18ddd6b28869ef3d628f7996d7b1327d/Linux.png" width="700" height="300" />

PUBLIC SERVER

<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/fcf41c9ec6b2b51788423767765c2d263130a516/Public%20server.png" width="700"
height="300"/>

PRIVATE SERVER 

  ACCESSING PRIVATE SERVER THROUGH PUBLIC SERVER 

<img src="https://github.com/gowtthamm/AWS--VPC-PROJECT/blob/fccb8accb078809b9dc647d01c94e6212e073ab3/OutPut.png" width="700" height="300" />

