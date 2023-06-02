
Vagrant.configure("2") do |config|

    config.vm.box = "hashicorp/bionic64"

    config.vm.define "virtualMachine1" do |vm1|
        vm1.vm.hostname = "virtualMachine1"
        vm1.vm.network "public_network", ip: "192.168.33.10"

        vm1.vm.provider "virtualbox" do |vb|
            vb.memory = "4096"
        end

#         vm1.vm.provision "ansible" do |ansible|
#             ansible.playbook = "playbook.yml"
#         end
    end

    config.vm.define "virtualMachine2" do |vm2|
        vm2.vm.hostname = "virtualMachine2"
        vm2.vm.network "public_network", ip: "192.168.33.11"

        vm2.vm.provider "virtualbox" do |vb|
            vb.memory = "4096"
        end
    end
end
