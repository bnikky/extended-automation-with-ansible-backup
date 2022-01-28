
# A2: Service deployment with Ansible
Using Ansible We can create only one task but using ansible playbook we can execute multiple tasks.
A webservice is implemented using NGNIX web server.
Bastion Host is used as jump host.
HAproxy is used as the Load balancer.
Standard SNMP daemon is used to respond requests from any IP.
Ansible Playbook is used to automate the above service deployments.
Ansible Playbook are executed on a set, group and classification of hosts which together makeup an ansible

I have created the servers in the city cloud using the ssh key-gen and saved my keys in '~/.ssh/'.

# IPs of the servers created in city cloud:

devA: 10.1.0.166

devB: 10.1.0.193

devC: 10.1.0.200

bastionET2598: 188.95.231.172

haproxy: 91.106.193.56

# Service-deployment-with-ansible

HAproxy: 91.106.193.56

BastionET2598: 188.95.231.172

dev A: 10.1.0.166

dev B: 10.1.0.193

dev C: 10.1.0.200

HAproxy acts as both UDP and TCP load balancer with the help of NGINX

#Folder structure is used based on the best practices suggested here
https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html
