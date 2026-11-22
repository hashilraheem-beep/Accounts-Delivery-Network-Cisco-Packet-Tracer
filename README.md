# Accounts and Delivery Department Network

## Project Overview

This project demonstrates the design and implementation of a departmental network using **Cisco Packet Tracer**.

The network connects the Accounts and Delivery departments through a router, allowing devices in the Delivery department to communicate with devices in the Accounts department.

## Network Topology

The network consists of:

- 1 Cisco 2911 Router
- 2 Cisco 2960 Switches
- 4 PCs (2 in each department)
- 2 Printers (1 in each department)

![Network Topology](screenshots/01-network-topology.png)

## IP Addressing

The given network address is `192.168.40.0`, divided into two subnets using a `/25` subnet mask.

| Device | IP Address | Default Gateway |
|---|---|---|
| Accounts PC0 | 192.168.40.2 | 192.168.40.1 |
| Accounts PC1 | 192.168.40.3 | 192.168.40.1 |
| Accounts Printer | 192.168.40.4 | 192.168.40.1 |
| Delivery PC2 | 192.168.40.130 | 192.168.40.129 |
| Delivery PC3 | 192.168.40.131 | 192.168.40.129 |
| Delivery Printer | 192.168.40.134 | 192.168.40.129 |

**Subnet Mask:** `255.255.255.128`

## Configuration Screenshots

### Accounts Department IP Configuration

![Accounts IP Configuration](screenshots/02-accounts-ip-config.png)

### Delivery Department IP Configuration

![Delivery IP Configuration](screenshots/03-delivery-ip-config.png)

### Router Interface Configuration

![Router Interfaces](screenshots/04-router-interfaces.png)

## Connectivity Testing

Connectivity was tested using the `ping` command from Delivery PCs to Accounts PCs.

### Delivery PC2 to Accounts PCs

![Delivery to Accounts Ping](screenshots/05-delivery-to-accounts-ping.png)

### Delivery PC3 to Accounts PCs

![Connectivity Verification](screenshots/06-connectivity-verification.png)

## Result

- Both departments were connected through a router.
- IP addressing and subnetting were configured.
- Successful communication was verified between Delivery and Accounts PCs using ping tests.

## Tools Used

- Cisco Packet Tracer
- IPv4 Addressing
- Subnetting
- Router and Switch Configuration
- Ping Connectivity Testing

## Project File

The Packet Tracer project file is available in this repository.

## Conclusion

This project demonstrates the implementation of a basic departmental network and successful communication between two different subnets using Cisco Packet Tracer.
