MultiArea OSPF Routing Configuration on Multilayer Switch CISCO PACKET TRACER


![image](https://github.com/user-attachments/assets/fe68ee96-66cd-4908-a10b-a3bf8cfd028c)


On this occasion, I will present the MultiArea OSPF Routing configuration on a multilayer Switch device in Cisco Packet Tracer. 

First of all I will add IP Address to each interface of each device.

On The RouterClient1

![image](https://github.com/user-attachments/assets/63ed47cd-1ddd-4fb1-9e8d-8cac030dfd16)

On The CoreSwitchLayer3-1

![image](https://github.com/user-attachments/assets/ecfc81e3-01cd-442a-a0cc-f6441a07418b)

On The CoreSwitchLayer3-2

![image](https://github.com/user-attachments/assets/19a55af2-28fa-4564-aaff-ace19fdf8b51)

Then here there will be several different Area-IDs, Area 0 is connected from RouterClient1 to the external network, then Area 1 is in CoreSwitchLayer3-1 which is connected to RouterClient1, and Area 2 is in CoreSwitchLayer3-2 which is connected to RouterClient1, now this is where MultiArea OSPF Routing is able to connect these different areas so that they can communicate with each other even though they are in different areas.

Here I will configure OSPF routing on RouterClient1:

![image](https://github.com/user-attachments/assets/c7309c71-e95f-4a1e-994a-3c08545c914f)

Next I will configure OSPF routing on CoreSwitchLayer3-1

![image](https://github.com/user-attachments/assets/89e12dd3-9399-4685-89a9-9788156f5069)

Next I will configure OSPF Routing on CoreSwitchLayer3-2

![image](https://github.com/user-attachments/assets/54682815-abd4-4ac4-960c-43e497cec324)

Finally, make sure to test ping between networks on different devices, for example ping from CoreSwitchLayer3-1 to CoreSwitchLayer3-2.

![image](https://github.com/user-attachments/assets/3efafd90-5842-496a-8813-4fe60f505114)

![image](https://github.com/user-attachments/assets/2e78c2bf-a235-42fc-a17e-dce956402f1a)
