# Udacity Project: Linux Server Configuration
----

### 1.The IP address and port
  IP address :  13.57.208.123  
  SSH prot : 2200

### 2.The complete URL  
  http://13.57.208.123/  
  http://13.57.208.123/admin

### 3.Configuration changes  
apt-get upgrade  
adduser grader  
/etc/ssh/sshd_config :   
> Port 2200  
> PermitRootLogin no  
> PasswordAuthentication no  
 
/etc/sudoers :
> grader ALL=(ALL) ALL  

ufw :  
> ufw default deny incoming  
> ufw default allow outgoing  
> ufw allow ssh 2200/tcp  
> ufw allow 80/tcp  
> ufw allow 123/udp  



### 4.Third-party resources  
  libapache2-mod-wsgi-py3  
  git
