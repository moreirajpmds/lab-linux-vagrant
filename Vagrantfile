Vagrant.configure("2") do |config|
    (1..2).each do |i|
        config.vm.define "debian_#{i}" do |debian|
            debian.vm.box = "debian/jessie64"
            debian.vm.network "public_network", bridge: "enp8s0", ip: "192.168.0.12#{i}"
        end

        config.vm.provider "virtualbox" do |debian|
            debian.memory = "1024"
            debian.cpus = "2"
        end
    end
  
    (1..2).each do |i|
        config.vm.define "centos_#{i}" do |centos|
            centos.vm.box = "centos/7"
            centos.vm.network "public_network", bridge: "enp8s0", ip: "192.168.0.12#{i+2}"
        end

        config.vm.provider "virtualbox" do |centos|
            centos.memory = "1024"
            centos.cpus = "2"
        end
    end
end
