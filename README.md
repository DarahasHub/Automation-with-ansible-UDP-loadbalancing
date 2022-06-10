# Automation-with-ansible-UDP-loadbalancing
The assignment is about deploying the flask app and configuring the SNMP daemon on the web servers(devA, devB, devC). The deployment is done using an ansible-playbook. The deployment of the flask application is served through the HAproxy and the configuration of SNMP is carried through Nginx.

## 2.1: Deploying the flask app on the webservers
The packages installed in the HAproxy server are ansible, HAproxy, and flask.
The HAproxy server acted as an HAproxy load balancer for webservers.
The BastionHost(bastionNSO) is used as an entry point via SSH using an ssh config file('config') to the webservers.

## 2.2: Configuring SNMPd daemon on the webservers
The packages installed in the HAproxy server are ansible, nginx, and snmpd.
The HAproxy server acted as an nginx load balancer for webservers.

The ansible-playbook for both the tasks is included in the 'site.yaml' file.
