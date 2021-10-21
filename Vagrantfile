# -*- mode: ruby -*-

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"
  config.ssh.insert_key = false

  config.vm.provider :virtualbox do |vb|
    vb.memory = 8096
    vb.linked_clone = true
  end

  # NSO Server
  config.vm.define "nso" do |nso|
   nso.vm.hostname = "nso.test"
   nso.vm.network :private_network, ip: "172.28.128.3"
  end

end
