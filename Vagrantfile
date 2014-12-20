# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile for trainer project
# 2014 Carlos Pintado <carlosmpintado@gmail.com>


# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

# Beginning of main configuration section
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  # Beginning of vm "repo" configuration section
  config.vm.define "repo" do |repovm|
    repovm.vm.box      = "centos6.4"
    repovm.vm.hostname = "repo"
    repovm.vm.network :private_network, ip: "192.168.17.101"
  end
  # End of vm "repo" configuration section

  # Beginning of vm "monitor" configuration section
  config.vm.define "monitor" do |monitorvm|
    monitorvm.vm.box      = "centos6.4"
    monitorvm.vm.hostname = "monitor" 
    monitorvm.vm.network :private_network, ip: "192.168.17.102"
  end
  # End of vm "monitor" configuration section

  # Beginning of vm "test" configuration section
  config.vm.define "test" do |testvm|
    testvm.vm.box = "centos6.4" 
    testvm.vm.hostname = "test" 
    testvm.vm.network :private_network, ip: "192.168.17.103"
  end
  # End of vm "repo" configuration section

end
# end of main configuration section
