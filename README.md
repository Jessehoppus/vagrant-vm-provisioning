# vagrant-vm-provisioning
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.network "private_network", type: "dhcp"
  config.vm.provision "shell", path: "provision.sh"
end

