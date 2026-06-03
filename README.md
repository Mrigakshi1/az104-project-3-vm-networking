## AZ-104 Lab: Deploy and Secure an Azure Virtual Machine

## Objective

This lab demonstrates how to deploy a Windows Server 2022 virtual machine in Microsoft Azure, configure networking components, secure access using a Network Security Group (NSG), and validate connectivity using Remote Desktop Protocol (RDP).

## Architecture

Internet → Public IP → NSG → VNet → Subnet → Windows VM

## Resource Group

Created a resource group to organize all Azure resources used in this lab.

![Resource Group](screenshots/01-resource-group.png)

## Virtual Network

The Virtual Network (VNet) was created to provide network connectivity for Azure resources.

![VNet Overview](screenshots/02-vnet.png)

## Subnet

A subnet was created within the VNet to logically segment network resources.

![Subnet Configuration](screenshots/03-vnet-subnet.png)

## Virtual Machine

Deployed a Windows Server 2022 Datacenter virtual machine.

![VM Overview](screenshots/04-vm-overview.png)

## Network Security Group

Created and associated a custom NSG with the VM network interface.

![NSG](screenshots/05-nsg-overview.png)

## Inbound Security Rule

Configured an inbound RDP rule allowing TCP port 3389.

![RDP Rule](screenshots/06-rdp-rule.png)

## NSG Association

The custom Network Security Group (nsg-demo1) was associated with the virtual machine's network interface to enforce inbound and outbound traffic rules.

![NSG Association](screenshots/07-nic-association.png)

## Connectivity Test

Successfully connected to the VM using Remote Desktop Protocol (RDP).

![RDP Success](screenshots/08-rdp-success.png)

## Skills Demonstrated

* Azure Resource Groups
* Azure Virtual Networks
* Azure Subnets
* Azure Virtual Machines
* Network Security Groups
* RDP Connectivity
* Azure Networking
* Infrastructure as a Service (IaaS)

## Conclusion

Successfully deployed and secured a Windows Server 2022 virtual machine in Azure. Verified network connectivity and remote administration using a custom Network Security Group and RDP access.



