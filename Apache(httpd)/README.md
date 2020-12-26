### Apache (httpd) server

* Apache Server (httpd)
* Apache Server http Authentication
* Load Balancer(Server) and Reverse Proxy






__Load Balancer(Server) and Reverse Proxy__

> Update the inventory file with group variables

	[proxyserver]
	192.168.1.140 ansible_user=user_name ansible_ssh_pass=password

	[webserver]
	192.168.1.140 ansible_user=user_name ansible_ssh_pass=password 
	192.168.1.248 ansible_user=user_name ansible_ssh_pass=password

	
> Updating reverse proxy configuration file with following jinja2 code 
	
	{%  for i in groups['webserver']  %}
    	server  app{{ loop.index }}  {{ i }}:80  check
	{%  endfor  %}

	So whenever a new node gets added in inventory file it will updated in reverse proxy system too.

[Reverse Proxy(Haproxy) with Ansible](https://medium.com/@d0r1h/reverse-proxy-haproxy-with-ansible-962d83da1b09)

> In Role dir

	In role dir I have added roles for seprate services that needed in server and 
	you can run in single click by running setup.yml 
	Product  -- httpd, Haproxy



						
