---
title: "Computer Networking in a nutshell"
date: 2022-11-05
description: 'How the TCP/IP Model is all the Internet entails'
---

# Why computer networking seems too complicated for everyone?
I've seen that people tend to be afraid of getting into computer networking, specially when it comes to combining it with software.

The reason why computer networking is not understood by many, is because it's kinda abstract since it's grown to an enormous size which we can't study in detail. Therefore we need to be imaginatives by  all these pieces of hardware and software that enable the entire internet.

The key to learn it, is by starting small, in fact in 1969 the Internet was born, and definitely was much smaller. As a matter of fact it was just a connection between two computers! If you think how to computers communicate with each other, you'll easily get that all they do is sending bits of data one another through a copper wire.

## So what are the obstacles nowadays?

- Gigantic size of the Internet
- Understanding of communications
- Learning the protocols that entail the Internet

# Understanding the Internet

In practical environment, the Internet is made of 4 layers. You may ask why layers? This is just a nice representation to break down the Internet in smaller chunks. Otherwise it'd be harder to understand it.

The Internet Engineering Task Force created and maintains this layered model called TCP/IP. In other words these engineers have come up to standards that can be applied to any electronic device so that it can be connected to the internet:

- Application
- Transport
- Internetwork
- Network Access

## Application

Application layer is the user interface on your computer representing any kind of media, such as videos, text, images. Behind the scenes these files are simply bits of data.

### Bits of data
```
0101010101010111111010000010111100001110101010
```

## Transport

This layer is the most important for software. It contains a Segment(s), named after the fact that the original media data is broken down into smaller pieces (Segments) for easier transportation.

Each segment is added information about the ports they are mapped to, so they can interact with the correct program on your computer.

HTTPS uses port 433, so web servers listen on this port and can properly send back the response.

## Internetwork

The IP protocol, defines IP addresses so intermediary devices (routers) can route packets.

Wait, what's a packet? It's the segment itself with extra information added, such as the source IP address and destination address so the routers can forward it to the proper device.

## Network Access

You should see the pattern now, every layer simply keeps adding information to the original data in order to deliver the data successfully.

Befor sending out the bits out, we just add one more piece of information, producing a frame. A frame is used to pass the data from one device to another within the same local network. It enables the packet to be able to be transmitted properly along the way.

# Reversing the encapsulation

Decapsulation is when the process of going up each layer, reverses, bottom-top until we have the orginal data in the receiver.

# Conclusion

The internet is nothing but a bunch of devices that follow the same set of rules for communicating, just like human have grammar rules.

