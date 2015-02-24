# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "emincan/ecsbox"
  config.vm.network "private_network", ip: "192.168.33.33"
  config.vm.synced_folder "www", "/var/www", id: "vagrant-root", :nfs => false

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--memory", "1024"]
  end

end