```
service cgroups start
apk add containerd
containerd &> /var/log/containerd.log &
ctr i pull docker.io/library/alpine:3.10
ctr run --rm -d docker.io/library/alpine:3.10 alpine
ctr c list
ctr c info alpine | less
ctr t exec -t --exec-id alpine alpine sh
ctr t attach alpine
ctr c rm alpine
```
