Vagrant.require_version ">= 1.7.0"
Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.provision "shell", inline: "apt-get update && apt-get -qq install python python-pycurl python-apt"

  config.vm.provision "ansible", type: "ansible" do |ansible|
    ansible.verbose = "" # can be set to "vvv" for verbose logging.
    ansible.playbook = "playbook/playbook.yml"
    ansible.sudo = true
  end
end


