# Jonathan Moseley
## CEG3120
## Project 2

# Part 1 - Build a vpc


1.
Create a VPC:
![VPC creation](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project2/Images/Moseley-VPC.png)

2. Create a subnet:

![Subnet creation](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project2/Images/Moseley-Subnet.png)

3. Create a internet gateway:

![Internet gateway](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project2/Images/Moseley-gw.png)

4. Create a route table:

![Route table](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project2/Images/Moseley-routetable.png)

5. Create a security group:

![Security group](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project2/Images/Moseley-sg.png)


# Part 2 - EC2 instances

1. Ami Selected: Ubuntu 
  1.5: Default username: ubuntu 
  
2. The instance was attached to the VPC in the inital creation. By selecting 'edit' in the network section I was able to switch from the default VPC to my new new VPC
3. By default a public IP will not be assigned. I have opted to not auto assign a public IP due to the fact an elastic IP will overrite the auto-assigned public IP of the instance. 
4. A volume was attached at the time of instance creation. I was given the option to create a volume for this instance. By creatting a volume at the instance creation AWS would auto attach it. 
5. My instance was tagged with a name at the time of creation. AWS gives the option to name an instance when you create, which I used to tag with a name. 
6. I associated a security group with my instance at the time of creation. When I switched my VPC to the one I created I could select "associate with existing security group". From there I was able to select the security group I created. 
7. A elastic IP was reserved in the "Elastic IP section of the AWS dashboard. From there I could reserve an IP address; afterwards using thr dropdown menu I could select the instance to associate the elastic IP with. 
8. ![Moseley-instance](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project2/Images/Moseley-instance.png)
9. Currently I hvae been unable to establish an SSH connection with my instance. I have attempted to reform everything from scratch and still no success getting a connection. Even when using Amazon's tools to connect in the webconsole it does not allow me to connect. Curreently I have been unable to figure out the issue on where it may be originating. 

