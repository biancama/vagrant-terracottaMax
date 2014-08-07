# TerracottaMax with Vagrant and Ansible

This playbook install [TerracottaMax](http://terracotta.org/products/bigmemorymax) and [Terracotta Management Console](http://terracotta.org/documentation/4.1/tms) on a vagrant server. 

What gets installed:

*  openjdk 1.7

## Let's do this!

If you want to install Terracotta on a VM using Vagrant, you first need to install [Vagrant](http://www.vagrantup.com/) and a Virtual Machine provider of choice ([VirtualBox](https://www.virtualbox.org/) is free and works out of the box with Vagrant).



```
$ git clone https://github.com/biancama/vagrant-terracottaMax
$ cd /path/to/vagrant-terracottaMax
$ vagrant up
```

## Different OS

By default, the Vagrant box runs Ubuntu 14.04, but should support CentOS 6.4 (NOT TESTED)

## 
The script install terracotta server on host 192.168.33.20 and port 9520
and web management console http://192.168.33.20:9889/tmc/

two additional services are installed 
* terracotta
* tmc

## License
vagrant-terracottaMax/roles/terracotta/files/terracotta-license.key 
is a trial key so could be expiered when you try this script. Please replace with your key 

## Known issues / TODO

* TBD 

## Contribute

* Help is really appriciated. 