deck:: [[Computer Network]]

- What is Internet? #card
  id:: 6207cf8f-e996-4810-9c45-008a620f564d
	- Internet consists of devices and links. Packet switches transfer packets between devices using links to allow different users to communicate. Internet also provide API for applications to connect to different users.
- What is network protocol? #card
  id:: 6207cf8f-b06e-4e0f-8852-9704eec03f81
	- It's a set of rule to define how two parties can communicate to each other on the Internet
- Give a few examples of access network. #card
  id:: 6207ba59-f245-42cb-a504-491ea6b63d38
	- digital subscriber line (DSL)
	- cable network
	- home network
	- enterprise access network (Ethernet)
	- wireless access network
- How does cable network achieve shared access of network? #card
  id:: 6207cf8f-12c6-4898-85e5-867d232f620f
	- It uses frequency division multiplexing
- What exactly does 'network of network' means when describing network core? #card
  id:: 6207cf8f-085c-4c6c-96c8-3674d22c0fc8
	- The core of Internet consists of interconnected ISP router, and different level of ISPs are also connected
- What is the difference between routing and forwarding? #card
  id:: 6207ba59-3445-4135-9b53-5d52834edd7c
	- Routing is determining the route to packet's destination, forwarding happens in router, determining which output port should this packet go
- What happen when packet arrival rate at a router exceeds transmission rate? #card
  id:: 6207ba59-077c-4438-ac51-194c3aa57dec
	- Packets will be queued, but if the congestion become too severe, new packets may be dropped and lost
- What is circuit switching? #card
  id:: 6207ba59-d4f2-4c3c-aca9-08d050d4681b
	- It's a mechanism to connect devices, instead of shared links, it allocate dedicated resources for every pair of devices, so resources utilization may be very low
- What is the disadvantage of packet switching compared to circuit switching? #card
  id:: 6207ba59-d200-4609-9608-4af6cfea6343
	- Packets may lost when congestion is high, so reliable data transfer must be implemented
- Name every source of packet delay #card
  id:: 6207cf8f-d559-4fe6-b232-6e8c6c550fe3
	- processing delay
	- queueing delay
	- transmission delay
	- propagation delay
- What does throughput mean? #card
  id:: 6207cf8f-fd43-44ee-ba91-8566a752b0df
	- It is the rate of bits transferred between sender and receiver
- Why do we need protocol reference model? #card
  id:: 6207ba59-c8f4-4494-a678-31dee8138628
	- Communication functions of network have become too complex, so divide them into several sections and define them as layers, PRM describes these layers and their relations
- What is data link layer's responsibility? #card
  id:: 6207ba59-af92-4ac4-870f-0d4ff17d9145
	- Transfer data frames between two hosts connected to the same physical link, it is also responsible for error detection and recovery
- What is network layer's responsibility? #card
  id:: 6207cf8f-86cd-4dcd-8fe8-60777bb58ca3
	- Use packet forwarding and routing to transmit packet to its destination through numerous networks. Also responsible for host addressing and congestion control
- What is transport layer's responsibility? #card
  id:: 6207cf8f-ab2a-4039-a3a0-a447b9b77c05
	- Control and manage communication between processes on different machines, also responsible for reliable and efficient data transfer, naming and flow control
- What is session layer's responsibility? #card
  id:: 6207cf8f-0cc8-4d90-a76a-7600b2e52d72
	- Opening, closing and managing sessions between end users
- What is presentation layer's responsibility? #card
  id:: 6207cf8f-dd07-4b02-b820-d0736dcb1a45
	- Managing syntax and semantics to make sure different machines can read the same information, including encoding/decoding, data compression and encryption
- What is application layer's responsibility? #card
  id:: 6207cf8f-01a9-4a72-aba6-403b9912df0d
	- Provide interfaces for user application
- Why do we need network standard? #card
  id:: 6207ba59-dcca-4990-bbc4-0be5cdc698f3
	- To achieve compatibility and interoperability
- What are the two most common network application architectures? #card
  id:: 6207ba59-348e-4643-beb1-885bc425ecba
	- P2P
	- client-server
- What is socket? #card
  id:: 6207ba59-91f9-449e-891c-50ab624f20bc
	- It is a software structure that serve as an endpoint for a process to send or receive data from the network. In TCP/IP protocols, a socket is identified by values of (source IP, source port, destination IP, destination port, protocol).
- What is a application layer protocol responsible for? #card
  id:: 6207ba59-d322-4e00-b6b3-3f62eaa3cf6e
	- Define different types of messages, message syntax and semantics, and how two parties should interact
- What transport service does a network application need? #card
  id:: 6207ba59-5045-4dc9-9e87-63170d3106ff
	- data integrity
	- timing
	- throughput
	- security
- What protocol does web application use? #card
  id:: 6207ba59-a599-47ef-8e66-554429960d23
	- HTTP
- What happen if we visit a website using non-persistent HTTP? #card
  id:: 6207cf8f-d1fc-4a11-9ee7-8f06e84fe057
	- Browser will create an initial connection to request index.html, and there are maybe a lot of reference objects in that HTML file. So we would have to create an connection for every individual objects
- What is the purpose of cookies in web application? #card
  id:: 6207cf8f-03e6-448f-871f-1700aa2fbb3d
	- Because HTTP is a stateless protocol, and we may have to use stateful information in web applications, so cookies serve as the medium at client side, to let serve know what is this user's state on the website
- Why do we need cache or proxy server? #card
  id:: 6207ba59-fc7f-4338-a5a4-4b826bef783d
	- Setting up a cache server can help client and server to reduce network traffic and response time, because once a content is cached in the cache server, we won't need to access the original server for future connection, and so do other clients
- Which transport layer protocol and port does FTP use? #card
  id:: 6207cf8f-1da6-4211-b73b-3b99b8a3220d
	- TCP at port 21 for command, and port 20 for file transfer
- What are the three major components for electronic mail service? #card
  id:: 6207ba59-7605-4172-8144-d1a4410846e7
	- user agent
	- mail server
	- SMTP
- Why does DNS use distributed and hierarchical architecture? #card
  card-last-interval:: -1
  card-repeats:: 0
  card-ease-factor:: 2.5
  card-last-reviewed:: nil
  card-next-schedule:: nil
  card-last-score:: nil
  id:: 6207ba59-45b2-4cb4-b91d-83963d4f87a5
	- Distributed architecture allow the system to avoid single point of failure, and reduce the complexity for maintenance, and hierarchical architecture allow us to scale the system easily
- What is the role of authoritative DNS server? #card
  id:: 6207cf8f-55e5-4348-974f-c2f8d1fed84d
	- It's normally a DNS server for specific organization
- What services does DNS provide? #card
  id:: 6207ba59-880d-4bd9-bd99-e61625295f08
	- hostname and IP translation
	- host, mail server aliasing
	- load distribution
- Explain the difference between iterated query and recursive query in DNS? #card
  id:: 6207cf8f-f29a-43be-9dda-6fb03490a9a6
	- Iterated approach continue to ask different DNS server until getting the resolution, while recursive approach commission the contacted DNS server to do the query for us
- What types can a DNS record have? #card
  id:: 6207cf8f-f16b-494c-acc7-0d2272f55efb
	- A
		- pure translation
	- NS
		- DNS server for that domain
	- CNAME
		- alias name for canonical name
	- MX
		- mail server for that domain
- How does DNS achieve load distribution? #card
  id:: 6207ba59-6907-4c8b-921e-18ea61d1a298
	- Content provider can replicate it contents to different server with different IP, than setup those server to have same domain name using DNS record, and DNS server will rotate the response IPs when that domain name is queried
- Why P2P architecture can increase the efficiency of file distribution? #card
  id:: 6207ba59-67df-41d0-9445-02628b183ab9
	- Because each client can also act as a server, upload file chunk for other user, while downloading chunks that it doesn't have from other user
- What is DHT? #card
  id:: 6207ba59-a7fa-48d1-968b-21fd37e936a8
	- It's a distributed hash table to store key-value pairs on network of peers, it achieve this by assigning key-value pair to the peer with identifier closest to the key
- How does CDN work? #card
  id:: 6207ba59-1acf-44ff-8999-251999a7e3bc
	- For content provider, to increase assets' response time and reduce traffic to its server, it can use CDN to replicate contents to CDN servers at the edge, so client can access to CDN server that is geographically closest to him. For client, once he connect to content provider, he will get the hostname of CDN provider's DNS, than upon accessing that DNS, it will determine which CDN server should this client access for best experience
- What is DASH in video streaming? #card
  id:: 6207ba59-f894-4b88-8c0b-8ba44d6b541d
	- Dynamic, adaptive streaming over HTTP is a technique to stream video on the the Internet, it breaks a video down to pieces, and encode each pieces with different rates, than send a manifest file to client which allow client to choose the optimal way to access video base on it bandwidth
- What kind of service does transport layer provide? #card
  id:: 6207cf8f-3930-405c-8818-36f8c45d0e0c
	- It provides communication service for two processes on different host
- Which transport layer protocol guarantee network delay and bandwidth? #card
  id:: 6207cf8f-d17c-4307-a722-b411055e403f
	- None of TCP and UDP
- What is multiplexing and demultiplexing? #card
  id:: 6207ba59-7d34-4490-9a88-33eca1b5b2f1
	- They are process that transport layer protocol interacts with application layer and network layer. Multiplexing means transport layer collects data from application layer and transform them into segment to send them into network layer. Demultiplexing means use the information inside segment header to determine which socket should this segment be sent to
- What is the difference between TCP and UDP demultiplexing? #card
  id:: 6207ba59-3262-470a-ae91-82655822ed5a
	- UDP segments from different processes on different hosts, but have same destination IP and port will be sent to same socket, while TCP use (source IP, source port, destination IP, destination port, protocol) to identify which socket should this segment be sent to
- What is the benefit of using UDP as transport layer protocol? #card
  id:: 6207cf8f-ee96-47ef-8436-b53da77bb4e6
	- Sender doesn't need to establish connection with receiver, so UDP can reduce network delay. Also, UDP doesn't have congestion control, so sender can send its packets at any rate
- Why do we need reliable data transfer? #card
  id:: 6207cf8f-5513-443c-94b0-47dc9c9c4378
	- The way network layer handle datagrams may cause some packet loss, so we need to find a way to guarantee our messages can exchange reliably using this unreliable channel
- Explain why rdt 3.0 has low network efficiency? #card
  id:: 6207ba59-7e7c-4aa1-b338-08271787c60e
	- Because it requires sender to send next packet only when it receives ACK from receiver, so it waste network bandwidth for 2 RTT for every packet sent
- Explain the difference between go-back-N method and selective repeat method. #card
  id:: 6207ba59-ecf6-45ab-9e42-9a1148515baf
	- Both methods can send multiple unACKed packets receiver, but in go-back-N, receiver only send one packet, along with a sequence number to indicate up to which packet it has received, while in selective repeat, receiver would send ACK for every packet received. Also, sender only place one timer on the oldest unACKed packet, while selective repeat will place timer on every unACKed packet
- What properties does TCP has? #card
  id:: 6207cf8f-dd4d-47c0-b861-61034f94cb2c
	- point to point transmission
	- reliable and in-order data transfer
	- pipelined data transfer
	- buffer at both sides
	- bi-directional data flow in one connection
	- connection-oriented
	- flow control
- Explain how TCP three-way handshake work? #card
  id:: 6207cf8f-289d-4c7b-abc9-5e9b6ee8366c
	- The client chooses an initial sequence number, set in the first SYN packet. The server also chooses its own initial sequence number, set in the SYN/ACK packet. Each side acknowledges each other’s sequence number by incrementing it: this is the acknowledgement number. The use of sequence and acknowledgement numbers allows both sides to detect missing or out-of-order segments.
- Explain how TCP four-way handshake work? #card
  id:: 6207ba59-b88e-487a-9108-179d68994c51
	- The client first send a FIN packet, if server receive it successfully, it will return a ACK packet, than immediately follow by its own FIN packet and enter closing phase. Upon receiving FIN from server, the client will send a ACK and enter timed wait period, in which the client will respond last ACK when it receive a FIN
- What is the use of sequence number in TCP? #card
  id:: 6207ba59-e166-40c7-9988-7014aa7fe7fc
	- It is used along side with ACK to indicate packet with that sequence number is expected next time from the other end, also means packets with sequence number before that number are received successfully
- How does TCP implement flow control feature? #card
  id:: 6207ba59-ec3c-4bd8-a727-4f9f1c1bdbca
	- Receiver will add information in RcvWindow field in the header to tell sender how much spare space it has, and the sender should keep the number of unACKed packets smaller than that number
- How does TCP implement congestion control feature? #card
  id:: 6207cf8f-fd96-49d5-8108-1cc06e1324d1
	- TCP relies on end systems to inference congestion from network delay and packet loss, and to avoid congestion, end system will maintain congestion window carefully, once the window hit a certain threshold, it will only increase the size by one every RTT
- What happen when a service using TCP compete with a service using UDP for network bandwidth? #card
  id:: 6207ba59-d386-4078-89c2-2054798516b3
	- Service using UDP will take most of the bandwidth, because UDP doesn't care the packets it send is lost or not, but TCP will detect congestion through packet loss, which result in decreasing its own sending rate
- What is the responsibility of network layer? #card
  id:: 6207ba59-2577-43d7-9880-54ecda0dbb07
	- Transport segment from sending host to receiving host
- How does virtual circuits work? #card
  id:: 6207cf8f-f7a5-414c-bfe1-30c6f7704355
	- A connection between sender and receiver need to be set up beforehand, every packet being sent need to carry a VC number, and every router in between maintain a forwarding table that translate incoming VC number to outgoing VC number
- What are three types of switching fabrics inside routers? #card
  id:: 6207ba59-683d-40f0-a0fe-361d85af116b
	- memory
	- bus
	- crossbar
- What is head-of-the-line queuing? #card
  id:: 6207ba59-f09c-4eb6-bb50-6fc05e098c3a
	- Inside a router, if two datagrams at the front of the input ports need to go to the same output port, than datagrams behind one of these datagram will be blocked, even if their desired output port is idle
- Why does Internet protocol need fragmentation? #card
  id:: 6207cf8f-40e6-4f26-95a5-07f314116878
	- Different links have different maximum transmission unit, to guarantee every packet can pass to its destination, fragmentation is needed so that it won't get blocked on the way
- What is CIDR? #card
  id:: 6207cf8f-cae0-42c8-80fc-c59cb81d08d3
	- It's a way to allocate IP address and IP routing
- What is DHCP? #card
  id:: 6207ba59-fb0e-4618-b841-7ff5b260f7a8
	- It's a protocol that allows client to dynamically get IP address from server, client can also get first hop router, IP of DNS server and network mask using DHCP
- What is the benefit of using DHCP? #card
  id:: 6207ba59-b09f-409b-8eab-63a09325361d
	- allow reuse of address
	- allow address lease renewal
- How to identify subnet? #card
  id:: 6207ba59-eab2-42fd-8fad-0480cf11745e
	- IP addresses that have the same most significant bit group are in the same subnet
- What is NAT? #card
  id:: 6207cf8f-a10f-4d5c-8eb0-813b5e5e991a
	- It's a service that allows hosts in the same subnet to communicate with outside world using one IP address, router achieve this by maintaining the mapping between outgoing port and local host's address
- What is ICMP? #card
  id:: 6207ba59-64f4-4291-aecd-d9d11a082ea8
	- It's a network protocol used by hosts and routers to communicate network information like errors
- How long is a IPv6 header? #card
  id:: 6207ba59-3ab8-4a5c-a8da-954f114c20f6
	- 40 byte
- How does a IPv6 datagram get passed between two IPv4 routers? #card
  id:: 6207ba59-75a0-4a52-9544-4c7057313e92
	- Use tunneling, wrap IPv6 datagram inside IPv4 datagram
- What is the difference between routing algorithm that use global information and decentralized information? #card
  id:: 6207cf8f-e9f1-4d65-9a11-7c3092c761fe
	- Global information means routers know link cost of the entire network, while decentralized information means router only knows link cost information about its neighbors
- What is the difference between link state algorithm and distance vector algorithm? #card
  id:: 6207ba59-4742-428e-bac4-6c0f0b3e6572
	- Link state algorithm assumes every router know network topology while distance vector algorithm assume routers only know information about their neighbors. Distance vector algorithm require routers frequently exchange their forwarding table, but this isn't required by link state algorithm. Link state algorithm uses Dijkstra's algorithm while distance vector algorithm uses Bellman-Ford algorithm
- What is oscillation problem? #card
  id:: 6207ba59-12c1-450e-a209-7eae63fda1ff
	- Oscillation may occur in network using link state algorithm. Essentially, since network flow determine each link's cost, the path choose by a router may not be optimal after a short time and required correction. If this situation happens back and forth between two paths, its called oscillation
- What is count to infinity problem? #card
  id:: 6207cf8f-7c55-4abf-b97e-5ec5b21b97d9
	- Count to infinity problem may occur in network using distance vector algorithm. If a router detect a link is down, and it choose another path base on its another neighbor's distance vector, but that path also pass through that dead link, then count to infinity problem occur. This problem may be solved by poison reverse
- Why do we need hierarchical routing? #card
  id:: 6207cf8f-b941-4fe9-bb7e-1a087e9d73bf
	- We have to store all the information inside every router and congest network bandwidth, which make the network hard to scale
- What are some of the intra-AS algorithm? #card
  id:: 6207cf8f-3028-43d5-8bb5-d1157431d031
	- RIP
	- OSPF
	- IGRP
- What is BGP? #card
  id:: 6207ba59-037b-4f1f-ad13-cf576511a980
	- It's a protocol to achieve inter-AS routing, different AS can make different policy to serve their purpose
- What is the responsibility of link layer? #card
  id:: 6207ba59-4696-401e-981e-f0c0162d689a
	- It is responsible for transferring datagram from one node to physically adjacent node over a link
- What type of service does link layer provide? #card
  id:: 6207ba59-4ef0-4574-a0f1-60e47ad36326
	- framing
	- link access
	- reliable delivery
	- flow control
	- error detection
	- error correction
	- half duplex and full duplex
- What kind of network device will implement link layer? #card
  id:: 6207cf8f-a7e7-4c65-b57b-9ce42822aa54
	- Every device that want to connect to the Internet
- How does link layer achieve error detection feature? #card
  id:: 6207cf8f-4b4d-4788-9d35-f467cf259a36
	- Protocols may attach error detection bits to the frame
- What kinds of error detection method does link layer use? #card
  id:: 6207ba59-f344-4e1b-b325-86e82698cfcc
	- parity checking
	- cyclic redundancy check
- Why do we need multiple access protocol? #card
  id:: 6207ba59-8902-4974-b544-2a340c6307c6
	- Two or more nodes may contend for a single shared channel for transmission, so we need a protocol to decide how nodes should share this channel
- What types do multiple access protocols have? #card
  id:: 6207cf8f-6fd7-4107-a4b2-f1024fe4c425
	- channel partitioning
	- random access
	- taking turns
- What are the disadvantages of channel partitioning protocols? #card
  id:: 6207cf8f-c67f-481b-8343-941e88aac731
	- Low channel usage at low load
- What are the disadvantages of random access protocols? #card
  id:: 6207ba59-4563-4f53-9e25-1b935c552b90
	- Low efficiency at high load because of collision
- What is the main difference between ALOHA and CSMA? #card
  id:: 6207ba59-9db3-48d5-847e-1b387cc535f7
	- Both can detect collision when it occurs, but CSMA will listen to the  channel first, it will allow node to transmit only when the channel is sensed idle
- What are the disadvantages of taking turns protocols? #card
  id:: 6207cf8f-26a0-40b9-938f-2bfa45099034
	- Possibility of single point of failure and overhead
- What is the purpose of MAC address? #card
  id:: 6207ba59-ec0e-4d36-8565-2822c47a910f
	- It is used to get frame from one interface to another interface under same network
- What is ARP? #card
  id:: 6207ba59-a1f3-4cd2-a279-80bbc3122b66
	- Address resolution protocol, it determines interface's MAC address given its IP address using ARP table
- How is ARP table constructed? #card
  id:: 6207ba59-b1b6-43b0-bddd-e0467c16ffa8
	- Use broadcasted ARP query containing target IP address
- How does switch know which interface to send the frame? #card
  id:: 6207ba59-d9fc-490b-9101-774d44b4513c
	- Use switch table
- How does switch table construct? #card
  id:: 6207ba59-1498-4fa6-8f53-66b6dbd9ce91
	- By incoming frame
- What does switch do when the destination address is unknown? #card
  id:: 6207ba59-6283-4a20-ba68-c2a3466496cc
	- It sends the frame to every interface except the incoming one
- What is VLAN? #card
  id:: 6207ba59-d474-4a6d-994f-dcd19085954f
	- It's a technology that allows user to define multiple LANs over single physical LAN infrastructure
- Why do we need VLAN? #card
  id:: 6207cf8f-117d-4151-a703-bbe0769f0e51
	- Separate traffic with different roles or purposes, reduce traffic and overcome physical barrier