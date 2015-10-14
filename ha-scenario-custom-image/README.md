# HA CLuster Setup for PAYG boxes
This is an Azure Resource Management template that deploys 2 NG Firewall boxes in an HA setup. (with custom images)

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

Template parameters:

| Name | Description
|:--- |:---|
|Vm Name|Name of the primary VM, an "ha" is added for the secondary box|
|Dns Name For Public IP|DNS for accessing the primary box through SSH/SPoE|
|Virtual Network Name|Name of the virtual network in which the 2 boxes are deployed|
|Address Prefix|Virtual network address range|
|Subnet1 Name||Subnet name in which the boxes are deployed|
|Subnet1 Name||Subnet address range|
|Primary HA Box Ip|IP address of the active box|
|Secondary HA box IP|IP address of the secondary box(standby)|
|Location|Data center where the boxes are created|
|Vm Size|Size of the Azure box|
|Admin Password|Initial password for root user on both boxes|
|userImageVhdURI|HTTP address to custom image|
|userImageStorageAccountName|ARM storage account - must contain userImageVhdURI|
|userImageStorageContainerName|ARM container - must contain userImageVhdURI|
