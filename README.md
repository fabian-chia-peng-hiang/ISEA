Student Name:	Fabian Chia
Student ID:	CT0391834
GitHub Repository Link:	https://github.com/fabian-chia-peng-hiang/ISEA





Upload DocX File – Reflective Journal report to Kaplan LMS:
FileName: CTID-YourName-AssignmentISEA.docx
upload to SharePoint site: VideoUpload
Video Walkthrough Filename: FileName: CTID-YourName-AssignmentISEA.mp4 

1.	Installing a Linux Environment on your PC
The first step of the lab was to create an account on GITHUB. Github is a platform that allows users to share their personal projects or code online. The repositories online can be shared with other users to build upon. The screenshot below shows the newly created repository in my new GITHUB account. The readme.md is usually used as the front page of a repository. It is supposed to contain some sort of introduction or instruction you’re your code however, it will be used in this assignment to keep track of all labs done across the entire module. 
 

The next part of the lab is to install a linux environment. Linux is an open source ooperating system it is built around the Linux kernel and can come in many different distributions such as Ubuntu, Kali Linux and Debian. The terminal is mainly used for control within these environments. The distribution installed for this module is the Ubuntu distribution. 
An ISO file was downloaded from the official Ubuntu website. An ISO is a complete copy of a disk and is saved as a single file. It contains the operating system, files structures and everything required to create the original disk completely. 
Since the ISO file represents a complete disk image of a machine, we will be able to run it with a hypervisor. A hypervisor is a software that allows you to run multiple virtual machines on a single computer. It splits the computer’s CPU, RAM and storage between the different virtual machines if required. Some common hypervisors used are VirtualBox and Vmware. I chose to use VMware as I already have experience running different virtual machines on it. 
In order to run the virtual machine, you can use the vmware software to add a new ISO file to be used. You can then choose the specifications of your new virtual machine. I chose to go with 4GB memory and 20GB storage. Do refer to the screenshot below. The specifications can be changed at any time as long as the machine is hibernating or turned off. 
 





2.	Exploring Ubuntu Desktop and Linux services
As mentioned previously, terminal is mainly used for control in Linux environments. They are operated using command lines. You can refer to the screenshot below to see that terminal has been opened. 
 
Some command we played around with are ‘pwd’ which is used to print the working directory which is the current directory you are currently in. ‘ls’ which is to list files and directories within a linux machine. ls can be paired with many other flags to be able to obtain more extensive results about the files or directories you are interested in. Another command I used is ‘cd’. This command is the command that allows you to navigate through directories. It allows you to change the directory you are in based on your own specifications and is very similar to windows command prompt. Just input ‘cd’ followed by the directory you want to go to. Mastering this will allow you to navigate through the machine using only your keyboard very easily.
Some other commands I used are ‘mkdir’ and ‘touch’. These two commands are used for creating directories and files respectively. ‘mkdir’ followed by the name of your choice  allows you to create a directory within the directory you are currently in. ‘touch’ followed by the name of your choice can be used to create a file within the current directory. These commands are great if changes has to be made within a directory. The following screenshot shows the creation of the directory as well as the creation of a new file. 
 
I followed up by exploring the different directories within the machine. The directories include ‘/etc’, ‘/var’ and ‘/home’. These are key directories within every linux machines. The ‘/etc’ folder contains system wide configuration files. Such files include ‘/etc/passwd’ , ‘/etc/ssh/’ and ‘/etc/hosts’.  The next folder I exploered was the ‘/var’ folder. Yje /var folder contains variable data. All that means is that it contains data that will change. Some important files within the folder include ‘/var/log’ contains system logs. ‘/var/www’ this folder contains webserver files. ‘/var/cache’ contains cached data. 
Lastly, the ‘/home’ folder. This folder is used to store the personal directory of each user. Whenever a new user is created, a new directory for that user will be created in the ‘/home’ directory. 
1b
The next part of the labs is to manage the different services within a linux environment. The first command used is ‘systemctl list-units --type=service’ . this command can be used for all linux systems that use system to show all currently loaded services. The flag –type specifies to list only all the services. The UNIT, LOAD, ACTIVE, SUB, DESCRIPTION. 
 

3.	Managing and controlling Linux services
The systemctl command is generally used to check the status of services. Mostly used in the case of troubleshooting when a service that is supposed to run is not working. 

As previously mentioned, that the command systemctl is used for troubleshooting and checking for services that are running. One service that I installed on my machine is apache2. Apache2 is a web server software. It is used to host websites on a server. It sends web pages to users when users try to access a site. It commonly handles requests from web browsers.  'sudo systemctl start apache2’ is used to start the service first. Next, I used ‘sudo systemctl status apache2’ this command is used to check the status of the service. It will show you if the service is running or not. Refer to the screenshot below. 
 
4.	Understanding and Applying Linux Permissions

The next part of the labs has to do with permission management. ‘ls -l’ allows you to view the permissions of every single file within a folder. ‘chmod’ allows you to change the permissions of the file. Each file is given permissions it can come in the form of read, write and execute. The values for read is 4. The value for write is 2. The value for execute is 1. By adding them up you get the permission for the file. There are 3 types of permissions. First by the owner, secondly the group and thirdly everyone else. 

The permission 777 indicates read write and execute permissions for all users regardless of groups, users and owner. This is a very dangerous permission to allocate especially on sensitive files. I created a file and allocated the permission to be 777. In the labs I will use the chmod command to change it into 755. 755 is much safer since only the owner has full read write and execute permissions. Where as users within the same group or other users only have read and execute permissions. They are unable to make modifications to the file. This is especially important for scripts or executables as these are things that will run frequently. Access should only be given to the appropriate users. Not everyone should be able to make changes to the script. Refer to the screenshot for the changes made to the file I created. 
 
Another command that can be used to change permissions is ‘chown’. This command does not really change the permission but instead it changes the owner of the file. This can be used to give another user more privileges over the file. In the example below, I changed the owner from ‘ubuntu’ to ‘fabian’. 
 
5.	Navigating the Linux File system
The next part of the labs is to search for files within the system. The command used for that is ‘find’. ‘find’ is the linux command to search for files and directories. You can decide the conditions of your find command, these conditions can be specified based on name, type, size, permission and time. In this lab I used the name as the condition to look for the file so the command I used was ‘find. -name “file.txt”’. The commands start by using find followed by ‘.’ The full stop indicates that it searches for the file within the current directory. ‘-name’ specifies that is uses the name to look for. The command is then followed up by “file.txt” which is the file that I am looking for. This command will show the full file path of that file. Another way to look for files is using grep. The command ‘grep -r’ followed by a keyword like ‘hello’ in the case of hello.sh and lastly the directory of which the file is stored. Refer to the image below. 
 
6.	Total Cost of Ownership(TCO) in cloud infrastructure
The next part of the lab is to find out the TCO of running a sever on premise versus running a server in the cloud. Running a server on the cloud is much for efficient and cost effective than running a server on premises. Running a server on premise requires storage space, hardware costs, maintenance costs, electricity cost and much more other inconvenience. With the use of cloud technology, we can run our servers remotely and run our businesses without worrying about all the issues mentioned above. The breakdown of the costs are as such. Typical cost of a hard server is about 5000SGD. The cost of an SSD or HDD is about $800SGD. The cost of network gears such as the Network Interface card(NIC), switches and routers are about $500SGD. The UPS costs about $700SGD. Which brings the total cost to about 7000SGD upfront to run a single server. In the case where business expands and the workload increases more costs will be incurred and more hardware costs will follow suit. Here is the breakdown of the annual operating costs maintenance is about 10% of the total hardware costs so it is about 700/year. The electricity usage for a typical server is about 250W-500W, based on Singapore’s electricity rate of about $0.35/kWh it brings our yearly cost to about $1200SGD a year. Those are the basic costs for running a server on premises.

7.	Provisioning and Securing a Cloud VM
Next, I will discuss running a server on the cloud. I will use AWS as the cloud provider. Using AWS calculator here is the cost breakdown. Firstly, to run an AWS server we can select the instance we wish to use. In this case of a single server, I will choose EC2 t3.medium, this is the typical server used for a small app server. The cost breakdown is as such. The aws pricing in Singapore is about 0.0416USD per hour so using that breakdown it brings us to about 45SGD a month. As for the storage, I will assume 100GB storage with the cost being $0.08USD per GB per month. It would bring our monthly cost to about 22SGD a month. In the case that there is outbound traffic required for customers and what not the cost of data transfers is as such. 0.12USD per GB, assuming about 200GB a month of outbound traffic, it would bring the monthly cost to about 32SGD for data transfer. Since the server also requires some sort of security, the Amazon cloudwatch can be used for logging and monitoring. It costs about 10SGD a month. That would bring our total cost to about 109SGD a month for running a server on the cloud which is about 1308SGD a year. 

The next part of the lab is to launch and secure a Cloud VM. For this part of the lab, I used AWS and launched an ec2 instance. I used the t3.micro instance as it is the only compatible instance for the free account. The next part of the lab is securing the VM. The first thing I did was to disable password login. By disabling password login, it eliminates the chance of brute force attacks. The server can only be logged in via the SSH key which is generated at the start. This provides a much more secure way to access the server rather than it being accessed remotely by anyone online. Disabling password login can be done by making changes to the sshd_config file. You can add two new lines into the config file to ensure no password authentication can occur. The first line being ‘PasswordAuthentication no’ and the second line being ‘PermitRootLogin no’. 
 

Another change you can make to your server is to change the port used for your ssh service. Attackers will aim to attack the default port as the default port for SSH is port 22. Changing the port to a different number will make things harder for any attacker to attempt to breach your server. You can also change the default port by making changes to the sshd_config’ file. To change the port used you need to uncomment the line which contains the port 22 and change it to whatever you like. In my case I changed it to 2222. Do refer to the image below. 
 
Some other changes that I made to secure my server is to enable the firewall. A firewall decides what traffic is allowed and what traffic is not allowe din your server. It can control in the outbound traffic. The first step I have taken by using the firewall is to enable it as seen in the image below. 
 
Some of the rules I created are ‘sudo ufw allow OpenSSH’ , ‘sudo ufw allow 80’ and ‘sudo ufw allow 443’. The first rule created is to allow connection via ssh which allows me to connect to the servere remotely. The second and third rule allows common web ports such as port 80 and 443. These 2 ports are commonly used in HTTP and HTTPS respectively. Thus if my server is running a webserver, it is very important to allow traffic from these ports. Refer to the screenshot below for changes made to the firewall. 
 


Another type of firewall is the firewall provider by the cloud provider. In this case since I am using AWS, the firewall used it security group. Within the security group that is linked to your instance, you can create, delete or edit rules that control the traffic to and from your server. I created 3 of the following rules on top of the existing rule that allows SSH. The first rule created is to allow all traffic from port 80 from any Ip addresses. This is created as a webserver will be hosted on my server. Thus, using port 80 is very important and blocking the traffic will render the server useless. The next rule created is a rule that allows the traffic from port 443. The protocol that uses port 443 is HTTP. Once again since the server I am running will run web services, allowing port 443 is necessary. Another protocol allowed is ICMP. ICMP does not use any port, it uses IP address to send packets. I allowed this protocol as it is useful for network diagnostics and testing for connections. Refer to the image below for the rules created. 

 

The next step to securing my server is to create an ssh key pair. How it works is it allows you to authenticate a user without a password. When the key pair is generated, a private key is created that stays on your personal machine and a public key that you will place in your server. Upon login, the server checks for the public key and sends a challenge. Your personal machine will then use the private key and verify the signature with the public key. In the case that it matches you will be granted access to the server. Using an ssh key pair for login is important in a server as it eliminates the risk of password attacks. Refer to the image below on the creation of the ssh private key. This key must be transferred over to your personal device. 
 

The next step is to update and patch the server into the latest updates. This step is important as it fixes security vulnerabilities, improves stability and keeps your system reliable. Not updating your system can expose your server to vulnerabilities that can be abused. Updating the server can also fix bug fixes which help to prevent crashes or expected behaviours. The commands used for updating the server are as follows ‘sudo apt update’, ‘sudo apt upgrade’ and ‘sudo apt autoremove’. 
‘sudo apt update’ refreshes your system’s package index and tells your server the latest list of available software versions. The next command ‘sudo apt upgrade’ is the command that installs the newest version of packages on your server. Lastly, sudo apt autoremove’ this command cleans your system by removing the packages that are no longer in use. Refer to the screenshot for the patching. 

 

 

 

8.	Writing Bash Scripts and Using regular Expressions

The next part of the lab is to create a script for automation within the server. The script I created will be used for updating the server. This script will be run daily at 12am using a cron job. The script contains the following command ‘sudo apt update && sudo apt upgrade -y’ this command is similar to the command used in the previous example in updating the server. Refer to the screenshot for the contents of the script. 

 

The next step is to add the script into a cron job to be scheduled daily. I decided to schedule it daily at 12am. I used the command ‘crontab -e’  to manage cron jobs within my ubuntu server. Based on the screenshot below you can see the line ‘0 0 * * * /bin/bash /home/ubuntu/patch.sh’ which causes my script to run everyday at 12am. 
 

Since the script will be running daily, the permissions will need to be changed so that the script does not run malicious commands. So the command I used is ‘chmod 750 /home/ubuntu/patch.sh’. The permission 750 gives the owner read, write and execute permissions, gives the users in the same group read and execute permissions and gives everyone else no permission to do anything. This allows only the owner to be able to modify the script. Refer to the image below on the permissions. 

 

9.	Configuring DNS Testing and Domain resolution
The next part of the labs is the creation of a DNS sever. The first step is to purchase a domain to be used for your DNS. I purchased the domain from cloudflare. The domain name I purchased was ‘fabian-isea-bridging.com’. Now for the new domain, I have to create a new record for it to be resolved. I linked the domain to the external IP address of the AWS instance which can be found in the AWS console. The external IP address being ‘3.26.37.84’. Refer to the screenshot below for the creation of DNS records. 

 

Now for the last step, I needed to verify if the DNS is working. This can be done by using nslookup to check for the domain. The command used is ‘nslookup fabian-isea-bridging.com’ Refer to the image below for a successful result. The image shows that the DNS resolves the domain successfully to the IP address that I assigned. 

 

The next part of the lab is to set up nginx. Nginx is a webserver and networking tool that is used to handle web traffic. It is a webserver that serves websites and static files. Some other capabilities include reverse proxying, load balancing and SSL/TLS encryption. The first thing to do to enable nginx is to install it on my server. It can be done using the command “sudo apt install nginx -y’. Refer to the t image below. 
 


10.	Obtaining and Managing Digital certificates with Let’s Encrypt
Next part is to download certbot. Certbot is a tool that is used to set up HTTPS very easily on websites. The capabilities of certbot include obtaining SSL/TLS certificates for your domain, installing and configuring the certificates, enabling HTTPS so that traffic between users and your site is encrypted, renewing certificates before they expire. The command to install certbot is ‘sudo apt install certbot python3-certbot-nginx -y’.

 

The next thing to do is to create an SSL certificate for my webpage. An SSL certificate is important as it is used to encrypt data in transit, verify the website’s identity and proves that the website is real. It can be verified by looking at the padlock icon at the address bar of the browser. Browsers will mark websites without a valid certificate as not secure. 

The following command is used to create an SSL certificate for my server. ‘sudo certbot –nginx’. I then input the domain that I wished to use and tested it. Do refer to the image below. 

 

Once the SSL certificate has been created, the last step is to verify that it is working. As mentioned before, what I am looking out for is the padlock icon at the address bar of my browser. Do refer to the image below. 

 






11.	Scripting Linux Server Functions For Automation
The next part of the lab is server automation. The whole idea is to create scripts that will do your daily server tasks for you. Some tasks include updating or backing up data into logs. This script will update the system and save it into ‘/var/log’. Here is the full script
‘#!/bin/bash

echo "===== Server Maintenance Started: $(date) ====="

# Update system packages
echo "Updating system..."
sudo apt update -y >> /var/log/task.log 2>&1
sudo apt upgrade -y >> /var/log/task.log 2>&1

# Backup /etc folder
echo "Creating backup..."
tar -czf /var/backups/etc-backup-$(date +%F).tar.gz /etc >> /var/log/task.log 2>&1

echo "===== Server Maintenance Completed: $(date) ====="
echo "" >> /var/log/task.log’

It starts by updating the packages and the upgrading it. After every action it saves the results in /var/log/task.log. The next part of the script creates a backup. It compresses the ‘/etc’ folder into a dated backup file and logs everything into ‘/var/log/task.log’.

The last part of the script echoes the date in which the server was last updated into the log.
Refer to the image below for the script inside the server.
 


Lastly, I need to test my script by running it. The script requires sudo privileges in order to write into ‘/var/log’. Refer to the image below on successful execution of the script. 
 

I will now have to automate it. Since I want it to execute daily, I can make use of cron jobs to schedule it daily at 2am. Similar to the previous script I will use the command ‘crontab -e’ then write into the file. Refer to the image below. 
 










12.	Additional Server service(VSFTPD) 
The next part of the lab is to add an additional service within my server. For this I have chosen VSFTPD. VSFTPD stand for ‘Very Secure FTP daemon’. It is ran on LINUX or UNIX systems and allows users to upload files to server or download files from a server or mange remote file storage using FTP. It is generally used for moving files between client to server or local machine to remote server. 

I began by installing vsftpd on my server by running the command ‘sudo apt install vsftpd -y’. 
 
 Next step as per all services is to start and enable the service. Using the commands ‘sudo systemctl start vsftpd’ and ‘sudo systemctl enable vsftpd’. 
 

Next step is to test that VSFTPD is running and is accessible. I created a file called test.txt to be used to download into my local machine. The next step is to allow traffic into the firewall by the port used by VSFTPD. The default port used by VSFTPD is port 21 therefore I need to create a new inbound rule for port 21 to be able to connect to the VSFTPD service. 
Refer to the image below for the new allow rule for port 21 for any IP address. 

 

Next up I will test if I can connect to the server via VSFTPD. I created a new user with low privileges ‘fabian’. This will be used to test the connection and retrieve the file ‘test.txt’ which is stored in the directory ‘/home/fabian’. Upon login, I will navigate to the ‘/home/fabian’ folder and download the file using the command ‘get test. txt’. Refer to the images below for the steps taken. 

 
 

Some security considerations for the service VSFTPD is that there is no encryption thus any attacker sniffing the network will be able to see the credentials in plaintext. Anyone can also upload or download files, this may lead to the server being used for malicious activities. Since the passive ports 40000-50000/TCP are required, it may lead to compromise of those ports as opening a large number of ports opens the attack surface for attackers. 

I believe that VSFTPD is a very useful tool for file transfer, due to its nature, large files can be transferred over the internet very quickly though not as secure as ssh would allow you to. However, if the correct security precautions are put in place, running VSFTPD on your server will not be an issue. 
Problem 	How I solved it
Could not connect to server using browser on http://3.26.37.84 
Ufw was blocking connections on port 80 so I had to create a new inbound rule on ufw, the security group was also blocking the connection thus a new inbound rule to allow port 80 was created as well on AWS security group 
Could not connect to ftp	UFW blocked connections on port 21, FTP also required ports 40000-50000/TCP to enable passive mode, created allow rules on both UFW and AWS security group to allow connections
	
	

13.	Industry relevance
I feel like the career roles in this lab series relates most to a Sysadmin. The typical role of a Sysadmin is to mange servers, network and security. They manage the patches of the operating system which is a huge part of the labs. They also configure the IP address and manage the network connections to and from the server as done using the security groups from AWS and the UFW on the server. They also handle the security aspect as per creation of the firewall rules. A huge part of the role of a Sysadmin is also automation, which means writing scripts to be executed at a timely basis. As used in the labs by making use of cron jobs. 
The experience of the labs allowed me to understand the structure and flow on setting up a server on the cloud. From the creation of an instance to the configuration of the DNS to creation of services and troubleshooting of the server. All these allow me to familiarize myself with different types of operating systems instead of the usual windows OS. Upon learning how to set up everything from scratch, it has allowed me to build the confidence to set up servers on the cloud and the relevant services when I go out into the workforce in the future.
14.	Final reflection
The overall learning experience for the entire module was excellent. I feel like having labs that are very hands on allowed me to have real experience instead of just studying its theory. By setting up an actual server and its services, it allowed me the experience of finding out why things do not work and finding out solutions. It allowed me the chance to learn the skill of troubleshooting the server and its services and to use this newfound knowledge in the workforce in the future. 
Some skills that I have improved is definitely my networking. Through the labs, there were many occasions whereby there were unsuccessful connections and thus knowing why each packet did not reach the destination is very important. Walking through the labs and troubleshooting the connections allowed me to see what are the common reasons why connections were unsuccessful. Another skill that I picked up is managing a server on the cloud. The labs have allowed me the opportunity to experiment with AWS instances to manage the firewall rules to use the AWS console interface which would make me more confident in performing them in the future. 
How I would do the server projects differently is to firstly map out whatever that needs to be done on paper first. To know what services are required, to take note of areas that could go wrong. This would save a lot of time troubleshooting as it would narrow down the reasons why things do not work. 
15.	AI Tools Used
Tools used for the assignment
-	Chatgpt
ChatGPT was used mainly for network troubleshooting and errors in connection. Chatgpt provided me insight into the ports that were needed to be opened in the case of VSFTPD. The ports being port TCP40000-50000. ChatGPT saved me a lot of time by telling me the answer right away so I did not have to look for solutions from scratch.

AI tools are very helpful in my learning as they provide an expedited means to gathering relevant data. AI tools such as ChatGPT gives you all the relevant information right away. If prompted right it may give you a direct answer to your query. It is extremely useful as it has access to a large pool of information that humans would otherwise have to look for on the internet. It as a result saves the user a lot of time in finding possible reasons that would result in certain errors or why applications do not work.

