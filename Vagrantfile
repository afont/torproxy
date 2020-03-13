
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-19.10"
  config.vm.hostname = "torproxy"
  config.vm.network "private_network", ip: "192.168.20.20"
  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.ssh.shell = "bash -c 'BASH_ENV=/etc/profile exec bash'"
  config.vm.provision "file", source: "provision", destination: "/home/vagrant/"
  config.vm.provision :shell, :path => "shell/ansible-setup.sh"
end
