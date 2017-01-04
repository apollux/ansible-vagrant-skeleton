# Ansible Vagrant Skeleton

Skeleton to develop Ansible playbooks using Vagrant for test and debugging.

## Usage
Run `vagrant up` to create a VM and run the provisioning
Run `vagrant provision` to re-run the playbook on a already provisioned VM.
Run `vagrant destroy && vagrant up` to destroy and re-create a VM.

Ansible can also be invoked directly like so: `ansible-playbook -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory -become playbook.yml`.
