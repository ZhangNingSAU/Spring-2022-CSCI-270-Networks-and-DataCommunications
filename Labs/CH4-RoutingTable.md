# Lab: Ch4 - Routing Table

# Step 1: Construct the network topology.

![lab1-routing-1](../Resources/lab1-routing-1.png)

Always a good idea to show the port/interface names. Follow the following instruction to do so.

![lab1-routing-2](../Resources/lab1-routing-2.png)

# Step 2: Set up IP/Mask for each port.
+ Do not forget the default gateway.

![lab1-routing-3](../Resources/lab1-routing-3.png)

![lab1-routing-4](../Resources/lab1-routing-4.png)

+ Do not forget to turn on the interfaces we use on routers.

![lab1-routing-5](../Resources/lab1-routing-5.png)


# Step 3: On each router, create the routing table.
+ You do not need to provide the information for the networks that are connected to the router directly(The ones with 0 hop count).
+ You need to enter:
  - Network (ID)
  - (Subnet) Mask
  - Next Hop
  
![lab1-routing-6](../Resources/lab1-routing-6.png)

# Step 4: Use `ping` command to check if the routing tables are working or not.

![lab1-routing-7](../Resources/lab1-routing-7.png)


![lab1-routing-8](../Resources/lab1-routing-8.png)
