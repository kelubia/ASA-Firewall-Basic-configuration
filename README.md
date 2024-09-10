# ASA-Firewall-Basic-configuration

Cisco ASA Firewall Basic Configuration

REQUIREMENTS:
ZONES:3
CLIENT NETWORK(TRUSTED)-NET: 192.168.100.0/24
DMZ-SERVER FARM(PARTIALLY TRUSTED)-NET: 10:10:10:0/28
ISP-(UNTRUSTED)-NET: 20.20.20.0/24
ASA FIREWALL- ASA 5506-X

CONFIGURE
-Cisco ASA hostname, 
-Enable passwords, 
-Username and password.
-Cisco ASA system clock and date

CONFIGURE ASA FIREWALL
-Assign an IP address to the interface of ASA.
01
![1](https://github.com/user-attachments/assets/dda90f6a-c8b2-4329-9fb8-721441ad4792)


CLIENT NETWORK(TRUSTED)-NET: 192.168.100.0/24

-Create security level for connected Networks
	ip add 192.168.100.1 255.255.255.0 INSIDE- 100%
02
![02](https://github.com/user-attachments/assets/68880a35-a089-4b6a-8549-b9be8e1542b5)

DMZ-SERVER FARM(PARTIALLY TRUSTED)-NET: 10:10:10:0/28

-Create security level for connected Networks
	ip add 10.10.10.1 255.255.255.240 DMZ- 70%

03
![03](https://github.com/user-attachments/assets/aeb3edba-7344-45d2-880d-6ff723467b36)

ISP-(UNTRUSTED)-NET: 20.20.20.0/24

-Create security level for connected Networks
	ip add 20.20.20.1 255.255.255.0 OUTSIDE- 0%

04
![04](https://github.com/user-attachments/assets/5a8b8116-aae0-4546-a1c0-e1931afc35ff)

05
![05](https://github.com/user-attachments/assets/9f7094d8-7c98-4289-89f8-1d27f7fa29e0)

