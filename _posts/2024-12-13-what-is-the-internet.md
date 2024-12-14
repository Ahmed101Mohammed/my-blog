---
title: What is the internet?
date: 2024-12-13
---

The Internet is not simple to define, but in general, people summarize it as a network of networks. Let's dive deeper to explore the components of the Internet:

---

## Internet Edges  

![Some devices around the data center](https://info.teledynamics.com/hubfs/blog-images/Edge%20computing%20-%20TeleDynamics%20Blog.jpg)  

The edge of the Internet includes end-user devices such as laptops, phones, cars, and even smart homes. These devices are often referred to as "hosts".  

---

## Packet Switches  

![Two switches between four users' devices](https://www.rfwireless-world.com/images/circuit-switching-vs-packet-switching-fig2.webp)  

A **packet** is a chunk of data, while a **switch** is a device that transfers packets from one device to another.  

The connection between multiple devices (edges) through **packet switches** forms a network.  

- **Switches** are used to create local networks.  
- **Routers** are used to connect multiple networks.  

---

## Communication Links  

![Ways of communication: like fibers, and copper wires](https://collectionperformance.com/wp-content/uploads/2023/06/wired-networks-types.jpg)  

**Packet switches** and **Internet edges** communicate with each other through **communication links**, which can include fiber, copper, satellite, or radio connections.  

The maximum rate at which packets can be transmitted over a communication link is called **bandwidth**.  

---

## Network  

The combination of **Internet edges**, **packet switches**, and **communication links** within an organization (such as a local network at home or in a business) is called a **network**.  

When these networks are interconnected globally, we get what is commonly referred to as the **Internet**.  

---

## Protocols  

![Examples of Internet protocols like HTTP, HTTPS, and TCP/IP](https://eduinput.com/wp-content/uploads/2023/08/Examples-of-Internet-Protocols-image.png)  

**Protocols** are the rules that define how *packet switches* and *Internet edges* communicate through communication links.  

Protocols exist at various levels:  
- Between two edges.  
- Between an edge and a switch.  
- Between two switches.  
- Between one network and another.  

Examples of protocols include HTTP, streaming video, Skype, TCP, IP, WiFi, 4G, and Ethernet.  

In more detail, protocols define the format and order of messages sent and received between network entities, as well as the actions taken upon sending and receiving these messages.  

---

## Internet Standards  

Internet standards are widely agreed-upon sets of protocols and guidelines for the Internet.  

If you develop a protocol and believe it could be useful across the Internet, you can document it in what is called an **RFC** (Request for Comments).  

### RFC:  
An RFC is the documentation of your protocol, submitted to the **IETF** (Internet Engineering Task Force) for review. If accepted, your protocol can become an Internet standard.  

### IETF:  
The IETF is composed of groups of volunteer network engineers, developers, and researchers. They collaborate to improve Internet processes and architecture.  

---

### References  
- [Jim Kurose: Introduction (reposted) - What is the Internet](https://www.youtube.com/watch?v=74sEFYBBRAY)  
- [Network standards and protocols](https://isaaccomputerscience.org/concepts/net_network_protocols?examBoard=all&stage=all)
