### **CLI command in Switch**



* en-----enable the switch
* sh vlan brief--------show all vlan in switch
* conf t ---------configure terminal on---for configuration terminal
* 
* vlan 11--------creating vlan with a number
* 
* name BBA ---------now give vlan name
* 
* ex------ exit command after vlan configure or creation





**now create another vlan** 



* vlan 22
* name engr
* ex
* ex-------again exait command for exit the config mode





**for showing or checking the vlan in this switch**



* show vlan brief----show all vlan with name and number



**for assigning switch port under specific vlan in switch cli command**

* en-----enable switch
* conf t----enter configure terminal
* int F0/1----interface specific switch port for set up specific vlan
* switchport mode access ---for accessing switch port
* switchport access vlan 11------set a vlan in specific this switch





**Now set 2nd switch port for a specific vlan**

* int F0/2----enter or interface this swithport for set vlan
* switchport mode access
* switchport access vlan 11
* ex----for exit



**Now set another 2 switch port in different specific vlan**

* as well as before vlan set up



### 

### 











