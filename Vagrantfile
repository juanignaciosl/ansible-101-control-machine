# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "private_network", ip:"10.0.0.100"
  config.ssh.forward_agent = true
  config.vm.provider "virtualbox" do |v|
    v.name = "Ansible-101 - Control machine"
  end
  config.vm.provision "shell", path: "bootstrap.sh"
end

