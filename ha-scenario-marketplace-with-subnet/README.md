# HA CLuster Setup for PAYG boxes
This is an Azure Resource Management template that deploys 2 NG Firewall boxes in an HA setup.

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

### Template parameters: ###

| Name | Description
|:--- |:---|
|Vm Name|Name of the primary VM, an "ha" is added for the secondary box|
|Dns Name For Public IP|DNS for accessing the primary box through SSH/SPoE|
|Virtual Network Name|Name of the virtual network in which the 2 boxes are deployed|
|Address Prefix|Virtual network address range|
|Subnet1 Name||Subnet name in which the boxes are deployed|
|Gateway||IP address of gateway|
|Primary HA Box Ip|IP address of the active box|
|Secondary HA box IP|IP address of the secondary box(standby)|
|Location|Data center where the boxes are created|
|Vm Size|Size of the Azure box|
|Admin Password|Initial password for root user on both boxes|


#### Custom data ####
We also send custom data based on input parameters, and for legacy consistency, we have to
maintain not-so-good nameing for variables:
* _gateway_ : is infact the subnet
* _hexthop_ : is infact the gateway ip
