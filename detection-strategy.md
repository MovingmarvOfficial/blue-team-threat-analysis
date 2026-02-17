# Detection Strategy

## Log Sources Required

- DNS logs
- Firewall logs
- EDR telemetry
- Proxy logs

---

## Detection Opportunities

### 1. High-Frequency DNS Queries
Alert on:
- More than X DNS queries per minute from single host

### 2. Long Subdomain Length
Alert on:
- Subdomains exceeding 25–30 characters

### 3. High Entropy DNS Queries
Detect:
- Base64-like patterns
- Randomized strings

### 4. Repeating Beacon Interval
Detect:
- Periodic traffic at fixed intervals

---

## Preventive Measures

- DNS filtering
- Network segmentation
- Egress filtering
- DNS logging retention
- Threat intelligence integration
