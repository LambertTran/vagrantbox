Vagrant.configure("2") do |config|
  config.vm.define "controller1" do |box1|
    box1.vm.box = "hashicorp/bionic64"
    box1.vm.hostname = 'controller1'
    box1.vm.provision "shell", path: "common-pkg.sh"
    #box1.vm.provision "shell", path: "docker.sh"
    box1.vm.network :public_network, ip: "10.0.0.200", bridge: "en1: Wi-Fi (AirPort)"
  end

  config.vm.define "controller2" do |box2|
    box2.vm.box = "hashicorp/bionic64"
    box2.vm.hostname = 'controller2'
    box2.vm.provision "shell", path: "common-pkg.sh"
    #box2.vm.provision "shell", path: "docker.sh"
    box2.vm.network :public_network, ip: "10.0.0.201", bridge: "en1: Wi-Fi (AirPort)"
  end

  config.vm.define "dns" do |box3|
    box3.vm.box = "hashicorp/bionic64"
    box3.vm.hostname = 'dns'
    box3.vm.provision "shell", path: "common-pkg.sh"
    #box3.vm.provision "shell", path: "docker.sh"
    box3.vm.network :public_network, ip: "10.0.0.202", bridge: "en1: Wi-Fi (AirPort)"
  end

  config.vm.define "kube-lb" do |box4|
    box4.vm.box = "hashicorp/bionic64"
    box4.vm.hostname = 'kube-lb'
    box4.vm.provision "shell", path: "common-pkg.sh"
    #box4.vm.provision "shell", path: "docker.sh"
    box4.vm.network :public_network, ip: "10.0.0.203", bridge: "en1: Wi-Fi (AirPort)"
  end

  config.vm.define "worker1" do |box5|
    box5.vm.box = "hashicorp/bionic64"
    box5.vm.hostname = 'worker1'
    box5.vm.provision "shell", path: "common-pkg.sh"
    #box5.vm.provision "shell", path: "docker.sh"
    box5.vm.network :public_network, ip: "10.0.0.204", bridge: "en1: Wi-Fi (AirPort)"
  end

  config.vm.define "worker2" do |box6|
    box6.vm.box = "hashicorp/bionic64"
    box6.vm.hostname = 'worker2'
    box6.vm.provision "shell", path: "common-pkg.sh"
    #box6.vm.provision "shell", path: "docker.sh"
    box6.vm.network :public_network, ip: "10.0.0.205", bridge: "en1: Wi-Fi (AirPort)"
  end
end
