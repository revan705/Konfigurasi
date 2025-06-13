# BGP, OSPF, and Eigrp Routing Configuration on Cisco Packet Tracer
![image](https://github.com/user-attachments/assets/9e0cde01-32aa-446e-8e62-8c0f1fd5d06e)


In the topology above, here I experimented with connecting routers using several routing protocols.
First I will configure using cli, and go to each interface on each router, turn on the port and add the ip address:

On The RouterBackbone1

![image](https://github.com/user-attachments/assets/193eac4e-0168-4bfe-acec-259b71e5f89f)


On The RouterBackbone2

![image](https://github.com/user-attachments/assets/71d96d64-b085-4cad-8f28-521a9d2eb941)


On The RouterClient1

![image](https://github.com/user-attachments/assets/3ff44cd8-d0ed-475f-a446-c864323203d3)


On The RouterClient2

![image](https://github.com/user-attachments/assets/f76c5f30-172b-429c-970b-be72c56b1187)


Then here I will first add the BGP routing configuration between the Backbone Routers:


![image](https://github.com/user-attachments/assets/2f31505c-d0b2-49ed-a494-bc674476bed9)


![image](https://github.com/user-attachments/assets/50493641-c5f4-4430-92df-84d0cfedb57a)


Then I will add another routing configuration on each backbone router:


![image](https://github.com/user-attachments/assets/79d30c05-6c73-4132-9cc0-edd9f947b204)


![image](https://github.com/user-attachments/assets/fc1afb8a-2c4e-4100-bcf5-6e6459acb59e)


Next, add the Routing configuration to each Client Router:

![image](https://github.com/user-attachments/assets/f374e269-5c52-4fa8-8d9f-f8babae66bc1)


![image](https://github.com/user-attachments/assets/914ee16b-cca8-4c06-9e82-cd8216e3d61a)


Finally, we try to ping from Router Client 1 to Router Client 2.

![image](https://github.com/user-attachments/assets/7ac47ac2-6712-4791-9e1e-39e2e0c72ffe)
