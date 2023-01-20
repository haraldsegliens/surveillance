# iSpy Agent DVR MicroK8S server

MicroK8S deployment of iSpy Agent DVR server using ansible.

## How to run

1. Install ansible

2. Create inventory file. For example localhost_inventory file with following contents: 127.0.0.1 ansible_connection=local      ansible_user=username      ansible_become_password=password

2. Run command: ansible-playbook surveillance/deploy-surveillance.yaml --extra-vars "public_host=some.host.name root_deployment_directory=kubernetes env=prod" -i localhost_inventory

