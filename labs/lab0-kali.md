
┌──(sakib㉿Sakib)-[~]
└─$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute 
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 00:0c:29:95:d5:4d brd ff:ff:ff:ff:ff:ff
    inet 192.168.135.128/24 brd 192.168.135.255 scope global dynamic noprefixroute eth0
       valid_lft 1729sec preferred_lft 1729sec
    inet6 fe80::20c:29ff:fe95:d54d/64 scope link noprefixroute 
       valid_lft forever preferred_lft forever

┌──(sakib㉿Sakib)-[~]
└─$ ping -c 4 8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=128 time=29.0 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=128 time=27.7 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=128 time=27.6 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=128 time=27.0 ms

--- 8.8.8.8 ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3006ms
rtt min/avg/max/mdev = 27.038/27.839/29.031/0.731 ms
