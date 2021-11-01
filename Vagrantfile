Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.box_version = "1905.1"
  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
  end
  config.vm.define "cka-cls-01" do |server|
    server.vm.hostname="cka01"
    server.vm.network "private_network", ip: "172.28.128.11"
  end
  config.vm.define "cka-cls-02" do |server|
    server.vm.hostname="cka02"
    server.vm.network "private_network", ip: "172.28.128.12"
  end
  config.vm.define "cka-cls-03" do |server|
    server.vm.hostname="cka03"
    server.vm.network "private_network", ip: "172.28.128.13"
  end
  config.vm.define "cka-cls-04" do |server|
    server.vm.hostname="cka04"
    server.vm.network "private_network", ip: "172.28.128.14"
  end
end