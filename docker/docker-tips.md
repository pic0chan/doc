docker run -v のコマンド
ホストのデバイスが見える

```bash
$ docker run -it -v /home/test:/home/aaa/test --name mysqltest sakai-yasu/mysql:5.6 /bin/bash
```

```bash
root@1ff07c20e2d5:/home/aaa/test# df -h
Filesystem               Size  Used Avail Use% Mounted on
overlay                   41G  9.0G   33G  22% /
tmpfs                    3.9G     0  3.9G   0% /dev
tmpfs                    3.9G     0  3.9G   0% /sys/fs/cgroup
/dev/mapper/centos-root   41G  9.0G   33G  22% /etc/hosts
shm                       64M     0   64M   0% /dev/shm
/dev/mapper/centos-home   20G  5.4G   15G  27% /home/aaa/test
tmpfs                    3.9G     0  3.9G   0% /proc/scsi
tmpfs                    3.9G     0  3.9G   0% /sys/firmware
root@1ff07c20e2d5:/
```


