Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
 
  config.vm.provider "virtualbox" do |v|
    v.memory = 4100
    v.cpus = 4
  end

  config.vm.network "private_network", type: "dhcp"
  config.vm.synced_folder ".", "/vagrant", type: 'virtualbox'
  config.vm.provision "shell", path: "provision.sh"
end