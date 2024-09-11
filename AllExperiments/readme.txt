Inter-VLAN Routing
Inter-VLAN routing allows devices in different VLANs to communicate with each other through a Layer 3 device, such as a router or Layer 3 switch. VLANs isolate traffic within the same broadcast domain, but inter-VLAN routing bridges different VLANs by routing traffic between them. It is commonly achieved through Router-on-a-stick (single physical interface with subinterfaces for each VLAN) or Layer 3 Switches using Switched Virtual Interfaces (SVIs). The 802.1Q protocol is often used for VLAN tagging.

Smart Home Application Using Network Devices
A smart home network integrates various devices like lights, thermostats, security cameras, and home assistants using network technologies such as Wi-Fi, Zigbee, and Bluetooth. These devices communicate over a home router to allow centralized control through mobile applications or voice commands. Networking components like switches, routers, and access points provide the backbone for device connectivity, while security protocols and firewalls ensure data integrity and privacy.

Static Routing
Static routing involves manually configuring the routing table on routers. Each route is explicitly defined, mapping destination networks to specific interfaces or next-hop IP addresses. Static routing is simple and suitable for small networks but doesn't scale well for larger, dynamic networks. It requires manual updates whenever network topology changes, which can be error-prone and inefficient in rapidly changing environments.

Routing Using OSPF
Open Shortest Path First (OSPF) is a dynamic routing protocol used for routing within an Autonomous System (AS). It is based on the Link State Routing algorithm, which ensures faster convergence and efficient routing. OSPF routers share information about their direct links, construct a topology map, and compute the shortest path using Dijkstra's algorithm. OSPF is widely used in large-scale enterprise networks due to its scalability and support for load balancing.

FTP Server Configuration and Testing
FTP (File Transfer Protocol) servers allow users to upload and download files across a network. To configure an FTP server, the server software is installed and network settings are adjusted to allow connections over port 21. User authentication and permissions are configured to control access. Testing an FTP server involves using an FTP client to connect to the server, transfer files, and ensure that data can be uploaded or downloaded securely, often using both anonymous and authenticated users.
