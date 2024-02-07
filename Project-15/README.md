


## AWS Networking implementation (VPC, Subnets, IG, NAT, Routing)

**VPC Creation and Subnet Configuration**


**AWS VPC Creation and Subnet Configuration**


In this project, I will create a VPC in AWS where i will have 4 servers. 2 public servers and 2 private servers. I will be able to access my public servers via the internet and can only be able to access private via my public servers and not throught the internet. 


## Creating a new VPC


![alt text](<images/Unsaved Image 2.png>)


![alt text](<images/Unsaved Image 3.png>)

- I then proceeded to create my subnets from the cider block already associated to my new VPC. 

As shown bellow, I i created 4 subnets  , 2 will be assigned to my public servers and 2 is assigned to my private servers. 


![alt text](<images/Unsaved Image 5.png>)


- NOw , i created 2 route tables, public and private route table. and associated 2 public subnets to public route table and 2 private subnets to private route table 

![alt text](<images/Unsaved Image 8.png>)

![alt text](<images/Unsaved Image 9.png>)

 ![alt text](<images/Unsaved Image 6.png>)


- I created internet gateway and attachched it to my new VPC, and added the internet gateway to my public route table for internet access. I did not add internet gatway to my private route table to prevent public internet access.


![alt text](<images/Unsaved Image 7.png>)


I created NAT(Network address translation) to one of my private subnets. 

![alt text](<images/Unsaved Image 11.png>)

![alt text](<images/Unsaved Image 10.png>)


Time to test our configuration by spining 2 ubuntu instances . 1 will be assigned as public and 1 as private. 

i created the public server using the public subnet i created before that has internet gateway.

IN the security group, i edited security group allowing ping access and i was able to reach the server via the internet. 

![alt text](<images/Unsaved Image 12.png>)


I tried pinging the private server, and coudnt reach it because it has no internet access. 

![alt text](<images/Unsaved Image 13.png>)

- Using ssh agent, I connected to the public server and try pinging my private server from there and i got replies as shown bellow. 




![alt text](<images/Unsaved Image 14.png>)


## Project completed 

