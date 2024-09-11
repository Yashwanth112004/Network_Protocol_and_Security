In Cisco Packet Tracer, configuring VLANs (Virtual Local Area Networks) helps to segment networks into different broadcast domains, increasing security and reducing congestion. Here’s a step-by-step guide to VLAN configuration:

VLAN Configuration in Cisco Packet Tracer:
Launch Cisco Packet Tracer:

Open the Packet Tracer software and create a new project.
Add Devices:

Drag and drop Switches (e.g., Cisco 2960) and PCs from the devices list into the workspace.
Connecting Devices:

Use the copper straight-through cable to connect each PC to different switch ports.
Access CLI of the Switch:

Click on a switch to access its CLI (Command Line Interface) for VLAN configuration.
Configure VLANs:
enable
configure terminal

interface fastethernet 0/1
switchport mode access
switchport access vlan 10
exit

interface fastethernet 0/2
switchport mode access
switchport access vlan 20
exit

IP Address Assignment:

Assign IP addresses to the PCs (via Desktop > IP Configuration) so that they can communicate within the same VLAN.
Inter-VLAN Routing (Optional):

To enable communication between VLANs, configure router-on-a-stick or use Layer 3 switches to route between VLANs.
Example Use Case:
VLAN 10 for the Sales department and VLAN 20 for Marketing ensures that devices within each VLAN can only communicate with devices in the same VLAN unless inter-VLAN routing is enabled.
Benefits of VLANs:
Security: Isolates different departments or groups.
Reduced Broadcasts: Minimizes unnecessary traffic by limiting broadcasts to each VLAN.
Flexibility: Easier network management and segmentation.
This setup helps simulate VLAN management in a real network environment.







