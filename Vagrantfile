Vagrant.configure("2") do |config|
  config.vm.box = "kalilinux/rolling"
  config.vm.box_version = "2021.3.0"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
    vb.memory = "4096"
    vb.cpus = 2
    # vb.customize ["modifyvm", :id, "--graphicscontroller", "vboxsvga"]
    # vb.customize 'post-boot', ["controlvm", :id, "setvideomodehint", "1920", "1080", "128"]
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
  end
end
