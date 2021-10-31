Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.box_version = "1905.1"
  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
  end
  config.vm.define "cka-cls-01" do |server|
    server.vm.network "private_network", ip: "172.28.128.3", auto_config:false
  end
  config.vm.define "cka-cls-02" do |server|
    server.vm.hostname = "cka-cls-02"
    server.vm.network "private_network", ip: "172.28.128.4", auto_config:false
  end
  config.vm.define "cka-cls-03" do |server|
    server.vm.hostname = "cka-cls-03"
    server.vm.network "private_network", ip: "172.28.128.5", auto_config:false
  end
  config.vm.define "hello-iptables" do |server|
    server.vm.network "private_network", ip: "172.28.128.100", auto_config:false
  end
end