
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/xenial64"

  config.vm.provision "shell", inline: <<-SHELL
  echo "-- Insertar datos de ejemplo en la tabla 'menu'" > /home/vagrant/datos_menu.sql
  echo "INSERT INTO datos_menu.menu (nombre, descripcion, precio, categoria) VALUES" >> /home/vagrant/datos_menu.sql

  echo "('Caviar', 'Descripcion...', 100.5, 'Entrante')" >> /home/vagrant/datos_menu.sql
  echo "('Croquetas', 'Descripción...', 10.5, 'Entrante')" >> /home/vagrant/datos_menu.sql
  echo "('Gambas', 'Descripción...', 13.5, 'Entrante')" >> /home/vagrant/datos_menu.sql

  echo "('Lasaña', 'Descripción...', 15.5, 'Plato principal')" >> /home/vagrant/datos_menu.sql
  echo "('Cachopo', 'Descripción...', 15.5, 'Plato principal')" >> /home/vagrant/datos_menu.sql
  echo "('Merluza', 'Descripción...', 15.5, 'Plato principal')" >> /home/vagrant/datos_menu.sql

  echo "('Tarta de queso', 'Descripción...', 8.5, 'Postre')" >> /home/vagrant/datos_menu.sql
  echo "('Tarta de chocolate', 'Descripción...', 8.5, 'Postre')" >> /home/vagrant/datos_menu.sql
  echo "('Helado', 'Descripción...', 8.5, 'Postre')" >> /home/vagrant/datos_menu.sql
  SHELL
end
