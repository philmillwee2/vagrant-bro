# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"
  config.vm.box_check_update = false

  config.vm.provider "virtualbox" do |vb|
    vb.name = "vagrant-bro"
    vb.cpus = "2"
    vb.memory = "1024"
  end
  
  config.vm.provision "shell", inline: <<-SHELL
    yum clean all
    yum update -y
  SHELL
end
