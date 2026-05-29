EC2-soultionArchitect



Topics-:

elastic ip address

placement groups

Eni

Hibernet





\--public vs private ip

\-public ip can be access every where but private is accessible in private network only



\--elastic ip address

whenever you try to stop and start instance again and again the public ip address changes in that case here we use elastic ip address in ec2 only right navbar you will see



Network \& Security > Elastic ip> just create an elasticip > copy original instance > open elastic ip> attach instance in that elastic ip> click on associate >>Hola you have just done it





\--Placement group (3 Type)

you indirectly tell your aws that i want to function my server in a particular way



\-1 Cluster (provide speed but less availablity)

&#x09;all the ec2 instances are in same rack(place to store ec2) it is use if you want fast computing due to common due to common hardware



\-2 SPREAD (provide availability but less speed)

&#x09;if you want high availability then use spread it mean that put ec2 instance in all possible rack this how it provide high availablity



\-3 PARTITION (Both in balance)



&#x09;Check for it in image 2.1



**-hands on**> go to ec2 instance>Network and security>Placement Groups>select what you want acc to requirements



\--**ENI**

ENI is what gives your EC2 instance its IP address and network connectivity.



\-Each ENI has:

Private IP address

Public IP (if assigned)

MAC address

Security Groups



\-Hands on

Go to AWS Console

Search: EC2

Left menu → click:

&#x20;Network Interfaces



You will see:



eni-xxxx

Private IP

Status

Attached instance





\--HIBERNATE

Hibernate = Pause your EC2 instance and resume later EXACTLY where it stopped



\-What Happens in Hibernate?

When you hibernate an EC2:

&#x20;RAM (memory) is saved to EBS volume

&#x20;Instance stops

&#x20;When you start → everything comes back



\-

Stop        OS shuts down, RAM lost

Hibernate   RAM saved, resumes same state

Terminate   Instance deleted





