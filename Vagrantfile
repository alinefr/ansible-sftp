# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.define 'local' do |local|
    local.vm.box = 'ubuntu/xenial64'
  end
  config.vm.provision 'ansible' do |ansible|
    ansible.playbook = 'ansible/playbook.yml'
    ansible.galaxy_role_file = 'ansible/requirements.yml'
    ansible.galaxy_roles_path = 'ansible/roles'
  end
end
