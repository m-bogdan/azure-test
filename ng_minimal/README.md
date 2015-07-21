# ng_minimal
simple ng deployment

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

The source VHD must be on a v2 storage container.
The disk attached to the new virtual machine will be created in bmstoragex storage, container bm-vhd.

| Name | Description
|:--- |:---|
|vmName | Name of the primary VM, an "ha" is added for the secondary box|
|adminPassword| Initial password for root user on both boxes|
