Vagrant.configure(2) do |config|
  config.vm.box = "bento/ubuntu-14.04"
  config.vm.box_version = "201808.24.0"
  config.vm.network :forwarded_port, host: 8000, guest: 8000
  config.vm.provision "ansible" do |ansible|
    ansible.verbose = 'vvv'
    ansible.playbook = 'playbook.yml'
  end
end
