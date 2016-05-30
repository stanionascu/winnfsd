Vagrant.configure("2") do |c|
  c.vm.box = "ubuntu/trusty32"
  c.vm.synced_folder ".", "/vagrant", disabled: true
  c.vm.boot_timeout = 1800
  c.vm.provider :virtualbox do |p|
    p.customize ["modifyvm", :id, "--nictype1", "Am79C973"]
    p.customize ["modifyvm", :id, "--memory", "256"]
    p.gui = true
  end
end