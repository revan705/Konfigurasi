# InterVlan Routing and Vlan Trunking Protocol (VTP) Configuration on CiscoPacketTracer

![image](https://github.com/user-attachments/assets/bf46901c-74aa-41ef-b53e-96bdf6d76f8e)

Here I will show the configuration of InterVlan Routing and VTP on Multilayer Switch in CiscoPacketTracer.

VLAN or Virtual Local Area Network is a network protocol whose purpose is to divide or add several virtual networks in a device, 
usually used for needs when getting a device whose interface is not enough 
to meet the needs of many networks, for example used on Router devices, Multilayer Switches, and Switch Management.

First, create the VLAN that will be created, here VLAN 10 as the Client VLAN and VLAN 20 as the Client2 VLAN, 
and add the gateway IP to the VLAN interface on this Multilayer Switch on the interface that leads to the local area.

![image](https://github.com/user-attachments/assets/36dba871-a565-4d6e-aaf6-cdfdd7bcce0a)

![image](https://github.com/user-attachments/assets/d2ae5852-793d-4907-8afb-522740764be6)

Then set the CoreSwitchLayer 3-1 Trunking Port to the appropriate interface, 
the function of this trunking mode is to carry all VLANs on the configured port.

![image](https://github.com/user-attachments/assets/6a0ec84a-fb07-4567-96dd-b9a0d6bc420e)

Set the VTP that will be used on CoreSwitchLayer3-1 as the VTP Server and set the VTP domain and VTP password that will be adjusted and matched to those that will be used on the VTP client:

![image](https://github.com/user-attachments/assets/035d5f7f-ce53-49ee-ba2d-ec4475b03741)

Then check the active VTP status:

![image](https://github.com/user-attachments/assets/75681c27-6930-40eb-ab43-8a198bd0fdd7)
