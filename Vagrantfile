# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.host_name = "postgresql"

  config.vm.provision :shell, :path => "vagrant-setup/bootstrap.sh"
  config.vm.network :forwarded_port, guest: 5432, host: 15432
end
