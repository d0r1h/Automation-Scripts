# Automation Scripts
Ansible (Automation) Scripts for different IT tasks -

 * Hadoop
 * Docker
 * Apache Server (httpd)
 * Load Balancer (Server)
 
 
 
## Note :

	These are individual scripts for learning purpose.
	
	

## Usage :

	Install Python36 & Ansible 
	
	yum install python36 (RedHat)
	apt install python36 (Ubuntu)


	pip3 install ansible 
	
	
	After Installation Done :
	
	Create a file as hosts.txt and write the inventory
	
	ip_address ansible_user = user ansible_ssh_pass = pass
	
	Update the address of hosts.txt in /etc/ansible/ansible.cfg
	
	[defaults]
	inventory = /path/hosts.txt
	
	
	ansible-playbook file.yml  -> to run playbook
	
	
