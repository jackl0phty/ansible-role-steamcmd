Vagrant.configure(2) do |config|

  # Setup Ubuntu Xenial64 16.04 Box.
  config.vm.define "xenial", primary: true do |xenial|
    xenial.vm.box = "ubuntu/xenial64"
  end

  # Setup Ubuntu Trusty64 14.04 Box.
  config.vm.define "trusty", primary: true do |trusty|
    trusty.vm.box = "ubuntu/trusty64"
  end

  # Setup CentOS 7 Box.
  #config.vm.define "centos7" do |centos7|
  #  centos7.vm.box = "centos/7"
  #end

  # Enable ansible as the provisioner.
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "tasks/main.yml"
    ansible.playbook = "tasks/killing_floor.yml"
  end

end
