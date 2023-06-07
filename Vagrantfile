Vagrant.configure("2") do |config|

    config.vm.define "vm1" do |node1|
        node1.vm.box = "hashicorp/bionic64"
        node1.vm.hostname = "vm1"
        node1.vm.network "public_network", ip: "192.168.33.10"
    end

    config.vm.define "vm2" do |node2|
	    node2.vm.box = "hashicorp/bionic64"
        node2.vm.hostname = "vm2"
        node2.vm.network "public_network", ip: "192.168.33.11"
    end

    config.ssh.forward_agent = true
end