# KATA-CONTAINERS

https://katacontainers.io

Es un proyecto opensource que busca crear un container runtime seguro con maquinas virtuales livianas que se sientan y sean eficientes como los contenedores, pero proveyendo un fuerte aislamiento usando una tecnologia de virtualizacion de hardware como segunda linea de defensa.

## Escenario de pruebas

Para minimisar la complejidad de el test, usare una imagen de ubuntu 20.10 para sacar ventaja de el paquete snap dispoinible de kata.

Para crear maquinas virtuales dentro de una maquina virtual necesitaré KVM, para ello me apoye de este post [Inception: running Vagrant inside Vagrant with KVM](https://nts.strzibny.name/inception-running-vagrant-inside-vagrant-with-kvm/) donde explican como utilizar vagrant dentro de vagrant, una configuracion muy parecida a lo que kata propone.

En el [Vagrantfile](./Vagrantfile) se encuentran los pasos necesarios para configurar el entorno de pruebas.

Para instalar y configurar kata se uso esta documetación [Kata Containers snap package](https://github.com/kata-containers/documentation/blob/master/install/snap-installation-guide.md)

Para variar un poco use podman desde `apt`

## Ejecutar

Es posible que necesites ejecutar estos comandos como root

```
root:~# vagrant up --provision && vagrant ssh
```

## Dependencias

### libvirt

Ya que el ejemplo estaba en libvirt y aun no habia tenido la oportunidad de experimentar con ese virtualizador y aun más importante no queria invertir tiempo en buscar como hacerlo con virtualbox; me decidí a instalar el paquete.

```
adawolfs:~$ sudo apt install libvirt-daemon-system -y
```
