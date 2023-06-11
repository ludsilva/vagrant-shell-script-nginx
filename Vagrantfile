Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |v|
	  v.name = "ubuntu_vm"
	  v.memory = 2048
	  v.cpus = 2
  end

  config.vm.box = "hashicorp/bionic64"
  config.vm.network "forwarded_port", guest:80, host:8080
  config.vm.provision "shell", path: "script.sh"
  config.vm.synced_folder "cep/", "/var/www/html"
end
