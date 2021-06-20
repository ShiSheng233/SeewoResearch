# 网络接口 「IOT」

**待补充**

在 控制面板->网络连接 中可以看到该网络接口

该接口的网关是校内网中一台部署了OpenWrt + LUCI的服务器 ~~大概是希沃提供的已经部署好的~~ ，意义不明

~~校信息老师说这是希沃尚未开发完成的模块，他们也不知道有什么用~~

Zenmap扫描结果如下 (配置为:Intense scan plus UDP)   
*隐去了部分信息*

```
Nmap scan report for *.*.*.*

Host is up (0.000098s latency).

Not shown: 1980 closed ports

PORT      STATE         SERVICE       VERSION

22/tcp    open          ssh           Dropbear sshd 2015.67 (protocol 2.0)

53/tcp    open          domain        dnsmasq 2.73

80/tcp    open          http          LuCI Lua http config

| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Site doesn't have a title (text/html).

443/tcp   open          ssl/http      LuCI Lua http config

| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-title: Site doesn't have a title (text/html).
| ssl-cert: Subject: organizationName=CVTE/stateOrProvinceName=Guangdong/countryName=CN
| Issuer: organizationName=CVTE/stateOrProvinceName=Guangdong/countryName=CN
| Public Key type: rsa
| Public Key bits: 1024
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2020-04-01T07:27:07
| Not valid after:  2120-03-08T07:27:07
| MD5:   6369 689f f9b5 5fd1 7dbf 75cb f226 3279
|_SHA-1: 2e18 edcb 12d9 1741 7331 70cd e742 740b a293 fe30
|_ssl-date: 2020-06-08T13:06:34+00:00; -1y10d15h24m23s from scanner time.

53/udp    open          domain        dnsmasq 2.73

| dns-nsid: 
|_  bind.version: dnsmasq-2.73

67/udp    open          dhcps?

686/udp   open|filtered hcp-wismar

1101/udp  open|filtered pt2-discover

1993/udp  open|filtered snmp-tcp-port

2049/udp  open|filtered nfs

10000/udp open|filtered ndmp

16573/udp open|filtered unknown

16680/udp open|filtered unknown

16896/udp open|filtered unknown

19283/udp open|filtered keysrvr

20004/udp open|filtered unknown

20449/udp open|filtered unknown

21834/udp open|filtered unknown

49640/udp open|filtered unknown

62958/udp open|filtered unknown

MAC Address: **:**:**:**:**:** (Ralink Technology)

Device type: WAP

Running: Linux 3.X

OS CPE: cpe:/o:linux:linux_kernel:3.10

OS details: OpenWrt Barrier Breaker (Linux 3.10)

Uptime guess: 0.217 days (since Sat Jun 19 07:18:05 2021)

Network Distance: 1 hop

TCP Sequence Prediction: Difficulty=251 (Good luck!)

IP ID Sequence Generation: All zeros

Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel


Host script results:

|_clock-skew: -375d15h24m23s

TRACEROUTE

HOP RTT     ADDRESS

1   0.10 ms *.*.*.*

NSE: Script Post-scanning.
Initiating NSE at 12:30
Completed NSE at 12:30, 0.00s elapsed
Initiating NSE at 12:30
Completed NSE at 12:30, 0.00s elapsed
Initiating NSE at 12:30
Completed NSE at 12:30, 0.00s elapsed


Nmap done: 1 IP address (1 host up) scanned in 1292.62 seconds

           Raw packets sent: 2434 (111.414KB) | Rcvd: 3224 (215.055KB)
```

![Zenmap Scan Result](img\ZenmapResult.png)