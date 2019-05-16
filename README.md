# Projecte_18

Axel Verdugo y Nilson Issaoui

## Instalación

Pasos a seguir:

```
mkdir vagrant
cd ./vagrant
vagrant init

```

## Vagrantfile

```
Vagrant.configure("2") do |config|
#Elegimos versión Ubuntu
    config.vm.box = "ubuntu/xenial64"
    config.vm.provider "virtualbox" do |vb|
#Habilitamos la interfaz gráfica
        vb.gui = true
#Nombre de la máquina
        vb.name = "UbuntuServer"
#La memoria RAM que quremos
        vb.memory = "2048"
    end 
#Nombre de la máquina
    config.vm.hostname = "lamp"
#Hacemos la red privada y que nos asigne una IP aleatoria
    config.vm.network "private_network", type: "dhcp"
end

```

## Script 

```


```

## Ejecutar vagrant

Ejecutamos el comando vagrant up para inicializar la máquina virtual.
