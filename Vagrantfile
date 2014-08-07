# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.define "terracotta" do |terracotta|
    # terracotta.vm.box = "centos-6-4"
    terracotta.vm.box = "ubuntu/trusty64"
    terracotta.vm.network :private_network, ip: "192.168.33.20"

    terracotta.vm.provision "ansible" do |ansible| 
      ansible.playbook = "terracotta.yml"
      #ansible.verbose = 'vvv'
    end 
  end

  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--memory", "4096"]
  end

end
