# Basic Linux Setup
This repo provides some Ansible roles and scripts that allow me to automate some tasks that I oftenly do on a new workstation setup.

## How to use
If you haven't installed Ansible yet, you can execute the provided installation script

    sudo bash ./install-ansible.sh

Then you can overwrite the content of the ``/etc/ansible`` dir with the content of this repo. Remember to setup your own user and password in the ``host_vars/localhost`` file.

Now you should execute the playbooks using the following commands:
1. ``cd playbooks`` 
2. ``ansible-playbook create-dirs.yml``
3. ``ansible-playbook galaxy/main.yml``
4. ``ansible-playbook execute-roles.yml``

## Support
This configuration has been tested on the following distributions

| Distribution | Version |
| ------------ | ------- |
| Fedora       | 38      |
