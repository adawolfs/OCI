# CONTAINERD

## Escenario de pruebas

En el [Vagrantfile](./Vagrantfile) se encuentran los pasos necesarios para configurar el entorno de pruebas.

## Ejecutar

```
adawolfs:~$ vagrant up --provision && vagrant ssh
```

##

```
/run/containerd/io.containerd.runtime.v2.task/default/alpine/rootfs/root/
```

## Comandos

```
sudo -i
apk add containerd
containerd &> /var/log/containerd &
ctr image pull docker.io/library/alpine:3.7
ctr container run --rm --tty docker.io/library/alpine:3.7 alpine sh
```

Para más información:

```
ctr --help
```
