Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision :shell, path: "bootstrap.sh"

  config.vm.network "forwarded_port", guest: 4000, host: 4000, auto_correct: true

  config.vm.synced_folder ".", "/vagrant"

  config.ssh.forward_agent = true

end
