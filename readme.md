## LoadBalancer

A simple load balancer / reverse proxy written in GoLang.

### Features
- Acts as a reverse proxy, sitting between clients and web servers.
- Distributes load between different web servers based on number of connections currently active
- Falls back on other web-servers if one goes down

### What is Load Balancer?

The role of a load balancer is to distribute the incoming network traffic among the cluster of the distributed servers so that the work has been done by the single computer will be distributed among multiple computers which makes the process faster and highly available.
### Diagram

![Diagram](https://miro.medium.com/max/1400/1*tEaZGz-p1-E2ytNjl5RPJg.jpeg)


## Algorithm Used

In a distributed environment, there are various techniques used for load balancing, like Round Robin, Weighted Round Robin, Least connection, IP Hash, etc.
This program is implemented using Round Robin algorithm.

Round‑robin load balancing is one of the simplest methods for distributing client requests across a group of servers. Going down the list of servers in the group, the round‑robin load balancer forwards a client request to each server in turn. When it reaches the end of the list, the load balancer loops back and goes down the list again (sends the next request to the first listed server, the one after that to the second server, and so on)
