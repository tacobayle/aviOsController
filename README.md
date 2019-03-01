# aviOsController
## Prerequisites:
1. Make sure openstacksdk is installed:
```
pip install --user openstacksdk
```
## Input:

## Use the ansible playbook to:
- Create a new Project in OpenStack
- Grant admin role to the new tenant
- Create Network
- Create Subnet
- Create Router
- Create Security Groups
- Create rules
- Create SSH key
- Upload Glance image
- Create Flavor
- Create Neutron Port (for fixed IPs)
- Spin-up Avi Controller(s)

## Parameters:
All the variables are stored in var/params.yml

## Run the playbook:
ansible-playbook aviOsController.yml

## Tests:
Playbooks have been tested against:
- Ansible 2.7.0, 2.8.0.dev0
- Openstack Pike, queens (devstack)

## Improvement:
Make sure the quota are configured according to Avi controller needs. 
