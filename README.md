Implementing VLAN Segmentation with Inter-Switch Trunking for Network Isolation and Efficiency

Components Needed:
4 PCs: Labeled PC1, PC2, PC3, and PC4.
2 Switches: Labeled Switch1 and Switch2.
Network Cables: To connect PCs to switches and interconnect switches.

Step 1: Physically Connect the Devices
  PC to Switch Connections:
    Connect PC0 and PC1 to Switch1.
    Connect PC2 and PC3 to Switch2.
  Switch to Switch Connection:
    Connect Switch1 to Switch2 using a network cable on designated trunk ports.
Step 2: Configure VLANs on Switch1
  Create VLANs:
    Create VLAN 1 and VLAN 2 on Switch1.
  Assign Ports to VLANs:
    Assign the ports connected to PC0 and PC1 to VLAN 1.
    Configure the port connected to Switch2 as a trunk port and allow VLAN 1 and VLAN 2 traffic.
Step 3: Configure VLANs on Switch2
  Create VLANs:
    Create VLAN 1 and VLAN 2 on Switch2 (matching IDs as on Switch1).
  Assign Ports to VLANs:
    Assign the ports connected to PC2 and PC3 to VLAN 20.
    Configure the port connected to Switch1 as a trunk port and allow VLAN 1 and VLAN 2 traffic.
For Switch 1 and Switch 2:
step 1: en (enable)
step 2: conf t (configure terminal)
step 3: int f0/1 (interface)
step 4: switchport mode access
step 5: switchport ac vlan 1
step 6: int f0/2 (interface)
step 7: switchport mode access
step 8: switchport ac vlan 2

Trunking Switches:
step 1: en (enable)
step 2: conf t (configure terminal)
step 3: int f0/3 (interface)
step 4: switchport mode trunk

For Verification:
ping different PCS of different vlan
Output : Request Timed Out
