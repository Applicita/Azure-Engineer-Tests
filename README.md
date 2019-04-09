# Technical Test - Platform Engineer - Azure

## General Description

Complete the following Stories by updating the ARM Template provided. 

## Task requirements

- All stories to be completed with an appropriate level of testing.
- Please don't spend too long on it, 60 minutes at most.

## Extra Credit

TODO: Should we add something here @Adam

## Task Stories

### Task 1 - Add a second subnet

I want to add a second subnet called 'frontend' with a network mask of 255.255.255.240. The VM needs to be deployed into this subnet. A Network Security Group also needs to be applied to allow ports 3389 and 80.  

#### Acceptance criteria

- A new subnet called frontend is created with a subnet mask of 255.255.255.240
- The VM deploys into this new subnet.
- The Network Security Group is assoicated to the frontend subnet and allows ports 3389 and 80. 

---

### Task 2 - A new virtual network

I want to create a new Virtual Network in West US and create a peer this two the original Virtual Network.

#### Acceptance criteria

- The new Virtual Network should be peered to the original Virtual Network. 
- The Original Virtual Network should be peered to the new Virtual Network. 
- The Peering should only allow Virtual Network Access. 

---

### Task 3 - Add Log Analytics

I want to deploy a log analytics workspace and install the monitoring agent onto the VM. The Log Analytics template must be deployed as a linked template. The Log Analytics data sources must be configured to collect the
System and Application Windows Event Logs. 

#### Acceptance criteria

- The Log Analytics Workspace must be deployed in the same resource group. 
- The Log Analytics Workspace must be deployed as a linked template.
- The Log Analytics Workspace must be configured to collect the System and Application Event Logs. 
- The monitoring agent must be connected to the Log Analytics worksapce.

---