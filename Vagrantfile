# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "chef/ubuntu-14.04"

  config.vm.synced_folder "chef", "/home/vagrant/.chef"
  config.vm.synced_folder "cookbooks", "/home/vagrant/cookbooks"
  config.vm.provision "shell", path: "provision.sh"
end
