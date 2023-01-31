---
id: n6rqupy85w23qsf8timdaxq
title: Network Models
desc: ''
updated: 1672264005534
created: 1667510310726
---


---
id: 0j1kojhj0vuphwkf2kslalp
title: PDU
desc: ''
updated: 1668787212474
created: 1668787212474
---


<link href="style.css" rel="stylesheet"></link> 

# Network Models


<div class="intro">

## Introduction

Different models are used in networking to help us understand how communication between devices takes place. There are two main network models that you have to get familiar with: 
- the ***Open Systems Interconnection (OSI)*** model consisting of seven layers and 
- the  ***Transmission Control Protocol/Internet Protocol (TCP/IP)*** model consisting of four layers.

You have to learn the different layers of both the OSI and TCP/IP models as well as get familiar with different terms, such as: 
- ***Protocol Data Units (PDUs)***
- ***Transport Layer (layer 4) Protocols*** and 
- ***IP Header Protocol Identifiers***.

</div>

<br>

<div class="toc">

## Table of Contents

- [OSI Model](CCENT.Network%20Fundamentals.Network%20Models.OSI.md)  
- [TCP/IP Model](CCENT.Network%20Fundamentals.Network%20Models.TCPIP.md)
- [Protocol Data Units (PDUs)](CCENT.Network%20Fundamentals.Network%20Models.PDU.md)
- [Transport Layer (layer 4) Protocols](CCENT.Network%20Fundamentals.Network%20Models.TLProtocols.md)
- [IP Header Protocol Identifiers](CCENT.Network%20Fundamentals.Network%20Models.IPHeaders.md)

</div>

<br>

<div class="summary">

## Summary



- The ***Open Systems Interconnection (OSI)*** model describes ***seven layers*** that computer systems use to communicate over a network.
- The seven layers of the OSI model, from top to bottom are as follows: Application, Presentation, Session, Transport, Network, Data Link and Physical. 
- The acronyms used to remember the layers of the OSI model are:
  - "**A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing"
(Layer 7 to 1 Acronym) 
  - "**P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way"
(Layer 1 to 7 Acronym)
- TCP/IP stands for Transmission Control Protocol/Internet Protocol.
- TCP/IP is a set of standardized rules that allow computers to communicate on a network such as the Internet. It consists of ***four*** layers, Application, Transport, Internet and Network Interface.
- A good way of using an acronym to remember the TCP/IP model is to think of a tin of beans!
- A ***protocol data unit (PDU)*** is the basic unit of exchange between devices that communicate using a specified networking protocol.
- The PDUs for the bottom four layers of the OSI model, from layer4 to layer 1, are: Segments, Packets, Frames and Bits.
- A good way of remembering the PDUs for each of the bottom four layers of the OSI model is "**S**ome **P**eople **F**ear **B**irthdays!"
- The transport layer (OSI layer 4) is represented by two protocols: ***TCP*** (Transmission Control Protocol) and ***UDP*** (User Datagram Protocol). 
- TCP is connection-oriented as opposed to UDP which is connectionless.
- TCP has more overhead than UDP and uses flow control, sequencing,  acknowledgements and guarantees reliable delivery by using error recovery.
- UDP is used for ***voice*** and ***video*** communications, where  ***efficiency*** and ***non-delay*** are key at the 
<font color="red">***sacrifice of reliability***</font>! 

- The IP header protocol identifier is a number embedded in the header of the packet to identify the type of protocol used.
- The most commond protocol identifiers are: ICMP (1), TCP (6), UDP (17),  EIGRP (88) and OSPF (89).
<br>



</div>

