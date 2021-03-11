# PODMAN

Podman es un container engine que no require de un daemon utilizado para crear, manejar y ejecutar OCI Containers en un sistema Linux. Permite ejecutar contenedores tanto en modo root como rootless. Es tan simple como escribir `alias docker=podman`

## CRUN

Por default podman hace uso de crun, un OCI Rutime escrito en C. Aparte de eso no tiene nada en especial.

## Escenario de pruebas

En el [Vagrantfile](./Vagrantfile) se encuentran los pasos necesarios para configurar el entorno de pruebas.

## Ejecutar

```
adawolfs:~$ vagrant up --provision && vagrant ssh
```
