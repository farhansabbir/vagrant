Vagrant.configure("2") do |config|

  (1..5).each do |i|
    config.vm.define "vm#{i}" do |node|
      node.vm.box = "devn-centos7"
      node.vm.hostname = "vm#{i}"
      node.vm.box_url = "file:///vagrant/centos-hashicorp.box"
      node.vm.network "private_network", ip: "172.28.128.#{i+1}", auto_config: true, virtualbox__inet: true
      
      config.vm.provider "virtualbox" do |vb|
		vb.memory = 1024	
      end
      config.vm.synced_folder '.', '/vagrant', disabled: true
    end
  end
end
