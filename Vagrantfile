# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|


  if Vagrant.has_plugin? "vagrant-vbguest"
    config.vbguest.no_install  = true
    config.vbguest.auto_update = false
    config.vbguest.no_remote   = true
  end


  config.vm.define :azureCompunube do |azureCompunube|
    azureCompunube.vm.box = "bento/ubuntu-22.04"
    azureCompunube.vm.network :private_network, ip: "192.168.100.9"
    azureCompunube.vm.hostname = "azureCompunube"
    azureCompunube.vm.boot_timeout = 800
  end

end

