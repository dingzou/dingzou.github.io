---
title: Socket Basics
layout: post
---

The TCP/IP model can be splitted into 5 abstract layer, stacked upon each other.
   - Application: P2P vs Client Server, HTTP, SMTP, POP, IMAP, DNS.
   - Transport: TCP, TCP segment, UDP, RTT, Window Scaling.
   - Network: Control plane, Static/Dynaic Routing, IPv4, packets, packet segmentation, DHCP, ICMP, Firewall, NATs, Border Gateway.
   - Data Link: Ethernet, Ethernet frame, MAC, Error Detection, VLANs
   - Physical


Network application normally consists of two programes: one as a server program and another one as client program. These two program reside on two seperate end systems

When any of of the program need to communicate with another, they write data to their sockets. The underlining network protocol is responsible to deliever the message to the other side.


source: Grokking Computer Networking for Software Engineers
