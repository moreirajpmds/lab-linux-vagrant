Vagrant.configure("2") do |config|
    (1..2).each do |i|
        config.vm.define "fenix_#{i}" do |fenix|
            fenix.vm.box = "debian/jessie64"
            fenix.vm.network "public_network", bridge: "enp8s0", ip: "192.168.0.12#{i}"
        end

        config.vm.provider "virtualbox" do |fenix|
            fenix.memory = "1024"
            fenix.cpus = "2"
        end
    end
  
    (1..2).each do |i|
        config.vm.define "eagle_#{i}" do |eagle|
            eagle.vm.box = "centos/7"
            eagle.vm.network "public_network", bridge: "enp8s0", ip: "192.168.0.12#{i+2}"
        end

        config.vm.provider "virtualbox" do |eagle|
            eagle.memory = "1024"
            eagle.cpus = "2"
        end
    end
end
