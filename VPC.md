### Virtual private clouds (VPC)
A VPC is a virtual network that that you can use in your virtual servers. After you create a VPC, you can add subnets.

### Subnets
A subnet is a range of IP addresses in your VPC. A subnet must reside in a single Availability Zone. After you add subnets, you can deploy AWS resources in your VPC.

### Gateway
A gateway connects your VPC to another network. For example, use an internet gateway to connect your VPC to the internet. Use a VPC endpoint to connect to AWS services privately, without the use of an internet gateway or NAT device.

### NACL
A network access control list (NACL) is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets.

### CIDR Blocks
CIDR blocks are groups of addresses that share the same prefix and contain the same number of bits.

### Route Tables
A route table contains a set of rules, called routes, that determine where network traffic from your subnet or gateway is directed.

![vpc drawio](https://user-images.githubusercontent.com/106158041/200299803-1eaf640c-801d-483a-8536-57e7d32d2867.png)

### Private & Public Subnets
The difference between a private and public subnet is that a public subnet has an internet gateway attached to its route table so it can be accessed directly from the internet, while a private subnet does not.
Anything deployed within a private subnet cannot be accessed from the Internet.
