# ansible

I have no idea what I'm doing.

## VirtualBox + Vagrant with `ansible_local` provisioner method

Install `vagrant` and `virtualbox`, then:
```
$ git clone https://github.com/josephchapman/ansible.git

$ cd ansible

$ vagrant up
```

## Ansible method

Install `ansible`, then:
```
# git clone https://github.com/josephchapman/ansible.git

# ansible-playbook -i "localhost," -c local ansible/provisioning/site.yml
```