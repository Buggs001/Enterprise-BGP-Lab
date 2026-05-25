# Enterprise BGP Lab

## Overview

Enterprise BGP Lab is a practical network engineering project built in GNS3 to understand how enterprises connect to multiple Internet Service Providers (ISPs) using Border Gateway Protocol (BGP).

The lab focuses on real-world enterprise edge routing concepts including eBGP neighbor relationships, multi-homing, redundancy, failover, route advertisement, and basic traffic engineering.

This project is designed as a hands-on learning environment to gain practical experience with Internet edge architecture and BGP operations.

---

# Network Topology

| Device | Role | ASN |
|---|---|---|
| R1 | Enterprise Edge Router | AS 65001 |
| R2 | ISP A | AS 200 |
| R3 | ISP B | AS 300 |

## Topology Diagram

![Enterprise BGP Topology](topology/topology-diagram.png)

---

# BGP Configurations
### eBGP Connections

- R1 ↔ R2
- R1 ↔ R3

The enterprise router establishes eBGP sessions with two separate ISPs to simulate a multi-homed enterprise environment.

---

# Project Objectives

This lab is focused on understanding and implementing:

- BGP Fundamentals
- eBGP Neighbor Formation
- Multi-Homing
- Route Advertisement
- BGP Path Selection
- Redundancy and Failover
- Internet Edge Design
- Basic Traffic Engineering

---

# Lab Environment

| Component | Details |
|---|---|
| Platform | GNS3 |
| Router Image | Cisco c7200 |
| Routing Protocol | BGP |
| Topology Type | Enterprise Multi-Homing |

---

# Repository Structure

```text
Enterprise-BGP-Lab/
│
├── README.md
├── topology/
├── configs/
├── screenshots/
├── docs/
└── notes/
```

---

# Documentation Included

This repository contains:

- Router configurations
- Network topology diagrams
- IP addressing plans
- BGP configuration steps
- Verification outputs
- Testing screenshots
- Learning notes and observations

---

# Learning Goals

This project is intended to strengthen practical knowledge in:

- Enterprise WAN Connectivity
- ISP Edge Routing
- BGP Operations
- Network Troubleshooting
- Routing Policy Understanding
- Infrastructure Documentation

---

# Future Expansion

The lab will later expand into advanced networking concepts including:

- iBGP
- OSPF Integration
- Route Reflectors
- Local Preference
- AS Path Prepending
- MED
- Route Filtering
- Default Route Control
- Internet Simulation
- MPLS Concepts

---

# Author

**Shivmani Shinde**

Network Engineering & Infrastructure Learning Project