# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = 'chef-server'
  config.vm.network :private_network, ip: "192.168.2.10"		
  config.vm.provider :virtualbox do |v|
	v.customize ["modifyvm", :id, "--memory", 1024]
	v.customize ["modifyvm", :id, "--name","chef-server"]
	end

end
