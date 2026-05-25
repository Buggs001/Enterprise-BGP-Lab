# IP Addressing Plan

## Point-to-Point Links

| Connection | Interface | IP Address | Subnet |
|---|---|---|---|
| R1 ↔ R2 | R1 Fa0/0 | 10.0.12.1 | 255.255.255.252 |
| R1 ↔ R2 | R2 Fa0/0 | 10.0.12.2 | 255.255.255.252 |
| R1 ↔ R3 | R1 Fa0/1 | 10.0.13.1 | 255.255.255.252 |
| R1 ↔ R3 | R3 Fa0/0 | 10.0.13.2 | 255.255.255.252 |

---

# Autonomous System Numbers

| Router | ASN |
|---|---|
| R1 | 65001 |
| R2 | 200 |
| R3 | 300 |

---

# Topology Overview

- R1 acts as the enterprise edge router.
- R2 simulates ISP A.
- R3 simulates ISP B.
- R1 establishes eBGP peerings with both ISPs.

---

# Addressing Notes

- /30 subnetting is used for point-to-point WAN links.
- Each WAN segment contains exactly two usable IP addresses.
- Private IPv4 addressing is used for lab simplicity.