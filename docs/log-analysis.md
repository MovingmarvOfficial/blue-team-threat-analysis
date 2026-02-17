# Log Analysis – DNS Traffic Investigation

## Objective

Analyze DNS log entries to identify potential DNS tunneling behavior.

---

## Step 1 – Identify Frequency Anomalies

Observation:

Multiple DNS queries to the same domain occur at exact 60-second intervals.

Example:

10:01:00  
10:02:00  
10:03:00  
10:04:00  

This pattern is consistent with beaconing behavior.

---

## Step 2 – Analyze Subdomain Length

Legitimate DNS queries typically contain short hostnames.

Suspicious entries contain long subdomains:

Example:
YWxhZGRpbjpvcGVuc2VzYW1l.example-domain.com

Long subdomains (>25 characters) may indicate encoded data.

---

## Step 3 – Entropy Consideration

High-entropy strings appear random and structured like Base64.

Indicators:
- Mixed uppercase and lowercase letters
- No readable words
- Repeating encoded patterns

This suggests potential data encoding within DNS queries.

---

## Step 4 – Hypothesis

The behavior matches characteristics of:

- DNS tunneling
- Command-and-Control beaconing
- Possible data exfiltration

Further endpoint investigation would be required.
