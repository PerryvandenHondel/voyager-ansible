Ansible scripts from

System: voyager

CI:     CI0094

Directory: /home/ansible/ansible


# Upgrade all the Ubuntu servers.
ansible ubuntu -m apt -a "upgrade=yes update_cache=yes" -b

# Upgrade all the CentOS servers.
ansible centos -m yum -a "name=* state=latest" -b


Test Ansible

One Command
$ ansible ubunti -m ping


Playbook

$ ansible-playbook update-os-ubuntu.yml

