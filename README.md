# Network Design
# Scenario
A multi-national company is expanding and has rented an office space occupying 3 levels of a
building to set up a branch office. The company has engaged your team to design and
implement a scalable enterprise network with redundancy to support the followings:
- a Country Director office at level 3 with 1 x Country Director and 1 x Secretary;
- a Finance department at level 3 with 1 x Finance Manager and 2 x Finance Executives;
- a Human Resource department with 1 x HR Manager and 1 x HR Executive at level 3, 1 x HR Executive at level 2, and 1 x HR Executive at level 1 so as to provide better HR support to all departments;
- a Technical department at level 2 with 2 x Technical Managers, 4 x Principal Engineers and 8 x Engineers;
- a Sales department at level 1 with 1 x Sales Manager and 5 x Sales Executives;
- a meeting room at level 1 with 12 x Ethernet ports available for BYOD connections.
To cater for potential direct WAN connections with other branches in future, the IT
department of the company has mandated the use of IP address block 10.1.1.0/25 for this
branch office.
# Internet Access
The company has subscribed to 2 x ISPs to achieve better reliability to Internet access.
To implement connections to ISPs for Internet access, open up the removable floorboard
covering nearest to the network rack that your team is working on. Look out for Ethernet ports
marked NL1-BSxx or NL2-BSxx, where xx ranges from 1 to 56, and connect them to your
network devices using the 5m light-blue Ethernet cables. (Note: Most racks may already have
one cable connected for you.)

The odd-number ports of NL1-BSxx and NL2-BSxx are for connection to ISP1 whereas the even number
ports are for connection to ISP2.
For connection to ISP1, the ISP1 has allocated the IP address 172.27.47.4(x – 1)+1/30 for your
network device to connect to it, where x ranges from 1 to 20 corresponding to your rack
number; e.g. rack 1 will be 4(1 – 1)+1 = 1, i.e. 172.27.47.1, and so on.
In addition, for Internet access, the ISP1 has allocated the public IP address block
129.126.164.8(x – 1)/29, where x ranges from 1 to 20 corresponding to your rack number; e.g.
rack 20 will be 8(20 – 1) = 152, i.e. 129.126.163.152/29.
Similarly, for connection to ISP2, the ISP2 has allocated the IP address 172.27.47.4(x –
1)+129/30 for your network device to connect to it, where x ranges from 1 to 20 corresponding
to your rack number; e.g. rack 1 will be 4(1 – 1)+129 = 1, i.e. 172.27.46.129, and so on.
In addition, for Internet access, the ISP2 has allocated the public IP address block
118.189.139.8(x – 1)/29, where x ranges from 1 to 20 corresponding to your rack number; e.g.
rack 20 will be 8(20 – 1) = 152, i.e. 118.189.139.152/29.

# Topology Diagram 
![image](https://github.com/ZFCrow/NetworkDesign/assets/113918404/d58d4fe8-7a79-48ce-b4b2-b0bbe02d33ae)
