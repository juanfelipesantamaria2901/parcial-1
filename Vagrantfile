Vagrant.configure("2") do |config|

  if Vagrant.has_plugin? "vagrant-vbguest"
    config.vbguest.no_install = true
    config.vbguest.auto_update = false
    config.vbguest.no_remote = true
  end

  config.vm.define :server2PXE do |server2PXE|
    server2PXE.vm.box = "centos/7"
    server2PXE.vm.network :private_network, ip: "192.168.50.5"
    server2PXE.vm.hostname = "server2PXE"
    end
end 