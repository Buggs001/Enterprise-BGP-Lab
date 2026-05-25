# Enterprise BGP Lab

## Overview

Enterprise BGP Lab is a practical network engineering project built in GNS3 to understand how enterprises connect to multiple Internet Service Providers (ISPs) using Border Gateway Protocol (BGP).

The lab focuses on real-world enterprise edge routing concepts including eBGP neighbor relationships, multi-homing, redundancy, failover, route advertisement, and basic traffic engineering.

This project is designed as a hands-on learning environment to gain practical experience with Internet edge architecture and BGP operations.

---

The lab simulates a resilient enterprise Internet edge architecture with dual ISP connectivity, internal dynamic routing, gateway redundancy, and simulated Internet reachability. The design incorporates OSPF for internal routing, eBGP for external connectivity, and HSRP for first-hop redundancy.

---
# Network Topology

| Device | Role |
|---|---|
| CORE-1 | Enterprise Core Router |
| CORE-2 | Enterprise Core Router |
| EDGE-1 | Enterprise Edge Router |
| EDGE-2 | Enterprise Edge Router |
| ISP-1 | Internet Service Provider |
| ISP-2 | Internet Service Provider |
| INTERNET | Simulated Internet Router |

---


## Topology Diagram

![Enterprise BGP Topology](topology/topology-diagram.png)

---

# External BGP Connectivy

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

# Architecture Features

- Enterprise Multi-Homing
- Dual ISP Connectivity
- eBGP External Routing
- OSPF Internal Routing
- HSRP Gateway Redundancy
- Internet Simulation
- BGP Best Path Selection
- Dynamic Route Failover
- Enterprise WAN Resiliency

---

# Routing Protocols Used

| Protocol | Purpose |
|---|---|
| BGP | External ISP routing |
| OSPF | Internal enterprise routing |
| HSRP | Gateway redundancy |

---

# Verification & Testing

The following functionality was successfully verified during testing:

- eBGP neighbor establishment
- Route advertisement and learning
- Dual ISP connectivity
- Internet reachability
- BGP best path selection
- HSRP Active/Standby operation
- Failover and reconvergence behavior
- Backup path activation

---

# Project Screenshots

Verification screenshots for:

- BGP neighbor establishment
- Best path selection
- HSRP redundancy
- Failover testing
- Route validation
- Internet reachability

are available inside the `screenshots/` directory.

---

# Author

**Shivmani Shinde**

Network Engineering & Infrastructure Learning Project