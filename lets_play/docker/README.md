# Docker

## Escenario de pruebas

En el [Vagrantfile](./Vagrantfile) se encuentran los pasos necesarios para configurar el entorno de pruebas.

## Ejecutar

```
adawolfs:~$ vagrant up --provision && vagrant ssh
```

```
apk add cri-o
```

```
VERSION="v1.20.0"
wget https://github.com/kubernetes-sigs/cri-tools/releases/download/$VERSION/crictl-$VERSION-linux-amd64.tar.gz
sudo tar zxvf crictl-$VERSION-linux-amd64.tar.gz -C /usr/local/bin
rm -f crictl-$VERSION-linux-amd64.tar.gz
```

```
crio &> /var/log/crio &
```

```
alias crictl='crictl -r unix:///run/crio/crio.sock'
```

```
crictl pull docker.io/library/alpine:3.7
```

https://kubernetes.io/docs/tasks/debug-application-cluster/crictl/
