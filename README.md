## **_Project-12-Automating-Loadbalancer-Configuration-with-Shellscripting_**
------------------------------------------------------------
### Overview

Hello and welcome! My name is Cecilia, and in this amazing project, I will demonstrate the deployment of Nginx as a Load balancer using shell script

Deploying and configuring the webservers

we need to codify the process we need to deploy in the shell scripting.

--------------------------------------------------------------------------

#### Step 1: Run the Script

step 1: provision an Ec2 instance running on ubuntu 20.04.

Result:

![](images/your-image.png)



step2: open port 8000 to allow traffic from anywhere using the security group.

Result:

![](images/your-image.png)


step 3: connect to the webserver via the terminal using SSH client.

Result:

![](images/your-image.png)


step 4: open a file

Results:


![](images/your-image.png)



step 5: Run the shell script using this command: ./install.sh 54.177.88.13 (your public_ip address)

Results:

![](images/your-image.png)




Deploying and configuring Nginx load balancer

we need to provision an Ec2 instance Nginx-loadbalancer running ubuntu 22.04 and then open port 80 using the security group.

Results:





step1: connect to your web browser using SSH client



step2: On your terminal, open a file nginx.sh and change the permission on the file to make it executable.



step3: Run this command sudo vi nginx.sh and paste your file then close the file by typing Esc shift + :wq!.

First digits is the public IP address of the EC2 instance where Nginx is installed.

Second digits is the URL and port number of the first webserver to which the load balancer will distribute traffic.

Third digits is the URL and port number of the second webserver to which the load balancer will distribute traffic.

Results:





Result for webserver 1:



Result for webserver2:



Result for loadbalancer:



