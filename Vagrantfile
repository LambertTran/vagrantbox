$common = <<EOF
sudo apt-get update
sudo apt-get install -y dnsutils iputils-ping telnet aptitude
EOF


Vagrant.configure("2") do |config|
  config.vm.define "controller1" do |box1|
    box1.vm.box = "hashicorp/bionic64"
    box1.vm.hostname = 'controller1'
    #box1.vm.provision "shell", inline: $common
    box1.vm.provision "shell", path: "common-pkg.sh"
    box1.vm.network :public_network, ip: "10.0.0.200", bridge: "en1: Wi-Fi (AirPort)"
  end

  #config.vm.define "controller2" do |box2|
  #  box2.vm.box = "hashicorp/bionic64"
  #  box2.vm.hostname = 'controller2'

  #  box2.vm.network :public_network, ip: "10.0.0.201"
  #end

end
