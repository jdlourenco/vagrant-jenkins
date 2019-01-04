Vagrant.configure('2') do |config|
  config.vm.box      = 'centos/7'
  config.vm.hostname = 'jenkins'

  config.vm.provision 'ansible' do |ansible|
    ansible.playbook = 'playbook.yml'
  end

  config.vm.network "forwarded_port", guest: 8080, host: 8080
end
