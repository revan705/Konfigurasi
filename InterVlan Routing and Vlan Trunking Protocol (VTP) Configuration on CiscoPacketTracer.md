# InterVlan Routing and Vlan Trunking Protocol (VTP) Configuration on CiscoPacketTracer

![image](https://github.com/user-attachments/assets/bf46901c-74aa-41ef-b53e-96bdf6d76f8e)

Here I will show the configuration of InterVlan Routing and VTP on Multilayer Switch in CiscoPacketTracer.

VLAN or Virtual Local Area Network is a network protocol whose purpose is to divide or add several virtual networks in a device, 
usually used for needs when getting a device whose interface is not enough 
to meet the needs of many networks, for example used on Router devices, 
Multilayer Switches, and Switch Management.
And the Vlan Trunking Protocol is a protocol that is usually used on switches 
by racing on VTP which is set in server mode on the specified switch, 
then the switch that is set in VTP client mode will get the VLAN configuration 
created on the switch that is set in VTP server mode.

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

After that, on Switch1 and Switch2, set the trunking mode on the interface leading to the switch so that when VTP client mode is activated, all VLANs configured on the VTP server can be synchronized.

![image](https://github.com/user-attachments/assets/965d5fb2-f319-49f8-881a-83ef0a1d05c0)

![image](https://github.com/user-attachments/assets/4e35b114-86bd-4522-82a5-230f6784a99b)

![image](https://github.com/user-attachments/assets/cf88ee3a-500e-45e3-9b49-c47f18096c58)

Then add IP Vlan 10 on Switch1 and Switch2 as well as the default gateway that can be added to this switch.

![image](https://github.com/user-attachments/assets/b5c2c401-9419-4cb5-ac97-3e164e360214)

![image](https://github.com/user-attachments/assets/35c164c5-40e2-4b25-a3fe-0fbf8c52b1ac)

After that, set the access mode on the interface that leads to the computer and adjust it to the VLAN that will be provided.

![image](https://github.com/user-attachments/assets/3b7e0123-2adb-41a7-bbcb-932134d5ebae)

Finally, add an IP address to each computer, give it an IP that matches the network VLAN that has been created and the customized gateway that has been set, and ping test the computer to a different gateway and VLAN.

![image](https://github.com/user-attachments/assets/d948b38e-c805-439b-b103-24988839ba56)

![image](https://github.com/user-attachments/assets/151b5a17-fba4-4d8e-9416-89652e3f999f)




