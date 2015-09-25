# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  # Vagrant box: Ubuntu 14.04 LTS
  config.vm.box = "ubuntu/trusty64"

  # Port forwarding
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "forwarded_port", guest: 4433, host: 4433

  # Ansible provisioning
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
  
end
