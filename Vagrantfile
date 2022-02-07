Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu2004"
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.synced_folder "html/", "/var/www/html"
  config.vm.network :forwarded_port, guest: 80, host: 8080
  end