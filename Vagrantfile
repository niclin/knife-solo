# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define :web1 do |web1_config|
    web1_config.vm.box = "ubuntu-16-04"
    web1_config.vm.host_name = "web-1"
    web1_config.vm.network "private_network", ip: "10.0.0.10"
    web1_config.vm.network "forwarded_port", guest: 80, host: 8080
    web1_config.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 2
    end
  end
end
