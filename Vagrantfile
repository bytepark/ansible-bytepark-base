# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
  config.vm.define 'ansible-bytepark-base' do |machine|
    machine.vm.box = "ubuntu/precise32"
    #machine.vm.box = "ubuntu/trusty64"

    machine.vm.provision "ansible" do |ansible|
      ansible.playbook = "tests/test.yml"
      ansible.sudo = true
      ansible.verbose = ENV['ANSIBLE_VERBOSE'] ||= "v"
      ansible.tags = ENV['ANSIBLE_TAGS'] ||= "all"
    end
  end
end
