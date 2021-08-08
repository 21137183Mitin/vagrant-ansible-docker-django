Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network :forwarded_port, host: 8000, guest: 8000
  config.vm.provision "ansible" do |ansible|
    ansible.verbose = 'vvv'
    ansible.playbook = 'playbook.yml'
  end
end
