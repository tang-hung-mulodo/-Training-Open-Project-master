Vagrant.configure(2) do |config|

  config.vm.box = "centos6.5x64"

  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.network "private_network", ip: "192.168.33.10"


  config.vm.network "public_network"

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
