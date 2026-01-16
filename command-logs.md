khair_ubunt@KHAIRUL-Hp:~$ ls
health.sh  hello.txt  link-practise  newfile.sh  permission  text.txt  zip-practise
khair_ubunt@KHAIRUL-Hp:~$
khair_ubunt@KHAIRUL-Hp:~$ pwd
/home/khair_ubunt
khair_ubunt@KHAIRUL-Hp:~$ cd ..
khair_ubunt@KHAIRUL-Hp:/home$ ld
ld: no input files
khair_ubunt@KHAIRUL-Hp:/home$ ls
jethalal  khair_ubunt
khair_ubunt@KHAIRUL-Hp:/home$ cd khair_ubunt
khair_ubunt@KHAIRUL-Hp:~$ ls
health.sh  hello.txt  link-practise  newfile.sh  permission  text.txt  zip-practise
khair_ubunt@KHAIRUL-Hp:~$ mkdir
mkdir: missing operand
Try 'mkdir --help' for more information.
khair_ubunt@KHAIRUL-Hp:~$ mkdir devops-task-1
khair_ubunt@KHAIRUL-Hp:~$ cd devops-task-1
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -a
.  ..
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ vim hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls
hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -a
.  ..  hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ cat hello.txt
Hello elevate team this is my fist text file
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -l
total 4
-rw-r--r-- 1 khair_ubunt khair_ubunt 46 Jan 15 07:28 hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ touch newfile.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls
hello.txt  newfile.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ rm newfile.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls
hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ vim hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -l
total 4
-rw-r--r-- 1 khair_ubunt khair_ubunt 46 Jan 15 07:28 hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ chmod 777 hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -l
total 4
-rwxrwxrwx 1 khair_ubunt khair_ubunt 46 Jan 15 07:28 hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ chown ravi hello.txt
chown: invalid user: ‘ravi’
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ cat /etc/passwd
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
irc:x:39:39:ircd:/run/ircd:/usr/sbin/nologin
_apt:x:42:65534::/nonexistent:/usr/sbin/nologin
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
systemd-network:x:998:998:systemd Network Management:/:/usr/sbin/nologin
systemd-timesync:x:996:996:systemd Time Synchronization:/:/usr/sbin/nologin
dhcpcd:x:100:65534:DHCP Client Daemon,,,:/usr/lib/dhcpcd:/bin/false
messagebus:x:101:101::/nonexistent:/usr/sbin/nologin
syslog:x:102:102::/nonexistent:/usr/sbin/nologin
systemd-resolve:x:991:991:systemd Resolver:/:/usr/sbin/nologin
uuidd:x:103:103::/run/uuidd:/usr/sbin/nologin
landscape:x:104:105::/var/lib/landscape:/usr/sbin/nologin
polkitd:x:990:990:User for polkitd:/:/usr/sbin/nologin
khair_ubunt:x:1000:1000:,,,:/home/khair_ubunt:/bin/bash
jethalal:x:1001:1001::/home/jethalal:/bin/sh
shinchan:x:1002:1002::/home/shinchan:/bin/sh
doraeman:x:1003:1003::/home/doraeman:/bin/sh
tom:x:1004:1004::/home/tom:/bin/sh
jerry:x:1005:1005::/home/jerry:/bin/sh
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ chown tom hello.txt
chown: changing ownership of 'hello.txt': Operation not permitted
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ sudo chown tom hello.txt
[sudo] password for khair_ubunt:
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -l
total 4
-rwxrwxrwx 1 tom khair_ubunt 46 Jan 15 07:28 hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ chown :disney hello.txt
chown: invalid group: ‘:disney’
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ sudo groupadd disney
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ chown :disney hello.txt
chown: changing group of 'hello.txt': Operation not permitted
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ sudo chown :disney hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ ls -l
total 4
-rwxrwxrwx 1 tom disney 46 Jan 15 07:28 hello.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ top
top - 08:04:28 up  1:54,  1 user,  load average: 0.00, 0.00, 0.00
Tasks:  22 total,   1 running,  21 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.0 us,  0.0 sy,  0.0 ni,100.0 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
MiB Mem :   3739.2 total,   3253.0 free,    382.2 used,    177.1 buff/cache
MiB Swap:   1024.0 total,   1024.0 free,      0.0 used.   3357.0 avail Mem

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND
      1 root      20   0   21660  12512   9312 S   0.0   0.3   0:01.88 systemd
      2 root      20   0    3120   1920   1920 S   0.0   0.1   0:00.04 init-systemd(Ub
      6 root      20   0    3120   1792   1792 S   0.0   0.0   0:00.00 init
     45 root      19  -1   50352  15360  14336 S   0.0   0.4   0:00.40 systemd-journal
    102 root      20   0   25272   6400   4864 S   0.0   0.2   0:01.04 systemd-udevd
    110 systemd+  20   0   21456  12672  10496 S   0.0   0.3   0:00.17 systemd-resolve
    117 systemd+  20   0   91024   7680   6784 S   0.0   0.2   0:00.15 systemd-timesyn
    158 root      20   0    4236   2560   2432 S   0.0   0.1   0:00.02 cron
    159 message+  20   0    9624   5120   4608 S   0.0   0.1   0:00.09 dbus-daemon
    172 root      20   0   17964   8448   7552 S   0.0   0.2   0:00.12 systemd-logind
    189 syslog    20   0  222508   5632   4608 S   0.0   0.1   0:00.12 rsyslogd
    199 root      20   0    3160   2048   1920 S   0.0   0.1   0:00.01 agetty
    201 root      20   0  107024  22272  13184 S   0.0   0.6   0:00.36 unattended-upgr
    206 root      20   0    3116   1920   1792 S   0.0   0.1   0:00.01 agetty
    307 root      20   0    3124    896    768 S   0.0   0.0   0:00.00 SessionLeader
    308 root      20   0    3140   1156   1024 S   0.0   0.0   0:00.08 Relay(309)
    309 khair_u+  20   0    6204   4992   3456 S   0.0   0.1   0:00.19 bash
    310 root      20   0    6688   4096   3584 S   0.0   0.1   0:00.01 login
    358 khair_u+  20   0   20304  11264   9216 S   0.0   0.3   0:00.13 systemd
    359 khair_u+  20   0   21156   3520   1792 S   0.0   0.1   0:00.00 (sd-pam)
    379 khair_u+  20   0    6072   5120   3584 S   0.0   0.1   0:00.02 bash
    930 khair_u+  20   0    9276   5504   3456 R   0.0   0.1   0:00.03 top




khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ htop
Command 'htop' not found, but can be installed with:
sudo snap install htop  # version 3.4.1, or
sudo apt  install htop  # version 3.2.2-2
See 'snap info htop' for additional versions.
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ df -h
Filesystem      Size  Used Avail Use% Mounted on
none            1.9G     0  1.9G   0% /usr/lib/modules/6.6.87.2-microsoft-standard-WSL2
none            1.9G  4.0K  1.9G   1% /mnt/wsl
drivers         238G  192G   46G  81% /usr/lib/wsl/drivers
/dev/sdd       1007G  1.8G  954G   1% /
none            1.9G  176K  1.9G   1% /mnt/wslg
none            1.9G     0  1.9G   0% /usr/lib/wsl/lib
rootfs          1.9G  2.7M  1.9G   1% /init
none            1.9G  496K  1.9G   1% /run
none            1.9G     0  1.9G   0% /run/lock
none            1.9G     0  1.9G   0% /run/shm
none            1.9G   76K  1.9G   1% /mnt/wslg/versions.txt
none            1.9G   76K  1.9G   1% /mnt/wslg/doc
C:\             238G  192G   46G  81% /mnt/c
tmpfs           374M   20K  374M   1% /run/user/1000
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$ free -m
               total        used        free      shared  buff/cache   available
Mem:            3739         368        3249           3         198        3370
Swap:           1024           0        1024
khair_ubunt@KHAIRUL-Hp:~/devops-task-1$
