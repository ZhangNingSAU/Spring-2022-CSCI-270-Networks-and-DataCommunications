# CSCI 270 Spring 2022
# Homework 6 for chapter 8
# Due: 11:59 pm  4/28/2022

## Q1(30 points): Divide network **192.168.1.0/24** into **4** subnets (each subnet has the same number of IP addresses) . List the information of the subnets in the following table.
Note: 1. For the network ID column, you need to provide the subnet mask as well. <br>
      2. Host range is the IP range without the network ID and Broadcast IP.

|subnet|IP Range|Network ID|Host Range|Broadcast IP|
|----|----|----|----|----|
|1|||||
|2|||||
|3|||||
|4|||||

## Q2(30 points): Divide network **192.168.1.0/24** into **4** subnets. The subnets have different numbers of hosts.
Note: 1. For the network ID column, you need to provide the subnet mask as well. <br>
      2. Host range is the IP range without the network ID and Broadcast IP.

|subnet|number of hosts|
|----|----|
|1|110|
|2|55|
|3|20|
|4|10|

List the information of the subnets in the following table.

|subnet|IP Range|Network ID|Host Range|Broadcast IP|
|----|----|----|----|----|
|1|||||
|2|||||
|3|||||
|4|||||



## Q3(40 points): Use CISCO Packet Tracer to construct VLANs as follows.
![](../Resources/lab8-topology.png)
### Requirements:
+ PC0 and PC1 in a VLAN with number 100, name VLAN100
+ PC2 and PC3 in a VLAN with number 200, name VLAN200
+ PCs in two VLANs can communicate.
+ PC0 and PC1 use IPs from network 192.168.1.0/24 and defaut getway 192.168.1.1
+ PC2 and PC3 use IPs from network 192.168.2.0/24 and defaut getway 192.168.2.1

### Hint: see the [lab](../Labs/Ch8-VLAN.md).
+ In this lab, we only create one VLAN with number 20 and name lab1
### More hints 
+ We do not need to specify the ip address and mac address like what we did in step 3.1 in the lab, where we set the IP/MAC addresses for the default vlan (vlan 1)
+ Because we have two user-defined VLANs here, we need to use
~~~~
int g 0/0/0.1 
encapsulation dot1q 100
ip address 192.168.1.1 255.255.255.0
~~~~
to set VLAN100, then
~~~~
int g 0/0/0.2
encapsulation dot1q 200
ip address 192.168.2.1 255.255.255.0
~~~~
to set VLAN200.

**Set the IP addresses for two VLANs, not the defalut VLAN 1**

Here, I used 192.168.1.0/24 and 192.168.2.0/24 as example, you can also use your own network IDs


# Step 1: Save your answers for Q1-Q2 in a PDF file, name it as 'CSCI270_Homework6_JohnDoe(012345467).pdf' 
    (You can write down your answer in any text edit and print it as a pdf file later.)
# Step 2: create and save your cisco packet tracer project as 'CSCI270_Homework6_JohnDoe(012345467).pkt'

# Step 3: Zip the previous two files as one archive, name it as 'CSCI270_Homework6_JohnDoe(012345467)'

# Step 4: Submit your archive file on [Blackboard](https://blackboard.sau.edu)
