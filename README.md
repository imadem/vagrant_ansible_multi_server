# vagrant_ansible_multi_server
Lab resource for Ansible Multiple Servers

# In order to use a password less login use the command below
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

