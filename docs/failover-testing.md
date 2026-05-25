# Failover Testing

## Overview

Failover testing was performed to validate redundancy and path recovery behavior within the enterprise BGP architecture.

The enterprise network was designed with dual ISP connectivity to ensure continued external reachability during upstream failures.

---

# Test Objectives

The failover tests were designed to verify:

- ISP redundancy
- BGP convergence behavior
- Backup path activation
- Internet reachability during failures
- Recovery after link restoration

---

# Failover Scenario

The primary upstream path was intentionally disrupted to simulate an ISP or link failure.

During the outage:

- ICMP packet loss was observed temporarily
- BGP reconvergence occurred
- Traffic shifted toward the backup ISP path

Connectivity was later restored successfully.

---

# Verification Commands

```bash
ping 8.8.8.8
show ip bgp
show ip route
```

---

# Observed Behavior

## Before Failure

- Stable connectivity to external destinations
- Primary ISP path active
- Successful ICMP responses

---

## During Failure

- Temporary packet loss occurred
- ICMP timeouts were observed
- BGP reconvergence process initiated

---

## After Recovery

- Backup path became active
- Connectivity restored successfully
- Traffic resumed through alternate ISP path

---

# Verification Results

The following were successfully validated:

- Dual ISP redundancy
- BGP failover operation
- Route reconvergence
- Backup path availability
- Enterprise Internet resilience

---

# Design Purpose

The failover implementation simulates real-world enterprise WAN resiliency and demonstrates how BGP provides external connectivity redundancy using multiple ISP providers.