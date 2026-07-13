student@programming-lab:~$ ping google.com
PING google.com (192.178.174.100) 56(84) bytes of data.
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=1 ttl=112 time=34.5 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=2 ttl=112 time=34.7 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=3 ttl=112 time=35.0 ms
^C
--- google.com ping statistics ---
3 packets transmitted, 3 received, 0% packet loss, time 2004ms
rtt min/avg/max/mdev = 34.466/34.714/34.990/0.214 ms
student@programming-lab:~$ man ping
student@programming-lab:~$ ping -c 4 google.com
PING google.com (192.178.174.100) 56(84) bytes of data.
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=1 ttl=112 time=34.7 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=2 ttl=112 time=34.5 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=3 ttl=112 time=34.5 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=4 ttl=112 time=34.4 ms

--- google.com ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3005ms
rtt min/avg/max/mdev = 34.400/34.512/34.659/0.097 ms
student@programming-lab:~$ ping -c  google.com
ping: invalid argument: 'google.com'
student@programming-lab:~$ ping -c 6.6.6.6
ping: invalid argument: '6.6.6.6'
student@programming-lab:~$ ping -c 8.8.8.8
ping: invalid argument: '8.8.8.8'
student@programming-lab:~$ ping  8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=117 time=17.6 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=117 time=17.7 ms
64 bytes from 8.8.8.8: icmp_seq=6 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=7 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=8 ttl=117 time=17.7 ms
^C
--- 8.8.8.8 ping statistics ---
8 packets transmitted, 8 received, 0% packet loss, time 7011ms
rtt min/avg/max/mdev = 17.452/17.556/17.710/0.091 ms
student@programming-lab:~$ ping tesla.com
PING tesla.com (2.18.53.207) 56(84) bytes of data.
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=1 ttl=54 time=327 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=2 ttl=54 time=152 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=3 ttl=54 time=150 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=4 ttl=54 time=142 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=5 ttl=54 time=141 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=6 ttl=54 time=140 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=7 ttl=54 time=143 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=8 ttl=54 time=140 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=9 ttl=54 time=138 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=10 ttl=54 time=139 ms
64 bytes from a2-18-53-207.deploy.static.akamaitechnologies.com (2.18.53.207): icmp_seq=11 ttl=54 time=141 ms
^C
--- tesla.com ping statistics ---
11 packets transmitted, 11 received, 0% packet loss, time 10013ms
rtt min/avg/max/mdev = 137.613/159.360/326.978/53.189 ms
student@programming-lab:~$ ifconfig
enp1s0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.10.1.72  netmask 255.255.0.0  broadcast 10.10.255.255
        inet6 fe80::b27e:1e1e:30ab:f580  prefixlen 64  scopeid 0x20<link>
        ether d0:ad:08:55:ae:1c  txqueuelen 1000  (Ethernet)
        RX packets 764757  bytes 1080771326 (1.0 GB)
        RX errors 0  dropped 85  overruns 0  frame 0
        TX packets 426287  bytes 31463061 (31.4 MB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 2064  bytes 239722 (239.7 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 2064  bytes 239722 (239.7 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

student@programming-lab:~$ ping 10.10.1.72
PING 10.10.1.72 (10.10.1.72) 56(84) bytes of data.
64 bytes from 10.10.1.72: icmp_seq=1 ttl=64 time=0.024 ms
64 bytes from 10.10.1.72: icmp_seq=2 ttl=64 time=0.038 ms
64 bytes from 10.10.1.72: icmp_seq=3 ttl=64 time=0.032 ms
64 bytes from 10.10.1.72: icmp_seq=4 ttl=64 time=0.045 ms
64 bytes from 10.10.1.72: icmp_seq=5 ttl=64 time=0.019 ms
64 bytes from 10.10.1.72: icmp_seq=6 ttl=64 time=0.043 ms
64 bytes from 10.10.1.72: icmp_seq=7 ttl=64 time=0.050 ms
64 bytes from 10.10.1.72: icmp_seq=8 ttl=64 time=0.016 ms
^C
--- 10.10.1.72 ping statistics ---
8 packets transmitted, 8 received, 0% packet loss, time 7167ms
rtt min/avg/max/mdev = 0.016/0.033/0.050/0.011 ms
student@programming-lab:~$ ping 10.10.1.57
PING 10.10.1.57 (10.10.1.57) 56(84) bytes of data.
64 bytes from 10.10.1.57: icmp_seq=1 ttl=64 time=0.456 ms
64 bytes from 10.10.1.57: icmp_seq=2 ttl=64 time=0.199 ms
64 bytes from 10.10.1.57: icmp_seq=3 ttl=64 time=0.569 ms
64 bytes from 10.10.1.57: icmp_seq=4 ttl=64 time=0.574 ms
64 bytes from 10.10.1.57: icmp_seq=5 ttl=64 time=0.567 ms
64 bytes from 10.10.1.57: icmp_seq=6 ttl=64 time=0.457 ms
64 bytes from 10.10.1.57: icmp_seq=7 ttl=64 time=0.563 ms
64 bytes from 10.10.1.57: icmp_seq=8 ttl=64 time=0.489 ms
64 bytes from 10.10.1.57: icmp_seq=9 ttl=64 time=0.553 ms
64 bytes from 10.10.1.57: icmp_seq=10 ttl=64 time=0.500 ms
64 bytes from 10.10.1.57: icmp_seq=11 ttl=64 time=0.648 ms
64 bytes from 10.10.1.57: icmp_seq=12 ttl=64 time=0.635 ms
64 bytes from 10.10.1.57: icmp_seq=13 ttl=64 time=0.552 ms
64 bytes from 10.10.1.57: icmp_seq=14 ttl=64 time=0.475 ms
64 bytes from 10.10.1.57: icmp_seq=15 ttl=64 time=0.632 ms
64 bytes from 10.10.1.57: icmp_seq=16 ttl=64 time=0.545 ms
64 bytes from 10.10.1.57: icmp_seq=17 ttl=64 time=0.201 ms
64 bytes from 10.10.1.57: icmp_seq=18 ttl=64 time=0.658 ms
64 bytes from 10.10.1.57: icmp_seq=19 ttl=64 time=0.499 ms
64 bytes from 10.10.1.57: icmp_seq=20 ttl=64 time=0.540 ms
64 bytes from 10.10.1.57: icmp_seq=21 ttl=64 time=0.610 ms
64 bytes from 10.10.1.57: icmp_seq=22 ttl=64 time=0.138 ms
64 bytes from 10.10.1.57: icmp_seq=23 ttl=64 time=0.500 ms
64 bytes from 10.10.1.57: icmp_seq=24 ttl=64 time=0.213 ms
64 bytes from 10.10.1.57: icmp_seq=25 ttl=64 time=0.574 ms
^C
--- 10.10.1.57 ping statistics ---
25 packets transmitted, 25 received, 0% packet loss, time 24614ms
rtt min/avg/max/mdev = 0.138/0.493/0.658/0.144 ms
student@programming-lab:~$ traceroute google.com
traceroute to google.com (142.250.77.110), 64 hops max
  1   10.10.1.2  0.389ms  0.186ms  0.185ms 
  2   *  *  * 
  3   *  *  * 
  4   *  *  * 
  5   *  *  * 
  6   *  *  * 
  7   *  *  * 
  8   *  *  * 
  9   *  *  * 
 10   *  *  * 
 11   *  *  * 
 12   *  * ^C
student@programming-lab:~$ mtr google.com
student@programming-lab:~$ 
student@programming-lab:~$ netstat -u
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
udp        0      0 programming-lab:bootpc  _gateway:bootps         ESTABLISHED
udp        0      0 programming-lab:bootpc  _gateway:bootps         ESTABLISHED
student@programming-lab:~$ netstat -t
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 programming-lab:47598   lb-140-82-114-25-:https ESTABLISHED
tcp        0      0 programming-lab:43144   93.243.107.34.bc.:https ESTABLISHED
student@programming-lab:~$ netstat -su 
IcmpMsg:
    InType0: 291
    InType3: 95
    InType8: 103
    InType9: 5
    InType11: 1421
    OutType0: 103
    OutType3: 96
    OutType8: 2542
Udp:
    18437 packets received
    96 packets to unknown port received
    0 packet receive errors
    11608 packets sent
    0 receive buffer errors
    0 send buffer errors
    IgnoredMulti: 1494
UdpLite:
IpExt:
    InMcastPkts: 3053
    OutMcastPkts: 89
    InBcastPkts: 1494
    InOctets: 1055802222
    OutOctets: 25935678
    InMcastOctets: 490510
    OutMcastOctets: 13742
    InBcastOctets: 567760
    InNoECTPkts: 764526
MPTcpExt:
student@programming-lab:~$ netstat -ss 
usage: netstat [-vWeenNcCF] [<Af>] -r         netstat {-V|--version|-h|--help}
       netstat [-vWnNcaeol] [<Socket> ...]
       netstat { [-vWeenNac] -i | [-cnNe] -M | -s [-6tuw] }

        -r, --route              display routing table
        -i, --interfaces         display interface table
        -g, --groups             display multicast group memberships
        -s, --statistics         display networking statistics (like SNMP)
        -M, --masquerade         display masqueraded connections

        -v, --verbose            be verbose
        -W, --wide               don't truncate IP addresses
        -n, --numeric            don't resolve names
        --numeric-hosts          don't resolve host names
        --numeric-ports          don't resolve port names
        --numeric-users          don't resolve user names
        -N, --symbolic           resolve hardware names
        -e, --extend             display other/more information
        -p, --programs           display PID/Program name for sockets
        -o, --timers             display timers
        -c, --continuous         continuous listing

        -l, --listening          display listening server sockets
        -a, --all                display all sockets (default: connected)
        -F, --fib                display Forwarding Information Base (default)
        -C, --cache              display routing cache instead of FIB
        -Z, --context            display SELinux security context for sockets

  <Socket>={-t|--tcp} {-u|--udp} {-U|--udplite} {-S|--sctp} {-w|--raw}
           {-x|--unix} --ax25 --ipx --netrom
  <AF>=Use '-6|-4' or '-A <af>' or '--<af>'; default: inet
  List of possible address families (which support routing):
    inet (DARPA Internet) inet6 (IPv6) ax25 (AMPR AX.25) 
    netrom (AMPR NET/ROM) rose (AMPR ROSE) ipx (Novell IPX) 
    ddp (Appletalk DDP) x25 (CCITT X.25) 
student@programming-lab:~$ netstat -g
IPv6/IPv4 Group Memberships
Interface       RefCnt Group
--------------- ------ ---------------------
lo              1      mdns.mcast.net
lo              1      all-systems.mcast.net
enp1s0          1      mdns.mcast.net
enp1s0          1      all-systems.mcast.net
lo              1      ff02::fb
lo              1      ip6-allnodes
lo              1      ff01::1
enp1s0          1      ff02::fb
enp1s0          1      ff02::1:ffab:f580
enp1s0          1      ip6-allnodes
enp1s0          1      ff01::1
student@programming-lab:~$ whois google.com
   Domain Name: GOOGLE.COM
   Registry Domain ID: 2138514_DOMAIN_COM-VRSN
   Registrar WHOIS Server: whois.markmonitor.com
   Registrar URL: http://www.markmonitor.com
   Updated Date: 2019-09-09T15:39:04Z
   Creation Date: 1997-09-15T04:00:00Z
   Registry Expiry Date: 2028-09-14T04:00:00Z
   Registrar: MarkMonitor Inc.
   Registrar IANA ID: 292
   Registrar Abuse Contact Email: abusecomplaints@markmonitor.com
   Registrar Abuse Contact Phone: +1.2086851750
   Domain Status: clientDeleteProhibited https://icann.org/epp#clientDeleteProhibited
   Domain Status: clientTransferProhibited https://icann.org/epp#clientTransferProhibited
   Domain Status: clientUpdateProhibited https://icann.org/epp#clientUpdateProhibited
   Domain Status: serverDeleteProhibited https://icann.org/epp#serverDeleteProhibited
   Domain Status: serverTransferProhibited https://icann.org/epp#serverTransferProhibited
   Domain Status: serverUpdateProhibited https://icann.org/epp#serverUpdateProhibited
   Name Server: NS1.GOOGLE.COM
   Name Server: NS2.GOOGLE.COM
   Name Server: NS3.GOOGLE.COM
   Name Server: NS4.GOOGLE.COM
   DNSSEC: unsigned
   URL of the ICANN Whois Inaccuracy Complaint Form: https://www.icann.org/wicf/
>>> Last update of whois database: 2026-07-13T04:28:09Z <<<

For more information on Whois status codes, please visit https://icann.org/epp

NOTICE: The expiration date displayed in this record is the date the
registrar's sponsorship of the domain name registration in the registry is
currently set to expire. This date does not necessarily reflect the expiration
date of the domain name registrant's agreement with the sponsoring
registrar.  Users may consult the sponsoring registrar's Whois database to
view the registrar's reported date of expiration for this registration.

TERMS OF USE: You are not authorized to access or query our Whois
database through the use of electronic processes that are high-volume and
automated except as reasonably necessary to register domain names or
modify existing registrations; the Data in VeriSign Global Registry
Services' ("VeriSign") Whois database is provided by VeriSign for
information purposes only, and to assist persons in obtaining information
about or related to a domain name registration record. VeriSign does not
guarantee its accuracy. By submitting a Whois query, you agree to abide
by the following terms of use: You agree that you may use this Data only
for lawful purposes and that under no circumstances will you use this Data
to: (1) allow, enable, or otherwise support the transmission of mass
unsolicited, commercial advertising or solicitations via e-mail, telephone,
or facsimile; or (2) enable high volume, automated, electronic processes
that apply to VeriSign (or its computer systems). The compilation,
repackaging, dissemination or other use of this Data is expressly
prohibited without the prior written consent of VeriSign. You agree not to
use electronic processes that are automated and high-volume to access or
query the Whois database except as reasonably necessary to register
domain names or modify existing registrations. VeriSign reserves the right
to restrict your access to the Whois database in its sole discretion to ensure
operational stability.  VeriSign may restrict or terminate your access to the
Whois database for failure to abide by these terms of use. VeriSign
reserves the right to modify these terms at any time.

The Registry database contains ONLY .COM, .NET, .EDU domains and
Registrars.
student@programming-lab:~$ nslookup google.com
Server:		127.0.0.53
Address:	127.0.0.53#53

Non-authoritative answer:
Name:	google.com
Address: 142.250.66.14
Name:	google.com
Address: 2404:6800:4007:83d::200e

student@programming-lab:~$ nslookup -6 google.com
*** Invalid option: 6
Server:		127.0.0.53
Address:	127.0.0.53#53

Non-authoritative answer:
Name:	google.com
Address: 142.250.66.14
Name:	google.com
Address: 2404:6800:4007:83d::200e

student@programming-lab:~$ nmap -p-
Starting Nmap 7.94SVN ( https://nmap.org ) at 2026-07-13 10:03 IST
WARNING: No targets were specified, so 0 hosts scanned.
Nmap done: 0 IP addresses (0 hosts up) scanned in 0.05 seconds
student@programming-lab:~$ ifconfig
enp1s0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.10.1.72  netmask 255.255.0.0  broadcast 10.10.255.255
        inet6 fe80::b27e:1e1e:30ab:f580  prefixlen 64  scopeid 0x20<link>
        ether d0:ad:08:55:ae:1c  txqueuelen 1000  (Ethernet)
        RX packets 774811  bytes 1086640507 (1.0 GB)
        RX errors 0  dropped 102  overruns 0  frame 0
        TX packets 432471  bytes 32506823 (32.5 MB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 2993  bytes 345907 (345.9 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 2993  bytes 345907 (345.9 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

student@programming-lab:~$ nmap -p- 10.10.1.72
Starting Nmap 7.94SVN ( https://nmap.org ) at 2026-07-13 10:04 IST
Nmap scan report for programming-lab (10.10.1.72)
Host is up (0.000022s latency).
All 65535 scanned ports on programming-lab (10.10.1.72) are in ignored states.
Not shown: 65535 closed tcp ports (conn-refused)

Nmap done: 1 IP address (1 host up) scanned in 1.63 seconds
student@programming-lab:~$ nmap -p60 -sV  10.10.1.72
Starting Nmap 7.94SVN ( https://nmap.org ) at 2026-07-13 10:04 IST
Nmap scan report for programming-lab (10.10.1.72)
Host is up (0.000044s latency).

PORT   STATE  SERVICE VERSION
60/tcp closed unknown

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 0.45 seconds
student@programming-lab:~$ nmap -p- 10.10.1.72
Starting Nmap 7.94SVN ( https://nmap.org ) at 2026-07-13 10:05 IST
Nmap scan report for programming-lab (10.10.1.72)
Host is up (0.000021s latency).
All 65535 scanned ports on programming-lab (10.10.1.72) are in ignored states.
Not shown: 65535 closed tcp ports (conn-refused)

Nmap done: 1 IP address (1 host up) scanned in 0.42 seconds
student@programming-lab:~$ sudo nmap -A 10.10.1.72
[sudo] password for student: 
student is not in the sudoers file.
student@programming-lab:~$ ls
CSB-59	CSE-A-59  Desktop  Documents  Downloads  fahmida  GK  lab  Music  Pictures  Public  snap  Templates  Videos
student@programming-lab:~$ cd Lab
bash: cd: Lab: No such file or directory
student@programming-lab:~$ cd lab
student@programming-lab:~/lab$ ls
student@programming-lab:~/lab$ touch lab1.md
student@programming-lab:~/lab$ student@programming-lab:~$ ping google.com
PING google.com (192.178.174.100) 56(84) bytes of data.
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=1 ttl=112 time=34.5 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=2 ttl=112 time=34.7 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=3 ttl=112 time=35.0 ms
^C
--- google.com ping statistics ---
3 packets transmitted, 3 received, 0% packet loss, time 2004ms
rtt min/avg/max/mdev = 34.466/34.714/34.990/0.214 ms
student@programming-lab:~$ man ping
student@programming-lab:~$ ping -c 4 google.com
PING google.com (192.178.174.100) 56(84) bytes of data.
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=1 ttl=112 time=34.7 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=2 ttl=112 time=34.5 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=3 ttl=112 time=34.5 ms
64 bytes from lcbomo-in-f100.1e100.net (192.178.174.100): icmp_seq=4 ttl=112 time=34.4 ms

--- google.com ping statistics ---
4 packets transmitted, 4 received, 0% packet loss, time 3005ms
rtt min/avg/max/mdev = 34.400/34.512/34.659/0.097 ms
student@programming-lab:~$ ping -c  google.com
ping: invalid argument: 'google.com'
student@programming-lab:~$ ping -c 6.6.6.6
ping: invalid argument: '6.6.6.6'
student@programming-lab:~$ ping -c 8.8.8.8
ping: invalid argument: '8.8.8.8'
student@programming-lab:~$ ping  8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=117 time=17.6 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=117 time=17.7 ms
64 bytes from 8.8.8.8: icmp_seq=6 ttl=117 time=17.5 ms
64 bytes from 8.8.8.8: icmp_seq=7 ttl=117 time=17.5 ms
PING google.com (192.178.174.100) 56(84) bytes of data. 2004ms_seq=3 ttl=112 time=35.0 msc  snap  Templates  Videosming-lab:~$ ping google.com

