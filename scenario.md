# Scenario Description

## Environment

- Medium-sized enterprise network
- Windows-based endpoints
- Centralized DNS logging enabled
- Perimeter firewall with logging
- Endpoint Detection & Response (EDR) deployed

---

## Trigger Event

The SOC detected unusually high DNS request frequency originating from a single internal workstation.

Key observations:

- Repeated DNS queries every 60 seconds
- Long subdomain strings (30+ characters)
- High entropy patterns resembling encoded data
- Requests to an unknown external domain
- No corresponding web browsing activity

---

## Initial Hypothesis

The behavior is consistent with DNS tunneling, potentially used for:

- Command-and-Control (C2)
- Data exfiltration
- Beaconing communication

Further investigation required.
