# Investigation Process

## Step 1 – Log Review

Reviewed DNS logs for:

- Query frequency
- Subdomain length anomalies
- Entropy characteristics
- Repeated patterns
- External domain reputation

Observation:
Consistent beaconing pattern with uniform interval (60 seconds).

---

## Step 2 – Domain Analysis

- Domain not present in threat intelligence feeds
- Recently registered domain
- Low reputation score

---

## Step 3 – Traffic Pattern Analysis

Indicators:

- Periodic communication
- Small but consistent data payload encoded in subdomain
- No legitimate application behavior matching pattern

Conclusion:
Strong indicators of DNS-based C2 communication.

---

## Identified Indicators of Compromise (IoCs)

- Suspicious external domain
- Repeating beacon interval
- Long encoded subdomains
- High-frequency DNS queries
