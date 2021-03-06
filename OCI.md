## Crear VM con Vagrant

Así vida es más facil y segura.

```
mkdir runc
cd runc
vagrant init ubuntu/groovy64
vagrant run && vagrant ssh
```

## Instalar dependencias

Ya sabes... dependencias

```
sudo apt update
sudo apt install containerd ctr skopeo umoci jq python2 -y
```

## Obtener imagen desde Docker Hub con Skopeo

Nos permite hacer varias operaciones con imagenes y repositorios

```
skopeo --insecure-policy copy docker://alpine:latest oci:alpine:latest
```

## Crear OCI bundle con umoci

Nos permite crear, manipular e interactuar con OCI Images

```
umoci unpack --image alpine:latest alpine-bundle
```

## Ejecutar contenedor utilizando runc

Nos permite ejecutar contenedores deacuerdo a la especificación OCI

```
cd alpine-bundle
runc run sh
```

## Ejecutar un contenedor utilizando containerd

```
systemctl start containerd
ctr image pull docker.io/library/nginx:latest
ctr run --rm --net-host -d docker.io/library/nginx:latest nginx
ctr run --rm  -d docker.io/library/nginx:latest nginx
```
