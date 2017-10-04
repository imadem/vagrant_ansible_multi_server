[![](https://img.shields.io/badge/SISTECH-LAB-orange.svg)](http://cs.uph.edu)
[![](https://img.shields.io/badge/SISTECH-Software%20Engineering-green.svg)](http://cs.uph.edu)
[![](https://img.shields.io/badge/SISTECH--UPH-Cloud%20Computing-blue.svg)](http://cs.uph.edu)
[![](https://img.shields.io/badge/SISTECH--UPH-Homework-red.svg)](http://learn.uph.edu)

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

add an address below:
10.0.15.16 example.com 

#Test your load balancer using apache2-utils
1. Install apache2-utils : sudo apt-get install apache2-utils
2. run ab -n 1000 -c 1000 http://example.com

# Monitor the load balancer in action
Take a look at the load in http://10.0.15.16:81 or http://example.com:81

# Your task:
1. Automate the haproxy installation.
2. Using different workload, check the availability of the load balancer.
3. Upload your report to your github space. 

