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


## Configuration

Next, static IP address, subnet masks, and gateways will be configured on the PCS. The VlANS will be known ans VLAN 10 and VLAN 20. VLAN 10 will be the top 2 PCs, and VLAN 20 will be the bottom 2 PCs.
VLAN 10 will be comprised of PC0 and PC1, and will be assigned to gateway 192.168.1.1
VLAN 20 will be comprised of PC2 and PC3, and will be assigned to gateway 192.168.2.2


![image](https://github.com/user-attachments/assets/24918b38-41f7-4465-8c9d-558fa3184e3a)



![image](https://github.com/user-attachments/assets/7a40887d-896a-41dc-bb26-d65ce37a256d)



The VLAN configuration will be completed on the switch. To begin, we type "enable", the " config terminal".   From here we can name the VLANS for there corrosponding departments.
VLAN 10 will be named "HR", and VLAN 20 will be named "IT".



![image](https://github.com/user-attachments/assets/4ba40171-f41f-4d9a-8cb0-9dafdcdce6a6)


Next, we will asisng the ports. VLAN10 will be addressed first. We start by entering " int fa0/0". 
Next we will allow access for PC0. 
We enter " swithcport mode access"
Then enter " switchport access vlan 10"






![image](https://github.com/user-attachments/assets/9d5acd77-e445-4896-80a8-3b107b7e81a1)

Next will configure the port for PC1 as part of VLAN, by repeating the same sequence for fa/02




![image](https://github.com/user-attachments/assets/d1695d20-06a4-4ceb-8084-54a361b399ce)



Next, we will address VLAN 20, and configure the 3rd interface with the same sequences for fa/03



![image](https://github.com/user-attachments/assets/2b500b54-bb49-4b25-96b8-63c63e151943)



Next, we will address VLAN 20, and configure the 4th interface with the same sequences for fa/04




![image](https://github.com/user-attachments/assets/8daa56df-1f2a-4d44-81d1-63dacb85ede1)


Next we will interface the router, which is interface 5. 




![image](https://github.com/user-attachments/assets/69f57b1c-e559-4d8d-b4e7-09374453d935)


## Testing

Our next step is to test the network segregation. We will ping VLAN 20 from VLAN 10, between PC0 and PC3, by  using the terminal. The terminal confirms a time out, which is due becuase the router needs to be configured for inter-VLAN routing.



![image](https://github.com/user-attachments/assets/cbb340cf-83cb-4ca2-a7f5-0ccf1ed3dad3)




Beginning with VLAN 10, we can configure inter-VLAN routing using the following command on the router's CLI.




 ![image](https://github.com/user-attachments/assets/45079ee1-a092-4d8d-b60e-c776132971b0)



 Next, we repeat the process to configure VLAN 20 for inter-VLAN routing.

 

  ![image](https://github.com/user-attachments/assets/4dc0e05a-ef0e-45db-8d32-867df5670f5c)




Finally, we can retest the ping from PC0 to PC3 between VLANS. The ping confims a response. And all connection cables now reflect Green.





![image](https://github.com/user-attachments/assets/2e6b0533-0b5b-4af9-b1aa-d4a4177e1182)











![image](https://github.com/user-attachments/assets/95307e14-3b60-43b3-ad2e-00cc65519801)


## Conclusion

Understanding VLAN configuring fundamentals is crucial for effective network segmentation, which enhances security by isolating sensitive data and reducing the risk of unauthorized access. It also improves network performance by reducing broadcast traffic,
allowing for more efficient use of bandwidth. Additionally, mastering VLAN configuration enables network administrators to implement scalable and manageable networks that can adapt to changing organizational needs.







































































































































