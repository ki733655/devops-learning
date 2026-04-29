khair_ubunt@KHAIRUL-Hp:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet 10.255.255.254/32 brd 10.255.255.254 scope global lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1300 qdisc mq state UP group default qlen 1000
    link/ether 00:15:5d:43:17:d5 brd ff:ff:ff:ff:ff:ff
    inet 172.17.163.230/20 brd 172.17.175.255 scope global eth0
       valid_lft forever preferred_lft forever
    inet6 fe80::215:5dff:fe43:17d5/64 scope link
       valid_lft forever preferred_lft forever
khair_ubunt@KHAIRUL-Hp:~$ ipconfig
Command 'ipconfig' not found, did you mean:
  command 'ifconfig' from deb net-tools (2.10-0.1ubuntu4.4)
  command 'iwconfig' from deb wireless-tools (30~pre9-13.1ubuntu4)
  command 'iconfig' from deb ipmiutil (3.1.9-3)
  command 'hipconfig' from deb hipcc (5.2.3-12)
Try: sudo apt install <deb name>
khair_ubunt@KHAIRUL-Hp:~$ sudo apt install net-tools
[sudo] password for khair_ubunt:
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  net-tools
0 upgraded, 1 newly installed, 0 to remove and 7 not upgraded.
Need to get 204 kB of archives.
After this operation, 811 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 net-tools amd64 2.10-0.1ubuntu4.4 [204 kB]
Fetched 204 kB in 2s (101 kB/s)
Selecting previously unselected package net-tools.
(Reading database ... 40807 files and directories currently installed.)
Preparing to unpack .../net-tools_2.10-0.1ubuntu4.4_amd64.deb ...
Unpacking net-tools (2.10-0.1ubuntu4.4) ...
Setting up net-tools (2.10-0.1ubuntu4.4) ...
Processing triggers for man-db (2.12.0-4build2) ...
khair_ubunt@KHAIRUL-Hp:~$ ipconfig
Command 'ipconfig' not found, did you mean:
  command 'ifconfig' from deb net-tools (2.10-0.1ubuntu4.4)
  command 'iconfig' from deb ipmiutil (3.1.9-3)
  command 'hipconfig' from deb hipcc (5.2.3-12)
  command 'iwconfig' from deb wireless-tools (30~pre9-13.1ubuntu4)
Try: sudo apt install <deb name>
khair_ubunt@KHAIRUL-Hp:~$ ip config
Object "config" is unknown, try "ip help".
khair_ubunt@KHAIRUL-Hp:~$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1300
        inet 172.17.163.230  netmask 255.255.240.0  broadcast 172.17.175.255
        inet6 fe80::215:5dff:fe43:17d5  prefixlen 64  scopeid 0x20<link>
        ether 00:15:5d:43:17:d5  txqueuelen 1000  (Ethernet)
        RX packets 3547  bytes 6230436 (6.2 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 2413  bytes 169628 (169.6 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 159  bytes 16074 (16.0 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 159  bytes 16074 (16.0 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

khair_ubunt@KHAIRUL-Hp:~$ ping google.com
PING google.com (142.251.223.110) 56(84) bytes of data.
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=1 ttl=112 time=66.5 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=2 ttl=112 time=75.3 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=3 ttl=112 time=74.0 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=4 ttl=112 time=70.1 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=5 ttl=112 time=71.0 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=6 ttl=112 time=77.7 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=7 ttl=112 time=57.3 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=8 ttl=112 time=84.4 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=9 ttl=112 time=64.5 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=10 ttl=112 time=72.8 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=11 ttl=112 time=161 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=12 ttl=112 time=70.4 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=13 ttl=112 time=78.9 ms
64 bytes from tzdela-ar-in-f14.1e100.net (142.251.223.110): icmp_seq=14 ttl=112 time=78.0 ms
^C
--- google.com ping statistics ---
14 packets transmitted, 14 received, 0% packet loss, time 13020ms
rtt min/avg/max/mdev = 57.331/78.724/161.062/23.743 ms
khair_ubunt@KHAIRUL-Hp:~$ ss -tuln
Netid      State       Recv-Q      Send-Q            Local Address:Port             Peer Address:Port      Process
udp        UNCONN      0           0                    127.0.0.54:53                    0.0.0.0:*
udp        UNCONN      0           0                 127.0.0.53%lo:53                    0.0.0.0:*
udp        UNCONN      0           0                10.255.255.254:53                    0.0.0.0:*
udp        UNCONN      0           0                     127.0.0.1:323                   0.0.0.0:*
udp        UNCONN      0           0                         [::1]:323                      [::]:*
tcp        LISTEN      0           4096                 127.0.0.54:53                    0.0.0.0:*
tcp        LISTEN      0           4096              127.0.0.53%lo:53                    0.0.0.0:*
tcp        LISTEN      0           1000             10.255.255.254:53                    0.0.0.0:*
khair_ubunt@KHAIRUL-Hp:~$ netstat -tuln
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State
tcp        0      0 127.0.0.54:53           0.0.0.0:*               LISTEN
tcp        0      0 127.0.0.53:53           0.0.0.0:*               LISTEN
tcp        0      0 10.255.255.254:53       0.0.0.0:*               LISTEN
udp        0      0 127.0.0.54:53           0.0.0.0:*
udp        0      0 127.0.0.53:53           0.0.0.0:*
udp        0      0 10.255.255.254:53       0.0.0.0:*
udp        0      0 127.0.0.1:323           0.0.0.0:*
udp6       0      0 ::1:323                 :::*
khair_ubunt@KHAIRUL-Hp:~$ nslookup google.com
Command 'nslookup' not found, but can be installed with:
sudo apt install bind9-dnsutils
khair_ubunt@KHAIRUL-Hp:~$ sudo apt install bind9-dnsutils
[sudo] password for khair_ubunt:
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  bind9-host bind9-libs liblmdb0 libmaxminddb0 libuv1t64
Suggested packages:
  mmdb-bin
The following NEW packages will be installed:
  bind9-dnsutils bind9-host bind9-libs liblmdb0 libmaxminddb0 libuv1t64
0 upgraded, 6 newly installed, 0 to remove and 7 not upgraded.
Need to get 1633 kB of archives.
After this operation, 4664 kB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://archive.ubuntu.com/ubuntu noble/main amd64 libuv1t64 amd64 1.48.0-1.1build1 [97.3 kB]
Get:2 http://archive.ubuntu.com/ubuntu noble/main amd64 liblmdb0 amd64 0.9.31-1build1 [48.1 kB]
Get:3 http://archive.ubuntu.com/ubuntu noble/main amd64 libmaxminddb0 amd64 1.9.1-1build1 [24.4 kB]
Get:4 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 bind9-libs amd64 1:9.18.39-0ubuntu0.24.04.2 [1257 kB]
Get:5 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 bind9-host amd64 1:9.18.39-0ubuntu0.24.04.2 [50.5 kB]
Get:6 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 bind9-dnsutils amd64 1:9.18.39-0ubuntu0.24.04.2 [156 kB]
Fetched 1633 kB in 5s (357 kB/s)
Selecting previously unselected package libuv1t64:amd64.
(Reading database ... 40855 files and directories currently installed.)
Preparing to unpack .../0-libuv1t64_1.48.0-1.1build1_amd64.deb ...
Unpacking libuv1t64:amd64 (1.48.0-1.1build1) ...
Selecting previously unselected package liblmdb0:amd64.
Preparing to unpack .../1-liblmdb0_0.9.31-1build1_amd64.deb ...
Unpacking liblmdb0:amd64 (0.9.31-1build1) ...
Selecting previously unselected package libmaxminddb0:amd64.
Preparing to unpack .../2-libmaxminddb0_1.9.1-1build1_amd64.deb ...
Unpacking libmaxminddb0:amd64 (1.9.1-1build1) ...
Selecting previously unselected package bind9-libs:amd64.
Preparing to unpack .../3-bind9-libs_1%3a9.18.39-0ubuntu0.24.04.2_amd64.deb ...
Unpacking bind9-libs:amd64 (1:9.18.39-0ubuntu0.24.04.2) ...
Selecting previously unselected package bind9-host.
Preparing to unpack .../4-bind9-host_1%3a9.18.39-0ubuntu0.24.04.2_amd64.deb ...
Unpacking bind9-host (1:9.18.39-0ubuntu0.24.04.2) ...
Selecting previously unselected package bind9-dnsutils.
Preparing to unpack .../5-bind9-dnsutils_1%3a9.18.39-0ubuntu0.24.04.2_amd64.deb ...
Unpacking bind9-dnsutils (1:9.18.39-0ubuntu0.24.04.2) ...
Setting up liblmdb0:amd64 (0.9.31-1build1) ...
Setting up libmaxminddb0:amd64 (1.9.1-1build1) ...
Setting up libuv1t64:amd64 (1.48.0-1.1build1) ...
Setting up bind9-libs:amd64 (1:9.18.39-0ubuntu0.24.04.2) ...
Setting up bind9-host (1:9.18.39-0ubuntu0.24.04.2) ...
Setting up bind9-dnsutils (1:9.18.39-0ubuntu0.24.04.2) ...
Processing triggers for man-db (2.12.0-4build2) ...
Processing triggers for libc-bin (2.39-0ubuntu8.6) ...
khair_ubunt@KHAIRUL-Hp:~$ nslookup google.com
Server:         10.255.255.254
Address:        10.255.255.254#53

Non-authoritative answer:
Name:   google.com
Address: 142.250.182.238
Name:   google.com
Address: 2404:6800:4002:828::200e

khair_ubunt@KHAIRUL-Hp:~$ nslookup flipkart.com
Server:         10.255.255.254
Address:        10.255.255.254#53

Non-authoritative answer:
Name:   flipkart.com
Address: 103.243.32.90
Name:   flipkart.com
Address: 64:ff9b::67f3:205a

khair_ubunt@KHAIRUL-Hp:~$ dig google.com

; <<>> DiG 9.18.39-0ubuntu0.24.04.2-Ubuntu <<>> google.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 25514
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
;; QUESTION SECTION:
;google.com.                    IN      A

;; ANSWER SECTION:
google.com.             215     IN      A       142.250.182.238

;; Query time: 52 msec
;; SERVER: 10.255.255.254#53(10.255.255.254) (UDP)
;; WHEN: Mon Jan 19 14:20:29 UTC 2026
;; MSG SIZE  rcvd: 55

khair_ubunt@KHAIRUL-Hp:~$ traceroute google.com
Command 'traceroute' not found, but can be installed with:
sudo apt install inetutils-traceroute  # version 2:2.4-3ubuntu1, or
sudo apt install traceroute            # version 1:2.1.5-1
khair_ubunt@KHAIRUL-Hp:~$ sudo apt install traceroute
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  traceroute
0 upgraded, 1 newly installed, 0 to remove and 7 not upgraded.
Need to get 60.5 kB of archives.
After this operation, 162 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu noble/universe amd64 traceroute amd64 1:2.1.5-1 [60.5 kB]
Fetched 60.5 kB in 3s (22.3 kB/s)
Selecting previously unselected package traceroute.
(Reading database ... 40905 files and directories currently installed.)
Preparing to unpack .../traceroute_1%3a2.1.5-1_amd64.deb ...
Unpacking traceroute (1:2.1.5-1) ...
Setting up traceroute (1:2.1.5-1) ...
update-alternatives: using /usr/bin/traceroute.db to provide /usr/bin/traceroute (traceroute) in auto mode
update-alternatives: using /usr/bin/traceroute6.db to provide /usr/bin/traceroute6 (traceroute6) in auto mode
update-alternatives: using /usr/bin/lft.db to provide /usr/bin/lft (lft) in auto mode
update-alternatives: using /usr/bin/traceproto.db to provide /usr/bin/traceproto (traceproto) in auto mode
update-alternatives: using /usr/sbin/tcptraceroute.db to provide /usr/sbin/tcptraceroute (tcptraceroute) in auto mode
Processing triggers for man-db (2.12.0-4build2) ...
khair_ubunt@KHAIRUL-Hp:~$ traceroute google.com
traceroute to google.com (142.250.182.238), 30 hops max, 60 byte packets
 1  KHAIRUL-Hp.mshome.net (172.17.160.1)  1.476 ms  1.439 ms  1.422 ms
 2  172.20.10.1 (172.20.10.1)  3.297 ms  2.845 ms  4.420 ms
 3  * * *
 4  * * *
 5  * * *
 6  * * *
 7  * * *
 8  *
 * *
 9  * * *
10  * * *
11  * * *
12  * * *
13  * *
 *
14  * * *
15  * * *
16  * * *
17  * * *
18  * * *
19  * * *
20  * * *
21  * * *
22  * * *
23  * * *
24  *^C
khair_ubunt@KHAIRUL-Hp:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet 10.255.255.254/32 brd 10.255.255.254 scope global lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1300 qdisc mq state UP group default qlen 1000
    link/ether 00:15:5d:43:17:d5 brd ff:ff:ff:ff:ff:ff
    inet 172.17.163.230/20 brd 172.17.175.255 scope global eth0
       valid_lft forever preferred_lft forever
    inet6 fe80::215:5dff:fe43:17d5/64 scope link
       valid_lft forever preferred_lft forever
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=112 time=76.4 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=112 time=75.0 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=112 time=74.3 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=112 time=71.6 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=112 time=69.6 ms
64 bytes from 8.8.8.8: icmp_seq=6 ttl=112 time=68.7 ms
^C
--- 8.8.8.8 ping statistics ---
6 packets transmitted, 6 received, 0% packet loss, time 5009ms
rtt min/avg/max/mdev = 68.733/72.622/76.445/2.837 ms
khair_ubunt@KHAIRUL-Hp:~$ sudo ip link set eth0 down
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
ping: connect: Network is unreachable
khair_ubunt@KHAIRUL-Hp:~$ sudo ip link set eth0 up
khair_ubunt@KHAIRUL-Hp:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet 10.255.255.254/32 brd 10.255.255.254 scope global lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1300 qdisc mq state UP group default qlen 1000
    link/ether 00:15:5d:43:17:d5 brd ff:ff:ff:ff:ff:ff
    inet 172.17.163.230/20 brd 172.17.175.255 scope global eth0
       valid_lft forever preferred_lft forever
    inet6 fe80::215:5dff:fe43:17d5/64 scope link
       valid_lft forever preferred_lft forever
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
ping: connect: Network is unreachable
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
ping: connect: Network is unreachable
khair_ubunt@KHAIRUL-Hp:~$ ip a
ping 8.8.8.8
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet 10.255.255.254/32 brd 10.255.255.254 scope global lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1300 qdisc mq state UP group default qlen 1000
    link/ether 00:15:5d:43:17:d5 brd ff:ff:ff:ff:ff:ff
    inet 172.17.163.230/20 brd 172.17.175.255 scope global eth0
       valid_lft forever preferred_lft forever
    inet6 fe80::215:5dff:fe43:17d5/64 scope link
       valid_lft forever preferred_lft forever
ping: connect: Network is unreachable
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
ping: connect: Network is unreachable
khair_ubunt@KHAIRUL-Hp:~$ ip route
172.17.160.0/20 dev eth0 proto kernel scope link src 172.17.163.230
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
ping: connect: Network is unreachable
khair_ubunt@KHAIRUL-Hp:~$ sudo dhclient eth0
sudo: dhclient: command not found
khair_ubunt@KHAIRUL-Hp:~$ sudo ip route add default via 172.17.160.1 dev eth0
khair_ubunt@KHAIRUL-Hp:~$ ping 8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=112 time=69.1 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=112 time=70.1 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=112 time=76.6 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=112 time=74.9 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=112 time=72.8 ms
^C
--- 8.8.8.8 ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4006ms
rtt min/avg/max/mdev = 69.050/72.675/76.595/2.835 ms
