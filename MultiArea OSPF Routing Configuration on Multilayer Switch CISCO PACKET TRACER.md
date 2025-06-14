MultiArea OSPF Routing Configuration on Multilayer Switch CISCO PACKET TRACER


![image](https://github.com/user-attachments/assets/fe68ee96-66cd-4908-a10b-a3bf8cfd028c)


On this occasion, I will present the MultiArea OSPF Routing configuration on a multilayer Switch device in Cisco Packet Tracer. 

First of all I will add IP Address to each interface of each device.

On The RouterClient1

![image](https://github.com/user-attachments/assets/30d5f498-36a9-4d89-9d6d-a292ab9e550a)

On The CoreSwitchLayer3-1

![image](https://github.com/user-attachments/assets/94daea52-db02-4361-abec-40e9301a9a35)

On The CoreSwitchLayer3-2

![image](https://github.com/user-attachments/assets/d2392cb6-8769-4856-9b69-70a22d75b343)

Then here there will be several different Area-IDs, Area 0 is connected from RouterClient1 to the external network, then Area 1 is in CoreSwitchLayer3-1 which is connected to RouterClient1, and Area 2 is in CoreSwitchLayer3-2 which is connected to RouterClient1, now this is where MultiArea OSPF Routing is able to connect these different areas so that they can communicate with each other even though they are in different areas.

Here I will configure OSPF routing on RouterClient1:

![image](https://github.com/user-attachments/assets/8057e3e3-e07c-4bb6-b0bd-8a87dd5750c7)

Next I will configure OSPF routing on CoreSwitchLayer3-1

![image](https://github.com/user-attachments/assets/4a125404-762a-4484-8ed7-7b224dac88ec)

Next I will configure OSPF Routing on CoreSwitchLayer3-2

![image](https://github.com/user-attachments/assets/c5d4f622-19b4-4764-9a03-e73053c0571f)

Finally, make sure to test ping between networks on different devices, for example ping from CoreSwitchLayer3-1 to CoreSwitchLayer3-2.

![image](https://github.com/user-attachments/assets/3efafd90-5842-496a-8813-4fe60f505114)

![image](https://github.com/user-attachments/assets/2e78c2bf-a235-42fc-a17e-dce956402f1a)
