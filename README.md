# BGP, OSPF, and Eigrp Routing Configuration on Cisco Packet Tracer

![image](https://github.com/user-attachments/assets/d59435a5-00ee-409d-ae14-e728c2787cee)


In the topology above, here I experimented with connecting routers using several routing protocols.
First I will configure using cli, and go to each interface on each router, turn on the port and add the ip address:

On The RouterBackbone1

![image](https://github.com/user-attachments/assets/193eac4e-0168-4bfe-acec-259b71e5f89f)


On The RouterBackbone2

![image](https://github.com/user-attachments/assets/71d96d64-b085-4cad-8f28-521a9d2eb941)


On The RouterClient1

![image](https://github.com/user-attachments/assets/952016e7-5d74-492e-8d14-581b0f1f278b)


On The RouterClient2

![image](https://github.com/user-attachments/assets/f76c5f30-172b-429c-970b-be72c56b1187)


Then here I will first add the BGP routing configuration between the Backbone Routers:


![image](https://github.com/user-attachments/assets/03aea819-ee53-46d7-aefc-1e5ee4b29475)


![image](https://github.com/user-attachments/assets/50493641-c5f4-4430-92df-84d0cfedb57a)


Then I will add another routing configuration on each backbone router:


![image](https://github.com/user-attachments/assets/d6485e2f-17bf-408b-bf1b-cb96706a8277)


![image](https://github.com/user-attachments/assets/fc1afb8a-2c4e-4100-bcf5-6e6459acb59e)


Next, add the Routing configuration to each Client Router:

![image](https://github.com/user-attachments/assets/20540d04-8991-4008-86b8-015cf75e1330)


![image](https://github.com/user-attachments/assets/914ee16b-cca8-4c06-9e82-cd8216e3d61a)


Finally, we try to ping from Router Client 1 to Router Client 2.

![image](https://github.com/user-attachments/assets/7ac47ac2-6712-4791-9e1e-39e2e0c72ffe)
