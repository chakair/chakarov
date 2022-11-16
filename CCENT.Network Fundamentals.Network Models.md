---
id: n6rqupy85w23qsf8timdaxq
title: Network Models
desc: ''
updated: 1668636069866
created: 1667510310726
---


<link href="style.css" rel="stylesheet"></link> 

# Network Models

## Table of Contents 

  - [OSI Model](#osi-model)
    - [OSI Model Acronyms](#osi-model-acronyms)
      - [Layer 7 to 1 Acronym](#layer-7-to-1-acronym)
      - [Layer 1 to 7 Acronym](#layer-1-to-7-acronym)
  - [TCP/IP Model](#tcpip-model)
      - [Layer 1 to 4 Acronym](#layer-1-to-4-acronym)
  - [Protocol Data Units (PDUs)](#protocol-data-units-pdus)
  - [Transport Layer (layer 4) Protocols](#transport-layer-layer-4-protocols)
  - [IP Header Protocol Identifiers](#ip-header-protocol-identifiers)
 

<br>

## OSI Model
| Number| Layer Name | Protocol | Explanation
|------|-------| -------| -------|
| 7.| Application | FTP <br> HTTP <br> SMTP |  File Transfer Protocol <br> Hyper Text Transfer Protocol <br> Simple Mail Transfer Protocol| 
| 6.| Presentation | JPEG <br> MPEG| syntax layer (applications can understand the network formats) | 
| 5.| Session | NetBIOS <br> PPTP | establishes, manages and terminates connections between local and remote systems | 
| 4.| Transport | TCP <br> UDP | TCP - reliable delivery <br> UDP - unreliable delivery | 
| 3.| Network | IP <br> ICMP <br> | Internet Protocol <br> Internet Control Message Protocol  | 
| 2.| Data Link | ARP (Address Resolution Protoocol) <br> PPP <br> ATM | used to resolve layer 3 network to layer 2 addresses | 
| 1.| Physical | Ethernet <br> USB  | transport data using electrical, mechanical or procedural interfaces | 

<br>

- [Back to Table of Contents](#table-of-contents)

<br>
  
## OSI Model Acronyms
### Layer 7 to 1 Acronym
<br>
<figure>
    <img src="assets/images/data_processing_mini.jpg"
         alt="Pizza">
    <figcaption>

**A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing
    </figcaption>
</figure>


<br>

| Number| Layer Name | Acronym
|------|-------|-------|
| 7.| Application | All ⬇️| 
| 6.| Presentation | People |
| 5.| Session | Seem | 
| 4.| Transport | To |
| 3.| Network | Need |
| 2.| Data Link | Data |
| 1.| Physical | Processing |

<br>

- [Back to Table of Contents](#table-of-contents)
 
<br>

### Layer 1 to 7 Acronym
<br>

<figure>
    <img src="assets/images/sausage_pizza.jpg"
         alt="Pizza">
    <figcaption>

**P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way
    </figcaption>
</figure>



<br>

| Number| Layer Name | Acronym
|------|-------|-------|
| 7.| Application | Away | 
| 6.| Presentation | Pizza  |
| 5.| Session | Sausage | 
| 4.| Transport | Throw |
| 3.| Network | Not |
| 2.| Data Link | Do |
| 1.| Physical | Please ⬆️|



<br>

- [Back to Table of Contents](#table-of-contents)

<br>

## TCP/IP Model
| Number| Layer Name | 
|------|-------|
| 4.| Application | 
| 3.| Transport | 
| 2.| Internet |
| 1.| Network Interface |

<br>

- [Back to Table of Contents](#table-of-contents)

<br>

### Layer 1 to 4 Acronym
<br>

| Number| Layer Name | Acronym
|------|-------|-------|
| 4.| Application | A ⬇️| 
| 3.| Transport | t |
| 2.| Internet | i | 
| 1.| Network Interface | n |


<figure>
    <img src="assets/images/beans.jpg"
         alt="A tin of baked beans">
    <figcaption>


**A** &nbsp;  **t** **i** **n** of beans
    </figcaption>
</figure>

<br>

- [Back to Table of Contents](#table-of-contents)

<br>

## Protocol Data Units (PDUs)
| Number| PDU Name | 
|------|-------|
| 4.| Segments | 
| 3.| Packets | 
| 2.| Frames |
| 1.| Bits |


<br>
<figure>
    <img src="./assets/images/unhappy_birthday.jpg"
         alt="Birthday">
    <figcaption>


**S**ome **P**eople **F**ear **B**irthdays
    </figcaption>
</figure>

<br>

- [Back to Table of Contents](#table-of-contents)

<br>

## Transport Layer (layer 4) Protocols
| TCP| v. | UDP
|------|-------|-------|
| - connection-oriented|  | - connectionless | 
| - more overhead than UDP|  | - very little overhead |
| - flow control <br> - sequencing <br> - acknowledgements |  | - used for voice and video traffic | 
| - reliable delivery|  | - delivery is not guaranteed |
| - can multiplex using ports|  |  |
| - error recovery|  |  |

<br>

>  ⚠️ In voice and video communications efficiency and non-delay is key at the sacrifice of reliability! 

<br>

- [Back to Table of Contents](#table-of-contents)

<br>

## IP Header Protocol Identifiers
| Protocol number| Protocol | 
|------|-------|
| 1| ICMP | 
| 6| TCP | 
| 17| UDP |
| 88| EIGRP |
| 89| OSPF |

<br>

- [Back to Table of Contents](#table-of-contents)



> Test 
{bluecard}