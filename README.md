Apigee Maintenance Playbook - Validate Ports Prior to Installing Apigee OPDK
============================================================================

This playbook provides maintenance assistance for the tasks of 
validating that the ports required by Apigee OPDK are in fact accessible. 
The first playbook called validate-ports.yml will update the ansible cache
and install a python http server on the remote node using the specified port.
The host machine will serve as a client to perform a GET action. This 
playbook cleans up the server node and releases the port upon completion. 


Usage Instructions
==================

These are ansible playbooks and require ansible.

1. Please install and configure ansible as indicated in [opdk-setup-ansible](https://github.com/carlosfrias/apigee-opdk-playbook-setup-ansible).
1. `ansible-galaxy install -f -r requirements.yml`
1. `ansible-playbook -i <inventory file or folder> validate-ports.yml`

<!-- BEGIN Google Required Disclaimer -->

# Required Disclaimer

This is not an officially supported Google product.
<!-- END Google Required Disclaimer -->
