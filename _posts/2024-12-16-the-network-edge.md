---
title: Network edge: Access networks & Physical media
date: 2024-12-16
---
To understand the relation between the *internet* and the **network edge** we need to talk about two things: 
1. What networks are used to connect the **network edge** to the first hub router in the larger *Internet*?
2. What is the physical media that is used across the **internet network**?

Ok, you need also a third thing :). You need to recap what is the **edges** of the **network**?
## Network edge:
The edge of the Internet includes end-user devices such as laptops, phones, cars, and even smart homes. These devices are often referred to as "hosts".
Edges can be 2 categories:
1. Clients: such as laptops, phones, and cars ...etc.
2. Servers: You can say these are computers that save internet data around the world, and they are often in data centers.
---

## Access Networks
When we say **Access Networks** we mean: The network that connects the **edge router** to the first hub router in the larger **internet**.

There are 3 types of **access networks**:
- Residential access networks. ?
- Institutional access networks. ?
- Mobile access networks. ?

Let's start to discuss examples of **access networks**.
### Cable-based access
The ***cable-based access*** is the **access network** used near our homes.
The ***cable-based access***: is a single cable that connects multiple houses to a single **cable headend**. 
The signals that go *to* from *from* houses through ***cable-based access*** are sent in different frequencies, that do not interfere with each other.\
The approach that ***cable-based access*** used to send **packets** *from* and *to* houses in different frequencies is called **Frequency division multiplexing (FDM)**.
You should know that can two houses share the same frequency. (?)

#### Cable-based access characteristics
There are some important characteristics you need to know about **Cable-based access**:
1. The ***Cable-based network*** is asymmetric: this means that it is designed to transmit the **packets** at different rates between the house and the **cable headend**.
   In more detail: The ***Cable-based access*** is designed to be the **packets** transmission from home to the **cable headend** (downstream) *faster than* the **packets** transmission from **cable headend** to the house (upstream).
2. The ***Calbe-based network*** is a shared network: this means that if one of the units (like: a house) shares the same frequency with you, and this unit used to send and receive so much data, this can affect your transmission rate. 
3. The data transmission through the ***cable-based network*** is also affected by the distance between the edge (like: the house) and the **cable headend**.

### Digital subscriber line (DSL)
DSL networks: used the existing telephone line to **central office (DSLAM)** directly without any unit (like: a house) sharing your line or frequency.
The DSL can send things to the **central office**:
- Data: It goes through the dedicated phone line to the **central office** then to the **internet**.
- Voice: It goes through the dedicated phone line to the **central office** then to the *telephone net*.

#### DSL characteristics
1. The ***DSL*** is also **asymmetric** like *cable-based access*:
   - ***DSL*** downstream transmission rate through the dedicated phone line is 24-53 Mbps.
   - ***DSL*** upstream transmission rate through the dedicated phone line is 3.5-16 Mbps.
2. The ***DSL*** data transmission rate is also affected by the distance between the edge (like: a house) and the **central office**.

### Home network
We now know some ***access network*** types, and we see them from the perspective street :)
Now we want to see where the **cable-based** or **Digital subscriber line** access inside our home.
For the **cable-based** it accesses directly to the ***router*** but for the **Digital subscriber line** it accesses through ***DSL modem***.
Then the ***cable*** or the ***DSL modem*** access directly to the ***router*** that has a connection to the end-systems through ***wired ethernet*** links.
The devices (end-systems) that the ***router*** connected to, they maybe can be your *PC* or maybe a ***WiFI modem***.
The **wired ethernet access*** transmission rate can be 1 Gpbs.
The **Wireless WiFi access*** transmission rate can be 54 or 450 Mbps.
Usually, **DSL modem**, **router**, **WiFi**, and **ethernet** are combined in one single box.

### Wireless access network
**Wireless access network**: is a shared wireless access network connects *end system* to *router*, via **base station** aka **access point**.
There are two classes of **wireless access networks**:

#### Wireless local area networks (WLANs)
It works in a range of 100 meters
It works in different speeds maybe 11, 54, or 450 Mbps transmission rate.
These distance and speeds support for ***WLANs access*** are protocols standardized by **IEEE**, and these protocols are under the family *802.11* protocols. and they are not standardized by **ITEF**.

#### Wide-area cellular access networks
It works in a wide range of distances it can be 10's of kilometers.
It also can transmit data in different ranges maybe 1, 10, or multiple 10's Mbps.

### Enterprise networks
Enterprise networks can be in two forms:
1. Like house network: Maybe in companies or university, you can use the same **house network** but in a large scale.
     - It's a combination of **Wireless WiFi network** and **Ethernet wire** and multiple **modems** and **routers** to handle a large number of devices.
2. Data center networks: It's a massive number of servers connected to each others and connected to the **internet**.
     - It can transmit the data in 10's to 100's Gpbs.

## Physical media
The **physical media**: is used to transmit bits input side of the link to the output side of the link.
To understand more about **physical media** we need firstly to understand what it's mean that: sending packets of data.

### Host: sends packets of data
Let's go on a trip in this scenario: a *host* (like your computer) sends data to the first hub switch:
1. The host takes a message from the application.
2. Divide the message (data) into chunks, which we call ***packets***:
    - Every **packet** has a chunk of the app data, and a special data called ***packet header***.
    - The information in the ***packet header*** determines by a protocole.
    - Every **packet** has length (L) measured by bits, this length includes the whole **packt** its chunk of application  data, and the **packet header**.
3. Host transmits the **packet** into **access network** at transmission rate (R) measured in bps (Bits per second).
    - The transmission rate that the Host can send data at, is called also a *** link transmission rate*** aka ***lin capacity***, aka ***link bandwidth***.
    - If you want to measure how much your packet will take to transmit into a link you can use this formula: L(bits)/R(bits/sec) = **Packet Length**(bits)/**Link transmission rate**(bits/sec)
Now we can go back to the **physical media**, you need to know that ***bits***: is what does **propagates** between transmitter/receiver pares.
You also know that **physical media**: is what lies between the transmitter and the receiver.
Now you need to know that there are two categories of **physical media**:
1. Guided media: It propagates singles in a solid media. e.g. copper, fiber, and coax.
2. Unguided media: It propagates singles freely. e.g. radio.
Let's go deep in both of these categories.
### Physical guided media
It can include

#### Twisted pair (TP)
It's two insulated copper wires, that are used in *DSL*. 
There are 2 categories for Twisted pairs:
  - Category 5: 100 Mbps, 1 Gbps Ethernet.
  - Category 6: 10 Gbps Ethernet.

#### Coaxial cable
It's a bidirectional two-concentric copper conductor.
It has multiple frequency channels and sends 100's Mbps per channel.

#### Fiber optic cable
It's a glass fiber carrying light pulses, each pulse is one bit.
It has high-speed operations, and it can transmission the data at 10's to 100's Gbps.
It has a low error rate, because of:
- It is immune to electromagnetic noise.
- Its repeaters are spaced far apart.

### Physical unguided media
It includes

#### Wireless radio
In this media, the signal is carried in various *bands* in the electromagnetic spectrum.
This media is **unguided media** so it has no **physical wire* and its transmits tend to be broadcast, and this means that any device neat to the transmitter device may able to receive these signals. You may expect that it can lead to interference concerns.
Wireless is a hard environment to transfer data, the propagation environment can be affected by: [end point: 14:00](https://youtu.be/k8NmM-hImBU?feature=shared)
---
### References:
- [Jim Kurose | 1.2 The network edge](https://youtu.be/k8NmM-hImBU?feature=shared)
