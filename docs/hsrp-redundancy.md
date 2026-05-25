# HSRP Redundancy

## Overview

Hot Standby Router Protocol (HSRP) was implemented between the enterprise core routers to provide first-hop redundancy for end devices.

HSRP ensures gateway availability by maintaining an Active and Standby router pair.

---

# HSRP Configuration

| Device | Role |
|---|---|
| CORE-1 | Active |
| CORE-2 | Standby |

Virtual Gateway:
```text
192.168.1.1
```

---

# HSRP Features Implemented

- Active/Standby redundancy
- Virtual default gateway
- Gateway failover capability
- Preemption

---

# Verification Commands

```bash
show standby brief
```

---

# Verification Results

The following were successfully verified:

- Active router election
- Standby router state
- Virtual IP operation
- HSRP redundancy functionality

---

# Design Purpose

HSRP was implemented to simulate enterprise gateway redundancy and improve network availability during router or path failures.