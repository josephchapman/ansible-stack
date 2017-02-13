# ansible

I have no idea what I'm doing.

## Method 1: From your local machine, provision a VM

This uses VirtualBox + Vagrant with the `ansible_local` provisioner.

Install `vagrant` and `virtualbox`, then:
```
$ git clone https://github.com/josephchapman/ansible.git

$ cd ansible

$ vagrant up
```

## Method 2: Directly on a server

This method uses `ansible` locally.

Install `ansible`, then:
```
# git clone https://github.com/josephchapman/ansible.git

# ansible-playbook -i "localhost," -c local ansible/provisioning/site.yml
```