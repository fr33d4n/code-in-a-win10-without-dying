# encoding: utf-8
# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/bionic64"
  config.vm.synced_folder "C:/Users/XXXX/workspace", "/home/vagrant/workspace", :nfs => true # Change XXXX by your windows user
  config.ssh.forward_x11 = true

  config.vm.provision "shell" do |s|
  # replace Windows line endings with Unix line endings
  s.binary = true

  s.inline = "apt-get update
              apt-get install -y git
              curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash # Check the most recent nvm version!!
              apt-get install -y build-essential
              apt-get update
              apt-get upgrade -y
              apt-get autoremove -y"
  end
end