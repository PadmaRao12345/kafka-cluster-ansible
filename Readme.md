## Installation of Kafka Cluster Using Ansible

## Requirements
* vagrant

## Notes*
```
It assumes you have zookeeper already running in localmode or cluster mode.
OpenJDK8 will used by default.
```
**For Zookeeper Cluster Mode Installation**
https://github.com/116davinder/zookeeper-cluster-ansible

## To Start
* **STEP-1**
```
vagrant up
```

* **STEP-2**
```
vagrant ssh controller
```

* **STEP-3**
```
cd /home/vagrant/projects/playbooks
```

* **STEP-4**
```
ansible-playbook -i hosts/cluster-hosts.ini kafka-cluster.yml
```

# Supported/Tested OS
* CentOS 7
* RedHat 7