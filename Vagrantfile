Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.provision "shell",
    inline: "apt update && apt install nginx -y && systemctl start nginx"
end
