# -*- mode: ruby -*-
# vi: set ft=ruby :VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(2) do |config|
config.ssh.insert_key = false
config.vm.provider :virtualbox do |vb|
vb.customize ["modifyvm", :id, "--memory", "256"] end

# Application server 1.
config.vm.define "app1" do |app|
app.vm.hostname = "app1.dev"
app.vm.box = "centos/7"
app.vm.network "private_network", ip: "192.168.33.11"
end

# Application server 2.
config.vm.define "app2" do |app|
app.vm.hostname = "app2.dev"
app.vm.box = "centos/7"
app.vm.network "private_network", ip: "192.168.33.12"
end

end

