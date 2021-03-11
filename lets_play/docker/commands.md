```
    1  ls
    2  cat /etc/hostname
    3  git status
    4  git add /
    5  git commit -m "first start"
    6  git status
    7  git search docker
    8  apk search docker
    9  apk add docker
   10  docker ps
   11  df -h
   12  git status
   13  vim /git_size
   14  git add /
   15  git commit -m "apk add docker"
   16  git log
   17  chmod +x /git_size
   18  /git_size  5966c9fbc3374fac5808a366a81af6155bcae05c
   19  ls
   20  docker ps
   21  dockerd &> /var/log/dockerd.log
   22  cat /var/log/dockerd.log
   23  dockerd
   24  service cgroups start
   25  dockerd
   26  dockerd &> /var/log/dockerd.log &
   27  docker ps
   28  ps -fea
   29  pkill dockerd
   30  ps -fea
   31  service docker stop
   32  service docker start
   33  ps -fea
   34  docker ps
   35  docker run -d alpine:3.10 bash
   36  docker run -d alpine:3.10 sh
   37  docker ps
   38  docker ps -a
   39  ps -fea
   40  ctr
   41  ctr c list
   42  ps
   43  ctr
   44  alias ctr=ctr -a /var/run/docker/containerd/containerd.toml
   45  alias ctr='ctr -a /var/run/docker/containerd/containerd.toml'
   46  ctr
   47  ctr c ls
   48  ls /var/run/docker/containerd/containerd.toml
   49  cat /var/run/docker/containerd/containerd.toml
   50  alias ctr='ctr -a /var/run/docker/containerd/containerd.sock'
   51  ctr c ls
   52  ctr n
   53  ctr n ls
   54  ctr ns ls
   55  ctr ns --help
   56  ctr ns ls moby
   57  ctr c -n moby ls
   58  ctr
   59  ctr c
   60  ctr c ls
   61  ctr c ls --help
   62  ctr
   63  ctr -n moby c ls
   64  ctr -n mxoby c ls
   65  ctr -n moby c ls
   66  ocker ps
   67  docker ps
   68  docker ps -a
   69  git status
   70  ls /var/lib/docker/volumes/
   71  ls /var/lib/docker/**/**
   72  docker ps -a
   73  docker run --name alpine-null -d alpine:3.10 tail -f /dev/null
   74  docker ps
   75  ctr -n moby c ls
   76  ps
   77  git status
   78  docker stop alpine
   79  docker ps
   80  docker stop alpine-null
   81  docker ps
   82  docker rm $(docker ps -q)
   83  docker ps
   84  docker rm $(docker ps -aq)
   85  docker ps -a
   86  docker run --name alpine-null -ti --rm alpine:3.10 sh
   87  docker ps -a
   88  git status
   89  git add /
   90  git status
   91  git commit -m "docker pull"
   92  git status
   93  docker run --name alpine-null -d alpine:3.10 tail -f /dev/null
   94  git status
   95  docker ps
   96  docker run --name alpine-null2 -d alpine:3.10 tail -f /dev/null
   97  git status
   98  ls /var/lib/docker/overlay2/l/7DE3SUJLZ3CMTHM57SFBV3U7V5
   99  ls /var/lib/docker/overlay2/l/7DE3SUJLZ3CMTHM57SFBV3U7V5/
  100  git status
  101  ls /var/lib/docker/overlay2/0bf8f87c362550eebe9159fd05716d45c77e609839468319b45e14423a613de3-init/work/work/#55
  102  docker ps
  103  ls
  104  git status
  105  git add /
  106  git commit -m "docker run"
  107  ls
  108  docker ps
  109  docker --help
  110  docker exec --help
  111  docker exec -it alpine-null sh
  112  docker ps
  113  git status
  114  history
```
