## Jonathan Moseley
## Project4


# Part 2

1. The file ```/etc/hosts/``` was configured firest with the private IP of the AWS Virtual Machine/Instance. Next to it was the correstponding hostname. 
2. To SSH between the systems first teh VOCKEY file must be copied to each instance with the ```SCP``` command. From there with the ```/etc/hosts``` file setup the machines can be SSHd via ```ssh -i VOCKEY.pem ubuntu@hostname```
3. To setup HA Proxy first copy the default configuration to a .old file. Then setup a new configuration. Once defaults, frontend and backend are defined ensure the program is running
4. To setup the webservers, what needs to be done is to copy the
5. On my system I was unable to get HAProxy to stars rendering me unable to navigate to the webpages to test. In attempting to debug the software it pointed to configureation file erros, which were fixed. 
6. 
