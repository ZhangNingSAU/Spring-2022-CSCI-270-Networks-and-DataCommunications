# CSCI270 
# Chapter 4
# Lab: ARP

# Step 1: Create the following network

![arp1](../Resources/ARP1.png)

# Step 1: Use the following command to check the initial ARP tables 
+ use `arp -a` on PCs

![arp2](../Resources/ARP2.png)


+ use `show arp` on Routers

![arp4](../Resources/ARP4.png)

+ use `show mac-address-table` on swtich

![arp3](../Resources/ARP3.png)

+ Note that
  - make sure you change to the correct mode on routers or switches.
  - A switch does not contain an ARP table, only a mac address table.
  
# Step 2: At PC0, ping to the other interfaces
+ Note that you can see the ARP protocol is being used.

![arp5](../Resources/ARP5.png)

~~~~
ping 192.168.1.1
ping 192.168.1.3
ping 192.168.1.4
~~~~

# Step 3: Repeat Step 1

+ PC0

![arp6](../Resources/ARP6.png)

+ PC1

![arp7](../Resources/ARP7.png)


+ PC2

![arp8](../Resources/ARP8.png)


+ Router

![arp9](../Resources/ARP9.png)

+ Switch

![arp10](../Resources/ARP10.png)

+ Please take a look at the difference between PC0's ARP table with other ARP tables.
+ Question: What will happen when the router receives data from another LAN?


