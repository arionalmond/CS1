# CSP Unit 2 – The Internet: Vocabulary & Concepts

## How to read this

Each lesson lists only what's new: formal vocabulary and the concepts students should walk away with. Timing, prep, links, teaching tips, and teacher dialogue are cut.

- **Vocabulary** is copied word for word from the lesson's formal vocabulary box. Lessons without a box say "No formal vocabulary" and get concepts only.
- **Good to know** terms are defined in passing in the lesson but aren't in a formal vocabulary box. Their basic definitions are my own wording.
- **Key concepts** are condensed from the lesson's overview, objectives, presenter notes, discussion goals, and Check for Understanding.

Source: Code.org CS Principles (2025–26), Unit 2 lesson plans, licensed CC BY-NC-SA 4.0. Changes made: content condensed, reorganized, and paraphrased; teacher-facing material removed.

## Lesson 1: Welcome to the Internet

**Vocabulary:** No formal vocabulary.

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Net Neutrality | The principle that Internet service providers should give equal access to all content and apps, without favoring or blocking particular products or websites |
| Internet Censorship | Attempts to control or suppress what certain people can access, publish, or view on the Internet |

**Key concepts**

- Unit 1 was about representing information digitally. Unit 2 is about communicating that information with others.
- The Internet works in layers, just as digital information is built on layers of abstraction (binary → decimal → ASCII).
- The Internet Simulator is the tool used all unit to explore how the Internet works. Its first version connects only two people by a single direct line.
- Like the real Internet, the simulator sends information that all comes down to 0s and 1s. Unlike it, the first version only sends text and only to one person.
- Big societal issues like net neutrality and Internet censorship depend on understanding how the Internet works. Many of them come from people taking advantage of the Internet's open protocols.

## Lesson 2: Building a Network

**Vocabulary**

| Term | Definition |
| --- | --- |
| Bandwidth | the maximum amount of data that can be sent in a fixed amount of time, usually measured in bits per second |
| Computing Device | a machine that can run a program, including computers, tablets, servers, routers, and smart sensors |
| Computing Network | a group of interconnected computing devices capable of sending or receiving data. |
| Computing System | a group of computing devices and programs working together for a common purpose |
| Path | the series of connections between computing devices on a network starting with a sender and ending with a receiver |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Routing | The process of finding a path from the sender to the receiver |

**Key concepts**

- A single wire between two devices has two problems: you can only talk to one device, and there's no backup if that wire fails.
- A network connects many devices so they can communicate. Two devices that aren't directly connected can still communicate along a path through other devices.
- There are usually many possible paths between a sender and a receiver.
- Network design means balancing competing goals. Connecting every device directly to every other device is one extreme, and connecting too few is the other. Good designs land in between, and each choice has strengths and weaknesses.
- How fast a message arrives depends on bandwidth. Higher bandwidth means more bits per second.
- A computing network is a type of computing system. Devices plus the paths between them make up the network, and these are the same building blocks as the Internet.

## Lesson 3: The Need for Addressing

**Vocabulary**

| Term | Definition |
| --- | --- |
| IP Address | The unique number assigned to each device on the Internet |
| Internet Protocol (IP) | a protocol for sending data across the Internet that assigns unique numbers (IP addresses) to each connected device |
| Protocol | An agreed-upon set of rules that specify the behavior of some system |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Broadcast | Sending a message to every device on a network at once, instead of to one specific device |

**Key concepts**

- When every message goes to everyone (broadcast), communication gets confusing. You can't tell who a message is for or who sent it, and people talk over each other.
- To communicate on a shared network, every message needs to identify both the sender and the receiver.
- Communication rules only work if they're clear and everyone agrees to follow them.
- The Internet Protocol (IP) is the shared rule set for addressing. Every device gets a unique IP address (stored in binary), and every device formats sender and receiver information the same way. That lets devices on different networks communicate.
- Protocols need to be open and shared, not secret, so any device can join and communicate. The Internet is really a set of protocols for communicating over networks.

## Lesson 4: Routers and Redundancy

**Vocabulary**

| Term | Definition |
| --- | --- |
| Fault Tolerant | Can continue to function even in the event of individual component failures. This is important because elements of complex systems like a computer network fail at unexpected times, often in groups. |
| Redundancy | The inclusion of extra components so that a system can continue to work even if individual components fail, for example by having more than one path between any two connected devices in a network |
| Router | A type of computer that forwards data across a network |

**Key concepts**

- Every device has its own IP address, and each message carries a "to" and a "from" address, much like mail.
- Devices connect to a router, and routers connect to each other. A message often passes through several routers before reaching its destination instead of taking a direct route.
- Router logs show which routers handled each message. The same message shows up once for each router it passed through.
- Messages between the same two devices don't always take the same path. Routes are dynamic and can change from one message to the next.
- Messages might take different paths because some paths have heavy traffic or because a connection has been cut.
- Redundancy (more than one path between devices) is what makes the network fault tolerant. If one path fails, data can still get through on another.

## Lesson 5: Packets

**Vocabulary**

| Term | Definition |
| --- | --- |
| Packet | A chunk of data sent over a network. Larger messages are divided into packets that may arrive at the destination in order, out-of-order, or not at all |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Packet Metadata | Extra data added to a packet, like IP addresses or a packet number, that helps route it and put the message back together |
| UDP (User Datagram Protocol) | A simple, fast protocol that just sends all the packets, with no check for lost or out-of-order packets |
| TCP (Transmission Control Protocol) | A protocol that numbers packets, re-orders them, and resends lost ones, so the full message arrives correctly |

**Key concepts**

- Large messages (like movies or big images) are split into packets and sent as a stream of packets.
- Part of each packet is metadata, which leaves less room for the actual message. In the simulator, 16 of each packet's 80 bits are metadata, leaving 64 bits (8 ASCII characters).
- Packets can take different paths, arrive out of order, or be dropped entirely. A person might fill in the gaps from context, but a computer can't.
- Sending protocols trade off speed against accuracy. UDP is simple and fast but unreliable. TCP is more accurate but takes longer. Each is used depending on what the situation needs.
- A reliable protocol numbers each packet, says how many packets to expect, lets the receiver request missing packets or confirm received ones, and lets both sides know when the full message has arrived.
- Splitting data into packets and using TCP together make the Internet more reliable.

## Lesson 6: HTTP and DNS

**Vocabulary**

| Term | Definition |
| --- | --- |
| Domain Name System (DNS) | the system responsible for translating domain names like example.com into IP addresses |
| HyperText Transfer Protocol (HTTP) | the protocol used for transmitting web pages over the Internet |
| World Wide Web | a system of linked pages, programs, and files |

**Good to know** (not in the formal vocabulary box)

| Term | Basic definition |
| --- | --- |
| Scalability | The ability of a system to keep working well as it grows to handle many more users or devices |
| Domain Name | A human-readable name for a website, like example.com, that DNS translates into an IP address |
| HTTPS (SSL/TLS) | A secure version of HTTP that encrypts communication so it isn't sent as plain text |
| Certificate Authority | A trusted organization that confirms a website is who it claims to be when you make a secure connection |

**Key concepts**

- IP addresses change as devices join and leave networks, so it's impossible for every device to keep its own accurate list of everyone's address.
- DNS is a network of servers that tracks which IP address goes with each domain name. If the first DNS server you ask doesn't know an address, it asks other servers.
- DNS helps the Internet scale. Billions of devices can join without any single computer having to know every IP address.
- Visiting a website means a server sends your computer a file. HTTP is the protocol your computer uses to request it. HTTP is plain text: the request literally includes "GET" and the file name.
- Because HTTP is plain text, secure versions (HTTPS using SSL/TLS) are needed. Certificate authorities confirm you're talking to the real website.
- The World Wide Web is one of many things that runs on the Internet. It's the system of linked pages and files that HTTP sends.
- Each layer of the Internet relies on the layers below it. When you visit code.org:
    1. DNS finds code.org's IP address.
    2. Your browser sends an HTTP GET request to that address.
    3. Code.org's server responds with the HTML for its page.
    4. TCP or UDP splits these messages into packets. TCP also checks for errors.
    5. IP routes the packets between your computer and the server.
    6. Everything travels over the physical network of wires, cables, Wi-Fi, and routers.

## Lesson 7: Project – Internet Dilemmas

**Vocabulary**

| Term | Definition |
| --- | --- |
| Digital Divide | differing access to computing devices and the Internet, based on socioeconomic, geographic, or demographic characteristics |

**Key concepts**

- This two-day project answers the "so what" of the unit: why it matters to understand how the Internet works.
- Students pick one of three dilemmas: Net Neutrality, Internet Censorship, or the Digital Divide.
- Acting as a candidate's technology advisor, students research their dilemma and write a policy one-pager with a recommendation.
- Analyzing a dilemma means identifying who benefits and who is harmed, and how the Internet's technical structure and design contribute to the problem.
- Digital Divide is the only formal vocabulary term because it's part of the AP CSP Conceptual Framework. Every student should know it, even if they choose a different dilemma.
- The project pairs with the Unit 2 Assessment and closes with the Unit 2 vocabulary review.
