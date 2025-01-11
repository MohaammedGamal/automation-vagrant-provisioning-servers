Vagrant.configure("2") do |config|
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true
  config.vm.boot_timeout = 600
  config.vm.network "public_network", bridge: "Realtek PCIe FE Family Controller"

  config.vm.define "server1" do |server1|
    server1.vm.box = "ubuntu/jammy64"
    server1.vm.hostname = "server1"
    server1.vm.provider "virtualbox" do |vb|
      vb.memory = "500"
    end
  end
end
