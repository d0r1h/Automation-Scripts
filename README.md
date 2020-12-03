# Automation Scripts
Ansible (Automation) Scripts for different IT tasks -

 * Hadoop
 * Docker
 * Apache Server (httpd)
 * Load Balancer (Server)
 
 
 
## Note:

	These are individual scripts for learning purpose.
	
	

## Usage:

	Install Python 3 & Ansible 
	
	yum install python 3 (RedHat)
	apt install python 3 (Ubuntu)


	pip3 install ansible 
	
	
	After Installation:
	
	Create a file as hosts.txt and write the inventory
	
	ip_address ansible_user=user ansible_ssh_pass=pass
	
	ip_address = target node IP
	ansible_user = target node username
	ansible_ssh_pass = targetnode passoword
	
	Update the address of hosts.txt in /etc/ansible/ansible.cfg
	
	[defaults]
	inventory = /path/hosts.txt
	
	
	ansible-playbook file.yml  -> to run playbook
	
	
