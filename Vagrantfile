Vagrant.configure("2") do |config|
	
	config.vm.box = "hashicorp/precise64"
	
	config.vm.define :ubu do |ubu_config|
		ubu_config.vm.network "private_network", ip: "192.168.50.10"
		ubu_config.vm.provision "puppet" do |puppet| 						
			puppet.manifests_path = ["vm", "/vagrant/manifests"]
			puppet.manifest_file = "default.pp"
		end		
    end	
end	