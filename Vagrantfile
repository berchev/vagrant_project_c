Vagrant.configure("2") do |config|
  (1..2).each do |i|
    config.vm.define vm_name="web0#{i}" do |node|
      node.vm.box = "berchev/nginx64"
      node.vm.hostname = vm_name
    end
  end

  config.vm.define vm_name="mysql" do |node|
    node.vm.box = "berchev/mysql64"
    node.vm.hostname = vm_name
  end 
 
end



