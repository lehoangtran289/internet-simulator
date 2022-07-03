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
