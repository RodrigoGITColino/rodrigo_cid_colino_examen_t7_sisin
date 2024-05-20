# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"

  config.vm.provision "shell", inline: <<-SHELL

      echo "INSERT INTO gestion_restaurante.menu (nombre, descripcion, precio, categoria)" > /home/vagrant/datos_menu.sql
      echo "VALUES ('Ensalada', 'Ensalada simple', 2.50, 'Primero')," >> /home/vagrant/datos_menu.sql
      echo " ('Solomillo', 'Solomillo de cerdo', 7.99, 'Segundo')," >> /home/vagrant/datos_menu.sql
      echo " ('Helado', 'Helado de vainilla', 1.00, 'Postre')" >> /home/vagrant/datos_menu.sql

   SHELL
end
