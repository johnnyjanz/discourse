
Vagrant.configure(2) do |config|
  config.vm.box     = 'trusty64'
  config.vm.box_url = "file:///C:/Users/JQUIJANO/Documents/vagrant/projects/package.box"
  config.vm.network "private_network", ip: "192.168.10.203"
	config.vm.hostname = "puppet"
  config.vm.provider :virtualbox do |vb|
      vb.name = "puppet"
  end

  config.vm.provision "puppet" do |puppet|
    puppet.module_path = "modules"
  end

end