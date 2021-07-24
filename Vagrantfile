# set up the default terminal
ENV["TERM"]="linux"

Vagrant.configure("2") do |config|
  
  # set the image for the vagrant box
  config.vm.box = "opensuse/Leap-15.3.x86_64"
  ## Set the image version
  #config.vm.box_version = "15.2.31.212"

  # st the static IP for the vagrant box
  config.vm.network "private_network", ip: "192.168.9.150"
  
  # consifure the parameters for VirtualBox provider
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "3048"
    vb.cpus = 1
    vb.customize ["modifyvm", :id, "--ioapic", "on"]
  end
end
