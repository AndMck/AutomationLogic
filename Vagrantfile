# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'virtualbox'

Vagrant.configure("2") do |config|
  
    config.vm.define "ans" do |ans|
      ans.vm.box = "puppetlabs/ubuntu-14.04-64-nocm"
      ans.vm.hostname = "ans"
      ans.vm.network "private_network", ip: "192.168.20.10"
    end

    config.vm.define "web" do |web|
      web.vm.box = "nrel/CentOS-6.7-x86_64"
      web.vm.hostname = "web1"
      web.vm.network "private_network", ip: "192.168.20.20"
      web.vm.network "forwarded_port", guest: 80, host: 8080
    end

      # Run Ansible from the Vagrant VM
      config.vm.provision "ansible_local" do |ansible|
      
    end
    
end