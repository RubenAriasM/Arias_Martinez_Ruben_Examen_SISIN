
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/xenial64"

  config.vm.provision "shell", inline: <<-SHELL
  echo "-- Insertar datos de ejemplo en la tabla 'menu'" > /home/vagrant/datos_menu.sql
  SHELL
end
