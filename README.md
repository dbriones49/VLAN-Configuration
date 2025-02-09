# VLAN-Configuration



## Introduction

In this project, I am creating two VLANS using Cisco Packet Tracer. The lab focuses on configuring tow VLANS on a single switch, with two end points assigned to each VLAN, allwowing for isolated communication between the groups. This project aims to demonstrate
the fundamentals o fVLAN implementation and the role f basic networkdevices such as switches and routers in managing network traffic.

The network setup will be configured  using a command line interface to facilitate precise control over the network settings. This will enhance understanding of VLANS and their configuration process, re-inforcing the skills necessary for effective network management.

In a real world environment, utilzing VLANS to segment a newtork is crucial for enhancing security, improving performance, and simplifying network management for businesses. Proper configuration is vital, as it ensures that network segments fucntion correctly and 
securely, minimizing the risk of unauthrorized accesa dn optimizing resource allocation.


## Topology

We begin by connecting the PCs to the switch using straight through cable and connecting them to seperate ports on the switch. The router is then connected to the swith also using straight through cable




![image](https://github.com/user-attachments/assets/caae3b50-8114-4c21-85ed-de4a7647c1d4)


# Configuration

Next, static IP address, subnet masks, and gateways will be configured on the PCS. The VlANS will be known ans VLAN 10 and VLAN 20. VLAN 10 will be the top 2 PCs, and VLAN 20 will be the bottom 2 PCs.
VLAN 10 will be comprised of PC0 and PC1, and will be assigned to gateway 192.168.1.1
VLAN 20 will be comprised of PC2 and PC3, and will be assigned to gateway 192.168.2.2


![image](https://github.com/user-attachments/assets/24918b38-41f7-4465-8c9d-558fa3184e3a)



![image](https://github.com/user-attachments/assets/7a40887d-896a-41dc-bb26-d65ce37a256d)



The VLAN configuration will be completed on the switch. To begin, we type "enable", the " config terminal".   From here we can name the VLANS for there corrosponding departments.
VLAN 10 will be named "HR", and VLAN 20 will be named "IT".



![image](https://github.com/user-attachments/assets/4ba40171-f41f-4d9a-8cb0-9dafdcdce6a6)


Next, we will asisng the ports. There are two types of ports that we will use for this lab, Access ports and Trunk ports. 



























































































































