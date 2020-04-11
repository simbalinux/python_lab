# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.vm.define  "python" do |host|
    host.vm.synced_folder ".", "/vagrant", type: 'virtualbox'
#    host.vm.box = "centos/7"
    host.vm.box = "bento/ubuntu-18.04"
    host.vm.hostname = "python"
    host.vm.network "private_network", ip: "192.168.50.119"
    host.vm.provision "shell", path: "./config/strap_python"
  end
end

