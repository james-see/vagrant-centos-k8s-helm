# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = "fidi"
  config.vm.define "fidi"
  DISCO_PROJECT_FOLDER = "/Users/jc/projects/fidi"
  config.vm.synced_folder DISCO_PROJECT_FOLDER, "/home/vagrant/projects/primer/fidi", type: "virtualbox"
  config.vm.provider "virtualbox" do |vb|
      vb.customize ["modifyvm", :id, "--cpus", 2]
      vb.customize ["modifyvm", :id, "--memory", "4096"]
  end
end
