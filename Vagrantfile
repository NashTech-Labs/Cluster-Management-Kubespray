Vagrant.configure("2") do |config|
  config.vm.define "master1" do |master1|
    master1.vm.box_download_insecure = true
    master1.vm.box = "hashicorp/bionic64"
    master1.vm.network "private_network", ip: "192.168.10.1"
    master1.vm.hostname = "master1"
    master1.vm.provider "virtualbox" do |v|
      v.name = "master1"
      v.memory = 2048
      v.cpus = 2
    end
  end

  config.vm.define "kubmaster1" do |kubmaster1|
    kubmaster1.vm.box_download_insecure = true
    kubmaster1.vm.box = "hashicorp/bionic64"
    kubmaster1.vm.network "private_network", ip: "192.168.10.2"
    kubmaster1.vm.hostname = "kubmaster1"
    kubmaster1.vm.provider "virtualbox" do |v|
      v.name = "kubmaster1"
      v.memory = 3072
      v.cpus = 3
    end
  end

  config.vm.define "worker1" do |worker1|
    worker1.vm.box_download_insecure = true
    worker1.vm.box = "hashicorp/bionic64"
    worker1.vm.network "private_network", ip: "192.168.10.3"
    worker1.vm.hostname = "worker1"
    worker1.vm.provider "virtualbox" do |v|
      v.name = "worker1"
      v.memory = 3072
      v.cpus = 3
    end
  end

end
