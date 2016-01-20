# swarmbox-ansible
Swarmbox provisioning with ansible

# Sample inventory file:
```
[boxes]
192.168.0.75  hostname=swarmbox-01 hostname_suffix=01 swarm_master=true
192.168.0.197 hostname=swarmbox-02 hostname_suffix=02
192.168.0.85  hostname=swarmbox-03 hostname_suffix=03
192.168.0.131 hostname=swarmbox-04 hostname_suffix=04
```

# Prepare your certificates needed for the swarm nodes and copy them to ./certs/docker

# How to run
ansible-playbook -i inventory.file -s site.yml
