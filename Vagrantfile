# -*- mode: ruby -*-
# vi: set ft=ruby :


VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "ubuntu/vivid64"
  config.vm.box_url = "https://atlas.hashicorp.com/ubuntu/vivid64"
  config.vm.hostname = "vnext"
  config.vm.network :forwarded_port, guest: 3002, host: 3002
  config.ssh.forward_agent = true

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
  end

end