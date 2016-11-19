# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'virtualbox'

Vagrant.configure("2") do |config|
  
  config.vm.define "ans" do |ans|
    ans.vm.box = "puppetlabs/ubuntu-14.04-64-nocm"
    ans.vm.hostname = "acs"
    ans.vm.network "private_network", ip: "192.168.20.10"
  end
end