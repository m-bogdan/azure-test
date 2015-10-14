# HA CLuster Setup for PAYG boxes
This is an Azure Resource Management template that deploys 2 NG Firewall boxes in an HA setup.

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

Different view for the template (but exactly the same functionality), embedded directly in Azure portal:

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fm-bogdan%2Fazure-test%2Fmaster%2Fha-scenario-marketplace%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

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
