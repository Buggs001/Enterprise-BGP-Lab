# Routing Overview

## Architecture Summary

The Enterprise BGP Lab simulates a multi-homed enterprise network connected to two separate Internet Service Providers (ISPs).

The topology includes:

- Core routers
- Edge routers
- ISP routers
- Simulated Internet connectivity
- Enterprise LAN segment

---

# Routing Technologies Used

| Technology | Purpose |
|---|---|
| OSPF | Internal enterprise routing |
| BGP | External ISP connectivity |
| HSRP | Gateway redundancy |

---

# Internal Routing

OSPF was implemented within the enterprise network to provide dynamic internal routing between core and edge devices.

The internal network exchanges routes dynamically and provides path redundancy across the enterprise infrastructure.

---

# External Routing

BGP was implemented between enterprise edge routers and ISP routers using eBGP peerings.

The enterprise receives external routes from both ISPs and performs best-path selection for outbound traffic.

---

# Redundancy Design

The network includes multiple redundancy mechanisms:

- Dual ISP connectivity
- HSRP gateway redundancy
- Dynamic routing failover
- Multiple external BGP paths

---

# Internet Simulation

A simulated Internet router/network was implemented to emulate external public reachability.

Connectivity testing was performed using:

```text
8.8.8.8
```

---

# Verification

The following were successfully verified:

- Internal OSPF route exchange
- eBGP neighbor establishment
- End-to-end connectivity
- BGP best-path selection
- Failover and recovery behavior
- HSRP gateway redundancy

---

# Design Goals

This project was designed to simulate a real-world enterprise Internet edge architecture with resiliency, redundancy, and dynamic routing behavior.