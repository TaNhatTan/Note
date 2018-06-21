# Giới hạn 15 connect/ip tới 

iptables -I LOCALINPUT -d 103.200.23.97 -p tcp --syn --dport 6666 -m connlimit --connlimit-above 15 --connlimit-mask 32 -j DROP
