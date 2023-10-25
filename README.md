# Active-Directory-Lab
I created two Virtual Machines. One for the domain controller (Windows Server 2019) and the other for the client (Windows 10)

In the Domain Controller I did the following:

Went to Add Roles and Features and added Active Directory Domain Services
![Adding Active Directory Services](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/841407dd-ed32-4621-8d89-d5681ee2e3cc)

Added a new forest called mydomain.com
![Adding New Forest](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/b5ba7da2-3ff4-4bab-88e0-4d09acabd18b)

Added a new Organizational Unit called Admins
![image](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/e9fb4d8d-35a8-4761-a904-1f20b0af3895)

Added a new users in the Admin OU
![Maually adding New users in AD](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/ec85bd79-41c7-40a7-a581-41f7223f29de)

Went to Add Roles and Features and added Remote Access and Routing. Then I configured NAT.
![Remote Access 1](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/67f1dc9a-83fd-4faa-bb76-8893a181cc1c)
![Remote Access 2](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/6e6cfb7a-e3d7-4381-a0b8-3ba780e19a09)
![Remote Access 3](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/4d2b9c32-bb7d-4861-80c8-fc2147f0ae54)
![Remote Access 4](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/1d0baa8f-6d7e-4bac-8506-68518b874934)
![Remote Access 5](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/8618d1f0-1e00-4933-9457-ac850140d399)

Went to Add Roles and Features and added DHCP and New Scope to IPv4
![DHCP 1](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/cef86877-36b9-420d-9fb0-8c2cb2a19228)
![DHCP 2](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/4861bd52-eb5c-43c1-af71-bfeb531199cc)
![DHCP 3](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/a4c5f89c-c3cd-417f-9573-625f958b0e60)
![DHCP 4](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/f2abd7d2-1ac9-4bd5-8374-a782bff41e20)
![DHCP 5](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/ae0cfb46-faa8-4b75-aace-c45be5f7c986)
![DHCP 6](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/71f4d53a-b127-4907-93f9-0e829664de4f)
![DHCP 7](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/32fb3904-6b75-4395-8063-64ca7540e88b)
![DHCP 8](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/2814fd85-fd72-4961-9bee-e974b2b1f53b)
![DHCP 9](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/cfb2bf98-eb7e-4180-8d44-73e6bcfe4ad8)

The following screenshots shows the PowerShell script that I ran to created a new organizational unit called _USERS and added 1000 new users from a text file
![PowerShell Script](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/f5fa5ea5-047f-42e8-aa8a-40168ba1e907)
![Addig Users by PowerShell](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/9f747f9b-cb64-4ee8-9471-7a310490e5cc)

The following screenshot shows the Roles and Server gruops I added
![Services added](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/8fd1b5c4-d513-4dcb-80c3-00f88e391f39)

In the Client I did the following:

Changed the Computer name to CLIENT1 and added the computer to be a Member of: mydomain.com
![Rename 1](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/b9d065e5-648b-4d1a-9c8b-0d31e93332ee)
![Rename 2](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/10cb6ac8-ca30-4f22-9784-61a878adb796)

The following screenshot shows the DHCP in the Domain Controller assigning an IP Address to the Client computer
![IP](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/ef234a60-1b30-4800-9ee5-5af1e53cff51)

The following screenshot shows the Client computer now part of the domain
![Client in Domain](https://github.com/WarRoc22/Active-Directory-Lab/assets/148729293/3d448117-101c-4695-86ab-03d98672f74f)



