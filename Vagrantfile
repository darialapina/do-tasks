# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  (1..2).each do |i|
    config.vm.define "machine-#{i}" do |machine|
      machine.vm.box = "ubuntu/bionic64"
      machine.vm.network "private_network", type: "dhcp"
    end
  end
end
