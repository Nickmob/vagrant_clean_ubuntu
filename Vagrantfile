Vagrant.configure(2) do |config|

    N = 2
    (1..N).each do |i|
      config.vm.define "host#{i}" do |node|
        node.vm.box = "ubuntu/jammy64"
        node.vm.synced_folder ".", "/vagrant"
        node.vm.hostname = "host#{i}"
        node.vm.network "private_network", ip:"10.0.26.1#{i}"
        node.vm.provider "virtualbox" do |vb|
          vb.memory = "1024"
          vb.name = "host#{i}"
          vb.cpus = 2
        end
      end
    end
 
end