# CSCI 270 Fall 2021
# Homework 2
# Due: 11:59 pm 09/23/2019

## Q1: Use ipconfig(windows) or ifconfig(mac) to find out all the MAC address of you computer, then list the part of each MAC address that is unique to each manufacturer.(10 points)

hint: 
+ use `ipconfig /all` for windows, find all the `physical addresses`
+ use `ifconfig` for mac, find `ether`in `en0` and `en1` (or you can use `ifconfig | grep "ether"`)

## Q2: For class A IP address `1.x.y.z to 126.x.y.z`, the approximate number of IP addresses in each network is 16 million, can you find out the exact number?(10 points)

## Q3: Suppose two network devices with IP addresses 192.168.1.1/24 and 192.168.1.2/16 are on the same LAN, can they communicate with each other directly? explain why they can or can not.(10 points)

hint: 
+ /24 means the first 24 bits of the subnet mask are 1s, the rest are 0s. (the subnet mask is 255.255.255.0)
+ the `and` operation between IP and subnet mask
+ If one network ID is part of(belongs to) another one, they can communicate.
+ One way to double-check your answer is to use the Packet Tracer to build a topology (you just need to use one wire to connect two PCs), set up the IP address and subnet mask for each PC, then use ping command to see if they can communicate.

## Q4: (10 points)
____ substitutes privite IP with public IP.
+ A. NAT
+ B. PAT

____ assigns each session between two ports a unique number.
+ A. NAT
+ B. PAT

## Q5: Explain the difference between SNAT and DNAT. (10 points)

## Q6: Describe the process to find the IP address associated with the domain name `blackboard.sau.edu` for the first time. 
## What will happen if you request for the DNS service for the second time. (20 points)

## Q7: Use CISCO Packet Trace to construct a LAN(several PCs, a switch and a router), choose and set up the static IP addresses for each PC and the router, make sure each interface of the PCs and the router inside the LAN can communicate with each other. (30 points)

Hint: 
+ choose private IP addresses for the interfaces/ports of PCs and router inside the LAN
+ <b>choose a public IP address for the interface/port of the router outside the LAN</b>
+ make sure you turn on the interfaces of the router. (click on the router icon->Config->INTERFACE->GigabitEthernet0/0/0 and GigabitEthernet0/0/1 -> Port Status -> check `on`)
+ use `ping` command to see if you can get response from another interface.
+ use `Realtime` mode rather than `Simulation` mode to `ping` an IP address.


# Step 1: Save your answers for Q1-Q6 in a PDF file, name it as 'CSCI270_Homework2_JohnDoe(012345467).pdf' 
    (You can write down your answer in any text edit and print it as a pdf file later.)
# Step 2: create and save your cisco packet tracer project as 'CSCI270_Homework2_JohnDoe(012345467).pkt'

# Step 3: Zip the previous two files as one archive, name it as 'CSCI270_Homework2_JohnDoe(012345467)'

# Step 4: Submit your archive file on [Blackboard](https://blackboard.sau.edu)
