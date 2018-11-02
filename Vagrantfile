# -*- mode: ruby -*-
# vi: set ft=ruby :
#

Vagrant.configure('2') do |config|
  config.vm.box = 'debian/contrib-stretch64'
  config.vm.define 'stretch'
  config.vm.define 'jessie' do |j|
    j.vm.box = 'debian/jessie64'
  end

  config.vm.provision :shell, inline: <<-SHELL
    apt-get install vim curl -y
  SHELL

  config.vm.provision :ansible do |a|
    a.playbook = 'vagrant.yml'
  end
end
