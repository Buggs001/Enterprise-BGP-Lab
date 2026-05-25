# BGP Design

## Overview

The Enterprise BGP Lab uses external Border Gateway Protocol (eBGP) to simulate enterprise connectivity to multiple Internet Service Providers (ISPs).

The enterprise edge routers establish BGP peerings with two separate ISP routers to provide:

- Redundancy
- Multiple upstream paths
- Route failover capability
- Basic traffic engineering behavior

---

# Autonomous System Numbers

| Device | ASN |
|---|---|
| Enterprise | AS 65000 |
| ISP-1 | AS 100 |
| ISP-2 | AS 200 |

---

# eBGP Peerings

| Neighbor Relationship | Type |
|---|---|
| EDGE-1 ↔ ISP-1 | eBGP |
| EDGE-1 ↔ ISP-2 | eBGP |

---

# Route Advertisement

The enterprise edge routers receive external routes from both ISPs.

Example advertised prefixes:

- 100.100.100.0/24
- 200.200.200.0/24
- 8.8.8.8/32

---

# Best Path Selection

The enterprise edge router receives multiple paths for external destinations and selects the preferred path using the BGP best-path algorithm.

Verification was performed using:

```bash
show ip bgp
show ip bgp 8.8.8.8
show ip bgp summary
```

---

# BGP Verification

The following were verified successfully:

- eBGP neighbor establishment
- Route learning from both ISPs
- Best path selection
- Route propagation
- Internet reachability

---

# Design Goals

The BGP design was implemented to simulate:

- Enterprise multi-homing
- ISP redundancy
- Internet edge routing
- Failover behavior
- Real-world enterprise WAN architecture