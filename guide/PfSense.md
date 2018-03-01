#pfSense

https://www.pfsense.org/download/

###Virtual Box
BSD, FreeBSD (64 bit) 
1GB Ram, 20GB Storage
#####Network
1. Adapter 1<br>
	Bridged Adapter<br>
	Advanced<br>
	Allow VMs<br>
2. Adapter 2<br>
	Internal Network<br>
	Advanced<br>
	Allow VMs<br>


The system has started:<br>
1<br>
n<br>
em0<br>
em1<br>
Enter<br>
y<br>
WAN (wan -> em0)<br>
LAN (lan -> em1)<br>

#####Some Use Full Command
ipconfig<br>
ipconfig /release<br>
ipconfig /renew<br>

Default Web Address : 192.168.1.1<br>
In Other machine open web browser, go to this link -> Advanced -> Add Exception<br>
######Username = admi, Password = pfsense<br>
######Domain = Domain of yor company<br>
######Primary DNS Server = 8.8.8.8<br>
######Secondary DNS Server = 8.8.4.4<br>
######Timezone = America/Florida or Texas<br>
######Selected Type = static
######Ip Address = Given Static IP
######Subnet Mask = 24
######Upstream Gateway = Router Ip Address
######LAN IP address (In case no VPN) = 192.168.1.1
######Lan IP address (in case you have VPN) = 192.168.102.1


######New pfSense url address = 192.168.102.1


Always Block not reject
Use Reject in your private subnet

####Rule Are evaluated in following orders:
1. NAT rules
2. Service Rules
3. Floating Rules - Can match traffic in multiple directions and across multiple interfaces
4. Interface Group rules + VPN rules

###Firewall

####Aliases
Use Name instead of IP

####Schedules
Specify Time range and date range, the rule will be disabled when it is out of time frame.

####Rules
Reload the page to make them alive
 
