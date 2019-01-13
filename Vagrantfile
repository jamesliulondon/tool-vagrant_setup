Vagrant.configure("2") do |config|
  config.vm.provision "shell", inline: "echo Hello"
  config.vm.synced_folder ".", "/vagrant/ansible"

  config.vm.define "master" do |master|
    master.vm.box = "bento/centos-7.5"
  end

  config.vm.define "worker" do |worker|
    worker.vm.box = "bento/centos-7.5"
  end
end


