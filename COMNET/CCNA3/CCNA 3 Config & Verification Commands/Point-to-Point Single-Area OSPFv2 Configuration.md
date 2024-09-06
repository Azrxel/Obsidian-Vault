---
tags: []
---

---
"R1(config-router)"# = router ospf config mode

#### Configure router IDs

Start the OSPF routing process
`Router(config)# router ospf process-id`

Use the router-id command to set the OSPF IDs of routers
`Router(config-router)# router-id rid`
#### Configure Networks for OSPF Routing (Configure networks for OSPF routing using network commands and wildcard masks)

Configure the routing process on R1 with the network statements and wildcard masks that are required to activate OSPF routing for all the attached networks. The network statement values should be the network or subnet addresses of the configured networks.
`Router(config-router)# network network-address wildcard-mask area area-id`

Verify that OSPF has been configured properly by the displaying the running configuration. If you find an error, delete the network statement using the no command and reconfigure it.

#### Configure networks for OSPF routing using interface IP addresses and quad-zero masks.

On router R2, configure OSPF using network commands with the IP addresses of the interfaces and quad-zero masks. The syntax of the network command is the same as was used above.
`Router(config-router)# network network-address 0.0.0.0 area area-id`

#### Configure OSPF routing on required router interfaces
`Router(config-if)# ip ospf process-id area area-id`

#### Configure Passive Interfaces

OSPF will send its protocol traffic out of all interfaces that are participating in the OSPF process. On links that are not configured to other networks, such as LANs, this unnecessary traffic consumes resources. The passive-interface command will prevent the OSPF process from sending unnecessary routing protocol traffic out LAN interfaces.

`Router(config-router)# passive-interface interface`