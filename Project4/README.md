# Jonathan Moseley
# Project4


# Part 2

1. The file ```/etc/hosts/``` was configured firest with the private IP of the AWS Virtual Machine/Instance. Next to it was the correstponding hostname. 
2. To SSH between the systems first the VOCKEY.pem file must be copied to each instance with the ```SCP``` command. From there with the ```/etc/hosts``` file setup ```~/.ssh/config``` must be setup using the hostname, username and location of ```VOKEY.pem```for the maching. Once that is setup the machines can be SSHed via ```ssh [HOSTNAME]```
3:
3.1 For HAProxy configuration the file which was modified was haproxy.cfg located in ```/etc/haproxy/haproxy.cfg```
3.2 The configurations which were set were maxconn 1000, mode http, frontend 
3.3 site content files were located on webserv1 and webserv2 located in ```/var/www/html/index.html``` this is because for apache2 webservers this is the default location for all html files to be loaded by the server
3.4 to restart after a configuration change ```sudo systemctl restart haproxy```
3.5 resources https://www.digitalocean.com/community/tutorials/how-to-troubleshoot-common-haproxy-errors ,https://www.haproxy.com/blog/the-four-essential-sections-of-an-haproxy-configuration/ , https://www.digitalocean.com/community/tutorials/how-to-use-haproxy-to-set-up-http-load-balancing-on-an-ubuntu-vps , https://www.haproxy.com/blog/haproxy-configuration-basics-load-balance-your-servers/ , https://linuxhint.com/how-to-install-and-configure-haproxy-load-balancer-in-linux/


4. How to setup a webserver
4.1 The files which were modified were the default index.html. I copied the html example from class to the corresponding serviers to demonstrate load balancing working
4.2 No configureations weree set. 
4.3 site content files are located in ```/var/www/html/```
4.4 to restart a service the command would be ```sudo systemctl restart apache2```

5. Browser screenshots

5.1 webserv1

![Webserv1](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project4/Images/webserv-1.png)

5.2 webserv2

![Webserv2](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Project4/Images/webserv-2.png)
