# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  create_machine(config, 1)
  create_machine(config, 2)
end

def create_machine(config, number)
  config.vm.define "machine-#{number}" do |machine|
    machine.vm.box = "ubuntu/bionic64"

    machine.vm.network "private_network", ip: "192.168.50.#{number}"
  end
end
