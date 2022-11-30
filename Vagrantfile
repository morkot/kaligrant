Vagrant.configure("2") do |config|
  banner = <<-MSG
   _         _ _                       _
  | |       | (_)                     | |
  | | ____ _| |_  __ _ _ __ __ _ _ __ | |_
  | |/ / _` | | |/ _` | '__/ _` | '_ \\\| __|
  |   < (_| | | | (_| | | | (_| | | | | |_
  |_|\\\_\\\__,_|_|_|\\\__, |_|  \\\__,_|_| |_|\\\__|
                  __/ |
                 |___/

MSG

  puts(banner)

  config.vm.box = "kalilinux/rolling"
  config.vm.box_version = "2022.3.2"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
    vb.memory = "4096"
    vb.cpus = 2
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
  end
end
