# -*- mode: ruby -*-

Vagrant.configure(2) do |config|
  config.vm.define "devvm" do |devvm_config|
    devvm_config.vm.box = "ubuntu/trusty64"
    devvm_config.vm.hostname = "devvm"
    devvm_config.vm.network "private_network", ip: "192.168.10.5"
    devvm_config.vm.box_check_update = false

    devvm_config.vm.provider "virtualbox" do |vb|
      vb.name = "devvm"
      vb.memory = "1024"
    end

    devvm_config.vm.provision "ansible" do |ansible|
      ansible.playbook = "provision.yml"
    end
  end
end
