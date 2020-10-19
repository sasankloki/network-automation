# network-automation
The project involves deploying a simple Nginx and PHP script on webservers and deploying a HAProxy loadbalancer using Ansible-Playbook script.

Bastion Host

Bastion host is used to access a private network from the external network
the bastion server is created with public_ip and private_ip address the public ip address is used for the user to connect to webservers through private address.
In this the project requires a proper ssh configaration, the ssh data configaration is done in a cofig file to connect from local machine.
the servers are accessed through the loadbalancer and communicates the backend servers using the rouondrobin load-balancing algorithm for delivering the service.

HAproxy

HAproxy is used for High Availabilty proxy,it is an open source load balancer which is used for for distributing the load on multiple servers and improve the reliabilty.

This project has been designed to run in two ways it can be done through 'ansible-playbook -i hosts sites.yaml' it will be directly run the curl command also, and this can be done by typing curl ip also.



