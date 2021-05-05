Vagrant.configure("2") do |config|
  config.vm.box = "devn-centos7"

config.vm.define "vm1" do |vm1|

	vm1.vm.box = "devn-centos7"
	vm1.vm.hostname = 'vm1'
	vm1.vm.box_url = "file:///vagrant/centos-hashicorp.box"
	#vm1.vm.network "private_network", :type=> 'dhcp'
	vm1.vm.network "private_network", ip: '172.28.128.2'
	config.vm.provider "virtualbox" do |vb|
		vb.memory = 2048	
		end
	config.vm.synced_folder '.', '/vagrant', disabled: true
	end

	config.vm.define "vm2" do |vm2|
	vm2.vm.box = "devn-centos7"
	vm2.vm.hostname = 'vm2'
	vm2.vm.box_url = "file:///vagrant/centos-hashicorp.box"
	#vm2.vm.network "private_network", :type=> 'dhcp'
	vm2.vm.network "private_network", ip: '172.28.128.3'
	config.vm.provider "virtualbox" do |vb|
		vb.memory = 2048	
		end
	config.vm.synced_folder '.', '/vagrant', disabled: true
	end

	config.vm.define "vm3" do |vm3|
	vm3.vm.box = "devn-centos7"
	vm3.vm.hostname = 'vm3'
	vm3.vm.box_url = "file:///vagrant/centos-hashicorp.box"
	#vm3.vm.network "private_network", :type=> 'dhcp'
	vm3.vm.network "private_network", ip: '172.28.128.4'
	config.vm.provider "virtualbox" do |vb|
		vb.memory = 2048	
		end
	config.vm.synced_folder '.', '/vagrant', disabled: true
	end
	
	config.vm.define "vm4" do |vm4|
	vm4.vm.box = "devn-centos7"
	vm4.vm.hostname = 'vm4'
	vm4.vm.box_url = "file:///vagrant/centos-hashicorp.box"
	#vm4.vm.network "private_network", :type=> 'dhcp'
	vm4.vm.network "private_network", ip: '172.28.128.5'
	config.vm.provider "virtualbox" do |vb|
		vb.memory = 2048	
		end
	config.vm.synced_folder '.', '/vagrant', disabled: true
	end
end
