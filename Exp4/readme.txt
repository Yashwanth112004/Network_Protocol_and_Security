Experiment 4: Configuring VLAN on Layer 3 Switches using 802.1Q (Inter-VLAN Routing)
In this experiment, you will configure VLANs and enable Inter-VLAN Routing on a Layer 3 switch using the 802.1Q encapsulation method. This allows devices in different VLANs to communicate with each other through a router or Layer 3 switch.

Objective:
Create and configure VLANs on a Layer 3 switch.
Use 802.1Q encapsulation to enable Inter-VLAN routing.
Verify connectivity between different VLANs.
Requirements:
Cisco Packet Tracer
Layer 3 Switch (e.g., Cisco 3560)
PCs (connected to the switch)
Straight-through cables to connect devices
Theory:
VLAN: A Virtual Local Area Network allows for logical segmentation of networks on Layer 2.
802.1Q: An IEEE standard for tagging VLANs in Ethernet frames, enabling inter-VLAN routing.
Inter-VLAN Routing: Allows communication between devices in different VLANs using a Layer 3 device.
Steps for Configuration:
1. Set Up the Network:
Drag and drop a Layer 3 switch (e.g., Cisco 3560) and some PCs into the workspace.
Use copper straight-through cables to connect PCs to different switch ports.

Configure 802.1Q Trunking:
To allow VLANs to communicate, configure a trunk on the port that connects to the router or another switch.
interface fastethernet 0/24
switchport mode trunk
switchport trunk encapsulation dot1q
exit
Configure Inter-VLAN Routing:
Enable Inter-VLAN Routing on the Layer 3 switch by creating Switched Virtual Interfaces (SVIs) for each VLAN.
interface vlan 10
ip address 192.168.10.1 255.255.255.0
no shutdown
exit
interface vlan 20
ip address 192.168.20.1 255.255.255.0
no shutdown
exit
5. Assign IP Addresses to PCs:
For each PC, assign an IP address in the range of the VLAN it belongs to:
PC in VLAN 10:

IP Address: 192.168.10.2
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.10.1
PC in VLAN 20:

IP Address: 192.168.20.2
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.20.1

By following the above steps, you have configured a Layer 3 switch using 802.1Q encapsulation for Inter-VLAN routing.
Devices in different VLANs can now communicate through the Layer 3 switch, simulating a real-world network with VLAN segmentation and routing capabilities.
