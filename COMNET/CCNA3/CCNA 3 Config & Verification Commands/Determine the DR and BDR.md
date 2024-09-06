---
tags: []
---

---
#### Verify the current OSPF neighbor states
Use the appropriate command on each router to examine the current DR and BDR. If a router shows FULL/DROTHER it means that the router is not a DR or a BDR.

`show ip ospf neighbor`

```
RA# show ip ospf neighbor
Neighbor ID Pri State Dead Time Address Interface
192.168.31.33 2 FULL/DR 00:00:35 192.168.1.3 GigabitEthernet0/0
192.168.31.22 1 FULL/BDR 00:00:35 192.168.1.2 GigabitEthernet0/0
```

```
RB# show ip ospf neighbor
Neighbor ID Pri State Dead Time Address Interface
192.168.31.11 1 FULL/DROTHER 00:00:36 192.168.1.1 GigabitEthernet0/0
192.168.31.33 2 FULL/DR 00:00:36 192.168.1.3 GigabitEthernet0/0
```
 

```
RC# show ip ospf neighbor
Neighbor ID Pri State Dead Time Address Interface
192.168.31.11 1 FULL/DROTHER 00:00:39 192.168.1.1 GigabitEthernet0/0
192.168.31.22 1 FULL/BDR 00:00:38 192.168.1.2 GigabitEthernet0/0
```

##### Turn on IP OSPF adjacency debugging.
You can monitor the DR and BDR election process with a **debug** command. On **RA** and **RB,** enter the following command.