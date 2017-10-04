[![](https://img.shields.io/badge/SISTECH-LAB-orange.svg)](http://cs.uph.edu)
[![](https://img.shields.io/badge/SISTECH-Software%20Engineering-green.svg)](http://cs.uph.edu)
[![](https://img.shields.io/badge/SISTECH--UPH-Cloud%20Computing-blue.svg)](http://cs.uph.edu)

# vagrant_ansible_multi_server
Lab resource for Ansible Multiple Servers

# Test connection to all machines in your ansible environment
ansible all -m ping --ask-pass

the password is: vagrant

# Install Apache Web server
ansible-playbook apache.yml --ask-pass

#Install Haproxy
ansible-playbook haproxy.yml --ask-pass

# Set your mgmt server
as root user: 
sudo vi /etc/hosts

add one line with:
10.0.15.16 example.com 

#Test your load balancer using Jmeter or Tsung

