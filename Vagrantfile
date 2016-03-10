Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "private_network", ip: "10.10.10.10"
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "site.yml"

end

end
