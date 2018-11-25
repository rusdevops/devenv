# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/bionic64"
  config.vm.network "public_network"

  config.vm.provider "virtualbox" do |vb|

    vb.gui = true
    vb.memory = "2048"
  end

  config.vm.provision "shell", path: install.sh
  config.vm.provision "shell", privileged: false, path: bootstrap.sh
end
