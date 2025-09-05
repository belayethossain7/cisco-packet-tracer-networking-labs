### **Dynamic Host Configuration Protocol**



#### CLI command in Router for for Automatic assigning IP by using DHCP



* router CLI
* en--------enable router
* conf t -----go to configuration mode for configuration
* ip dhcp pool r4 ------ pooling for dhcp,, do pooling using DHCP, pool name r4(router name)
* net 192.168.1.0 255.255.255.0------give network ip with subnet mask which network under this router.
* default-router 192.168.1.1-----provide first ip as the gateway of this network.
* dns-server 192.168.1.2----provide dns server ip of this network



#### now set the gateway ip in the gateway port in router



* ex------exit and go to config mode
* int f0/0----- now go to interface or enter the port number,,this port set gateway
* ip add 192.168.1.1 255.255.255.0----set the gateway ip in gateway f0/0 port.
* no shut-----port on or line up



#### now if need exclude the dns ip in end devices or pc



* go to config mode in router
* ip dhcp excluded-address 192.168.1.2------excluded the dns ip in end devices or pc.





#### if update the dns ip or change dns ip



* ip dhcp pool r1--------go to dhcp pool with the pool name which set before than
* dns 192.168.2.2----------than set this or change the dns ip
