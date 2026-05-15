
# NET731 Week 9 Practical – Azure Environment Documentation

Tristan Piek

20240476



## Diagram of Architecture




![Architecture Diagram](Diagram/architecture-diagram.png)




## Introduction to the Environment

### In Azure, workloads and practical deployments are partitioned using the many resource groups that make up the environment. Principal Azure services that have been deployed are:

VNets, or virtual networks.

Virtual Machines for Linux.

Group for Network Security (NSG).

Azure Health Check.

Workspaces in Log Analytics


### This setup, which showcases fundamental ideas in cloud networking and infrastructure, is live in the North Azure region of South Africa. At the heart of the implementation are:

An overview of segmenting networks

Implementing a secure infrastructure

Analysis and monitoring

Oversight of shared cloud resources




## Resource Group Order

Azure resources were grouped by workload and deployment stage using Resource Groups.

| Resource Group | Purpose |
|---|---|
| NET731-Week3 | Networking practical resources |
| NET731-Week6 | Virtual machine deployment resources |
| TechBridge-Solutions-SA-TP | Simulated business environment |
| NetworkWatcherRG | Azure network diagnostics |
| MA_defaultazuremonitorworksp | Monitoring workspace resources |


Resource lifecycle management is made easier and operational visibility is improved with this framework.



## Network Infrastructure 

Multiple Virtual Networks (VNets) provide secure resource connectivity in Azure. VNet-Week3, VM-Week6, and TechBridge-Solutions-SA-VNet are implemented.

These networks separated workloads and improved environment network organization. VNet separation isolates resources and manages service communication, increasing security. The network design shows cloud networking
features like private communication, workload segregation, and structured infrastructure deployment.


## Infrastructure for Virtual Machines

The practical environment included two Linux virtual machines, VM-Week6 and Week6-VM. The two VMs are using the cost-effective Standard B2ts v2 size, which is great for small workloads and classrooms.

Practicals in networking, Linux administration, and cloud administration were all conducted on the virtual machines. Network Security Groups were used to regulate traffic and increase security when they were installed
within Azure Virtual Networks.




## Security Configuration

Network Security Groups (NSGs) were used to manage and filter network traffic to the virtual machines.


| NSG Name | Purpose |
|---|---|
| VM-Week3-nsg | VM traffic filtering |
| VM-Week6-nsg | VM network protection |
| TechBridge-Solutions-NSG | Business environment security |


The NSGs help protect the environment by limiting unnecessary access and improving network security.



## Monitoring as well as Recording 


The Azure Monitor and Log Analytics Workspace provides the means by which monitoring and diagnostics are carried out. Keeping an Eye on the Resource Target aswell as performance monitoring provided by Azure Monitor
defaultworkspace-914ac7fd Centralised log aggregation via Azure Monitor


Troubleshooting is made easier with the assistance of these services, which also provide visibility into the environment. By utilising B-series virtual machines and deallocating virtual machines that are not in use when
they are not required, the environment was designed in a manner that was both cost-effective and efficient. However Azure managed storage was used automatically for virtual machine discs and monitoring services. This was
accomplished without the deployment of a dedicated Storage Account.



## Challenges That Were Encountered

Among the difficulties encountered during deployment were the following:

Gain an understanding of Azure Networking.
Ensure that NSGs are configured correctly.
Dealing with a Number of Different Resource Groups
An overview of the monitoring tools for Azure


Through the completion of these challenges, abilities in practical cloud management were developed.



### Recommendations 

Improvements in the future could include the incorporation of  Accounts for Azure Storage Configuration of backups that are automated.Monitoring alarms could be improved. Azure Bastion is being deployed.  Activating services that use HTTPS
