### Apache (httpd) server

* Apache Server (httpd)
* Apache Server http Authentication
* Load Balancer(Server) and Reverse Proxy






__Load Balancer(Server) and Reverse Proxy__

Update the inventory file with group variables

[proxyserver]
192.168.1.140 ansible_user=user_name ansible_ssh_pass=password

[webserver]
192.168.1.140 ansible_user=user_name ansible_ssh_pass=password 
192.168.1.248 ansible_user=user_name ansible_ssh_pass=password


