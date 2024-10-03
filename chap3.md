# Analyzing and managing networks

### Analyzing networks with ifconfig
For examining and interacting with active networks interfaces. 

![image](https://github.com/user-attachments/assets/4505bc3a-4ae5-46f4-890d-e6caf3a2f731)

1. + name of the first detected interface.
   + *eth0* (Etherneto), this is the first wired network connection. If there were more wired Ethernet interfaces, they would show up *eth1,eth2...*
   + *HWaddr* : the unique address stamped on every piece of network hardware - NIC referred to as the MAC

2. IP address (in this case is 192.168.181,131).

3. *Bcast* : broadcast address, used to send out information to all IPs on the subnet

4. *Mask* : network mask, determine what part of the IP address is connected to the local network.

5. *lo* : loopback address or localhost, this is a special software address that connects you to your own system. Software and services not running on your system can't use it. You can use *lo* to test something on your system, such as your won web server. The localhost is generally represented with the IP address 127.0.0.1

6. *wlan* : only appears if you have a wireless (mạng không dây) or adapter.

### Checking wireless network devices with iwconfig
**1. Changing your IP address**
