# internet-simulator

### install frr
> sudo snap install frr

### kiem tra frr status
> sudo nano /etc/frr/deamons

> sudo rm /etc/frr/frr.conf

> sudo service frr restart

> sudo service frr status

### catch package
> sudo tcpdump -i enp0s9 -envv -X (content in bytes)

> traceroute -n <ip>

### OSPF external routing table
redistribute connected - loan báo những mạng connect trực tiếp tới router
-> redistribute static/kernel - loan báo những mạng ko connect trực tiếp

=========================================================================

IGP (network layer) ~ RIP, OSPF,...
BGP (app layer)
	routing by policy, between AS

Tier 1 networks = core backbone routers

2 admin cua 2 router bgp (thuoc 2 AS khac nhau) khai bao neighbor voi nhau
-> Cau hinh dia chi IP (static routing)

BGPs inside a AS -> routing su dung IGP de 2 BGP tim thay nhau trong cung 1 AS

khi loan bao (export) 1 network tren BGP -> ko can connect truc tiep network do voi BGP
khai bao export: 10.0.0.0/8
